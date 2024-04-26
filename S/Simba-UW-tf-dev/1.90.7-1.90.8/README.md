# Comparing `tmp/Simba-UW-tf-dev-1.90.7.tar.gz` & `tmp/Simba-UW-tf-dev-1.90.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.90.7.tar", last modified: Fri Apr 26 00:17:09 2024, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.90.8.tar", last modified: Fri Apr 26 11:34:37 2024, max compression
```

## Comparing `Simba-UW-tf-dev-1.90.7.tar` & `Simba-UW-tf-dev-1.90.8.tar`

### file list

```diff
@@ -1,651 +1,651 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.90.7/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5883 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8835 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9544 2024-04-26 00:11:08.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    25598 2024-04-17 23:32:48.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/roi_size_standardizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4682 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9048 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8376 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3351 2024-04-25 16:26:59.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10787 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9121 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
--rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9419 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1821 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    81527 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4470 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3290 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.90.7/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.7/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.7/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.90.7/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.90.7/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.90.7/simba/labelling/targeted_annotations_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/cluster_validation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/cluster_video_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/cluster_videos_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/transform_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/embedding_correlations_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/data_extractor_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/fit_cluster_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/cluster_xai_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/print_embedding_info_popup.py
--rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/unsupervised_main.py
--rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/outlier_detector.py
--rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/cluster_frequentist_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/embedding_correlation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/cluster_xai_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/clusterer_comparison_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.90.7/simba/unsupervised/tsne.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.90.7/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    18436 2024-04-25 18:36:04.000000 Simba-UW-tf-dev-1.90.7/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_4bp.py
--rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.90.7/simba/feature_extractors/amber_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     1033 2024-04-11 12:52:35.000000 Simba-UW-tf-dev-1.90.7/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/annotator_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    84153 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/timeseries_features_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    48035 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)    56304 2024-04-17 23:32:32.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/circular_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    38770 2024-04-21 12:08:55.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/network_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    24040 2024-04-18 18:35:47.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/video_processing_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    36231 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/feature_extraction_supplement_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   169619 2024-04-22 13:26:42.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/statistics_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    44711 2024-04-22 19:40:36.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    73186 2024-04-25 23:55:15.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/abstract_classes.py
--rw-r--r--   0 simon      (501) staff       (20)    61924 2024-04-21 12:08:55.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/image_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   132883 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)   166028 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/geometry_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/mixins/feature_extraction_circular_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/boris_source_cleaner.py
--rw-r--r--   0 simon      (501) staff       (20)    18982 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18852 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    15281 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.90.7/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    26038 2024-03-27 13:42:19.000000 Simba-UW-tf-dev-1.90.7/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.7/simba/utils/custom_feature_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.90.7/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7737 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.7/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)    52940 2024-04-25 19:17:22.000000 Simba-UW-tf-dev-1.90.7/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    79462 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)    15355 2024-04-16 18:54:43.000000 Simba-UW-tf-dev-1.90.7/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    46271 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.90.7/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/SimBA_logo.ico
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.90.7/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/
--rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/dprime.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/linear_fretchet.py
--rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/piotr_120324 3.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/dunn_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/colinear_features.py
--rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/horizontal_videos_concat.py
--rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/silhouette_score.py
--rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/two_fish_feature_extractor_040924.py.zip
--rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/cuda_jit.ipynb
--rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/directed_hausdorff.py
--rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/shannon_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/sequential_lag_analysis.py
--rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/wilcoxon.py
--rw-r--r--   0 simon      (501) staff       (20)    21599 2024-04-22 16:40:51.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 14:48:22.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/data.npy
--rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/distances.py
--rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     2699 2024-03-10 16:29:57.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/cohens_kappa.py
--rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/paths.py
--rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/outliers_tietjen.py
--rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/train_model.py
--rw-r--r--   0 simon      (501) staff       (20)     2346 2024-04-19 14:10:16.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/img_stack_to_bw.py
--rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/amber_tests.py
--rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/line_locate_point.py
--rw-r--r--   0 simon      (501) staff       (20)     1841 2024-04-19 16:19:10.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/sorensen_dice_coefficient.py
--rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/multifrm_to_points.py
--rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/lcs.py
--rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/two_fish_feature_extractor_040924.py
--rw-r--r--   0 simon      (501) staff       (20)     6119 2024-04-20 17:58:22.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/ez_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/add_body_part.py
--rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/grubbs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/slide_circ_mean.py
--rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/calinski_harabasz.py
--rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/roi_feature_visualizer_example.py
--rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/spontaneuous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/runs_test.py
--rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/pct_counts_in_top_N.py
--rw-r--r--   0 simon      (501) staff       (20)     1095 2024-04-19 18:37:50.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/concordance_ratio.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/total_variation_distance.py
--rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/crop_single_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)    15977 2024-04-23 22:52:42.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/joint_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     1529 2024-04-19 15:08:24.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/segment_image_horizontal.py
--rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
--rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/elliptic_envelope.py
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/roi_definition_csvs_to_h5.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/add_body_part.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/roi_feature_visualizer_example.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/sliding_crosscorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/roi_definition_csvs_to_h5.py
--rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/distance_velocity.py
--rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/line_plot_plotly.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/unsupervised_lof.py
--rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/siegel_tukey.py
--rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/berger_parker.py
--rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/isolation_forest.py
--rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/davis_bouldin.py
--rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/vertical_video_concatenator.py
--rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/batch_video_to_greyscale.py
--rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/crop_circles_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/heading.py
--rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/piotr_120324 2.py.zip
--rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/grangercausalitytests.py
--rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/multiframe_is_shape_covered.py
--rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/redis.py
--rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/piotr_120324.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/hartley_fmax.py
--rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/calc_N_degree_direction_switches.py
--rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/fix_clahe.py
--rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/cochran_q.py
--rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/menhinicks_index.py
--rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1559 2024-04-19 15:50:37.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/brillouins_index.py
--rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/spontanous_alternations.py
--rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/piotr_120324.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/velocity_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/abod.py
--rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1374 2024-04-18 13:56:20.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/violin.py
--rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/simpson_diversity_index.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/clip_videos_by_frm.py
--rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/piotr_120324 4.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1106 2024-04-18 13:46:43.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/rotate image.py
--rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/geometry_ex.py
--rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/line_plot.py
--rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/unsupervised_outliers.py
--rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/statistics_ex.py
--rw-r--r--   0 simon      (501) staff       (20)    16646 2024-04-22 16:43:10.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/sliding_displacement.py
--rw-r--r--   0 simon      (501) staff       (20)     7819 2024-04-18 14:47:28.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/path_plots.py
--rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/wald_wolfowitz.py
--rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/sliding_autoc.py
--rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/linestring_path.py
--rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/cronbach_alpha.py
--rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/mcnamar.py
--rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/AmberFeatureExtractor.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/mosaic.py
--rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/bouts_df
--rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/amber_featurizer.py
--rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/make_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/margalef_diversification_index.py
--rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/biweight_midcorrelation.py
--rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/madmedianrule.py
--rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/adjusted_rand_score.py
--rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.90.7/simba/sandbox/plotly_gantt.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/directing_animals_to_bodypart_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10127 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    22845 2024-04-25 19:50:25.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:27:39.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    19270 2024-03-31 17:21:01.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    11716 2024-04-25 20:20:54.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15819 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10604 2024-04-25 23:58:57.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     8467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/circular_plotting.py
--rw-r--r--   0 simon      (501) staff       (20)    16868 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    10328 2024-04-25 15:48:10.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/ez_path_plot.py
--rw-r--r--   0 simon      (501) staff       (20)    17432 2024-04-17 23:57:27.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    21805 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13623 2024-04-25 20:03:22.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    13509 2024-04-26 00:07:47.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16477 2024-04-25 18:30:53.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14389 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    23459 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    24604 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/spontaneous_alternation_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    21979 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    16926 2024-04-25 19:01:12.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    17513 2024-04-25 19:50:25.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/geometry_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    16661 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/clf_validator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    14224 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    12552 2024-04-25 18:30:28.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    11453 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/circular_feature_overlay_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    14576 2024-02-21 04:11:21.000000 Simba-UW-tf-dev-1.90.7/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.90.7/simba/dash_app/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)    14926 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/spontaneous_alternation_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-21 11:48:06.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/directing_animal_to_bodypart.py
--rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    20617 2024-04-18 21:13:37.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4838 2024-04-25 19:39:11.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/boolean_conditional_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/gibbs_sampler.py
--rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    23782 2024-04-16 15:02:05.000000 Simba-UW-tf-dev-1.90.7/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/model/train_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/model/inference_multiclass_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.90.7/simba/model/grid_search_multiclass_rf.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.90.7/simba/model/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    16987 2024-02-22 11:58:09.000000 Simba-UW-tf-dev-1.90.7/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/model/inference_validation.py
--rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/model/train_multilabel_rf.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)    11198 2024-04-25 19:50:25.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    50018 2024-04-24 14:43:27.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_size_standardizer.py
--rw-r--r--   0 simon      (501) staff       (20)    20511 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    15408 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    12313 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    29612 2024-04-24 14:39:14.000000 Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14268 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/bp_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/no_animals/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/configuration_names/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)   119697 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-26 15:01:23.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/roi_selector_circle.py
--rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    11439 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/roi_selector.py
--rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/roi_selector_polygon.py
--rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/outlier_tools/outlier_corrector_location_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/outlier_tools/outlier_corrector_movement_advanced.py
--rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/outlier_tools/skip_outlier_correction.py
--rw-r--r--   0 simon      (501) staff       (20)    82082 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.7/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.90.7/simba/assets/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/feature_categories/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    10244 2024-04-09 23:07:16.000000 Simba-UW-tf-dev-1.90.7/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.90.7/simba/assets/lookups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/lookups/critical_values_05.pickle
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/lookups/unsupervised_example_x.csv
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.90.7/simba/assets/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.90.7/simba/assets/stl/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/img/splash_2024.mp4
--rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/img/bg_2024.png
--rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.90.7/simba/assets/img/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/img/~$splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/gif.png
--rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/pose.png
--rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/dimensionality_reduction.png
--rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/simba_logo_2.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/readthedocs_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/circle.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/polygon.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/restart.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/add_on.png
--rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/print.png
--rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/concat_icons/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/clean.png
--rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/clf_2.png
--rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/boris.png
--rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/clahe.png
--rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/about.png
--rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/reorganize.png
--rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.7/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/Simba_UW_tf_dev.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-26 00:17:08.000000 Simba-UW-tf-dev-1.90.7/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)    23493 2024-04-26 00:17:08.000000 Simba-UW-tf-dev-1.90.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)       44 2024-04-26 00:17:08.000000 Simba-UW-tf-dev-1.90.7/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-r--r--   0 simon      (501) staff       (20)      797 2024-04-26 00:17:08.000000 Simba-UW-tf-dev-1.90.7/Simba_UW_tf_dev.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        6 2024-04-26 00:17:08.000000 Simba-UW-tf-dev-1.90.7/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2024-04-26 00:17:08.000000 Simba-UW-tf-dev-1.90.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.90.7/LICENSE
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/tests/
--rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.90.7/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.90.7/tests/test_circlular_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.90.7/tests/test_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.7/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.7/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.7/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.90.7/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.7/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4435 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.7/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.7/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8570 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.7/tests/test_video_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.7/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.7/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     3910 2024-04-25 13:56:16.000000 Simba-UW-tf-dev-1.90.7/tests/test_roi_tools.py
--rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.90.7/MANIFEST.in
--rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.90.7/README.md
--rw-r--r--   0 simon      (501) staff       (20)     1426 2024-04-26 00:17:07.000000 Simba-UW-tf-dev-1.90.7/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2024-04-26 00:17:09.000000 Simba-UW-tf-dev-1.90.7/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-28 13:50:53.000000 Simba-UW-tf-dev-1.90.8/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)    11467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-03-29 20:30:28.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1676 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5883 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2873 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8835 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9544 2024-04-26 00:11:08.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4631 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    11362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    25598 2024-04-17 23:32:48.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1184 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6692 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/roi_size_standardizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6997 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4682 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7898 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9048 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8529 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3221 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4231 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8376 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9785 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/spontaneous_alternation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6076 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3437 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3351 2024-04-25 16:26:59.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3468 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9154 2024-04-12 00:32:53.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9235 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10787 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9121 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      584 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9419 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1821 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7312 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6546 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    81527 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7800 2024-04-04 16:47:32.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6160 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4470 2024-04-22 13:59:07.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3622 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6166 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1072 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12174 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4673 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3290 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4134 2024-03-31 17:07:13.000000 Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    16701 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.90.8/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6573 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.8/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14374 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.8/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    14487 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.90.8/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    38871 2024-04-16 13:37:42.000000 Simba-UW-tf-dev-1.90.8/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24423 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     2362 2024-02-21 02:33:04.000000 Simba-UW-tf-dev-1.90.8/simba/labelling/targeted_annotations_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    31269 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)    10012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    15004 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5077 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/cluster_validation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3645 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:33:55.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     9036 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/cluster_video_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     4642 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/cluster_videos_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4027 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/transform_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     5048 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/embedding_correlations_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-02 14:39:26.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4070 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)    11182 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2546 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/data_extractor_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4536 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/cluster_validation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9305 2024-02-15 23:45:22.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/fit_cluster_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2574 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/clusterer_comparison_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     6527 2024-03-26 23:50:53.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     4332 2024-03-28 20:02:59.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/cluster_xai_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     3820 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     2355 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/print_embedding_info_popup.py
+-rw-r--r--   0 simon      (501) staff       (20)     9946 2024-04-02 18:34:25.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12982 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/unsupervised_main.py
+-rw-r--r--   0 simon      (501) staff       (20)    10175 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)    16005 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5241 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/outlier_detector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10397 2024-03-29 16:15:58.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/cluster_frequentist_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5798 2024-03-27 12:56:51.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/embedding_correlation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18194 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/cluster_xai_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15581 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)     5582 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/clusterer_comparison_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4652 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    14765 2024-03-26 19:09:58.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3862 2024-02-15 21:37:53.000000 Simba-UW-tf-dev-1.90.8/simba/unsupervised/tsne.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8511 2024-02-08 00:53:55.000000 Simba-UW-tf-dev-1.90.8/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    27255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    10064 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     7146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    12066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    18436 2024-04-25 18:36:04.000000 Simba-UW-tf-dev-1.90.8/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    57052 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28094 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1757 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2883 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 20:55:52.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 20:55:43.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    36307 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-02-21 02:05:27.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4091 2024-02-16 21:14:07.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    26471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10043 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    61607 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    37328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    31163 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21427 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_4bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    65534 2024-03-01 16:55:51.000000 Simba-UW-tf-dev-1.90.8/simba/feature_extractors/amber_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     1033 2024-04-11 12:52:35.000000 Simba-UW-tf-dev-1.90.8/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    40917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/annotator_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    84153 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/timeseries_features_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-03 14:38:30.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    53232 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    48035 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)    56304 2024-04-17 23:32:32.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/circular_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    38770 2024-04-21 12:08:55.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/network_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    24040 2024-04-18 18:35:47.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3020 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/video_processing_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    36231 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/feature_extraction_supplement_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   169619 2024-04-22 13:26:42.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/statistics_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    44711 2024-04-22 19:40:36.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73186 2024-04-25 23:55:15.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      391 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/abstract_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)    61924 2024-04-21 12:08:55.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/image_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)      880 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   132883 2024-03-29 19:51:46.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)   166028 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/geometry_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    24978 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/mixins/feature_extraction_circular_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6639 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12306 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9739 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5508 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/boris_source_cleaner.py
+-rw-r--r--   0 simon      (501) staff       (20)    18982 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18852 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9215 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     7456 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5662 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     8841 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    14451 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    19237 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15281 2024-04-25 13:46:55.000000 Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    13211 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.90.8/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    26038 2024-03-27 13:42:19.000000 Simba-UW-tf-dev-1.90.8/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10420 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.8/simba/utils/custom_feature_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.90.8/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7737 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.8/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)    52940 2024-04-25 19:17:22.000000 Simba-UW-tf-dev-1.90.8/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    79462 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)    15355 2024-04-16 18:54:43.000000 Simba-UW-tf-dev-1.90.8/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    17086 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    46271 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     4205 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.90.8/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)   243998 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/SimBA_logo.ico
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8626 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5840 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2872 2024-02-15 23:39:58.000000 Simba-UW-tf-dev-1.90.8/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     6313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/
+-rw-r--r--   0 simon      (501) staff       (20)      786 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    29328 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2387 2024-03-08 14:35:02.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/dprime.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-03-18 17:01:43.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/linear_fretchet.py
+-rw-r--r--   0 simon      (501) staff       (20)     2705 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2391 2024-03-14 12:45:59.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/piotr_120324 3.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2036 2024-03-28 18:29:59.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/dunn_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3640 2024-04-08 13:30:56.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)     2689 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    16727 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     3494 2024-04-03 13:42:02.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/colinear_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     8921 2024-03-22 13:56:46.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21658 2024-04-10 16:31:38.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/horizontal_videos_concat.py
+-rw-r--r--   0 simon      (501) staff       (20)     2144 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     1103 2024-03-29 16:26:34.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/silhouette_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     3607 2024-04-09 14:21:58.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/two_fish_feature_extractor_040924.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)    33092 2024-02-22 15:57:45.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/cuda_jit.ipynb
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     1867 2024-03-12 19:23:40.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/directed_hausdorff.py
+-rw-r--r--   0 simon      (501) staff       (20)      963 2024-03-13 18:20:52.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/shannon_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     3726 2024-03-12 13:31:58.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/sequential_lag_analysis.py
+-rw-r--r--   0 simon      (501) staff       (20)     1254 2024-03-13 16:09:50.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/wilcoxon.py
+-rw-r--r--   0 simon      (501) staff       (20)    21599 2024-04-22 16:40:51.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 14:48:22.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3328 2024-03-08 15:05:36.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/data.npy
+-rw-r--r--   0 simon      (501) staff       (20)    12626 2024-03-25 20:59:27.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/distances.py
+-rw-r--r--   0 simon      (501) staff       (20)    26425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     2699 2024-03-10 16:29:57.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/cohens_kappa.py
+-rw-r--r--   0 simon      (501) staff       (20)     2465 2024-03-08 17:38:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/paths.py
+-rw-r--r--   0 simon      (501) staff       (20)     1048 2024-03-13 14:41:23.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/outliers_tietjen.py
+-rw-r--r--   0 simon      (501) staff       (20)     1424 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/train_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     2346 2024-04-19 14:10:16.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/img_stack_to_bw.py
+-rw-r--r--   0 simon      (501) staff       (20)     3171 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/amber_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)     3590 2024-03-11 17:05:31.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/line_locate_point.py
+-rw-r--r--   0 simon      (501) staff       (20)     1841 2024-04-19 16:19:10.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/sorensen_dice_coefficient.py
+-rw-r--r--   0 simon      (501) staff       (20)     3182 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/multifrm_to_points.py
+-rw-r--r--   0 simon      (501) staff       (20)       69 2024-03-18 18:17:24.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/lcs.py
+-rw-r--r--   0 simon      (501) staff       (20)    12448 2024-04-09 14:14:37.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/two_fish_feature_extractor_040924.py
+-rw-r--r--   0 simon      (501) staff       (20)     6119 2024-04-20 17:58:22.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/ez_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     2350 2024-03-12 17:58:33.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/add_body_part.py
+-rw-r--r--   0 simon      (501) staff       (20)     1008 2024-03-12 13:29:20.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/grubbs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     3399 2024-02-16 01:12:37.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/slide_circ_mean.py
+-rw-r--r--   0 simon      (501) staff       (20)     1835 2024-03-28 22:56:59.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/calinski_harabasz.py
+-rw-r--r--   0 simon      (501) staff       (20)     1282 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/roi_feature_visualizer_example.py
+-rw-r--r--   0 simon      (501) staff       (20)    10076 2024-03-22 16:51:40.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/spontaneuous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)      895 2024-03-12 14:09:55.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/runs_test.py
+-rw-r--r--   0 simon      (501) staff       (20)     2516 2024-04-06 11:33:24.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/pct_counts_in_top_N.py
+-rw-r--r--   0 simon      (501) staff       (20)     1095 2024-04-19 18:37:50.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/concordance_ratio.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:46:33.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2287 2024-03-25 16:45:04.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/total_variation_distance.py
+-rw-r--r--   0 simon      (501) staff       (20)     3056 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/crop_single_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)    15977 2024-04-23 22:52:42.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8010 2024-03-24 19:48:22.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/joint_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1529 2024-04-19 15:08:24.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/segment_image_horizontal.py
+-rw-r--r--   0 simon      (501) staff       (20)    11145 2024-04-15 15:02:56.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/clip_multiple_videos_by_frame_numbers.py
+-rw-r--r--   0 simon      (501) staff       (20)     2552 2024-04-02 14:48:59.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/elliptic_envelope.py
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-03-14 14:57:29.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/roi_definition_csvs_to_h5.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1276 2024-03-12 17:58:38.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/add_body_part.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      921 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/roi_feature_visualizer_example.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     2631 2024-04-05 16:23:07.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/sliding_crosscorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     1274 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     2174 2024-03-14 14:56:26.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/roi_definition_csvs_to_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1656 2024-03-30 18:32:44.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/distance_velocity.py
+-rw-r--r--   0 simon      (501) staff       (20)     5011 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5666 2024-04-11 15:28:58.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/line_plot_plotly.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1351 2024-03-26 21:10:40.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/unsupervised_lof.py
+-rw-r--r--   0 simon      (501) staff       (20)     2553 2024-03-11 15:09:38.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/siegel_tukey.py
+-rw-r--r--   0 simon      (501) staff       (20)      958 2024-03-13 18:05:08.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/berger_parker.py
+-rw-r--r--   0 simon      (501) staff       (20)     4177 2024-04-10 01:56:43.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/isolation_forest.py
+-rw-r--r--   0 simon      (501) staff       (20)     2845 2024-03-28 19:23:54.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/davis_bouldin.py
+-rw-r--r--   0 simon      (501) staff       (20)     4094 2024-04-10 14:09:54.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/vertical_video_concatenator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2770 2024-04-07 19:14:13.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/batch_video_to_greyscale.py
+-rw-r--r--   0 simon      (501) staff       (20)     7215 2024-02-26 15:46:14.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/crop_circles_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1410 2024-03-19 12:49:24.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/heading.py
+-rw-r--r--   0 simon      (501) staff       (20)     2243 2024-03-13 18:35:02.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/piotr_120324 2.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)      736 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2907 2024-03-14 19:31:25.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/grangercausalitytests.py
+-rw-r--r--   0 simon      (501) staff       (20)     2432 2024-03-19 20:48:43.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/multiframe_is_shape_covered.py
+-rw-r--r--   0 simon      (501) staff       (20)      592 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/redis.py
+-rw-r--r--   0 simon      (501) staff       (20)     2893 2024-02-26 20:49:33.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     2055 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6186 2024-03-18 12:44:45.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/piotr_120324.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1004 2024-03-12 13:11:45.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/hartley_fmax.py
+-rw-r--r--   0 simon      (501) staff       (20)       84 2024-04-03 17:05:23.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/calc_N_degree_direction_switches.py
+-rw-r--r--   0 simon      (501) staff       (20)     2307 2024-02-27 21:31:33.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/fix_clahe.py
+-rw-r--r--   0 simon      (501) staff       (20)     1836 2024-03-10 15:38:46.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/cochran_q.py
+-rw-r--r--   0 simon      (501) staff       (20)      682 2024-03-13 19:19:43.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/menhinicks_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     2932 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1559 2024-04-19 15:50:37.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/brillouins_index.py
+-rw-r--r--   0 simon      (501) staff       (20)    13575 2024-03-20 11:47:11.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/spontanous_alternations.py
+-rw-r--r--   0 simon      (501) staff       (20)     2268 2024-03-13 13:59:07.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/piotr_120324.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     4655 2024-03-06 18:18:27.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/velocity_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     4478 2024-04-08 20:43:42.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/abod.py
+-rw-r--r--   0 simon      (501) staff       (20)    37024 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1374 2024-04-18 13:56:20.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/violin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1073 2024-03-13 16:46:16.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/simpson_diversity_index.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-04-14 19:07:54.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/clip_videos_by_frm.py
+-rw-r--r--   0 simon      (501) staff       (20)     2396 2024-03-17 16:55:38.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/piotr_120324 4.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1106 2024-04-18 13:46:43.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/rotate image.py
+-rw-r--r--   0 simon      (501) staff       (20)     5336 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/geometry_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)     1613 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1505 2024-03-28 14:36:24.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/line_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)     5515 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15996 2024-04-09 13:41:30.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/unsupervised_outliers.py
+-rw-r--r--   0 simon      (501) staff       (20)     5690 2024-02-10 20:28:08.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/statistics_ex.py
+-rw-r--r--   0 simon      (501) staff       (20)    16646 2024-04-22 16:43:10.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1391 2024-03-18 23:21:46.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/sliding_displacement.py
+-rw-r--r--   0 simon      (501) staff       (20)     7819 2024-04-18 14:47:28.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/path_plots.py
+-rw-r--r--   0 simon      (501) staff       (20)      925 2024-03-11 13:06:04.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/wald_wolfowitz.py
+-rw-r--r--   0 simon      (501) staff       (20)     1814 2024-04-05 14:36:58.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/sliding_autoc.py
+-rw-r--r--   0 simon      (501) staff       (20)     2369 2024-03-14 17:07:10.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/linestring_path.py
+-rw-r--r--   0 simon      (501) staff       (20)     2233 2024-03-18 15:20:48.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/cronbach_alpha.py
+-rw-r--r--   0 simon      (501) staff       (20)     2809 2024-03-08 21:15:58.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/mcnamar.py
+-rw-r--r--   0 simon      (501) staff       (20)    37022 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     6220 2024-02-24 20:57:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/AmberFeatureExtractor.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     1933 2024-04-10 15:09:25.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/mosaic.py
+-rw-r--r--   0 simon      (501) staff       (20)      441 2024-04-12 17:03:24.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/bouts_df
+-rw-r--r--   0 simon      (501) staff       (20)    69423 2024-02-20 14:30:23.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/amber_featurizer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6286 2024-04-17 19:28:51.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/make_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)      837 2024-03-13 18:56:21.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/margalef_diversification_index.py
+-rw-r--r--   0 simon      (501) staff       (20)      997 2024-03-17 17:49:00.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/biweight_midcorrelation.py
+-rw-r--r--   0 simon      (501) staff       (20)     2186 2024-03-18 15:31:23.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/madmedianrule.py
+-rw-r--r--   0 simon      (501) staff       (20)     2915 2024-04-01 14:12:59.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/adjusted_rand_score.py
+-rw-r--r--   0 simon      (501) staff       (20)     2068 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     1957 2024-04-12 14:55:03.000000 Simba-UW-tf-dev-1.90.8/simba/sandbox/plotly_gantt.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8538 2024-02-23 18:25:51.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/directing_animals_to_bodypart_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10127 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:43:56.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5946 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    22833 2024-04-26 11:33:33.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:27:39.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    19270 2024-03-31 17:21:01.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11716 2024-04-25 20:20:54.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15819 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10604 2024-04-25 23:58:57.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8467 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/circular_plotting.py
+-rw-r--r--   0 simon      (501) staff       (20)    16868 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    10328 2024-04-25 15:48:10.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/ez_path_plot.py
+-rw-r--r--   0 simon      (501) staff       (20)    17432 2024-04-17 23:57:27.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21805 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13623 2024-04-25 20:03:22.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    13509 2024-04-26 00:07:47.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5253 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     6517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    20950 2024-04-11 20:25:55.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)     8732 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    10667 2024-04-03 23:24:04.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16477 2024-04-25 18:30:53.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14389 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    23459 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24604 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11824 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13091 2024-03-26 23:49:10.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/spontaneous_alternation_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    21979 2024-04-25 18:18:16.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    16926 2024-04-25 19:01:12.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    17513 2024-04-25 19:50:25.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    10034 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/geometry_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    16661 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/clf_validator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    14224 2024-04-25 18:19:38.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    11994 2024-04-11 22:38:54.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    19073 2024-04-11 20:26:33.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    12552 2024-04-25 18:30:28.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11453 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/circular_feature_overlay_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    14576 2024-02-21 04:11:21.000000 Simba-UW-tf-dev-1.90.8/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:15.000000 Simba-UW-tf-dev-1.90.8/simba/dash_app/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    72715 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     4965 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    47546 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    12720 2024-04-26 10:52:50.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/spontaneous_alternation_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11813 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-21 11:48:06.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    13224 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    39110 2024-03-19 12:54:07.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    10968 2024-02-21 19:10:40.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/directing_animal_to_bodypart.py
+-rw-r--r--   0 simon      (501) staff       (20)     9580 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20617 2024-04-18 21:13:37.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4838 2024-04-25 19:39:11.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/boolean_conditional_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)    15989 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8957 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/gibbs_sampler.py
+-rw-r--r--   0 simon      (501) staff       (20)    10054 2024-04-04 16:23:22.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18517 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3118 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13660 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8738 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)    12919 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10196 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    23782 2024-04-16 15:02:05.000000 Simba-UW-tf-dev-1.90.8/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     4969 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    14036 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/model/train_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/model/inference_multiclass_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    15931 2024-02-20 14:30:06.000000 Simba-UW-tf-dev-1.90.8/simba/model/grid_search_multiclass_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:19.000000 Simba-UW-tf-dev-1.90.8/simba/model/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    16987 2024-02-22 11:58:09.000000 Simba-UW-tf-dev-1.90.8/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3768 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/model/inference_validation.py
+-rw-r--r--   0 simon      (501) staff       (20)     6872 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/model/train_multilabel_rf.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)    11198 2024-04-25 19:50:25.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-25 18:17:26.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    50018 2024-04-24 14:43:27.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3616 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9876 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_size_standardizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    20088 2024-04-26 11:11:36.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    15408 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     4386 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2313 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3716 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    12313 2024-04-25 16:23:13.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11974 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5470 2024-02-21 03:51:46.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    16129 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    29612 2024-04-24 14:39:14.000000 Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)    10711 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:31.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8084 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2577 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-22 19:49:42.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14268 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8161 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-20 21:35:22.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8645 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     7464 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2024-03-19 18:18:43.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:10.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/bp_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4485 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       27 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:18.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/no_animals/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:05.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:47:14.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/configuration_names/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      273 2024-03-04 19:10:54.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    34231 2024-02-20 18:50:39.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)   119697 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-03-26 15:01:23.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     5577 2024-04-08 11:29:52.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/roi_selector_circle.py
+-rw-r--r--   0 simon      (501) staff       (20)     9073 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    35053 2024-02-26 15:42:07.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    11439 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     3066 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6598 2024-02-26 21:50:01.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/roi_selector.py
+-rw-r--r--   0 simon      (501) staff       (20)    10007 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     5963 2024-02-27 21:31:05.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/roi_selector_polygon.py
+-rw-r--r--   0 simon      (501) staff       (20)     4926 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    15117 2024-04-11 20:42:04.000000 Simba-UW-tf-dev-1.90.8/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7837 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14462 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/outlier_tools/outlier_corrector_location_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    13117 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/outlier_tools/outlier_corrector_movement_advanced.py
+-rw-r--r--   0 simon      (501) staff       (20)    10396 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/outlier_tools/skip_outlier_correction.py
+-rw-r--r--   0 simon      (501) staff       (20)    82082 2024-04-15 18:43:27.000000 Simba-UW-tf-dev-1.90.8/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:36.000000 Simba-UW-tf-dev-1.90.8/simba/assets/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:25.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/feature_categories/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:21.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2024-04-09 23:07:16.000000 Simba-UW-tf-dev-1.90.8/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:11.000000 Simba-UW-tf-dev-1.90.8/simba/assets/lookups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    26256 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/lookups/critical_values_05.pickle
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/lookups/unsupervised_example_x.csv
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:41:54.000000 Simba-UW-tf-dev-1.90.8/simba/assets/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:31.000000 Simba-UW-tf-dev-1.90.8/simba/assets/stl/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)   489479 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/img/splash_2024.mp4
+-rw-r--r--   0 simon      (501) staff       (20)    79863 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/img/bg_2024.png
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:45:02.000000 Simba-UW-tf-dev-1.90.8/simba/assets/img/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      165 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/img/~$splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/gif.png
+-rw-r--r--   0 simon      (501) staff       (20)     4566 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/pose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1943 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2024-04-09 15:42:22.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     4896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/dimensionality_reduction.png
+-rw-r--r--   0 simon      (501) staff       (20)     4823 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)   171446 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/simba_logo_2.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)    59896 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/readthedocs_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1921 2024-02-26 14:29:54.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/circle.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:37.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)     1148 2024-02-26 20:39:14.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/polygon.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/restart.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/add_on.png
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/print.png
+-rw-r--r--   0 simon      (501) staff       (20)     4653 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)        0 2024-02-07 19:44:45.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/concat_icons/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/clean.png
+-rw-r--r--   0 simon      (501) staff       (20)     4725 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/clf_2.png
+-rw-r--r--   0 simon      (501) staff       (20)     4795 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/boris.png
+-rw-r--r--   0 simon      (501) staff       (20)     4804 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/clahe.png
+-rw-r--r--   0 simon      (501) staff       (20)     4637 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/about.png
+-rw-r--r--   0 simon      (501) staff       (20)     4666 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/reorganize.png
+-rw-r--r--   0 simon      (501) staff       (20)     4784 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2024-02-07 18:56:19.000000 Simba-UW-tf-dev-1.90.8/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/Simba_UW_tf_dev.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2797 2024-04-26 11:34:36.000000 Simba-UW-tf-dev-1.90.8/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)    23493 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)       44 2024-04-26 11:34:36.000000 Simba-UW-tf-dev-1.90.8/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-r--r--   0 simon      (501) staff       (20)      797 2024-04-26 11:34:36.000000 Simba-UW-tf-dev-1.90.8/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        6 2024-04-26 11:34:36.000000 Simba-UW-tf-dev-1.90.8/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2024-04-26 11:34:36.000000 Simba-UW-tf-dev-1.90.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)    35127 2024-02-07 18:56:10.000000 Simba-UW-tf-dev-1.90.8/LICENSE
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     4753 2024-04-11 20:40:04.000000 Simba-UW-tf-dev-1.90.8/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)    13415 2024-03-01 16:43:04.000000 Simba-UW-tf-dev-1.90.8/tests/test_circlular_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    13399 2024-04-11 20:36:51.000000 Simba-UW-tf-dev-1.90.8/tests/test_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    11863 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.8/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6525 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.8/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1739 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.8/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8120 2024-03-01 19:06:25.000000 Simba-UW-tf-dev-1.90.8/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1070 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.8/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4435 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.8/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1596 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.8/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8570 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.8/tests/test_video_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     3554 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.8/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3021 2024-02-07 18:56:20.000000 Simba-UW-tf-dev-1.90.8/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     3910 2024-04-25 13:56:16.000000 Simba-UW-tf-dev-1.90.8/tests/test_roi_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)      318 2024-03-04 20:16:28.000000 Simba-UW-tf-dev-1.90.8/MANIFEST.in
+-rw-r--r--   0 simon      (501) staff       (20)    18478 2024-04-17 19:58:21.000000 Simba-UW-tf-dev-1.90.8/README.md
+-rw-r--r--   0 simon      (501) staff       (20)     1426 2024-04-26 11:34:35.000000 Simba-UW-tf-dev-1.90.8/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2024-04-26 11:34:37.000000 Simba-UW-tf-dev-1.90.8/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.90.7/PKG-INFO` & `Simba-UW-tf-dev-1.90.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.90.7
+Version: 1.90.8
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/targeted_annotation_clips_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/roi_size_standardizer_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/roi_size_standardizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/spontaneous_alternation_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/spontaneous_alternation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/boolean_conditional_slicer_pup_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/directing_animal_to_bodypart_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/direction_animal_to_bodypart_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.90.8/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.90.8/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/labelling/targeted_annotations_clips.py` & `Simba-UW-tf-dev-1.90.8/simba/labelling/targeted_annotations_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.90.8/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.90.8/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.90.8/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/cluster_validation_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/cluster_validation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/cluster_video_visualizer.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/cluster_video_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/cluster_videos_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/cluster_videos_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/transform_cluster_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/transform_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/embedding_correlations_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/embedding_correlations_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/transform_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/fit_dim_reduction_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/data_extractor_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/data_extractor_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/cluster_validation_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/cluster_validation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/fit_cluster_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/fit_cluster_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/clusterer_comparison_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/clusterer_comparison_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/grid_search_visualizer_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/cluster_xai_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/cluster_xai_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/cluster_frequentist_stats_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/pop_ups/print_embedding_info_popup.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/pop_ups/print_embedding_info_popup.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/unsupervised_main.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/unsupervised_main.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/outlier_detector.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/outlier_detector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/cluster_frequentist_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/cluster_frequentist_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/embedding_correlation_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/embedding_correlation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/cluster_xai_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/cluster_xai_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/clusterer_comparison_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/clusterer_comparison_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.90.8/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.90.8/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.90.8/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.90.8/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.90.8/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.90.8/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/feature_extractors/amber_feature_extractor.py` & `Simba-UW-tf-dev-1.90.8/simba/feature_extractors/amber_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/requirements.txt` & `Simba-UW-tf-dev-1.90.8/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/annotator_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/annotator_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/timeseries_features_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/timeseries_features_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/circular_statistics.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/circular_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/network_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/network_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/feature_extraction_supplement_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/feature_extraction_supplement_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/statistics_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/statistics_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/image_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/image_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/geometry_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/geometry_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/mixins/feature_extraction_circular_mixin.py` & `Simba-UW-tf-dev-1.90.8/simba/mixins/feature_extraction_circular_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/boris_source_cleaner.py` & `Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/boris_source_cleaner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.90.8/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.90.8/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.90.8/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/utils/enums.py` & `Simba-UW-tf-dev-1.90.8/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/utils/custom_feature_extractor.py` & `Simba-UW-tf-dev-1.90.8/simba/utils/custom_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.90.8/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/utils/checks.py` & `Simba-UW-tf-dev-1.90.8/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.90.8/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.90.8/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.90.8/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/utils/errors.py` & `Simba-UW-tf-dev-1.90.8/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/utils/data.py` & `Simba-UW-tf-dev-1.90.8/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/utils/printing.py` & `Simba-UW-tf-dev-1.90.8/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/SimBA_logo.ico` & `Simba-UW-tf-dev-1.90.8/simba/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/doctests.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/dprime.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/dprime.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/linear_fretchet.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/linear_fretchet.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/read_in_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/piotr_120324 3.py.zip` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/piotr_120324 3.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/dunn_index.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/dunn_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/hausdorff.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/peaks.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/colinear_features.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/colinear_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/spontaneous_alternation_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/horizontal_videos_concat.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/horizontal_videos_concat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/silhouette_score.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/silhouette_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/two_fish_feature_extractor_040924.py.zip` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/two_fish_feature_extractor_040924.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/cuda_jit.ipynb` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/cuda_jit.ipynb`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/directed_hausdorff.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/directed_hausdorff.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/shannon_diversity_index.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/shannon_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/sequential_lag_analysis.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/sequential_lag_analysis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/wilcoxon.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/wilcoxon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/data.npy` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/data.npy`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/distances.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/distances.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/cohens_kappa.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/cohens_kappa.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/paths.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/paths.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/outliers_tietjen.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/outliers_tietjen.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/train_model.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/train_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/img_stack_to_bw.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/img_stack_to_bw.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/amber_tests.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/amber_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/line_locate_point.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/line_locate_point.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/sorensen_dice_coefficient.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/sorensen_dice_coefficient.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/multifrm_to_points.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/multifrm_to_points.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/two_fish_feature_extractor_040924.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/two_fish_feature_extractor_040924.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/ez_path_plot.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/ez_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/add_body_part.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/add_body_part.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/grubbs_test.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/grubbs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/slide_circ_mean.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/slide_circ_mean.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/calinski_harabasz.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/calinski_harabasz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/roi_feature_visualizer_example.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/roi_feature_visualizer_example.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/spontaneuous_alternation_plotter.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/spontaneuous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/runs_test.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/runs_test.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/pct_counts_in_top_N.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/pct_counts_in_top_N.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/concordance_ratio.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/concordance_ratio.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/total_variation_distance.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/total_variation_distance.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/crop_single_polygon.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/crop_single_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/ROI_analyzer.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/joint_plotter.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/joint_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/segment_image_horizontal.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/segment_image_horizontal.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/clip_multiple_videos_by_frame_numbers.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/clip_multiple_videos_by_frame_numbers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/elliptic_envelope.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/elliptic_envelope.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/roi_definition_csvs_to_h5.py.zip` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/roi_definition_csvs_to_h5.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/add_body_part.py.zip` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/add_body_part.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/roi_feature_visualizer_example.py.zip` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/roi_feature_visualizer_example.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/sliding_crosscorrelation.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/sliding_crosscorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/count_values_in_range.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/roi_definition_csvs_to_h5.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/roi_definition_csvs_to_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/distance_velocity.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/distance_velocity.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/graph_creator.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/line_plot_plotly.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/line_plot_plotly.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/termite_rois.csv` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/unsupervised_lof.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/unsupervised_lof.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/siegel_tukey.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/siegel_tukey.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/berger_parker.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/berger_parker.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/isolation_forest.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/isolation_forest.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/davis_bouldin.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/davis_bouldin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/vertical_video_concatenator.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/vertical_video_concatenator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/batch_video_to_greyscale.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/batch_video_to_greyscale.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/crop_circles_pop_up.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/crop_circles_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/heading.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/heading.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/piotr_120324 2.py.zip` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/piotr_120324 2.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/mutual_exclusive.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/grangercausalitytests.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/grangercausalitytests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/multiframe_is_shape_covered.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/multiframe_is_shape_covered.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/redis.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/redis.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/video_color.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/piotr_120324.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/piotr_120324.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/video_rotator.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/hartley_fmax.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/hartley_fmax.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/fix_clahe.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/fix_clahe.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/cochran_q.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/cochran_q.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/menhinicks_index.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/menhinicks_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/brillouins_index.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/brillouins_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/spontanous_alternations.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/spontanous_alternations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/piotr_120324.py.zip` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/piotr_120324.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/velocity_aggregator.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/velocity_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/make_splash.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/abod.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/abod.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/violin.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/violin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/simpson_diversity_index.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/simpson_diversity_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/clip_videos_by_frm.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/clip_videos_by_frm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/piotr_120324 4.py.zip` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/piotr_120324 4.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/rotate image.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/rotate image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/geometry_ex.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/geometry_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/line_plot.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/line_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/video_rotator_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/unsupervised_outliers.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/unsupervised_outliers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/statistics_ex.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/statistics_ex.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/ROI_plotter.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/sliding_displacement.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/sliding_displacement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/path_plots.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/path_plots.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/wald_wolfowitz.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/wald_wolfowitz.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/sliding_autoc.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/sliding_autoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/linestring_path.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/linestring_path.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/cronbach_alpha.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/cronbach_alpha.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/mcnamar.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/mcnamar.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/AmberFeatureExtractor.py.zip` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/AmberFeatureExtractor.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/mosaic.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/mosaic.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/amber_featurizer.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/amber_featurizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/make_path_plot.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/make_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/margalef_diversification_index.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/margalef_diversification_index.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/biweight_midcorrelation.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/biweight_midcorrelation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/madmedianrule.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/madmedianrule.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/adjusted_rand_score.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/adjusted_rand_score.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/sandbox/plotly_gantt.py` & `Simba-UW-tf-dev-1.90.8/simba/sandbox/plotly_gantt.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/directing_animals_to_bodypart_visualizer.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/directing_animals_to_bodypart_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/ROI_plotter_mp.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,17 +141,17 @@
     def __init__(self,
                  config_path: Union[str, os.PathLike],
                  video_path: Union[str, os.PathLike],
                  body_parts: List[str],
                  style_attr: Dict[str, bool],
                  threshold: Optional[float] = 0.0,
                  core_cnt: Optional[int] = -1):
-        #
-        if platform.system() == "Darwin":
-            multiprocessing.set_start_method("spawn", force=True)
+
+        # if platform.system() == "Darwin":
+        #     multiprocessing.set_start_method("spawn", force=True)
         check_float(name=f'{self.__class__.__name__} threshold', value=threshold, min_value=0.0, max_value=1.0)
         check_int(name=f'{self.__class__.__name__} core_cnt', value=core_cnt, min_value=-1)
         if core_cnt == -1: core_cnt = find_core_cnt()[0]
         check_if_keys_exist_in_dict(data=style_attr, key=STYLE_KEYS, name=f'{self.__class__.__name__} style_attr')
         check_file_exist_and_readable(file_path=video_path)
         _, self.video_name, _ = get_fn_ext(video_path)
         ConfigReader.__init__(self, config_path=config_path)
@@ -240,15 +240,15 @@
 
 
     def __create_shape_dicts(self):
         shape_dicts = {}
         for shape, df in self.roi_dict.items():
             if not df["Name"].is_unique:
                 df = df.drop_duplicates(subset=["Name"], keep="first")
-                DuplicateNamesWarning(f'Some of your ROIs with the same shape ({shape}) has the same names for video {self.video_name}. E.g., you have two rectangles named "My rectangle". SimBA prefers ROI shapes with unique names. SimBA will keep one of the unique shape names and drop the rest.', source=self.__class__.__name__)
+                DuplicateNamesWarning(msg=f'Some of your ROIs with the same shape ({shape}) has the same names for video {self.video_name}. E.g., you have two rectangles named "My rectangle". SimBA prefers ROI shapes with unique names. SimBA will keep one of the unique shape names and drop the rest.', source=self.__class__.__name__)
             d = df.set_index("Name").to_dict(orient="index")
             shape_dicts = {**shape_dicts, **d}
         return shape_dicts
 
     def __get_bordered_img_size(self) -> Tuple[int, int]:
         cap = cv2.VideoCapture(self.video_path)
         cap.set(1, 1)
@@ -271,15 +271,15 @@
         self.shape_dicts = self.__create_shape_dicts()
         self.__calculate_cumulative()
         check_video_and_data_frm_count_align(video=self.video_path, data=self.data_df, name=self.video_name, raise_error=False)
         data_lst = np.array_split(self.data_df.fillna(0), self.core_cnt)
         for cnt in range(len(data_lst)):
             data_lst[cnt]["group"] = cnt
 
-        print(f"Creating ROI images, multiprocessing (determined chunksize: {self.multiprocess_chunksize}, cores: {self.core_cnt})...")
+        print(f"Creating ROI images, multiprocessing (chunksize: {self.multiprocess_chunksize}, cores: {self.core_cnt})...")
         del self.roi_analyzer.logger
         with multiprocessing.Pool(self.core_cnt, maxtasksperchild=self.maxtasksperchild) as pool:
             constants = functools.partial(_roi_plotter_mp,
                                           loc_dict=self.loc_dict,
                                           scalers=self.scalers,
                                           video_meta_data=self.video_meta_data,
                                           save_temp_directory=self.temp_folder,
```

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/circular_plotting.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/circular_plotting.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/ez_path_plot.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/ez_path_plot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/spontaneous_alternation_plotter.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/spontaneous_alternation_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/geometry_plotter.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/geometry_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/clf_validator_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/clf_validator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/circular_feature_overlay_plotter.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/circular_feature_overlay_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.90.8/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.90.8/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.90.8/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.90.8/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/spontaneous_alternation_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/severity_bout_based_calculator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,315 +1,295 @@
-import argparse
+__author__ = "Simon Nilsson"
+
 import os
-import warnings
-from typing import List, Optional, Union
+from datetime import datetime
+from typing import Dict, List, Union
 
+import cv2
 import numpy as np
 import pandas as pd
 
-warnings.filterwarnings("ignore")
-
-import multiprocessing
-import platform
-
 from simba.mixins.config_reader import ConfigReader
-from simba.mixins.feature_extraction_supplement_mixin import \
-    FeatureExtractionSupplemental
-from simba.mixins.geometry_mixin import GeometryMixin
-from simba.utils.checks import (check_file_exist_and_readable, check_float,
-                                check_if_dir_exists, check_int, check_str,
-                                check_valid_lst, check_video_has_rois)
-from simba.utils.errors import (AnimalNumberError, InvalidInputError,
-                                NoFilesFoundError)
-from simba.utils.printing import stdout_success
-from simba.utils.read_write import (get_file_name_info_in_directory,
-                                    get_fn_ext, read_df)
-from simba.utils.warnings import NoFileFoundWarning
+from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
+from simba.utils.checks import (check_if_filepath_list_is_empty,
+                                check_that_column_exist)
+from simba.utils.data import create_color_palettes, detect_bouts, find_bins
+from simba.utils.errors import InvalidVideoFileError
+from simba.utils.printing import SimbaTimer, stdout_success
+from simba.utils.read_write import get_fn_ext, get_video_meta_data, read_df
+from simba.utils.warnings import NoDataFoundWarning
 
-TAIL_END = "tail_end"
 
-
-class SpontaneousAlternationCalculator(ConfigReader):
+class SeverityBoutCalculator(ConfigReader, FeatureExtractionMixin):
     """
-    Compute spontaneous alternations based on specified ROIs and animal detection parameters.
+    Computes the "severity" of classification bout events based on how much
+    the animals are moving within the bout. Bouts are scored as less or more severe at lower and higher movements, respectively.
+
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter dict settings: how to calculate the severity. E.g., {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'normalization': 'ALL VIDEOS', 'save_bin_definitions': True, 'visualize': True, 'visualize_event_cnt': 'ALL', 'video_speed': 1.0, 'show_pose': True}
 
     .. note::
-       This method computes spontaneous alternation by fitting the smallest viable geometry (a.k.a. shape, polygon) that
-       encompasses the animal key-points (but see buffer parameter below). It then checks the percent overlap between the
-       animal geometry and the defined arm and center geometries in each frame. If the percent overlap is more or equal to the
-       specified threshold, then the animal considered to visiting the relevant arm. The animal is considered exiting an arm
-       when the percent overlap with a different ROI is above the threshold.
-
-    .. attention::
-       Requires SimBA project with (i) only one tracked animal, (ii) at least three pose-estmated body-parts, and (iii) defined
-       ROIs representing the arms and the center of the maze.
-
-    :param Union[str, os.PathLike] config_path: Path to SimBA project config file.
-    :param List[str] arm_names: List of ROI names representing the arms.
-    :param str center_name: Name of the ROI representing the center of the maze
-    :param Optional[int] animal_area: Value between 51 and 100, representing the percent of the animal body that has to be situated in a ROI for it to be considered an entry.
-    :param Optional[float] threshold: Value between 0.0 and 1.0. Body-parts with detection probabilities below this value will be (if possible) filtered when constructing the animal geometry.
-    :param Optional[int] buffer: Millimeters area for which the animal geometry should be increased in size. Useful if the animal geometry does not fully cover the animal.
-    :param Optional[bool] detailed_data: If True, saves an additional CSV for each analyzed video with detailed data pertaining each error type and alternation sequence.
-    :param Optional[Union[str, os.PathLike]] data_path: Directory of path to the file to be analyzed. If None, then ``project_folder/outlier_corrected_movement_location`` directory.
-
-    :example:
-    >>> x = SpontaneousAlternationCalculator(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/spontenous_alternation/project_folder/project_config.ini', arm_names=['A', 'B', 'C'], center_name='Center', threshold=0.0, animal_area=100, buffer=2, detailed_data=True)
-    >>> x.run()
-    >>> x.save()
-    """
+       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md>`__.
 
-    def __init__(
-        self,
-        config_path: Union[str, os.PathLike],
-        arm_names: List[str],
-        center_name: str,
-        animal_area: Optional[int] = 80,
-        threshold: Optional[float] = 0.0,
-        buffer: Optional[int] = 2,
-        verbose: Optional[bool] = False,
-        detailed_data: Optional[bool] = False,
-        data_path: Optional[Union[str, os.PathLike]] = None,
-    ):
+    Examples
+    ----------
+    >>> settings = {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'normalization': 'ALL VIDEOS', 'save_bin_definitions': True, 'visualize': True, 'visualize_event_cnt': 'ALL', 'video_speed': 1.0, 'show_pose': True}
+    >>> processor = SeverityBoutCalculator(config_path='project_folder/project_config.ini', settings=settings)
+    >>> processor.run()
+    >>> processor.save()
+    """
 
+    def __init__(self, config_path: Union[str, os.PathLike], settings: Dict):
         ConfigReader.__init__(self, config_path=config_path)
-        if self.animal_cnt != 1:
-            raise AnimalNumberError(
-                msg=f"Spontaneous alternation can only be calculated in 1 animal projects. Your project has {self.animal_cnt} animals.",
-                source=self.__class__.__name__,
-            )
-        if len(self.body_parts_lst) < 3:
-            raise InvalidInputError(
-                msg=f"Spontaneous alternation can only be calculated in projects with 3 or more tracked body-parts. Found {len(self.body_parts_lst)}.",
-                source=self.__class__.__name__,
-            )
-        check_valid_lst(
-            data=arm_names,
-            source=SpontaneousAlternationCalculator.__name__,
-            valid_dtypes=(str,),
-            min_len=2,
-        )
-        check_str(name="CENTER NAME", value=center_name)
-        check_int(name="ANIMAL AREA", value=animal_area, min_value=51, max_value=100)
-        check_float(name="THRESHOLD", value=threshold, min_value=0.0, max_value=1.0)
-        check_int(name="BUFFER", value=buffer, min_value=1)
-        if data_path is None:
-            data_path = self.outlier_corrected_dir
-            file_paths = get_file_name_info_in_directory(
-                directory=data_path, file_type=self.file_type
-            )
-        elif os.path.isdir(data_path):
-            check_if_dir_exists(in_dir=data_path)
-            file_paths = get_file_name_info_in_directory(
-                directory=data_path, file_type=self.file_type
-            )
-        else:
-            check_file_exist_and_readable(file_path=data_path)
-            file_paths = {get_fn_ext(filepath=data_path)[1]: data_path}
-
-        self.read_roi_data()
-        files_w_missing_rois = list(
-            set(file_paths.keys()) - set(self.video_names_w_rois)
+        self.settings = settings
+        self.movement_animal_bp_dict = {
+            k: self.animal_bp_dict[k] for k in self.settings["animals"]
+        }
+        self.color_lst_lst = create_color_palettes(
+            no_animals=len(list(self.animal_bp_dict.keys())),
+            map_size=len(self.bp_headers),
         )
-        self.files_w_rois = [
-            x for x in list(file_paths.keys()) if x in self.video_names_w_rois
-        ]
-        if len(self.files_w_rois) == 0:
-            raise NoFilesFoundError(
-                msg=f"No ROI definitions found for any of the data fat {arm_names}",
-                source=__class__.__name__,
-            )
-        if len(files_w_missing_rois) > 0:
-            NoFileFoundWarning(
-                msg=f"{len(files_w_missing_rois)} file(s) at {data_path} are missing ROI definitions and will be skipped when performing spontaneous alternation calculations: {files_w_missing_rois}",
-                source=__class__.__name__,
-            )
-        check_video_has_rois(
-            roi_dict=self.roi_dict,
-            video_names=self.files_w_rois,
-            roi_names=arm_names + [center_name],
+        check_if_filepath_list_is_empty(
+            filepaths=self.machine_results_paths,
+            error_msg=f"SIMBA ERROR: Cannot process severity. {self.machine_results_dir} directory is empty",
         )
-        self.file_paths = list(
-            {file_paths[k] for k in self.files_w_rois if k in file_paths}
+        save_name = os.path.join(
+            f'severity_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv'
         )
-        self.threshold, self.buffer, self.animal_area, self.detailed_data = (
-            threshold,
-            buffer,
-            animal_area,
-            detailed_data,
+        definitions_save_name = os.path.join(
+            f'severity_bin_definitions_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv'
         )
-        self.verbose, self.center_name, self.arm_names = verbose, center_name, arm_names
+        self.save_path = os.path.join(self.logs_path, save_name)
+        self.definitions_path, self.fourcc = os.path.join(
+            self.logs_path, definitions_save_name
+        ), cv2.VideoWriter_fourcc(*"mp4v")
+
+    def __calculate_movements(self, data_paths: List[str]):
+        movements = {}
+        for file_cnt, file_path in enumerate(data_paths):
+            _, video_name, _ = get_fn_ext(file_path)
+            print(
+                f"Analyzing movements in {video_name} ({file_cnt+1}/{len(data_paths)})..."
+            )
+            _, px_per_mm, fps = self.read_video_info(video_name=video_name)
+            df = read_df(file_path=file_path, file_type=self.file_type)
+            if self.settings["clf"] not in df.columns:
+                NoDataFoundWarning(
+                    msg=f'Skipping file {video_name} - {self.settings["clf"]} data not present in file'
+                )
+                continue
+            video_movement = np.full((len(df)), 0)
+            for animal_name, animal_bodyparts in self.movement_animal_bp_dict.items():
+                animal_df = df[animal_bodyparts["X_bps"] + animal_bodyparts["Y_bps"]]
+                animal_df = self.create_shifted_df(df=animal_df)
+                for bp_x, bp_y in zip(
+                    animal_bodyparts["X_bps"], animal_bodyparts["Y_bps"]
+                ):
+                    video_movement = np.add(
+                        video_movement,
+                        self.euclidean_distance(
+                            animal_df[bp_x].values,
+                            animal_df[f"{bp_x}_shifted"].values,
+                            animal_df[bp_y].values,
+                            animal_df[f"{bp_y}_shifted"].values,
+                            px_per_mm,
+                        ),
+                    )
+            movements[video_name] = video_movement
+        return movements
 
     def run(self):
-        roi_geos, self.roi_clrs = GeometryMixin.simba_roi_to_geometries(
-            rectangles_df=self.rectangles_df,
-            circles_df=self.circles_df,
-            polygons_df=self.polygon_df,
-            color=True,
+        movements = self.__calculate_movements(data_paths=self.machine_results_paths)
+        video_bins_info = find_bins(
+            data=movements,
+            bracket_type=self.settings["bracket_type"],
+            bracket_cnt=self.settings["brackets"],
+            normalization_method=self.settings["normalization"],
         )
-        self.roi_geos = {k: v for k, v in roi_geos.items() if k in self.files_w_rois}
-        self.results = {}
-        for file_path in self.file_paths:
-            _, self.video_name, _ = get_fn_ext(filepath=file_path)
-            _, px_per_mm, fps = self.read_video_info(video_name=self.video_name)
-
-            self.data_df = read_df(file_path=file_path, file_type=self.file_type)
-            bp_df = self.data_df[
-                [
-                    x
-                    for x in self.bp_headers
-                    if not x.endswith("_p") and not TAIL_END in x.lower()
-                ]
-            ]
-            p_df = self.data_df[
-                [
-                    x
-                    for x in self.bp_headers
-                    if x.endswith("_p") and not TAIL_END in x.lower()
-                ]
+        self.results = pd.DataFrame(
+            columns=[
+                "VIDEO",
+                "EVENT",
+                "START TIME",
+                "END TIME",
+                "START FRAME",
+                "END FRAME",
+                "BOUT TIME",
+                "MOVEMENT",
+                "SEVERITY",
             ]
-            bp_arr = bp_df.values.reshape(
-                len(bp_df), int(len(bp_df.columns) / 2), 2
-            ).astype(np.int64)
-            p_arr = p_df.values.reshape(len(p_df), len(p_df.columns), 1)
-            if self.threshold > 0.0:
-                bp_arr = GeometryMixin.filter_low_p_bps_for_shapes(
-                    x=bp_arr, p=p_arr, threshold=self.threshold
-                ).reshape(bp_arr.shape[0], -1, 2)
-            self.animal_polygons = GeometryMixin().multiframe_bodyparts_to_polygon(
-                data=bp_arr,
-                parallel_offset=self.buffer,
-                pixels_per_mm=px_per_mm,
-                video_name=self.video_name,
-                animal_name="Animal",
-                verbose=self.verbose,
+        )
+        for file_cnt, file_path in enumerate(self.machine_results_paths):
+            _, video_name, _ = get_fn_ext(file_path)
+            _, px_per_mm, fps = self.read_video_info(video_name=video_name)
+            df = read_df(file_path=file_path, file_type=self.file_type)
+            check_that_column_exist(
+                df=df, column_name=self.settings["clf"], file_name=file_path
             )
-            self.roi_df = pd.DataFrame()
-            for geo_name, geo in self.roi_geos[self.video_name].items():
-                roi_geo = [geo for x in range(len(self.animal_polygons))]
-                pct_overlap = np.array(
-                    GeometryMixin().multiframe_compute_pct_shape_overlap(
-                        shape_1=self.animal_polygons,
-                        shape_2=roi_geo,
-                        denominator="shape_1",
-                        verbose=self.verbose,
-                        animal_names=geo_name,
-                        video_name=self.video_name,
-                    )
-                )
-                frames_in_roi = np.zeros(pct_overlap.shape)
-                frames_in_roi[np.argwhere(pct_overlap >= self.animal_area)] = 1
-                self.roi_df[geo_name] = frames_in_roi
-
-            self.video_results = FeatureExtractionSupplemental.spontaneous_alternations(
-                data=self.roi_df, arm_names=self.arm_names, center_name=self.center_name
+            bout_df = detect_bouts(
+                data_df=df, target_lst=[self.settings["clf"]], fps=fps
             )
-            self.results[self.video_name] = self.video_results
+            bout_df.columns = [
+                "EVENT",
+                "START TIME",
+                "END TIME",
+                "START FRAME",
+                "END FRAME",
+                "BOUT TIME",
+            ]
+            severity_lst, movement_lst = [], []
+            if len(bout_df) > 0:
+                for i in bout_df[["START FRAME", "END FRAME"]].values:
+                    bout_move_val = np.mean(movements[video_name][i[0] : i[1]])
+                    if bout_move_val >= video_bins_info[video_name][-1][1]:
+                        severity_lst.append(self.settings["brackets"])
+                        movement_lst.append(bout_move_val)
+                    else:
+                        for j_cnt, j in enumerate(video_bins_info[video_name]):
+                            if j[0] <= bout_move_val <= j[1]:
+                                severity_lst.append(j_cnt + 1)
+                                movement_lst.append(round(bout_move_val, 4))
+                bout_df["MOVEMENT"] = movement_lst
+                bout_df["SEVERITY"] = severity_lst
+                bout_df.insert(0, "VIDEO", video_name)
+                self.results = pd.concat([self.results, bout_df], axis=0).reset_index(
+                    drop=True
+                )
+        self.save()
+        if self.settings["save_bin_definitions"]:
+            self.save_bin_definitions(data=video_bins_info)
+        if self.settings["visualize"]:
+            self.visualize()
 
     def save(self):
-        print("Running alternation analysis...")
-        results_df = pd.DataFrame(
-            columns=[
-                "VIDEO NAME",
-                "ALTERNATION RATE",
-                "ALTERNATION COUNT",
-                "ERROR COUNT",
-                "SAME ARM RETURN ERRORS",
-                "ALTERNATE ARM RETURN ERRORS",
-            ]
+        self.results.to_csv(self.save_path)
+        self.timer.stop_timer()
+        stdout_success(
+            msg=f"Bout severity data saved at {self.save_path}",
+            elapsed_time=self.timer.elapsed_time_str,
         )
+
+    def save_bin_definitions(self, data=dict):
+        results = pd.DataFrame(columns=["VIDEO", "SEVERITY_BIN", ">=", "<"])
+        for video_name, video_bins in data.items():
+            for bin_cnt, video_bin in enumerate(video_bins):
+                results.loc[len(results)] = [
+                    video_name,
+                    bin_cnt + 1,
+                    video_bin[0],
+                    video_bin[1],
+                ]
         save_path = os.path.join(
-            self.logs_path, f"spontaneous_alternation_{self.datetime}.csv"
-        )
-        for video_name, d in self.results.items():
-            results_df.loc[len(results_df)] = [
-                video_name,
-                d["pct_alternation"],
-                d["alternation_cnt"],
-                d["error_cnt"],
-                d["same_arm_returns_cnt"],
-                d["alternate_arm_returns_cnt"],
-            ]
-        results_df.set_index("VIDEO NAME").to_csv(save_path)
-        stdout_success(
-            msg=f"Spontaneous alternation data for {len(list(self.results.keys()))} video(s) saved at {save_path}"
+            self.logs_path, f"severity_bin_definitions_{self.datetime}.csv"
         )
-        if self.detailed_data:
-            save_dir = os.path.join(
-                self.logs_path, f"detailed_spontaneous_alternation_data_{self.datetime}"
+        results.to_csv(save_path)
+        stdout_success(msg=f"Severity bracket definitions saved at {save_path}")
+
+    def visualize(self):
+        if self.settings["visualize_event_cnt"] == "ALL CLIPS":
+            self.settings["visualize_event_cnt"] = len(self.results)
+        elif self.settings["visualize_event_cnt"] > len(self.results):
+            self.settings["visualize_event_cnt"] = len(self.results)
+            print(
+                f'User specified {self.settings["visualize_event_cnt"]} visualization but only {len(self.results)} bouts where found. Creating {len(self.results)} videos...'
             )
-            sliced_keys = [
-                "same_arm_returns_dict",
-                "alternate_arm_returns_dict",
-                "alternations_dict",
-            ]
-            replace_keys = {
-                "same_arm_returns_dict": "same arm return",
-                "alternate_arm_returns_dict": "alternate arm return",
-                "alternations_dict": "alternations",
-            }
+        video_timer, save_dir = SimbaTimer(start=True), os.path.join(
+            self.project_path, "frames", "output", "severity_bouts"
+        )
+        if not os.path.exists(save_dir):
             os.makedirs(save_dir)
-            for video_name, d in self.results.items():
-                save_path = os.path.join(save_dir, f"{video_name}.csv")
-                sliced_data = {k: v for k, v in d.items() if k in sliced_keys}
-                sliced_data = {
-                    replace_keys.get(key, key): value
-                    for key, value in sliced_data.items()
-                }
-                row_idx = [(o, i) for o, i in sliced_data.items() for i in i.keys()]
-                values = [v for i in sliced_data.values() for v in i.values()]
-                values = [
-                    ["" if len(sublist) == 0 else ", ".join(map(str, sublist))]
-                    for sublist in values
-                ]
-                multi_index = pd.MultiIndex.from_tuples(
-                    row_idx, names=["Behavior", "Arm"]
-                )
-                df = pd.DataFrame(values, index=multi_index, columns=["Frames"])
-                df.to_csv(save_path)
-            stdout_success(
-                msg=f"Detailed spontaneous alternation data for {len(list(self.results.keys()))} video(s) saved at {save_dir}"
+        viz_df = self.results.sample(
+            n=self.settings["visualize_event_cnt"]
+        ).reset_index(drop=True)
+        for idx, r in viz_df.iterrows():
+            video_name, start_frm, end_frame, severity = (
+                r["VIDEO"],
+                r["START FRAME"],
+                r["END FRAME"],
+                r["SEVERITY"],
+            )
+            pose_df = None
+            if self.settings["show_pose"]:
+                pose_df = read_df(
+                    os.path.join(
+                        self.machine_results_dir, video_name + "." + self.file_type
+                    ),
+                    self.file_type,
+                    usecols=self.bp_headers,
+                ).astype(int)
+            clip_path = os.path.join(
+                save_dir,
+                f'{video_name}_{self.settings["clf"]}_{start_frm}_{end_frame}_{severity}.mp4',
+            )
+            video_path = self.find_video_of_file(
+                video_dir=self.video_dir, filename=video_name
             )
+            video_meta_data = get_video_meta_data(video_path)
+            self.space_scale, self.radius_scale, self.res_scale, self.font_scale = (
+                60,
+                12,
+                1500,
+                1.1,
+            )
+            self.max_dim = max(video_meta_data["width"], video_meta_data["height"])
+            self.circle_scale = int(self.radius_scale / (self.res_scale / self.max_dim))
+            video_fps = int(video_meta_data["fps"] * self.settings["video_speed"])
+            if video_fps < 1:
+                video_fps = 1
+            cap = cv2.VideoCapture(video_path)
+            writer = cv2.VideoWriter(
+                clip_path,
+                cv2.VideoWriter_fourcc(*"mp4v"),
+                video_fps,
+                (int(video_meta_data["width"]), int(video_meta_data["height"])),
+            )
+            event_frm_count, frm_cnt, current_frm = end_frame - start_frm, 0, start_frm
+            cap.set(1, current_frm)
+            while current_frm < end_frame:
+                ret, img = cap.read()
+                if self.settings["show_pose"]:
+                    frm_pose = pose_df.iloc[current_frm]
+                    for animal_cnt, (animal_name, animal_body_parts) in enumerate(
+                        self.animal_bp_dict.items()
+                    ):
+                        for bp_cnt, (x_name, y_name) in enumerate(
+                            zip(animal_body_parts["X_bps"], animal_body_parts["Y_bps"])
+                        ):
+                            x = frm_pose[[x_name, y_name]].values
+                            cv2.circle(
+                                img,
+                                (x[0], x[1]),
+                                0,
+                                self.color_lst_lst[animal_cnt][bp_cnt],
+                                self.circle_scale,
+                            )
+
+                if not ret:
+                    raise InvalidVideoFileError(
+                        msg=f'Could not find frame {current_frm} in video {video_path}. Video {video_path} contains {video_meta_data["frame_count"]} frames.'
+                    )
+                writer.write(img)
+                frm_cnt += 1
+                print(
+                    f"Frame {str(frm_cnt)} / {str(event_frm_count)}, Event {idx + 1}/{str(len(viz_df))}, Video {video_name}"
+                )
+                current_frm += 1
+            writer.release()
+        video_timer.stop_timer()
+        stdout_success(
+            msg=f"Videos complete: saved in {save_dir}",
+            elapsed_time=video_timer.elapsed_time_str,
+        )
 
 
-# if __name__ == "__main__":
-#     parser = argparse.ArgumentParser(description='SimBA Custom Feature Extractor')
-#     parser.add_argument('--config_path', type=str, help='SimBA project config path')
-#     parser.add_argument('--arm_names', nargs='+', help='List of ROI arm names')
-#     parser.add_argument('--center_name', type=str, help='Name of ROI center')
-#     parser.add_argument('--animal_area', type=int, default=80, help='Size of animal geometry required for scored entry/exit')
-#     parser.add_argument('--threshold', type=float, default=0.0, help='Body-part threshold')
-#     parser.add_argument('--buffer', type=int, default=2, help='Added buffer to animal geometry')
-#     parser.add_argument('--verbose', type=bool, default=False, help='If process print outs')
-#     parser.add_argument('--detailed_data', default=False, type=bool, help='If to create additional detailed data')
-#     parser.add_argument('--data_path', type=bool, default=None, help='Path to directory or file.')
-#     args = parser.parse_args()
-#     x = SpontaneousAlternationCalculator(config_path=args.config_path,
-#                                          arm_names=args.arm_names,
-#                                          center_name=args.center_name,
-#                                          threshold=args.threshold,
-#                                          animal_area=args.animal_area,
-#                                          buffer=args.buffer,
-#                                          verbose=args.verbose,
-#                                          detailed_data=args.detailed_data,
-#                                          data_path=args.data_path)
-#     x.run()
-#     x.save()
-
-
-# config_path = '/Users/simon/Desktop/envs/simba/troubleshooting/spontenous_alternation/project_folder/project_config.ini'
-# arm_names = ['A', 'B', 'C']
-# center_name = 'Center'
-# threshold = 0.0
-# animal_area = 60
-# buffer = 2
-# verbose = True
-#
-# x = SpontaneousAlternationCalculator(config_path=config_path,
-#                                      arm_names=arm_names,
-#                                      center_name=center_name,
-#                                      threshold=threshold,
-#                                      animal_area=animal_area,
-#                                      buffer=buffer,
-#                                      verbose=verbose)
-# x.run()
-# x.save()
+# settings = {'brackets': 10,
+#             'clf': 'Attack',
+#             'animals': ['Simon', 'JJ'],
+#             'normalization': 'ALL VIDEOS', #BY VIDEO
+#             'bracket_type': "QUANTIZE",
+#             'save_bin_definitions': True,
+#             'visualize': True,
+#             'visualize_event_cnt': 'ALL CLIPS',
+#             'video_speed': 0.1,
+#             'show_pose': True}
+# processor = SeverityBoutCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', settings=settings)
+# processor.run()
```

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/severity_frame_based_calculator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 __author__ = "Simon Nilsson"
 
 import os
 from datetime import datetime
-from typing import Dict, List, Union
+from typing import Dict, Union
 
 import cv2
 import numpy as np
 import pandas as pd
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.checks import (check_if_filepath_list_is_empty,
                                 check_that_column_exist)
-from simba.utils.data import create_color_palettes, detect_bouts, find_bins
-from simba.utils.errors import InvalidVideoFileError
+from simba.utils.data import (create_color_palettes, detect_bouts, find_bins,
+                              get_video_meta_data)
+from simba.utils.errors import InvalidVideoFileError, NoDataError
 from simba.utils.printing import SimbaTimer, stdout_success
-from simba.utils.read_write import get_fn_ext, get_video_meta_data, read_df
+from simba.utils.read_write import get_fn_ext, read_df
 from simba.utils.warnings import NoDataFoundWarning
 
 
-class SeverityBoutCalculator(ConfigReader, FeatureExtractionMixin):
+class SeverityFrameCalculator(ConfigReader, FeatureExtractionMixin):
     """
-    Computes the "severity" of classification bout events based on how much
-    the animals are moving within the bout. Bouts are scored as less or more severe at lower and higher movements, respectively.
+    Computes the "severity" of classification frame events based on how much
+    the animals are moving. Frames are scored as less or more severe at lower and higher movements, respectively.
 
     :parameter str config_path: path to SimBA project config file in Configparser format.
-    :parameter dict settings: how to calculate the severity. E.g., {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'normalization': 'ALL VIDEOS', 'save_bin_definitions': True, 'visualize': True, 'visualize_event_cnt': 'ALL', 'video_speed': 1.0, 'show_pose': True}
+    :parameter dict settings: how to calculate the severity. E.g., {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False}.
 
     .. note::
        `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md>`__.
 
     Examples
     ----------
-    >>> settings = {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'normalization': 'ALL VIDEOS', 'save_bin_definitions': True, 'visualize': True, 'visualize_event_cnt': 'ALL', 'video_speed': 1.0, 'show_pose': True}
-    >>> processor = SeverityBoutCalculator(config_path='project_folder/project_config.ini', settings=settings)
+    >>> settings = {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False, 'normalization': 'ALL VIDEOS', 'save_bin_definitions': True}
+    >>> processor = SeverityFrameCalculator(config_path='project_folder/project_config.ini', settings=settings)
     >>> processor.run()
     >>> processor.save()
     """
 
     def __init__(self, config_path: Union[str, os.PathLike], settings: Dict):
         ConfigReader.__init__(self, config_path=config_path)
         self.settings = settings
-        self.movement_animal_bp_dict = {
-            k: self.animal_bp_dict[k] for k in self.settings["animals"]
-        }
-        self.color_lst_lst = create_color_palettes(
-            no_animals=len(list(self.animal_bp_dict.keys())),
-            map_size=len(self.bp_headers),
-        )
         check_if_filepath_list_is_empty(
             filepaths=self.machine_results_paths,
             error_msg=f"SIMBA ERROR: Cannot process severity. {self.machine_results_dir} directory is empty",
         )
         save_name = os.path.join(
             f'severity_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv'
         )
+        self.movement_animal_bp_dict = {
+            k: self.animal_bp_dict[k] for k in self.settings["animals"]
+        }
+        self.color_lst_lst = create_color_palettes(
+            no_animals=len(list(self.animal_bp_dict.keys())),
+            map_size=len(self.bp_headers),
+        )
         definitions_save_name = os.path.join(
             f'severity_bin_definitions_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv'
         )
         self.save_path = os.path.join(self.logs_path, save_name)
-        self.definitions_path, self.fourcc = os.path.join(
-            self.logs_path, definitions_save_name
-        ), cv2.VideoWriter_fourcc(*"mp4v")
-
-    def __calculate_movements(self, data_paths: List[str]):
-        movements = {}
-        for file_cnt, file_path in enumerate(data_paths):
+        self.definitions_path = os.path.join(self.logs_path, definitions_save_name)
+        self.results = {}
+
+    def __calculate_movements(self):
+        self.movements = {}
+        for file_cnt, file_path in enumerate(self.machine_results_paths):
             _, video_name, _ = get_fn_ext(file_path)
             print(
-                f"Analyzing movements in {video_name} ({file_cnt+1}/{len(data_paths)})..."
+                f"Analyzing movements in {video_name} ({file_cnt+1}/{len(self.machine_results_paths)})..."
             )
             _, px_per_mm, fps = self.read_video_info(video_name=video_name)
             df = read_df(file_path=file_path, file_type=self.file_type)
             if self.settings["clf"] not in df.columns:
                 NoDataFoundWarning(
                     msg=f'Skipping file {video_name} - {self.settings["clf"]} data not present in file'
                 )
@@ -90,168 +90,175 @@
                             animal_df[bp_x].values,
                             animal_df[f"{bp_x}_shifted"].values,
                             animal_df[bp_y].values,
                             animal_df[f"{bp_y}_shifted"].values,
                             px_per_mm,
                         ),
                     )
-            movements[video_name] = video_movement
-        return movements
+            self.movements[video_name] = video_movement.astype(np.int)
 
     def run(self):
-        movements = self.__calculate_movements(data_paths=self.machine_results_paths)
-        video_bins_info = find_bins(
-            data=movements,
+        self.__calculate_movements()
+        self.visualization_data = {}
+        self.video_bins_info = find_bins(
+            data=self.movements,
             bracket_type=self.settings["bracket_type"],
             bracket_cnt=self.settings["brackets"],
             normalization_method=self.settings["normalization"],
         )
-        self.results = pd.DataFrame(
-            columns=[
-                "VIDEO",
-                "EVENT",
-                "START TIME",
-                "END TIME",
-                "START FRAME",
-                "END FRAME",
-                "BOUT TIME",
-                "MOVEMENT",
-                "SEVERITY",
-            ]
-        )
         for file_cnt, file_path in enumerate(self.machine_results_paths):
             _, video_name, _ = get_fn_ext(file_path)
+            print(
+                f"Matching brackets to movements in video {video_name} ({file_cnt+1}/{len(self.machine_results_paths)})..."
+            )
+            self.results[video_name] = {}
             _, px_per_mm, fps = self.read_video_info(video_name=video_name)
-            df = read_df(file_path=file_path, file_type=self.file_type)
+            df = read_df(file_path=file_path, file_type=self.file_type).astype(int)
             check_that_column_exist(
                 df=df, column_name=self.settings["clf"], file_name=file_path
             )
-            bout_df = detect_bouts(
-                data_df=df, target_lst=[self.settings["clf"]], fps=fps
+            move_df = pd.DataFrame(self.movements[video_name], columns=["MOVEMENT"])
+            video_bins = np.array((0))
+            video_bins = np.hstack(
+                (video_bins, self.video_bins_info[video_name][:, -1])
             )
-            bout_df.columns = [
-                "EVENT",
-                "START TIME",
-                "END TIME",
-                "START FRAME",
-                "END FRAME",
-                "BOUT TIME",
-            ]
-            severity_lst, movement_lst = [], []
-            if len(bout_df) > 0:
-                for i in bout_df[["START FRAME", "END FRAME"]].values:
-                    bout_move_val = np.mean(movements[video_name][i[0] : i[1]])
-                    if bout_move_val >= video_bins_info[video_name][-1][1]:
-                        severity_lst.append(self.settings["brackets"])
-                        movement_lst.append(bout_move_val)
-                    else:
-                        for j_cnt, j in enumerate(video_bins_info[video_name]):
-                            if j[0] <= bout_move_val <= j[1]:
-                                severity_lst.append(j_cnt + 1)
-                                movement_lst.append(round(bout_move_val, 4))
-                bout_df["MOVEMENT"] = movement_lst
-                bout_df["SEVERITY"] = severity_lst
-                bout_df.insert(0, "VIDEO", video_name)
-                self.results = pd.concat([self.results, bout_df], axis=0).reset_index(
-                    drop=True
-                )
-        self.save()
-        if self.settings["save_bin_definitions"]:
-            self.save_bin_definitions(data=video_bins_info)
+            hist = np.histogram([self.movements[video_name]], bins=video_bins)
+            move_df["BIN"] = np.fmin(
+                np.digitize(self.movements[video_name], hist[1]),
+                self.settings["brackets"],
+            )
+            df = pd.concat([df, move_df], axis=1)
+            if self.settings["visualize"]:
+                self.visualization_data[video_name] = df
+            clf_df = (
+                df["BIN"][df[self.settings["clf"]] == 1]
+                .astype(int)
+                .reset_index(drop=True)
+            )
+            for i in range(0, self.settings["brackets"]):
+                if self.settings["frames"]:
+                    self.results[video_name][f"Grade {str(i + 1)} (frames)"] = len(
+                        clf_df[clf_df == i]
+                    )
+                if self.settings["time"]:
+                    self.results[video_name][f"Grade {str(i + 1)} (s)"] = round(
+                        (len(clf_df[clf_df == i]) / fps), 4
+                    )
+        self.__save()
         if self.settings["visualize"]:
-            self.visualize()
+            self.__visualize()
 
-    def save(self):
-        self.results.to_csv(self.save_path)
+    def __save(self):
+        print("Saving data..")
+        out_df = pd.DataFrame(columns=["VIDEO", "MEASUREMENT", "VALUE"])
+        for video_name, video_data in self.results.items():
+            for grade, grade_data in video_data.items():
+                out_df.loc[len(out_df)] = [video_name, grade, grade_data]
+        out_df.to_csv(self.save_path)
         self.timer.stop_timer()
         stdout_success(
-            msg=f"Bout severity data saved at {self.save_path}",
+            msg=f"Severity data saved at {self.save_path}",
             elapsed_time=self.timer.elapsed_time_str,
         )
 
-    def save_bin_definitions(self, data=dict):
-        results = pd.DataFrame(columns=["VIDEO", "SEVERITY_BIN", ">=", "<"])
-        for video_name, video_bins in data.items():
-            for bin_cnt, video_bin in enumerate(video_bins):
-                results.loc[len(results)] = [
-                    video_name,
-                    bin_cnt + 1,
-                    video_bin[0],
-                    video_bin[1],
-                ]
-        save_path = os.path.join(
-            self.logs_path, f"severity_bin_definitions_{self.datetime}.csv"
-        )
-        results.to_csv(save_path)
-        stdout_success(msg=f"Severity bracket definitions saved at {save_path}")
-
-    def visualize(self):
-        if self.settings["visualize_event_cnt"] == "ALL CLIPS":
-            self.settings["visualize_event_cnt"] = len(self.results)
-        elif self.settings["visualize_event_cnt"] > len(self.results):
-            self.settings["visualize_event_cnt"] = len(self.results)
-            print(
-                f'User specified {self.settings["visualize_event_cnt"]} visualization but only {len(self.results)} bouts where found. Creating {len(self.results)} videos...'
+        if self.settings["save_bin_definitions"]:
+            results = pd.DataFrame(columns=["VIDEO", "SEVERITY_BIN", ">=", "<"])
+            for video_name, video_bins in self.video_bins_info.items():
+                for bin_cnt, video_bin in enumerate(video_bins):
+                    results.loc[len(results)] = [
+                        video_name,
+                        bin_cnt + 1,
+                        video_bin[0],
+                        video_bin[1],
+                    ]
+            save_path = os.path.join(
+                self.logs_path, f"severity_bin_definitions_{self.datetime}.csv"
             )
+            results.to_csv(save_path)
+            stdout_success(msg=f"Severity bracket definitions saved at {save_path}")
+
+    def __visualize(self):
+        bouts_df_lst = []
         video_timer, save_dir = SimbaTimer(start=True), os.path.join(
             self.project_path, "frames", "output", "severity_bouts"
         )
         if not os.path.exists(save_dir):
             os.makedirs(save_dir)
-        viz_df = self.results.sample(
-            n=self.settings["visualize_event_cnt"]
-        ).reset_index(drop=True)
-        for idx, r in viz_df.iterrows():
-            video_name, start_frm, end_frame, severity = (
+        for video_name, video_data in self.visualization_data.items():
+            bouts_df = detect_bouts(
+                data_df=video_data, target_lst=[self.settings["clf"]], fps=-1
+            )
+            bouts_df.insert(0, "VIDEO", video_name)
+            bouts_df_lst.append(bouts_df)
+        bouts_df = pd.concat(bouts_df_lst, axis=0)
+        if self.settings["visualize_event_cnt"] == "ALL CLIPS":
+            self.settings["visualize_event_cnt"] = len(bouts_df)
+        elif self.settings["visualize_event_cnt"] > len(bouts_df):
+            self.settings["visualize_event_cnt"] = len(bouts_df)
+            print(
+                f'User specified {self.settings["visualize_event_cnt"]} visualization but only {len(self.results)} bouts where found. Creating {len(self.results)} videos...'
+            )
+        bouts_df = bouts_df.sample(n=self.settings["visualize_event_cnt"]).reset_index(
+            drop=True
+        )
+        for idx, r in bouts_df.iterrows():
+            video_name, start_frm, end_frame = (
                 r["VIDEO"],
-                r["START FRAME"],
-                r["END FRAME"],
-                r["SEVERITY"],
-            )
-            pose_df = None
-            if self.settings["show_pose"]:
-                pose_df = read_df(
-                    os.path.join(
-                        self.machine_results_dir, video_name + "." + self.file_type
-                    ),
-                    self.file_type,
-                    usecols=self.bp_headers,
-                ).astype(int)
+                r["Start_frame"],
+                r["End_frame"],
+            )
+            print(start_frm)
+            bout_df = self.visualization_data[video_name].iloc[start_frm:end_frame]
             clip_path = os.path.join(
                 save_dir,
-                f'{video_name}_{self.settings["clf"]}_{start_frm}_{end_frame}_{severity}.mp4',
+                f'{video_name}_{self.settings["clf"]}_{start_frm}_{end_frame}.mp4',
             )
             video_path = self.find_video_of_file(
                 video_dir=self.video_dir, filename=video_name
             )
             video_meta_data = get_video_meta_data(video_path)
             self.space_scale, self.radius_scale, self.res_scale, self.font_scale = (
                 60,
                 12,
                 1500,
                 1.1,
             )
             self.max_dim = max(video_meta_data["width"], video_meta_data["height"])
             self.circle_scale = int(self.radius_scale / (self.res_scale / self.max_dim))
+            self.font_size = float(self.font_scale / (self.res_scale / self.max_dim))
             video_fps = int(video_meta_data["fps"] * self.settings["video_speed"])
             if video_fps < 1:
                 video_fps = 1
             cap = cv2.VideoCapture(video_path)
             writer = cv2.VideoWriter(
                 clip_path,
                 cv2.VideoWriter_fourcc(*"mp4v"),
                 video_fps,
                 (int(video_meta_data["width"]), int(video_meta_data["height"])),
             )
-            event_frm_count, frm_cnt, current_frm = end_frame - start_frm, 0, start_frm
+            event_frm_count, frm_cnt, current_frm = (
+                (end_frame - start_frm),
+                0,
+                start_frm,
+            )
             cap.set(1, current_frm)
+
             while current_frm < end_frame:
                 ret, img = cap.read()
                 if self.settings["show_pose"]:
-                    frm_pose = pose_df.iloc[current_frm]
+                    frm_pose = bout_df.loc[current_frm]
+                    cv2.putText(
+                        img,
+                        f'Severity bin: {frm_pose["BIN"]}',
+                        (10, 50),
+                        cv2.FONT_HERSHEY_COMPLEX,
+                        self.font_size,
+                        (255, 0, 0),
+                        2,
+                    )
                     for animal_cnt, (animal_name, animal_body_parts) in enumerate(
                         self.animal_bp_dict.items()
                     ):
                         for bp_cnt, (x_name, y_name) in enumerate(
                             zip(animal_body_parts["X_bps"], animal_body_parts["Y_bps"])
                         ):
                             x = frm_pose[[x_name, y_name]].values
@@ -266,30 +273,32 @@
                 if not ret:
                     raise InvalidVideoFileError(
                         msg=f'Could not find frame {current_frm} in video {video_path}. Video {video_path} contains {video_meta_data["frame_count"]} frames.'
                     )
                 writer.write(img)
                 frm_cnt += 1
                 print(
-                    f"Frame {str(frm_cnt)} / {str(event_frm_count)}, Event {idx + 1}/{str(len(viz_df))}, Video {video_name}"
+                    f"Frame {str(frm_cnt)} / {str(event_frm_count)}, Event {idx + 1}/{str(len(bouts_df))}, Video {video_name}"
                 )
                 current_frm += 1
             writer.release()
         video_timer.stop_timer()
         stdout_success(
             msg=f"Videos complete: saved in {save_dir}",
             elapsed_time=video_timer.elapsed_time_str,
         )
 
 
 # settings = {'brackets': 10,
 #             'clf': 'Attack',
 #             'animals': ['Simon', 'JJ'],
 #             'normalization': 'ALL VIDEOS', #BY VIDEO
-#             'bracket_type': "QUANTIZE",
+#             'bracket_type': "QUANTILE",
+#             'time': True,
+#             'frames': True,
 #             'save_bin_definitions': True,
 #             'visualize': True,
 #             'visualize_event_cnt': 'ALL CLIPS',
 #             'video_speed': 0.1,
 #             'show_pose': True}
-# processor = SeverityBoutCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', settings=settings)
+# processor = SeverityFrameCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', settings=settings)
 # processor.run()
```

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/directing_animal_to_bodypart.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/directing_animal_to_bodypart.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/boolean_conditional_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/boolean_conditional_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/gibbs_sampler.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/gibbs_sampler.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/outlier_tools/outlier_corrector_location_advanced.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,304 +1,299 @@
 __author__ = "Simon Nilsson"
 
+import glob
 import os
-from datetime import datetime
-from typing import Dict, Union
+from copy import deepcopy
+from typing import Union
 
-import cv2
 import numpy as np
 import pandas as pd
+from numba import jit, prange
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
-from simba.utils.checks import (check_if_filepath_list_is_empty,
-                                check_that_column_exist)
-from simba.utils.data import (create_color_palettes, detect_bouts, find_bins,
-                              get_video_meta_data)
-from simba.utils.errors import InvalidVideoFileError, NoDataError
-from simba.utils.printing import SimbaTimer, stdout_success
-from simba.utils.read_write import get_fn_ext, read_df
-from simba.utils.warnings import NoDataFoundWarning
+from simba.utils.enums import TagNames
+from simba.utils.errors import InvalidInputError, NoFilesFoundError
+from simba.utils.printing import SimbaTimer, log_event, stdout_success
+from simba.utils.read_write import (find_files_of_filetypes_in_directory,
+                                    get_fn_ext, read_df, write_df)
 
 
-class SeverityFrameCalculator(ConfigReader, FeatureExtractionMixin):
+class OutlierCorrecterLocationAdvanced(ConfigReader, FeatureExtractionMixin):
     """
-    Computes the "severity" of classification frame events based on how much
-    the animals are moving. Frames are scored as less or more severe at lower and higher movements, respectively.
-
-    :parameter str config_path: path to SimBA project config file in Configparser format.
-    :parameter dict settings: how to calculate the severity. E.g., {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False}.
+    Performs location outlier correction that allows different heuristic outlier criteria for different animals or body-parts.
+    For example, correct some outlier body-parts with a location heuristic criteria of 4x above the mean movement,
+    and other body-parts with a heuristic critera of 2x above the mean movement.
 
     .. note::
-       `Tutorial <https://github.com/sgoldenlab/simba/blob/master/docs/Scenario2.md>`__.
+       See `notebook <https://simba-uw-tf-dev.readthedocs.io/en/latest/nb/advanced_outlier_correction.html>`__. for example use-case.
+
+    .. image:: _static/img/location_outlier.png
+       :width: 400
+       :align: center
 
-    Examples
-    ----------
-    >>> settings = {'brackets': 10, 'clf': 'Attack', 'animals': ['Simon', 'JJ'], 'time': True, 'frames': False, 'normalization': 'ALL VIDEOS', 'save_bin_definitions': True}
-    >>> processor = SeverityFrameCalculator(config_path='project_folder/project_config.ini', settings=settings)
-    >>> processor.run()
-    >>> processor.save()
+    :parameter str config_path: path to SimBA project config file in Configparser format.
+    :parameter str input_dir: Directory containing input files. E.g., `project_folder/csv/input_csv` directory.
+    :parameter Literal['animal', 'body-part'] type: If the rules are defined on animal or body-part level. E.g., If one heuristic rule per animal then `animal`. If one heurstic rule prr body-part then `body-parts`
+    :parameter Literal['mean', 'median'] agg_method: If to use the mean or median to compute criterion.
+    :parameter dict criterion_body_parts: The body-parts used to calculate the size of the animals.
+    :parameter dict settings: The heuristic multiplier rules to use for each body part or animal.
+
+    :example:
+    >>> settings = {'Simon': 1.1, 'JJ': 1.2}
+    >>> criterion_body_parts = {'Simon': ['Nose_1', 'Tail_base_1'], 'JJ': ['Nose_2', 'Tail_base_2']}
+    >>> outlier_corrector = OutlierCorrecterLocationAdvanced(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', input_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/input_csv', type='animal', agg_method='mean', criterion_body_parts=criterion_body_parts, settings=settings)
+    >>> outlier_corrector.run()
+    >>> settings = {'Simon': {'Ear_left_1': 1.1, 'Ear_right_1': 5.1, 'Nose_1': 2.1, 'Center_1': 1.5, 'Lat_left_1': 3.1, 'Lat_right_1': 1.9, 'Tail_base_1': 2.3, 'Tail_end_1': 1.4}, 'JJ': {'Ear_left_2': 1.2, 'Ear_right_2': 1.2, 'Nose_2': 2, 'Center_2': 4.1, 'Lat_left_2': 9, 'Lat_right_2': 1.2, 'Tail_base_2': 1.6, 'Tail_end_2': 2.2}}
+    >>> outlier_corrector = OutlierCorrecterLocationAdvanced(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', input_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/input_csv', type='body-part', agg_method='mean', criterion_body_parts=criterion_body_parts, settings=settings)
     """
 
-    def __init__(self, config_path: Union[str, os.PathLike], settings: Dict):
+    def __init__(
+        self,
+        config_path: Union[str, os.PathLike],
+        input_dir: Union[str, os.PathLike],
+        type: str,
+        agg_method: str,
+        criterion_body_parts: dict,
+        settings: dict,
+    ):
         ConfigReader.__init__(self, config_path=config_path)
-        self.settings = settings
-        check_if_filepath_list_is_empty(
-            filepaths=self.machine_results_paths,
-            error_msg=f"SIMBA ERROR: Cannot process severity. {self.machine_results_dir} directory is empty",
-        )
-        save_name = os.path.join(
-            f'severity_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv'
+        FeatureExtractionMixin.__init__(self)
+        log_event(
+            logger_name=str(self.__class__.__name__),
+            log_type=TagNames.CLASS_INIT.value,
+            msg=self.create_log_msg_from_init_args(locals=locals()),
         )
-        self.movement_animal_bp_dict = {
-            k: self.animal_bp_dict[k] for k in self.settings["animals"]
-        }
-        self.color_lst_lst = create_color_palettes(
-            no_animals=len(list(self.animal_bp_dict.keys())),
-            map_size=len(self.bp_headers),
+        self.data_files = find_files_of_filetypes_in_directory(
+            directory=input_dir, extensions=["." + self.file_type]
         )
-        definitions_save_name = os.path.join(
-            f'severity_bin_definitions_{datetime.now().strftime("%Y%m%d%H%M%S")}.csv'
+        if len(self.data_files) == 0:
+            raise NoFilesFoundError(
+                msg=f"No data of filetype {input_dir} for in directory {self.file_type}",
+                source=self.__class__.__name__,
+            )
+        if type not in ["animal", "body-parts"]:
+            raise InvalidInputError(
+                msg=f"Type {type} not supported. Valid options: {['animal', 'body-parts']}",
+                source=self.__class__.__name__,
+            )
+        if agg_method not in ["mean", "median"]:
+            raise InvalidInputError(
+                msg=f"Aggregation method {agg_method} not supported. Valid options: {['mean', 'median']}",
+                source=self.__class__.__name__,
+            )
+        self.settings, self.type, self.agg_method, self.criterion_body_parts = (
+            settings,
+            type,
+            agg_method,
+            criterion_body_parts,
         )
-        self.save_path = os.path.join(self.logs_path, save_name)
-        self.definitions_path = os.path.join(self.logs_path, definitions_save_name)
-        self.results = {}
-
-    def __calculate_movements(self):
-        self.movements = {}
-        for file_cnt, file_path in enumerate(self.machine_results_paths):
-            _, video_name, _ = get_fn_ext(file_path)
-            print(
-                f"Analyzing movements in {video_name} ({file_cnt+1}/{len(self.machine_results_paths)})..."
-            )
-            _, px_per_mm, fps = self.read_video_info(video_name=video_name)
-            df = read_df(file_path=file_path, file_type=self.file_type)
-            if self.settings["clf"] not in df.columns:
-                NoDataFoundWarning(
-                    msg=f'Skipping file {video_name} - {self.settings["clf"]} data not present in file'
-                )
-                continue
-            video_movement = np.full((len(df)), 0)
-            for animal_name, animal_bodyparts in self.movement_animal_bp_dict.items():
-                animal_df = df[animal_bodyparts["X_bps"] + animal_bodyparts["Y_bps"]]
-                animal_df = self.create_shifted_df(df=animal_df)
-                for bp_x, bp_y in zip(
-                    animal_bodyparts["X_bps"], animal_bodyparts["Y_bps"]
-                ):
-                    video_movement = np.add(
-                        video_movement,
-                        self.euclidean_distance(
-                            animal_df[bp_x].values,
-                            animal_df[f"{bp_x}_shifted"].values,
-                            animal_df[bp_y].values,
-                            animal_df[f"{bp_y}_shifted"].values,
-                            px_per_mm,
-                        ),
-                    )
-            self.movements[video_name] = video_movement.astype(np.int)
 
-    def run(self):
-        self.__calculate_movements()
-        self.visualization_data = {}
-        self.video_bins_info = find_bins(
-            data=self.movements,
-            bracket_type=self.settings["bracket_type"],
-            bracket_cnt=self.settings["brackets"],
-            normalization_method=self.settings["normalization"],
+    def fix_settings_for_animal_input(self):
+        new_settings = {}
+        for animal_name, animal_bps in self.animal_bp_dict.items():
+            if animal_name in self.settings.keys():
+                if animal_name not in new_settings.keys():
+                    new_settings[animal_name] = {}
+                for body_part in animal_bps["X_bps"]:
+                    new_settings[animal_name][body_part[:-2]] = self.settings[
+                        animal_name
+                    ]
+        self.settings = new_settings
+
+    @staticmethod
+    @jit(nopython=True)
+    def three_dim_cdist(data: np.ndarray) -> np.ndarray:
+        results = np.full((data.shape[0], data.shape[1], data.shape[1]), np.nan)
+        for i in prange(data.shape[0]):
+            for j in prange(data[i].shape[0]):
+                for k in prange(data[i].shape[0]):
+                    results[i][j][k] = np.linalg.norm(data[i][j] - data[i][k])
+
+        return results
+
+    def _save_data_log(self, data_log: dict):
+        out = pd.DataFrame(
+            columns=[
+                "VIDEO",
+                "ANIMAL",
+                "BODY-PART",
+                "OUTLIER COUNT",
+                "OUTLIER RATIO (%)",
+            ]
         )
-        for file_cnt, file_path in enumerate(self.machine_results_paths):
-            _, video_name, _ = get_fn_ext(file_path)
-            print(
-                f"Matching brackets to movements in video {video_name} ({file_cnt+1}/{len(self.machine_results_paths)})..."
-            )
-            self.results[video_name] = {}
-            _, px_per_mm, fps = self.read_video_info(video_name=video_name)
-            df = read_df(file_path=file_path, file_type=self.file_type).astype(int)
-            check_that_column_exist(
-                df=df, column_name=self.settings["clf"], file_name=file_path
-            )
-            move_df = pd.DataFrame(self.movements[video_name], columns=["MOVEMENT"])
-            video_bins = np.array((0))
-            video_bins = np.hstack(
-                (video_bins, self.video_bins_info[video_name][:, -1])
-            )
-            hist = np.histogram([self.movements[video_name]], bins=video_bins)
-            move_df["BIN"] = np.fmin(
-                np.digitize(self.movements[video_name], hist[1]),
-                self.settings["brackets"],
-            )
-            df = pd.concat([df, move_df], axis=1)
-            if self.settings["visualize"]:
-                self.visualization_data[video_name] = df
-            clf_df = (
-                df["BIN"][df[self.settings["clf"]] == 1]
-                .astype(int)
-                .reset_index(drop=True)
-            )
-            for i in range(0, self.settings["brackets"]):
-                if self.settings["frames"]:
-                    self.results[video_name][f"Grade {str(i + 1)} (frames)"] = len(
-                        clf_df[clf_df == i]
-                    )
-                if self.settings["time"]:
-                    self.results[video_name][f"Grade {str(i + 1)} (s)"] = round(
-                        (len(clf_df[clf_df == i]) / fps), 4
-                    )
-        self.__save()
-        if self.settings["visualize"]:
-            self.__visualize()
-
-    def __save(self):
-        print("Saving data..")
-        out_df = pd.DataFrame(columns=["VIDEO", "MEASUREMENT", "VALUE"])
-        for video_name, video_data in self.results.items():
-            for grade, grade_data in video_data.items():
-                out_df.loc[len(out_df)] = [video_name, grade, grade_data]
-        out_df.to_csv(self.save_path)
-        self.timer.stop_timer()
-        stdout_success(
-            msg=f"Severity data saved at {self.save_path}",
-            elapsed_time=self.timer.elapsed_time_str,
+        save_path = os.path.join(
+            self.logs_path, f"location_outliers_{self.datetime}.csv"
         )
-
-        if self.settings["save_bin_definitions"]:
-            results = pd.DataFrame(columns=["VIDEO", "SEVERITY_BIN", ">=", "<"])
-            for video_name, video_bins in self.video_bins_info.items():
-                for bin_cnt, video_bin in enumerate(video_bins):
-                    results.loc[len(results)] = [
+        for video_name, video_data in data_log.items():
+            for animal_name, animal_data in video_data.items():
+                for body_part_name, body_part_data in animal_data.items():
+                    out.loc[len(out)] = [
                         video_name,
-                        bin_cnt + 1,
-                        video_bin[0],
-                        video_bin[1],
+                        animal_name,
+                        body_part_name,
+                        body_part_data["outlier_cnt"],
+                        body_part_data["outlier_ratio"],
                     ]
-            save_path = os.path.join(
-                self.logs_path, f"severity_bin_definitions_{self.datetime}.csv"
-            )
-            results.to_csv(save_path)
-            stdout_success(msg=f"Severity bracket definitions saved at {save_path}")
-
-    def __visualize(self):
-        bouts_df_lst = []
-        video_timer, save_dir = SimbaTimer(start=True), os.path.join(
-            self.project_path, "frames", "output", "severity_bouts"
+        write_df(df=out, file_type="csv", save_path=save_path)
+        stdout_success(
+            msg=f"Location outlier log saved at {save_path}",
+            source=self.__class__.__name__,
         )
-        if not os.path.exists(save_dir):
-            os.makedirs(save_dir)
-        for video_name, video_data in self.visualization_data.items():
-            bouts_df = detect_bouts(
-                data_df=video_data, target_lst=[self.settings["clf"]], fps=-1
-            )
-            bouts_df.insert(0, "VIDEO", video_name)
-            bouts_df_lst.append(bouts_df)
-        bouts_df = pd.concat(bouts_df_lst, axis=0)
-        if self.settings["visualize_event_cnt"] == "ALL CLIPS":
-            self.settings["visualize_event_cnt"] = len(bouts_df)
-        elif self.settings["visualize_event_cnt"] > len(bouts_df):
-            self.settings["visualize_event_cnt"] = len(bouts_df)
+
+    def run(self):
+        data_log = {}
+        if self.type == "animal":
+            self.fix_settings_for_animal_input()
+
+        for file_cnt, file_path in enumerate(self.data_files):
+            video_timer, video_log = SimbaTimer(start=True), {}
+            _, self.video_name, _ = get_fn_ext(file_path)
             print(
-                f'User specified {self.settings["visualize_event_cnt"]} visualization but only {len(self.results)} bouts where found. Creating {len(self.results)} videos...'
-            )
-        bouts_df = bouts_df.sample(n=self.settings["visualize_event_cnt"]).reset_index(
-            drop=True
-        )
-        for idx, r in bouts_df.iterrows():
-            video_name, start_frm, end_frame = (
-                r["VIDEO"],
-                r["Start_frame"],
-                r["End_frame"],
-            )
-            print(start_frm)
-            bout_df = self.visualization_data[video_name].iloc[start_frm:end_frame]
-            clip_path = os.path.join(
-                save_dir,
-                f'{video_name}_{self.settings["clf"]}_{start_frm}_{end_frame}.mp4',
-            )
-            video_path = self.find_video_of_file(
-                video_dir=self.video_dir, filename=video_name
-            )
-            video_meta_data = get_video_meta_data(video_path)
-            self.space_scale, self.radius_scale, self.res_scale, self.font_scale = (
-                60,
-                12,
-                1500,
-                1.1,
-            )
-            self.max_dim = max(video_meta_data["width"], video_meta_data["height"])
-            self.circle_scale = int(self.radius_scale / (self.res_scale / self.max_dim))
-            self.font_size = float(self.font_scale / (self.res_scale / self.max_dim))
-            video_fps = int(video_meta_data["fps"] * self.settings["video_speed"])
-            if video_fps < 1:
-                video_fps = 1
-            cap = cv2.VideoCapture(video_path)
-            writer = cv2.VideoWriter(
-                clip_path,
-                cv2.VideoWriter_fourcc(*"mp4v"),
-                video_fps,
-                (int(video_meta_data["width"]), int(video_meta_data["height"])),
-            )
-            event_frm_count, frm_cnt, current_frm = (
-                (end_frame - start_frm),
-                0,
-                start_frm,
+                "Processing video {}. Video {}/{}...".format(
+                    self.video_name, str(file_cnt + 1), str(len(self.data_files))
+                )
             )
-            cap.set(1, current_frm)
-
-            while current_frm < end_frame:
-                ret, img = cap.read()
-                if self.settings["show_pose"]:
-                    frm_pose = bout_df.loc[current_frm]
-                    cv2.putText(
-                        img,
-                        f'Severity bin: {frm_pose["BIN"]}',
-                        (10, 50),
-                        cv2.FONT_HERSHEY_COMPLEX,
-                        self.font_size,
-                        (255, 0, 0),
-                        2,
+            self.data_df = read_df(file_path, self.file_type, check_multiindex=True)
+            self.data_df = self.insert_column_headers_for_outlier_correction(
+                data_df=self.data_df, new_headers=self.bp_headers, filepath=file_path
+            )
+            self.results = deepcopy(self.data_df)
+            self.data_df_combined = self.create_shifted_df(df=self.data_df)
+            animal_movement_agg = {}
+            for animal_name, animal_bps in self.animal_bp_dict.items():
+                if animal_name in self.criterion_body_parts.keys():
+                    animal_criterion_bps = self.criterion_body_parts[animal_name]
+                    bp_1_headers = [
+                        animal_criterion_bps[0] + "_x",
+                        animal_criterion_bps[0] + "_y",
+                    ]
+                    bp_2_headers = [
+                        animal_criterion_bps[1] + "_x",
+                        animal_criterion_bps[1] + "_y",
+                    ]
+                    distances = self.framewise_euclidean_distance(
+                        location_1=self.data_df[bp_1_headers].values,
+                        location_2=self.data_df[bp_2_headers].values,
+                        px_per_mm=1,
+                    )
+                    if self.agg_method == "mean":
+                        animal_movement_agg[animal_name] = np.mean(distances).astype(
+                            int
+                        )
+                    if self.agg_method == "median":
+                        animal_movement_agg[animal_name] = np.median(distances).astype(
+                            int
+                        )
+
+            for animal_name, animal_bps in self.settings.items():
+                video_log[animal_name] = {}
+                animal_bp_headers = np.array(
+                    [
+                        item
+                        for pair in zip(
+                            self.animal_bp_dict[animal_name]["X_bps"],
+                            self.animal_bp_dict[animal_name]["Y_bps"],
+                        )
+                        for item in pair
+                    ]
+                )
+                animal_body_part_names = [
+                    x[:-2] for x in self.animal_bp_dict[animal_name]["X_bps"]
+                ]
+                animal_body_part_dict = {
+                    k: v
+                    for (v, k) in zip(
+                        animal_body_part_names, range(0, len(animal_body_part_names))
                     )
-                    for animal_cnt, (animal_name, animal_body_parts) in enumerate(
-                        self.animal_bp_dict.items()
-                    ):
-                        for bp_cnt, (x_name, y_name) in enumerate(
-                            zip(animal_body_parts["X_bps"], animal_body_parts["Y_bps"])
-                        ):
-                            x = frm_pose[[x_name, y_name]].values
-                            cv2.circle(
-                                img,
-                                (x[0], x[1]),
-                                0,
-                                self.color_lst_lst[animal_cnt][bp_cnt],
-                                self.circle_scale,
-                            )
-
-                if not ret:
-                    raise InvalidVideoFileError(
-                        msg=f'Could not find frame {current_frm} in video {video_path}. Video {video_path} contains {video_meta_data["frame_count"]} frames.'
+                }
+                animal_arr = self.data_df[animal_bp_headers].values.reshape(
+                    len(self.data_df), -1, 2
+                )
+                data = self.three_dim_cdist(data=animal_arr)
+                df = (
+                    pd.concat(
+                        [pd.DataFrame(arr) for arr in data], keys=np.arange(len(data))
                     )
-                writer.write(img)
-                frm_cnt += 1
-                print(
-                    f"Frame {str(frm_cnt)} / {str(event_frm_count)}, Event {idx + 1}/{str(len(bouts_df))}, Video {video_name}"
+                    .reset_index()
+                    .rename(columns={"level_0": "frame", "level_1": "body_part"})
                 )
-                current_frm += 1
-            writer.release()
-        video_timer.stop_timer()
+                df["body_part"] = df["body_part"].map(animal_body_part_dict)
+                above_criterion_dict = {}
+                for bp, criterion_multiplier in animal_bps.items():
+                    if animal_name in animal_movement_agg.keys():
+                        bp_criterion = (
+                            animal_movement_agg[animal_name] * criterion_multiplier
+                        )
+                        bp_df = df[df["body_part"] == bp]
+                        bp_df["counts_above_criterion"] = self.count_values_in_range(
+                            data=bp_df.drop(["frame", "body_part"], axis=1).values,
+                            ranges=np.array([[bp_criterion, np.inf]]),
+                        )
+                        above_criterion_dict[bp] = list(
+                            bp_df["frame"][bp_df["counts_above_criterion"] > 1]
+                        )
+
+                for (
+                    bp,
+                    body_part_frames_above_criterion,
+                ) in above_criterion_dict.items():
+                    self.results.loc[
+                        body_part_frames_above_criterion, [f"{bp}_x", f"{bp}_y"]
+                    ] = np.nan
+                    self.results[[f"{bp}_x", f"{bp}_y"]] = (
+                        self.results[[f"{bp}_x", f"{bp}_y"]].ffill().bfill().astype(int)
+                    )
+                    video_log[animal_name][bp] = {
+                        "outlier_cnt": len(body_part_frames_above_criterion),
+                        "outlier_ratio": len(body_part_frames_above_criterion)
+                        / len(self.results),
+                    }
+
+            df_save_path = os.path.join(
+                self.outlier_corrected_dir, self.video_name + f"{self.file_type}."
+            )
+            write_df(df=self.results, file_type=self.file_type, save_path=df_save_path)
+            video_timer.stop_timer()
+            stdout_success(
+                msg=f"Location outliers complete for video {self.video_name}.",
+                elapsed_time=video_timer.elapsed_time_str,
+                source=self.__class__.__name__,
+            )
+            data_log[self.video_name] = video_log
+
+        self._save_data_log(data_log=data_log)
         stdout_success(
-            msg=f"Videos complete: saved in {save_dir}",
-            elapsed_time=video_timer.elapsed_time_str,
+            msg=f"{len(self.data_files)} video(s) corrected for location outliers. Saved in {self.outlier_corrected_dir}",
+            source=self.__class__.__name__,
         )
 
 
-# settings = {'brackets': 10,
-#             'clf': 'Attack',
-#             'animals': ['Simon', 'JJ'],
-#             'normalization': 'ALL VIDEOS', #BY VIDEO
-#             'bracket_type': "QUANTILE",
-#             'time': True,
-#             'frames': True,
-#             'save_bin_definitions': True,
-#             'visualize': True,
-#             'visualize_event_cnt': 'ALL CLIPS',
-#             'video_speed': 0.1,
-#             'show_pose': True}
-# processor = SeverityFrameCalculator(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', settings=settings)
-# processor.run()
+# settings = {'Simon': 2.5} #
+# # settings = {'Simon': {'Ear_left_1': 1.1,
+# #                       'Ear_right_1': 5.1,
+# #                       'Nose_1': 2.1,
+# #                       'Center_1': 1.5,
+# #                       'Lat_left_1': 3.1,
+# #                       'Lat_right_1': 1.9,
+# #                       'Tail_base_1': 2.3},
+# #                       #'Tail_end_1': 1.4},
+# #                'JJ': {'Ear_left_2': 1.2,
+# #                       'Ear_right_2': 1.2,
+# #                       'Nose_2': 2,
+# #                       'Center_2': 4.1,
+# #                       'Lat_left_2': 9,
+# #                       'Lat_right_2': 1.2,
+# #                       'Tail_base_2': 1.6,
+# #                       'Tail_end_2': 2.2}}
+# criterion_body_parts = {'Simon': ['Nose_1', 'Tail_base_1'], } #'JJ': ['Nose_2', 'Tail_base_2']
+# test = OutlierCorrecterLocationAdvanced(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+#                                         input_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/input_csv',
+#                                         type='animal',
+#                                         agg_method='mean',
+#                                         criterion_body_parts=criterion_body_parts,
+#                                         settings=settings)
+# test.run()
+
+
+# test = OutlierCorrecterLocation(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
+# test.correct_location_outliers()
```

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.90.8/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.90.8/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/model/train_multiclass_rf.py` & `Simba-UW-tf-dev-1.90.8/simba/model/train_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/model/inference_multiclass_batch.py` & `Simba-UW-tf-dev-1.90.8/simba/model/inference_multiclass_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/model/grid_search_multiclass_rf.py` & `Simba-UW-tf-dev-1.90.8/simba/model/grid_search_multiclass_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.90.8/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.90.8/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/model/train_multilabel_rf.py` & `Simba-UW-tf-dev-1.90.8/simba/model/train_multilabel_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_size_standardizer.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_size_standardizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,40 +176,24 @@
                             video_name,
                             animal_name,
                             row["Name"],
                             roi_bouts["Bout_time"].sum(),
                         ]
                     for _, row in self.roi_dict[Keys.ROI_CIRCLES.value].iterrows():
                         center_x, center_y = row["centerX"], row["centerY"]
-                        animal_df[f'{row["Name"]}_distance'] = (
-                            FeatureExtractionMixin.framewise_euclidean_distance_roi(
-                                location_1=animal_df.values[:, 0:2],
-                                location_2=np.array([center_x, center_y]),
-                            )
-                        )
+                        animal_df[f'{row["Name"]}_distance'] = (FeatureExtractionMixin.framewise_euclidean_distance_roi(location_1=animal_df.values[:, 0:2], location_2=np.array([center_x, center_y]), px_per_mm=1))
                         animal_df[row["Name"]] = 0
-                        animal_df.loc[
-                            animal_df[row["Name"]] <= row["radius"], row["Name"]
-                        ] = 1
-                        animal_df.loc[
-                            animal_df[bp_names[2]] < self.threshold, row["Name"]
-                        ] = 0
-                        roi_bouts = detect_bouts(
-                            data_df=animal_df, target_lst=[row["Name"]], fps=self.fps
-                        )
+                        animal_df.loc[animal_df[f'{row["Name"]}_distance'] <= row["radius"], row["Name"]] = 1
+                        animal_df.loc[animal_df[bp_names[2]] < self.threshold, row["Name"]] = 0
+                        roi_bouts = detect_bouts(data_df=animal_df, target_lst=[row["Name"]], fps=self.fps)
                         roi_bouts["ANIMAL"] = animal_name
                         roi_bouts["VIDEO"] = video_name
                         self.roi_bout_results.append(roi_bouts)
                         animal_bout_results[row["Name"]] = roi_bouts
-                        self.entry_results.loc[len(self.entry_results)] = [
-                            video_name,
-                            animal_name,
-                            row["Name"],
-                            len(roi_bouts),
-                        ]
+                        self.entry_results.loc[len(self.entry_results)] = [video_name, animal_name, row["Name"], len(roi_bouts)]
                         self.time_results.loc[len(self.time_results)] = [
                             video_name,
                             animal_name,
                             row["Name"],
                             roi_bouts["Bout_time"].sum(),
                         ]
                     for _, row in self.roi_dict[Keys.ROI_POLYGONS.value].iterrows():
```

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.90.8/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.90.8/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/13.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.90.8/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.90.8/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/video_processors/roi_selector_circle.py` & `Simba-UW-tf-dev-1.90.8/simba/video_processors/roi_selector_circle.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.90.8/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.90.8/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.90.8/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.90.8/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/video_processors/roi_selector.py` & `Simba-UW-tf-dev-1.90.8/simba/video_processors/roi_selector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.90.8/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/video_processors/roi_selector_polygon.py` & `Simba-UW-tf-dev-1.90.8/simba/video_processors/roi_selector_polygon.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.90.8/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.90.8/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.90.8/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/outlier_tools/outlier_corrector_location_advanced.py` & `Simba-UW-tf-dev-1.90.8/simba/outlier_tools/outlier_corrector_movement_advanced.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,95 @@
 __author__ = "Simon Nilsson"
 
-import glob
 import os
-from copy import deepcopy
 from typing import Union
 
 import numpy as np
 import pandas as pd
-from numba import jit, prange
+
+try:
+    from typing import Literal
+except:
+    from typing_extensions import Literal
+
+from copy import deepcopy
 
 from simba.mixins.config_reader import ConfigReader
 from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
 from simba.utils.enums import TagNames
 from simba.utils.errors import InvalidInputError, NoFilesFoundError
 from simba.utils.printing import SimbaTimer, log_event, stdout_success
 from simba.utils.read_write import (find_files_of_filetypes_in_directory,
                                     get_fn_ext, read_df, write_df)
 
 
-class OutlierCorrecterLocationAdvanced(ConfigReader, FeatureExtractionMixin):
+class OutlierCorrecterMovementAdvanced(ConfigReader, FeatureExtractionMixin):
     """
-    Performs location outlier correction that allows different heuristic outlier criteria for different animals or body-parts.
-    For example, correct some outlier body-parts with a location heuristic criteria of 4x above the mean movement,
-    and other body-parts with a heuristic critera of 2x above the mean movement.
+    Performs outlier correction that allows different heuristic outlier criteria for different animals or body-parts.
+    For example, correct some outlier body-parts with a movement heuristic criteria of 2x above the mean movement,
+    and other body-parts with a heuristic critera of 1.5x above the mean movement.
 
     .. note::
        See `notebook <https://simba-uw-tf-dev.readthedocs.io/en/latest/nb/advanced_outlier_correction.html>`__. for example use-case.
 
-    .. image:: _static/img/location_outlier.png
+    .. image:: _static/img/movement_outlier.png
        :width: 400
        :align: center
 
     :parameter str config_path: path to SimBA project config file in Configparser format.
     :parameter str input_dir: Directory containing input files. E.g., `project_folder/csv/input_csv` directory.
     :parameter Literal['animal', 'body-part'] type: If the rules are defined on animal or body-part level. E.g., If one heuristic rule per animal then `animal`. If one heurstic rule prr body-part then `body-parts`
     :parameter Literal['mean', 'median'] agg_method: If to use the mean or median to compute criterion.
     :parameter dict criterion_body_parts: The body-parts used to calculate the size of the animals.
     :parameter dict settings: The heuristic multiplier rules to use for each body part or animal.
 
     :example:
     >>> settings = {'Simon': 1.1, 'JJ': 1.2}
     >>> criterion_body_parts = {'Simon': ['Nose_1', 'Tail_base_1'], 'JJ': ['Nose_2', 'Tail_base_2']}
-    >>> outlier_corrector = OutlierCorrecterLocationAdvanced(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', input_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/input_csv', type='animal', agg_method='mean', criterion_body_parts=criterion_body_parts, settings=settings)
+    >>> outlier_corrector = OutlierCorrecterMovementAdvanced(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', input_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/input_csv', type='animal', agg_method='mean', criterion_body_parts=criterion_body_parts, settings=settings)
     >>> outlier_corrector.run()
     >>> settings = {'Simon': {'Ear_left_1': 1.1, 'Ear_right_1': 5.1, 'Nose_1': 2.1, 'Center_1': 1.5, 'Lat_left_1': 3.1, 'Lat_right_1': 1.9, 'Tail_base_1': 2.3, 'Tail_end_1': 1.4}, 'JJ': {'Ear_left_2': 1.2, 'Ear_right_2': 1.2, 'Nose_2': 2, 'Center_2': 4.1, 'Lat_left_2': 9, 'Lat_right_2': 1.2, 'Tail_base_2': 1.6, 'Tail_end_2': 2.2}}
-    >>> outlier_corrector = OutlierCorrecterLocationAdvanced(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', input_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/input_csv', type='body-part', agg_method='mean', criterion_body_parts=criterion_body_parts, settings=settings)
+    >>> outlier_corrector = OutlierCorrecterMovementAdvanced(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', input_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/input_csv', type='body-part', agg_method='mean', criterion_body_parts=criterion_body_parts, settings=settings)
     """
 
     def __init__(
         self,
         config_path: Union[str, os.PathLike],
         input_dir: Union[str, os.PathLike],
-        type: str,
-        agg_method: str,
         criterion_body_parts: dict,
+        type: Literal["animal", "body-part"],
+        agg_method: Literal["mean", "median"],
         settings: dict,
     ):
         ConfigReader.__init__(self, config_path=config_path)
         FeatureExtractionMixin.__init__(self)
         log_event(
             logger_name=str(self.__class__.__name__),
             log_type=TagNames.CLASS_INIT.value,
             msg=self.create_log_msg_from_init_args(locals=locals()),
         )
+        if type not in ["animal", "body-parts"]:
+            raise InvalidInputError(
+                msg=f"Type {type} not supported. Valid options: {['animal', 'body-parts']}"
+            )
+        if agg_method not in ["mean", "median"]:
+            raise InvalidInputError(
+                msg=f"Aggregation method {agg_method} not supported. Valid options: {['mean', 'median']}"
+            )
         self.data_files = find_files_of_filetypes_in_directory(
             directory=input_dir, extensions=["." + self.file_type]
         )
         if len(self.data_files) == 0:
             raise NoFilesFoundError(
                 msg=f"No data of filetype {input_dir} for in directory {self.file_type}",
                 source=self.__class__.__name__,
             )
-        if type not in ["animal", "body-parts"]:
-            raise InvalidInputError(
-                msg=f"Type {type} not supported. Valid options: {['animal', 'body-parts']}",
-                source=self.__class__.__name__,
-            )
-        if agg_method not in ["mean", "median"]:
-            raise InvalidInputError(
-                msg=f"Aggregation method {agg_method} not supported. Valid options: {['mean', 'median']}",
-                source=self.__class__.__name__,
-            )
-        self.settings, self.type, self.agg_method, self.criterion_body_parts = (
-            settings,
-            type,
-            agg_method,
+        self.settings, self.type, self.agg_method = settings, type, agg_method
+        self.save_path, self.criterion_body_parts = (
+            self.outlier_corrected_movement_dir,
             criterion_body_parts,
         )
 
     def fix_settings_for_animal_input(self):
         new_settings = {}
         for animal_name, animal_bps in self.animal_bp_dict.items():
             if animal_name in self.settings.keys():
@@ -96,59 +97,47 @@
                     new_settings[animal_name] = {}
                 for body_part in animal_bps["X_bps"]:
                     new_settings[animal_name][body_part[:-2]] = self.settings[
                         animal_name
                     ]
         self.settings = new_settings
 
-    @staticmethod
-    @jit(nopython=True)
-    def three_dim_cdist(data: np.ndarray) -> np.ndarray:
-        results = np.full((data.shape[0], data.shape[1], data.shape[1]), np.nan)
-        for i in prange(data.shape[0]):
-            for j in prange(data[i].shape[0]):
-                for k in prange(data[i].shape[0]):
-                    results[i][j][k] = np.linalg.norm(data[i][j] - data[i][k])
-
-        return results
-
     def _save_data_log(self, data_log: dict):
         out = pd.DataFrame(
             columns=[
                 "VIDEO",
                 "ANIMAL",
                 "BODY-PART",
                 "OUTLIER COUNT",
                 "OUTLIER RATIO (%)",
             ]
         )
         save_path = os.path.join(
-            self.logs_path, f"location_outliers_{self.datetime}.csv"
+            self.logs_path, f"movement_outliers_{self.datetime}.csv"
         )
         for video_name, video_data in data_log.items():
             for animal_name, animal_data in video_data.items():
                 for body_part_name, body_part_data in animal_data.items():
                     out.loc[len(out)] = [
                         video_name,
                         animal_name,
                         body_part_name,
                         body_part_data["outlier_cnt"],
                         body_part_data["outlier_ratio"],
                     ]
         write_df(df=out, file_type="csv", save_path=save_path)
         stdout_success(
-            msg=f"Location outlier log saved at {save_path}",
+            msg=f"Movement outlier log saved at {save_path}",
             source=self.__class__.__name__,
         )
 
     def run(self):
         data_log = {}
         if self.type == "animal":
             self.fix_settings_for_animal_input()
-
         for file_cnt, file_path in enumerate(self.data_files):
             video_timer, video_log = SimbaTimer(start=True), {}
             _, self.video_name, _ = get_fn_ext(file_path)
             print(
                 "Processing video {}. Video {}/{}...".format(
                     self.video_name, str(file_cnt + 1), str(len(self.data_files))
                 )
@@ -156,123 +145,103 @@
             self.data_df = read_df(file_path, self.file_type, check_multiindex=True)
             self.data_df = self.insert_column_headers_for_outlier_correction(
                 data_df=self.data_df, new_headers=self.bp_headers, filepath=file_path
             )
             self.results = deepcopy(self.data_df)
             self.data_df_combined = self.create_shifted_df(df=self.data_df)
             animal_movement_agg = {}
+            self.movements = pd.DataFrame()
             for animal_name, animal_bps in self.animal_bp_dict.items():
                 if animal_name in self.criterion_body_parts.keys():
+                    animal_bp_headers = np.array(
+                        [
+                            item
+                            for pair in zip(animal_bps["X_bps"], animal_bps["Y_bps"])
+                            for item in pair
+                        ]
+                    ).reshape(len(animal_bps["X_bps"]), 2)
                     animal_criterion_bps = self.criterion_body_parts[animal_name]
                     bp_1_headers = [
                         animal_criterion_bps[0] + "_x",
                         animal_criterion_bps[0] + "_y",
                     ]
                     bp_2_headers = [
                         animal_criterion_bps[1] + "_x",
                         animal_criterion_bps[1] + "_y",
                     ]
+                    print(self.data_df.columns)
                     distances = self.framewise_euclidean_distance(
                         location_1=self.data_df[bp_1_headers].values,
                         location_2=self.data_df[bp_2_headers].values,
                         px_per_mm=1,
                     )
                     if self.agg_method == "mean":
                         animal_movement_agg[animal_name] = np.mean(distances).astype(
                             int
                         )
                     if self.agg_method == "median":
                         animal_movement_agg[animal_name] = np.median(distances).astype(
                             int
                         )
+                    for bps in animal_bp_headers:
+                        bp_name = bps[0][:-2]
+                        shifted_bps = [bps[0] + "_shifted", bps[1] + "_shifted"]
+                        distances = self.framewise_euclidean_distance(
+                            location_1=self.data_df_combined[bps].values,
+                            location_2=self.data_df_combined[shifted_bps].values,
+                            px_per_mm=1,
+                        )
+                        self.movements[bp_name] = distances
 
             for animal_name, animal_bps in self.settings.items():
                 video_log[animal_name] = {}
-                animal_bp_headers = np.array(
-                    [
-                        item
-                        for pair in zip(
-                            self.animal_bp_dict[animal_name]["X_bps"],
-                            self.animal_bp_dict[animal_name]["Y_bps"],
-                        )
-                        for item in pair
-                    ]
-                )
-                animal_body_part_names = [
-                    x[:-2] for x in self.animal_bp_dict[animal_name]["X_bps"]
-                ]
-                animal_body_part_dict = {
-                    k: v
-                    for (v, k) in zip(
-                        animal_body_part_names, range(0, len(animal_body_part_names))
-                    )
-                }
-                animal_arr = self.data_df[animal_bp_headers].values.reshape(
-                    len(self.data_df), -1, 2
-                )
-                data = self.three_dim_cdist(data=animal_arr)
-                df = (
-                    pd.concat(
-                        [pd.DataFrame(arr) for arr in data], keys=np.arange(len(data))
-                    )
-                    .reset_index()
-                    .rename(columns={"level_0": "frame", "level_1": "body_part"})
-                )
-                df["body_part"] = df["body_part"].map(animal_body_part_dict)
-                above_criterion_dict = {}
                 for bp, criterion_multiplier in animal_bps.items():
                     if animal_name in animal_movement_agg.keys():
                         bp_criterion = (
                             animal_movement_agg[animal_name] * criterion_multiplier
                         )
-                        bp_df = df[df["body_part"] == bp]
-                        bp_df["counts_above_criterion"] = self.count_values_in_range(
-                            data=bp_df.drop(["frame", "body_part"], axis=1).values,
-                            ranges=np.array([[bp_criterion, np.inf]]),
+                        over_criterion_idx = list(
+                            self.movements.index[self.movements[bp] > bp_criterion]
                         )
-                        above_criterion_dict[bp] = list(
-                            bp_df["frame"][bp_df["counts_above_criterion"] > 1]
+                        video_log[animal_name][bp] = {
+                            "outlier_cnt": len(over_criterion_idx),
+                            "outlier_ratio": len(over_criterion_idx)
+                            / len(self.movements),
+                        }
+                        self.results.loc[over_criterion_idx, [bp + "_x", bp + "_y"]] = (
+                            np.nan
+                        )
+                        self.results[[bp + "_x", bp + "_y"]] = (
+                            self.results[[bp + "_x", bp + "_y"]]
+                            .ffill()
+                            .bfill()
+                            .astype(int)
                         )
-
-                for (
-                    bp,
-                    body_part_frames_above_criterion,
-                ) in above_criterion_dict.items():
-                    self.results.loc[
-                        body_part_frames_above_criterion, [f"{bp}_x", f"{bp}_y"]
-                    ] = np.nan
-                    self.results[[f"{bp}_x", f"{bp}_y"]] = (
-                        self.results[[f"{bp}_x", f"{bp}_y"]].ffill().bfill().astype(int)
-                    )
-                    video_log[animal_name][bp] = {
-                        "outlier_cnt": len(body_part_frames_above_criterion),
-                        "outlier_ratio": len(body_part_frames_above_criterion)
-                        / len(self.results),
-                    }
 
             df_save_path = os.path.join(
-                self.outlier_corrected_dir, self.video_name + f"{self.file_type}."
+                self.outlier_corrected_movement_dir,
+                self.video_name + f".{self.file_type}",
             )
             write_df(df=self.results, file_type=self.file_type, save_path=df_save_path)
             video_timer.stop_timer()
             stdout_success(
-                msg=f"Location outliers complete for video {self.video_name}.",
+                msg=f"Movement outliers complete for video {self.video_name}.",
                 elapsed_time=video_timer.elapsed_time_str,
                 source=self.__class__.__name__,
             )
             data_log[self.video_name] = video_log
-
         self._save_data_log(data_log=data_log)
         stdout_success(
-            msg=f"{len(self.data_files)} video(s) corrected for location outliers. Saved in {self.outlier_corrected_dir}",
+            msg=f"{len(self.data_files)} video(s) corrected for movement outliers. Saved in {self.outlier_corrected_movement_dir}",
             source=self.__class__.__name__,
         )
 
 
-# settings = {'Simon': 2.5} #
+#
+# settings = {'Simon': 2.5} #'JJ': 1.2
 # # settings = {'Simon': {'Ear_left_1': 1.1,
 # #                       'Ear_right_1': 5.1,
 # #                       'Nose_1': 2.1,
 # #                       'Center_1': 1.5,
 # #                       'Lat_left_1': 3.1,
 # #                       'Lat_right_1': 1.9,
 # #                       'Tail_base_1': 2.3},
@@ -281,19 +250,19 @@
 # #                       'Ear_right_2': 1.2,
 # #                       'Nose_2': 2,
 # #                       'Center_2': 4.1,
 # #                       'Lat_left_2': 9,
 # #                       'Lat_right_2': 1.2,
 # #                       'Tail_base_2': 1.6,
 # #                       'Tail_end_2': 2.2}}
-# criterion_body_parts = {'Simon': ['Nose_1', 'Tail_base_1'], } #'JJ': ['Nose_2', 'Tail_base_2']
-# test = OutlierCorrecterLocationAdvanced(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
+# criterion_body_parts = {'Simon': ['Nose_1', 'Tail_base_1']} #'JJ': ['Nose_2', 'Tail_base_2']
+#
+#
+# test = OutlierCorrecterMovementAdvanced(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                         input_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/input_csv',
+#                                         criterion_body_parts=criterion_body_parts,
 #                                         type='animal',
 #                                         agg_method='mean',
-#                                         criterion_body_parts=criterion_body_parts,
 #                                         settings=settings)
 # test.run()
 
-
-# test = OutlierCorrecterLocation(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
-# test.correct_location_outliers()
+#
```

### Comparing `Simba-UW-tf-dev-1.90.7/simba/outlier_tools/outlier_corrector_movement_advanced.py` & `Simba-UW-tf-dev-1.90.8/simba/data_processors/spontaneous_alternation_calculator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,268 +1,182 @@
-__author__ = "Simon Nilsson"
-
+import argparse
 import os
-from typing import Union
+import warnings
+from typing import List, Optional, Union
 
 import numpy as np
 import pandas as pd
 
-try:
-    from typing import Literal
-except:
-    from typing_extensions import Literal
+warnings.filterwarnings("ignore")
 
-from copy import deepcopy
+import multiprocessing
+import platform
 
 from simba.mixins.config_reader import ConfigReader
-from simba.mixins.feature_extraction_mixin import FeatureExtractionMixin
-from simba.utils.enums import TagNames
-from simba.utils.errors import InvalidInputError, NoFilesFoundError
-from simba.utils.printing import SimbaTimer, log_event, stdout_success
-from simba.utils.read_write import (find_files_of_filetypes_in_directory,
-                                    get_fn_ext, read_df, write_df)
+from simba.mixins.feature_extraction_supplement_mixin import \
+    FeatureExtractionSupplemental
+from simba.mixins.geometry_mixin import GeometryMixin
+from simba.utils.checks import (check_float, check_int, check_str,
+                                check_valid_lst, check_video_has_rois, check_all_file_names_are_represented_in_video_log)
+from simba.utils.errors import (AnimalNumberError, InvalidInputError,
+                                NoFilesFoundError, ROICoordinatesNotFoundError)
+from simba.utils.printing import stdout_success
+from simba.utils.read_write import (get_fn_ext, read_df, read_data_paths)
+
+from simba.utils.warnings import NoFileFoundWarning
+
+TAIL_END = "tail_end"
 
 
-class OutlierCorrecterMovementAdvanced(ConfigReader, FeatureExtractionMixin):
+class SpontaneousAlternationCalculator(ConfigReader):
     """
-    Performs outlier correction that allows different heuristic outlier criteria for different animals or body-parts.
-    For example, correct some outlier body-parts with a movement heuristic criteria of 2x above the mean movement,
-    and other body-parts with a heuristic critera of 1.5x above the mean movement.
+    Compute spontaneous alternations based on specified ROIs and animal detection parameters.
 
     .. note::
-       See `notebook <https://simba-uw-tf-dev.readthedocs.io/en/latest/nb/advanced_outlier_correction.html>`__. for example use-case.
-
-    .. image:: _static/img/movement_outlier.png
-       :width: 400
-       :align: center
-
-    :parameter str config_path: path to SimBA project config file in Configparser format.
-    :parameter str input_dir: Directory containing input files. E.g., `project_folder/csv/input_csv` directory.
-    :parameter Literal['animal', 'body-part'] type: If the rules are defined on animal or body-part level. E.g., If one heuristic rule per animal then `animal`. If one heurstic rule prr body-part then `body-parts`
-    :parameter Literal['mean', 'median'] agg_method: If to use the mean or median to compute criterion.
-    :parameter dict criterion_body_parts: The body-parts used to calculate the size of the animals.
-    :parameter dict settings: The heuristic multiplier rules to use for each body part or animal.
+       This method computes spontaneous alternation by fitting the smallest viable geometry (a.k.a. shape, polygon) that
+       encompasses the animal key-points (but see buffer parameter below). It then checks the percent overlap between the
+       animal geometry and the defined arm and center geometries in each frame. If the percent overlap is more or equal to the
+       specified threshold, then the animal considered to visiting the relevant arm. The animal is considered exiting an arm
+       when the percent overlap with a different ROI is above the threshold.
+
+    .. attention::
+       Requires SimBA project with (i) only one tracked animal, (ii) at least three pose-estmated body-parts, and (iii) defined
+       ROIs representing the arms and the center of the maze.
+
+    :param Union[str, os.PathLike] config_path: Path to SimBA project config file.
+    :param List[str] arm_names: List of ROI names representing the arms.
+    :param str center_name: Name of the ROI representing the center of the maze
+    :param Optional[int] animal_area: Value between 51 and 100, representing the percent of the animal body that has to be situated in a ROI for it to be considered an entry.
+    :param Optional[float] threshold: Value between 0.0 and 1.0. Body-parts with detection probabilities below this value will be (if possible) filtered when constructing the animal geometry.
+    :param Optional[int] buffer: Millimeters area for which the animal geometry should be increased in size. Useful if the animal geometry does not fully cover the animal.
+    :param Optional[bool] detailed_data: If True, saves an additional CSV for each analyzed video with detailed data pertaining each error type and alternation sequence.
+    :param Optional[Union[str, os.PathLike]] data_path: Directory of path to the file to be analyzed. If None, then ``project_folder/outlier_corrected_movement_location`` directory.
 
     :example:
-    >>> settings = {'Simon': 1.1, 'JJ': 1.2}
-    >>> criterion_body_parts = {'Simon': ['Nose_1', 'Tail_base_1'], 'JJ': ['Nose_2', 'Tail_base_2']}
-    >>> outlier_corrector = OutlierCorrecterMovementAdvanced(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', input_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/input_csv', type='animal', agg_method='mean', criterion_body_parts=criterion_body_parts, settings=settings)
-    >>> outlier_corrector.run()
-    >>> settings = {'Simon': {'Ear_left_1': 1.1, 'Ear_right_1': 5.1, 'Nose_1': 2.1, 'Center_1': 1.5, 'Lat_left_1': 3.1, 'Lat_right_1': 1.9, 'Tail_base_1': 2.3, 'Tail_end_1': 1.4}, 'JJ': {'Ear_left_2': 1.2, 'Ear_right_2': 1.2, 'Nose_2': 2, 'Center_2': 4.1, 'Lat_left_2': 9, 'Lat_right_2': 1.2, 'Tail_base_2': 1.6, 'Tail_end_2': 2.2}}
-    >>> outlier_corrector = OutlierCorrecterMovementAdvanced(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini', input_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/input_csv', type='body-part', agg_method='mean', criterion_body_parts=criterion_body_parts, settings=settings)
+    >>> x = SpontaneousAlternationCalculator(config_path='/Users/simon/Desktop/envs/simba/troubleshooting/spontenous_alternation/project_folder/project_config.ini', arm_names=['A', 'B', 'C'], center_name='Center', threshold=0.0, animal_area=100, buffer=2, detailed_data=True)
+    >>> x.run()
+    >>> x.save()
     """
 
-    def __init__(
-        self,
-        config_path: Union[str, os.PathLike],
-        input_dir: Union[str, os.PathLike],
-        criterion_body_parts: dict,
-        type: Literal["animal", "body-part"],
-        agg_method: Literal["mean", "median"],
-        settings: dict,
-    ):
+    def __init__(self,
+                 config_path: Union[str, os.PathLike],
+                 arm_names: List[str],
+                 center_name: str,
+                 animal_area: Optional[int] = 80,
+                 threshold: Optional[float] = 0.0,
+                 buffer: Optional[int] = 2,
+                 verbose: Optional[bool] = False,
+                 detailed_data: Optional[bool] = False,
+                 data_path: Optional[Union[str, os.PathLike]] = None):
+
         ConfigReader.__init__(self, config_path=config_path)
-        FeatureExtractionMixin.__init__(self)
-        log_event(
-            logger_name=str(self.__class__.__name__),
-            log_type=TagNames.CLASS_INIT.value,
-            msg=self.create_log_msg_from_init_args(locals=locals()),
-        )
-        if type not in ["animal", "body-parts"]:
-            raise InvalidInputError(
-                msg=f"Type {type} not supported. Valid options: {['animal', 'body-parts']}"
-            )
-        if agg_method not in ["mean", "median"]:
-            raise InvalidInputError(
-                msg=f"Aggregation method {agg_method} not supported. Valid options: {['mean', 'median']}"
-            )
-        self.data_files = find_files_of_filetypes_in_directory(
-            directory=input_dir, extensions=["." + self.file_type]
-        )
-        if len(self.data_files) == 0:
-            raise NoFilesFoundError(
-                msg=f"No data of filetype {input_dir} for in directory {self.file_type}",
-                source=self.__class__.__name__,
-            )
-        self.settings, self.type, self.agg_method = settings, type, agg_method
-        self.save_path, self.criterion_body_parts = (
-            self.outlier_corrected_movement_dir,
-            criterion_body_parts,
-        )
-
-    def fix_settings_for_animal_input(self):
-        new_settings = {}
-        for animal_name, animal_bps in self.animal_bp_dict.items():
-            if animal_name in self.settings.keys():
-                if animal_name not in new_settings.keys():
-                    new_settings[animal_name] = {}
-                for body_part in animal_bps["X_bps"]:
-                    new_settings[animal_name][body_part[:-2]] = self.settings[
-                        animal_name
-                    ]
-        self.settings = new_settings
-
-    def _save_data_log(self, data_log: dict):
-        out = pd.DataFrame(
-            columns=[
-                "VIDEO",
-                "ANIMAL",
-                "BODY-PART",
-                "OUTLIER COUNT",
-                "OUTLIER RATIO (%)",
-            ]
-        )
-        save_path = os.path.join(
-            self.logs_path, f"movement_outliers_{self.datetime}.csv"
-        )
-        for video_name, video_data in data_log.items():
-            for animal_name, animal_data in video_data.items():
-                for body_part_name, body_part_data in animal_data.items():
-                    out.loc[len(out)] = [
-                        video_name,
-                        animal_name,
-                        body_part_name,
-                        body_part_data["outlier_cnt"],
-                        body_part_data["outlier_ratio"],
-                    ]
-        write_df(df=out, file_type="csv", save_path=save_path)
-        stdout_success(
-            msg=f"Movement outlier log saved at {save_path}",
-            source=self.__class__.__name__,
-        )
+        if self.animal_cnt != 1:
+            raise AnimalNumberError(msg=f"Spontaneous alternation can only be calculated in 1 animal projects. Your project has {self.animal_cnt} animals.", source=self.__class__.__name__)
+        if len(self.body_parts_lst) < 3:
+            raise InvalidInputError(msg=f"Spontaneous alternation can only be calculated in projects with 3 or more tracked body-parts. Found {len(self.body_parts_lst)}.", source=self.__class__.__name__)
+        if not os.path.isfile(self.roi_coordinates_path):
+            raise ROICoordinatesNotFoundError(expected_file_path=self.roi_coordinates_path)
+        check_valid_lst(data=arm_names, source=SpontaneousAlternationCalculator.__name__, valid_dtypes=(str,), min_len=2)
+        check_str(name="CENTER NAME", value=center_name)
+        check_int(name="ANIMAL AREA", value=animal_area, min_value=51, max_value=100)
+        check_float(name="THRESHOLD", value=threshold, min_value=0.0, max_value=1.0)
+        check_int(name="BUFFER", value=buffer, min_value=1)
+        data_paths = read_data_paths(path=data_path, default=self.outlier_corrected_paths, default_name=self.outlier_corrected_dir, file_type=self.file_type)
+        file_paths = {}
+        for file_path in data_paths: file_paths[get_fn_ext(file_path)[1]] = file_path
+        self.read_roi_data()
+        files_w_missing_rois = list(set(file_paths.keys()) - set(self.video_names_w_rois))
+        self.files_w_rois = [x for x in list(file_paths.keys()) if x in self.video_names_w_rois]
+        if len(self.files_w_rois) == 0:
+            raise NoFilesFoundError(msg=f"No ROI definitions found for any of the data fat {arm_names}", source=__class__.__name__,)
+        if len(files_w_missing_rois) > 0:
+            NoFileFoundWarning(msg=f"{len(files_w_missing_rois)} file(s) at {data_path} are missing ROI definitions and will be skipped when performing spontaneous alternation calculations: {files_w_missing_rois}", source=__class__.__name__)
+        check_video_has_rois(roi_dict=self.roi_dict, video_names=self.files_w_rois, roi_names=arm_names + [center_name],)
+        self.file_paths = list({file_paths[k] for k in self.files_w_rois if k in file_paths})
+        self.threshold, self.buffer, self.animal_area, self.detailed_data = threshold, buffer, animal_area, detailed_data
+        self.verbose, self.center_name, self.arm_names = verbose, center_name, arm_names
 
     def run(self):
-        data_log = {}
-        if self.type == "animal":
-            self.fix_settings_for_animal_input()
-        for file_cnt, file_path in enumerate(self.data_files):
-            video_timer, video_log = SimbaTimer(start=True), {}
-            _, self.video_name, _ = get_fn_ext(file_path)
-            print(
-                "Processing video {}. Video {}/{}...".format(
-                    self.video_name, str(file_cnt + 1), str(len(self.data_files))
-                )
-            )
-            self.data_df = read_df(file_path, self.file_type, check_multiindex=True)
-            self.data_df = self.insert_column_headers_for_outlier_correction(
-                data_df=self.data_df, new_headers=self.bp_headers, filepath=file_path
-            )
-            self.results = deepcopy(self.data_df)
-            self.data_df_combined = self.create_shifted_df(df=self.data_df)
-            animal_movement_agg = {}
-            self.movements = pd.DataFrame()
-            for animal_name, animal_bps in self.animal_bp_dict.items():
-                if animal_name in self.criterion_body_parts.keys():
-                    animal_bp_headers = np.array(
-                        [
-                            item
-                            for pair in zip(animal_bps["X_bps"], animal_bps["Y_bps"])
-                            for item in pair
-                        ]
-                    ).reshape(len(animal_bps["X_bps"]), 2)
-                    animal_criterion_bps = self.criterion_body_parts[animal_name]
-                    bp_1_headers = [
-                        animal_criterion_bps[0] + "_x",
-                        animal_criterion_bps[0] + "_y",
-                    ]
-                    bp_2_headers = [
-                        animal_criterion_bps[1] + "_x",
-                        animal_criterion_bps[1] + "_y",
-                    ]
-                    print(self.data_df.columns)
-                    distances = self.framewise_euclidean_distance(
-                        location_1=self.data_df[bp_1_headers].values,
-                        location_2=self.data_df[bp_2_headers].values,
-                        px_per_mm=1,
-                    )
-                    if self.agg_method == "mean":
-                        animal_movement_agg[animal_name] = np.mean(distances).astype(
-                            int
-                        )
-                    if self.agg_method == "median":
-                        animal_movement_agg[animal_name] = np.median(distances).astype(
-                            int
-                        )
-                    for bps in animal_bp_headers:
-                        bp_name = bps[0][:-2]
-                        shifted_bps = [bps[0] + "_shifted", bps[1] + "_shifted"]
-                        distances = self.framewise_euclidean_distance(
-                            location_1=self.data_df_combined[bps].values,
-                            location_2=self.data_df_combined[shifted_bps].values,
-                            px_per_mm=1,
-                        )
-                        self.movements[bp_name] = distances
-
-            for animal_name, animal_bps in self.settings.items():
-                video_log[animal_name] = {}
-                for bp, criterion_multiplier in animal_bps.items():
-                    if animal_name in animal_movement_agg.keys():
-                        bp_criterion = (
-                            animal_movement_agg[animal_name] * criterion_multiplier
-                        )
-                        over_criterion_idx = list(
-                            self.movements.index[self.movements[bp] > bp_criterion]
-                        )
-                        video_log[animal_name][bp] = {
-                            "outlier_cnt": len(over_criterion_idx),
-                            "outlier_ratio": len(over_criterion_idx)
-                            / len(self.movements),
-                        }
-                        self.results.loc[over_criterion_idx, [bp + "_x", bp + "_y"]] = (
-                            np.nan
-                        )
-                        self.results[[bp + "_x", bp + "_y"]] = (
-                            self.results[[bp + "_x", bp + "_y"]]
-                            .ffill()
-                            .bfill()
-                            .astype(int)
-                        )
-
-            df_save_path = os.path.join(
-                self.outlier_corrected_movement_dir,
-                self.video_name + f".{self.file_type}",
-            )
-            write_df(df=self.results, file_type=self.file_type, save_path=df_save_path)
-            video_timer.stop_timer()
-            stdout_success(
-                msg=f"Movement outliers complete for video {self.video_name}.",
-                elapsed_time=video_timer.elapsed_time_str,
-                source=self.__class__.__name__,
-            )
-            data_log[self.video_name] = video_log
-        self._save_data_log(data_log=data_log)
-        stdout_success(
-            msg=f"{len(self.data_files)} video(s) corrected for movement outliers. Saved in {self.outlier_corrected_movement_dir}",
-            source=self.__class__.__name__,
-        )
-
-
-#
-# settings = {'Simon': 2.5} #'JJ': 1.2
-# # settings = {'Simon': {'Ear_left_1': 1.1,
-# #                       'Ear_right_1': 5.1,
-# #                       'Nose_1': 2.1,
-# #                       'Center_1': 1.5,
-# #                       'Lat_left_1': 3.1,
-# #                       'Lat_right_1': 1.9,
-# #                       'Tail_base_1': 2.3},
-# #                       #'Tail_end_1': 1.4},
-# #                'JJ': {'Ear_left_2': 1.2,
-# #                       'Ear_right_2': 1.2,
-# #                       'Nose_2': 2,
-# #                       'Center_2': 4.1,
-# #                       'Lat_left_2': 9,
-# #                       'Lat_right_2': 1.2,
-# #                       'Tail_base_2': 1.6,
-# #                       'Tail_end_2': 2.2}}
-# criterion_body_parts = {'Simon': ['Nose_1', 'Tail_base_1']} #'JJ': ['Nose_2', 'Tail_base_2']
-#
-#
-# test = OutlierCorrecterMovementAdvanced(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
-#                                         input_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/input_csv',
-#                                         criterion_body_parts=criterion_body_parts,
-#                                         type='animal',
-#                                         agg_method='mean',
-#                                         settings=settings)
-# test.run()
-
+        roi_geos, self.roi_clrs = GeometryMixin.simba_roi_to_geometries(rectangles_df=self.rectangles_df, circles_df=self.circles_df, polygons_df=self.polygon_df, color=True)
+        self.roi_geos = {k: v for k, v in roi_geos.items() if k in self.files_w_rois}
+        self.results = {}
+        check_all_file_names_are_represented_in_video_log(video_info_df=self.video_info_df, data_paths=self.file_paths)
+        for file_path in self.file_paths:
+            _, self.video_name, _ = get_fn_ext(filepath=file_path)
+            _, px_per_mm, fps = self.read_video_info(video_name=self.video_name)
+            self.data_df = read_df(file_path=file_path, file_type=self.file_type)
+            bp_df = self.data_df[[x for x in self.bp_headers if not x.endswith("_p") and not TAIL_END in x.lower()]]
+            p_df = self.data_df[[x for x in self.bp_headers if x.endswith("_p") and not TAIL_END in x.lower()]]
+            bp_arr = bp_df.values.reshape(len(bp_df), int(len(bp_df.columns) / 2), 2).astype(np.int64)
+            p_arr = p_df.values.reshape(len(p_df), len(p_df.columns), 1)
+            if self.threshold > 0.0:
+                bp_arr = GeometryMixin.filter_low_p_bps_for_shapes(x=bp_arr, p=p_arr, threshold=self.threshold).reshape(bp_arr.shape[0], -1, 2)
+            self.animal_polygons = GeometryMixin().multiframe_bodyparts_to_polygon(data=bp_arr,
+                                                                                   parallel_offset=self.buffer,
+                                                                                   pixels_per_mm=px_per_mm,
+                                                                                   video_name=self.video_name,
+                                                                                   animal_name="Animal",
+                                                                                   verbose=self.verbose)
+            self.roi_df = pd.DataFrame()
+            for geo_name, geo in self.roi_geos[self.video_name].items():
+                roi_geo = [geo for x in range(len(self.animal_polygons))]
+                pct_overlap = np.array(GeometryMixin().multiframe_compute_pct_shape_overlap(shape_1=self.animal_polygons,
+                                                                                            shape_2=roi_geo,
+                                                                                            denominator="shape_1",
+                                                                                            verbose=self.verbose,
+                                                                                            animal_names=geo_name,
+                                                                                            video_name=self.video_name))
+                frames_in_roi = np.zeros(pct_overlap.shape)
+                frames_in_roi[np.argwhere(pct_overlap >= self.animal_area)] = 1
+                self.roi_df[geo_name] = frames_in_roi
+
+            self.video_results = FeatureExtractionSupplemental.spontaneous_alternations(data=self.roi_df, arm_names=self.arm_names, center_name=self.center_name)
+            self.results[self.video_name] = self.video_results
+
+    def save(self):
+        print("Running alternation analysis...")
+        results_df = pd.DataFrame(columns=["VIDEO NAME","ALTERNATION RATE","ALTERNATION COUNT","ERROR COUNT","SAME ARM RETURN ERRORS","ALTERNATE ARM RETURN ERRORS"])
+        save_path = os.path.join(self.logs_path, f"spontaneous_alternation_{self.datetime}.csv")
+        for video_name, d in self.results.items():
+            results_df.loc[len(results_df)] = [video_name, d["pct_alternation"], d["alternation_cnt"], d["error_cnt"], d["same_arm_returns_cnt"], d["alternate_arm_returns_cnt"]]
+        results_df.set_index("VIDEO NAME").to_csv(save_path)
+        stdout_success(msg=f"Spontaneous alternation data for {len(list(self.results.keys()))} video(s) saved at {save_path}")
+        if self.detailed_data:
+            save_dir = os.path.join(self.logs_path, f"detailed_spontaneous_alternation_data_{self.datetime}")
+            sliced_keys = ["same_arm_returns_dict","alternate_arm_returns_dict","alternations_dict"]
+            replace_keys = {"same_arm_returns_dict": "same arm return","alternate_arm_returns_dict": "alternate arm return","alternations_dict": "alternations",}
+            os.makedirs(save_dir)
+            print(self.results)
+            for video_name, d in self.results.items():
+                details_path = os.path.join(save_dir, f"{video_name}_details.csv")
+                arm_entry_sequence_path = os.path.join(save_dir, f"{video_name}_arm_entry_sequence.csv")
+                sliced_data = {k: v for k, v in d.items() if k in sliced_keys}
+                sliced_data = {replace_keys.get(key, key): value for key, value in sliced_data.items()}
+                row_idx = [(o, i) for o, i in sliced_data.items() for i in i.keys()]
+                values = [v for i in sliced_data.values() for v in i.values()]
+                values = [["" if len(sublist) == 0 else ", ".join(map(str, sublist))] for sublist in values]
+                multi_index = pd.MultiIndex.from_tuples(row_idx, names=["Behavior", "Arm"])
+                df = pd.DataFrame(values, index=multi_index, columns=["Frames"])
+                arm_entry_sequence_df = pd.DataFrame(data=d['arm_entry_sequence'], columns=['ARM_ENTRY_SEQUENCE'])
+                df.to_csv(details_path)
+                arm_entry_sequence_df.to_csv(arm_entry_sequence_path)
+
+            stdout_success(msg=f"Detailed spontaneous alternation data for {len(list(self.results.keys()))} video(s) saved at {save_dir}")
+
+# config_path = '/Users/simon/Desktop/envs/simba/troubleshooting/spontenous_alternation/project_folder/project_config.ini'
+# arm_names = ['A', 'B', 'C']
+# center_name = 'Center'
+# threshold = 0.0
+# animal_area = 60
+# buffer = 2
+# verbose = True
 #
+# x = SpontaneousAlternationCalculator(config_path=config_path,
+#                                      arm_names=arm_names,
+#                                      center_name=center_name,
+#                                      threshold=threshold,
+#                                      detailed_data=True,
+#                                      animal_area=animal_area,
+#                                      buffer=buffer,
+#                                      verbose=verbose)
+# x.run()
+# x.save()
```

### Comparing `Simba-UW-tf-dev-1.90.7/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.90.8/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.90.8/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/SimBA.py` & `Simba-UW-tf-dev-1.90.8/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.90.8/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.90.8/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.90.8/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.90.8/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.90.8/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/lookups/critical_values_05.pickle` & `Simba-UW-tf-dev-1.90.8/simba/assets/lookups/critical_values_05.pickle`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.90.8/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.90.8/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.90.8/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.90.8/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.90.8/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.90.8/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/img/splash_2024.mp4` & `Simba-UW-tf-dev-1.90.8/simba/assets/img/splash_2024.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/img/bg_2024.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/img/bg_2024.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.90.8/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.90.8/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.90.8/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/simba_logo_2.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/simba_logo_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/readthedocs_logo.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/readthedocs_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/circle.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/circle.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/polygon.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/polygon.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.90.8/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.90.8/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.90.8/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.90.8/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.90.7
+Version: 1.90.8
 Summary: Toolkit for computer classification of behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.90.7/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.90.8/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.90.8/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/LICENSE` & `Simba-UW-tf-dev-1.90.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.90.8/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_circlular_stats.py` & `Simba-UW-tf-dev-1.90.8/tests/test_circlular_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_stats.py` & `Simba-UW-tf-dev-1.90.8/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.90.8/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.90.8/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.90.8/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.90.8/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.90.8/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.90.8/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.90.8/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.90.8/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.90.8/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.90.8/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.90.8/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/README.md` & `Simba-UW-tf-dev-1.90.8/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.90.7/setup.py` & `Simba-UW-tf-dev-1.90.8/setup.py`

 * *Files identical despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 exclusion_patterns = ["pose_configurations_archive"]
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.90.7",
+    version="1.90.8",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of behaviors in experimental animals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sgoldenlab/simba",
     install_requires=requirements,
```
