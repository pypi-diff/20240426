# Comparing `tmp/comet_toolbox-0.3.4.tar.gz` & `tmp/comet_toolbox-0.3.5.tar.gz`

## Comparing `comet_toolbox-0.3.4.tar` & `comet_toolbox-0.3.5.tar`

### file list

```diff
@@ -1,248 +1,248 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/.gitattributes
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/adj.mat
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/adj_bin.mat
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/simulation.txt
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/test_template.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/universe_1.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/universe_10.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/universe_11.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/universe_12.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/universe_2.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/universe_3.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/universe_4.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/universe_5.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/universe_6.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/universe_7.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/universe_8.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/universe_9.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/results/forking_paths.pkl
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/example_multiverse/results/multiverse_summary.csv
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/__init__.py
--rwxr-xr-x   0        0        0     3821 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/cifti.py
--rwxr-xr-x   0        0        0     4027 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/data.py
--rw-r--r--   0        0        0    29936 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/graph.py
--rw-r--r--   0        0        0   137181 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/gui.py
--rwxr-xr-x   0        0        0    47496 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/methods.py
--rwxr-xr-x   0        0        0    25135 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/multiverse.py
--rw-r--r--   0        0        0    96617 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/simulation.pkl
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/simulation.txt
--rw-r--r--   0        0        0   192811 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/single_state.txt
--rwxr-xr-x   0        0        0  1038952 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii
--rwxr-xr-x   0        0        0      531 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/atlas/README.md
--rwxr-xr-x   0        0        0  1029992 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii
--rwxr-xr-x   0        0        0   655904 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii
--rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat
--rw-r--r--   0        0        0    40910 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/img/content.drawio
--rw-r--r--   0        0        0   175918 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/img/content.png
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/img/doi.svg
--rw-r--r--   0        0        0   202431 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/img/gui.png
--rw-r--r--   0        0        0   724684 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/img/logo.png
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/src/comet/resources/img/pypi.svg
--rw-r--r--   0        0        0   185059 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/example_analysis.ipynb
--rw-r--r--   0        0        0   450982 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/example_dfc.ipynb
--rw-r--r--   0        0        0  1311678 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/example_graph.ipynb
--rw-r--r--   0        0        0   114703 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/example_multiverse.ipynb
--rw-r--r--   0        0        0   804479 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/example_data/abide_50008.txt
--rw-r--r--   0        0        0   969955 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/example_data/aomic_multi.pkl
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/example_data/simulation.txt
--rw-r--r--   0        0        0  1564386 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/example_data/xcpd.tsv
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_1.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_10.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_11.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_12.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_13.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_14.py
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_15.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_16.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_17.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_18.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_19.py
--rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_2.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_20.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_21.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_22.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_23.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_24.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_25.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_26.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_27.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_28.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_29.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_3.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_30.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_31.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_32.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_33.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_34.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_35.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_36.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_37.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_38.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_39.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_4.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_40.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_41.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_42.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_43.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_44.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_45.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_46.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_47.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_48.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_49.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_5.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_50.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_51.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_52.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_53.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_54.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_55.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_56.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_57.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_58.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_59.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_6.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_60.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_61.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_62.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_63.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_64.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_65.py
--rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_66.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_67.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_68.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_69.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_7.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_70.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_71.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_72.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_73.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_74.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_75.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_76.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_77.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_78.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_79.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_8.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_80.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_81.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_82.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_83.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_84.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_85.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_86.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_87.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_88.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_89.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_9.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_90.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_91.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_92.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_93.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_94.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_95.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/universe_96.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/forking_paths.pkl
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/multiverse_summary.csv
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/pipelines.csv
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_1.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_10.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_11.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_12.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_13.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_14.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_15.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_16.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_17.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_18.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_19.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_2.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_20.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_21.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_22.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_23.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_24.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_25.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_26.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_27.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_28.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_29.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_3.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_30.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_31.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_32.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_33.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_34.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_35.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_36.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_37.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_38.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_39.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_4.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_40.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_41.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_42.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_43.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_44.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_45.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_46.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_47.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_48.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_49.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_5.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_50.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_51.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_52.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_53.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_54.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_55.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_56.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_57.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_58.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_59.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_6.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_60.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_61.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_62.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_63.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_64.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_65.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_66.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_67.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_68.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_69.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_7.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_70.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_71.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_72.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_73.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_74.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_75.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_76.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_77.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_78.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_79.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_8.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_80.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_81.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_82.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_83.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_84.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_85.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_86.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_87.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_88.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_89.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_9.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_90.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_91.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_92.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_93.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_94.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_95.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/tutorials/multiverse/results/universe_96.pkl
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/LICENSE
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/README.md
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 comet_toolbox-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/.gitattributes
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/adj.mat
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/adj_bin.mat
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/simulation.txt
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/test_template.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/universe_1.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/universe_10.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/universe_11.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/universe_12.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/universe_2.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/universe_3.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/universe_4.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/universe_5.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/universe_6.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/universe_7.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/universe_8.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/universe_9.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/results/forking_paths.pkl
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/example_multiverse/results/multiverse_summary.csv
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/__init__.py
+-rwxr-xr-x   0        0        0     3821 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/cifti.py
+-rwxr-xr-x   0        0        0     4027 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/data.py
+-rw-r--r--   0        0        0    29936 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/graph.py
+-rw-r--r--   0        0        0   137236 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/gui.py
+-rwxr-xr-x   0        0        0    47496 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/methods.py
+-rwxr-xr-x   0        0        0    25135 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/multiverse.py
+-rw-r--r--   0        0        0    96617 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/simulation.pkl
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/simulation.txt
+-rw-r--r--   0        0        0   192811 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/single_state.txt
+-rwxr-xr-x   0        0        0  1038952 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii
+-rwxr-xr-x   0        0        0      531 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/atlas/README.md
+-rwxr-xr-x   0        0        0  1029992 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii
+-rwxr-xr-x   0        0        0   655904 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii
+-rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat
+-rw-r--r--   0        0        0    40910 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/img/content.drawio
+-rw-r--r--   0        0        0   175918 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/img/content.png
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/img/doi.svg
+-rw-r--r--   0        0        0   202431 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/img/gui.png
+-rw-r--r--   0        0        0   724684 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/img/logo.png
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/src/comet/resources/img/pypi.svg
+-rw-r--r--   0        0        0   185059 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/example_analysis.ipynb
+-rw-r--r--   0        0        0   450982 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/example_dfc.ipynb
+-rw-r--r--   0        0        0  1311678 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/example_graph.ipynb
+-rw-r--r--   0        0        0   114703 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/example_multiverse.ipynb
+-rw-r--r--   0        0        0   804479 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/example_data/abide_50008.txt
+-rw-r--r--   0        0        0   969955 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/example_data/aomic_multi.pkl
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/example_data/simulation.txt
+-rw-r--r--   0        0        0  1564386 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/example_data/xcpd.tsv
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_1.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_10.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_11.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_12.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_13.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_14.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_15.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_16.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_17.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_18.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_19.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_2.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_20.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_21.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_22.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_23.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_24.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_25.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_26.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_27.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_28.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_29.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_3.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_30.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_31.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_32.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_33.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_34.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_35.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_36.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_37.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_38.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_39.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_4.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_40.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_41.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_42.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_43.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_44.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_45.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_46.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_47.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_48.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_49.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_5.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_50.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_51.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_52.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_53.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_54.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_55.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_56.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_57.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_58.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_59.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_6.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_60.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_61.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_62.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_63.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_64.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_65.py
+-rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_66.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_67.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_68.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_69.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_7.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_70.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_71.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_72.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_73.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_74.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_75.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_76.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_77.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_78.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_79.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_8.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_80.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_81.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_82.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_83.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_84.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_85.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_86.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_87.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_88.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_89.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_9.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_90.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_91.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_92.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_93.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_94.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_95.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/universe_96.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/forking_paths.pkl
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/multiverse_summary.csv
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/pipelines.csv
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_1.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_10.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_11.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_12.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_13.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_14.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_15.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_16.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_17.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_18.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_19.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_2.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_20.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_21.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_22.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_23.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_24.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_25.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_26.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_27.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_28.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_29.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_3.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_30.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_31.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_32.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_33.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_34.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_35.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_36.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_37.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_38.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_39.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_4.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_40.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_41.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_42.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_43.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_44.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_45.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_46.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_47.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_48.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_49.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_5.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_50.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_51.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_52.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_53.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_54.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_55.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_56.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_57.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_58.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_59.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_6.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_60.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_61.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_62.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_63.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_64.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_65.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_66.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_67.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_68.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_69.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_7.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_70.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_71.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_72.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_73.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_74.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_75.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_76.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_77.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_78.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_79.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_8.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_80.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_81.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_82.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_83.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_84.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_85.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_86.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_87.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_88.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_89.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_9.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_90.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_91.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_92.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_93.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_94.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_95.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/tutorials/multiverse/results/universe_96.pkl
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/LICENSE
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/README.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 comet_toolbox-0.3.5/PKG-INFO
```

### Comparing `comet_toolbox-0.3.4/adj.mat` & `comet_toolbox-0.3.5/adj.mat`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/adj_bin.mat` & `comet_toolbox-0.3.5/adj_bin.mat`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/simulation.txt` & `comet_toolbox-0.3.5/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/test_template.py` & `comet_toolbox-0.3.5/test_template.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/example_multiverse/universe_1.py` & `comet_toolbox-0.3.5/example_multiverse/universe_1.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/example_multiverse/universe_10.py` & `comet_toolbox-0.3.5/example_multiverse/universe_10.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/example_multiverse/universe_11.py` & `comet_toolbox-0.3.5/example_multiverse/universe_11.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/example_multiverse/universe_12.py` & `comet_toolbox-0.3.5/example_multiverse/universe_12.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/example_multiverse/universe_2.py` & `comet_toolbox-0.3.5/example_multiverse/universe_2.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/example_multiverse/universe_3.py` & `comet_toolbox-0.3.5/example_multiverse/universe_3.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/example_multiverse/universe_4.py` & `comet_toolbox-0.3.5/example_multiverse/universe_4.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/example_multiverse/universe_5.py` & `comet_toolbox-0.3.5/example_multiverse/universe_5.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/example_multiverse/universe_6.py` & `comet_toolbox-0.3.5/example_multiverse/universe_6.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/example_multiverse/universe_7.py` & `comet_toolbox-0.3.5/example_multiverse/universe_7.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/example_multiverse/universe_8.py` & `comet_toolbox-0.3.5/example_multiverse/universe_8.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/example_multiverse/universe_9.py` & `comet_toolbox-0.3.5/example_multiverse/universe_9.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/cifti.py` & `comet_toolbox-0.3.5/src/comet/cifti.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/data.py` & `comet_toolbox-0.3.5/src/comet/data.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/graph.py` & `comet_toolbox-0.3.5/src/comet/graph.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/gui.py` & `comet_toolbox-0.3.5/src/comet/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from scipy.io import loadmat, savemat
 from dataclasses import dataclass, field
 from importlib import resources as pkg_resources
 from typing import Any, Dict, get_type_hints, get_origin, Literal
 
 # Plotting imports
 from matplotlib.image import imread
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
+from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg as FigureCanvas
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from matplotlib.figure import Figure
 from matplotlib.ticker import FuncFormatter
 import matplotlib.gridspec as gridspec
 
 # Qt imports
 import qdarkstyle
@@ -294,15 +294,15 @@
         assert self.data.dfc_instance is not None, "Please provide the method object corresponding to your dFC data as the second argument to the GUI."
         
         # Init the data structures
         self.data.dfc_data = init_dfc_data
         self.data.dfc_instance = init_dfc_instance
         self.data.file_name = "loaded from script"
         self.data.dfc_name = init_dfc_instance.name
-        self.data.time_series = np.array([]) # for potential saving to .mat
+        self.data.file_data = np.array([]) # for potential saving to .mat
 
         # In case the method returns multiple values. The first one is always the NxNxT dfc matrix
         if isinstance(init_dfc_data, tuple):
             self.data.dfc_data = init_dfc_data[0]
             self.data.dfc_state_tc = None
             self.data.dfc_edge_ts = init_dfc_data[1][0] if isinstance(init_dfc_data[1], tuple) else None
 
@@ -315,16 +315,16 @@
         
         # Only a single matrix is returned (most cases)
         else:
             self.data.dfc_data = init_dfc_data
             self.data.dfc_state_tc = None
             self.data.dfc_edge_ts = None
         
-        # Add to data storage
-        self.data_storage.add_data(self.data)
+        # Add to data storage TOOD: this does not work yet (why? and is it even needed?)
+        #self.data_storage.add_data(self.data)
         
         # Disable the GUI elements
         self.methodComboBox.setEnabled(False)
         self.calculateButton.setEnabled(False)
         self.clearMemoryButton.setEnabled(False)
         self.keepInMemoryCheckbox.setEnabled(False)
 
@@ -637,16 +637,16 @@
         checkboxLayout.addWidget(self.preprocessingCheckBox)
         checkboxLayout.addWidget(self.graphCheckBox)
         checkboxLayout.addWidget(self.BCTCheckBox)
         checkboxLayout.setSpacing(10)
         checkboxLayout.addStretch()
 
         # Init checkbox states
-        self.preprocessingCheckBox.setChecked(False)
-        self.graphCheckBox.setChecked(False)
+        self.preprocessingCheckBox.setChecked(True)
+        self.graphCheckBox.setChecked(True)
         self.BCTCheckBox.setChecked(True)
         leftLayout.addLayout(checkboxLayout)
             
         # Create the combo box for selecting the graph analysis type
         self.graphAnalysisComboBox = QComboBox()
         leftLayout.addWidget(self.graphAnalysisComboBox)
```

### Comparing `comet_toolbox-0.3.4/src/comet/methods.py` & `comet_toolbox-0.3.5/src/comet/methods.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/multiverse.py` & `comet_toolbox-0.3.5/src/comet/multiverse.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/simulation.pkl` & `comet_toolbox-0.3.5/src/comet/resources/simulation.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/simulation.txt` & `comet_toolbox-0.3.5/src/comet/resources/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/single_state.txt` & `comet_toolbox-0.3.5/src/comet/resources/single_state.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii` & `comet_toolbox-0.3.5/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/atlas/README.md` & `comet_toolbox-0.3.5/src/comet/resources/atlas/README.md`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii` & `comet_toolbox-0.3.5/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii` & `comet_toolbox-0.3.5/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat` & `comet_toolbox-0.3.5/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/img/content.drawio` & `comet_toolbox-0.3.5/src/comet/resources/img/content.drawio`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/img/content.png` & `comet_toolbox-0.3.5/src/comet/resources/img/content.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/img/doi.svg` & `comet_toolbox-0.3.5/src/comet/resources/img/doi.svg`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/img/gui.png` & `comet_toolbox-0.3.5/src/comet/resources/img/gui.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/img/logo.png` & `comet_toolbox-0.3.5/src/comet/resources/img/logo.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/src/comet/resources/img/pypi.svg` & `comet_toolbox-0.3.5/src/comet/resources/img/pypi.svg`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/example_analysis.ipynb` & `comet_toolbox-0.3.5/tutorials/example_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/example_dfc.ipynb` & `comet_toolbox-0.3.5/tutorials/example_dfc.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/example_graph.ipynb` & `comet_toolbox-0.3.5/tutorials/example_graph.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/example_multiverse.ipynb` & `comet_toolbox-0.3.5/tutorials/example_multiverse.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/example_data/abide_50008.txt` & `comet_toolbox-0.3.5/tutorials/example_data/abide_50008.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/example_data/aomic_multi.pkl` & `comet_toolbox-0.3.5/tutorials/example_data/aomic_multi.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/example_data/simulation.txt` & `comet_toolbox-0.3.5/tutorials/example_data/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/example_data/xcpd.tsv` & `comet_toolbox-0.3.5/tutorials/example_data/xcpd.tsv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_1.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_1.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_10.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_10.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_11.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_11.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_12.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_12.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_13.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_13.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_14.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_14.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_15.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_15.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_16.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_16.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_17.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_17.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_18.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_18.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_19.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_19.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_2.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_2.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_20.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_20.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_21.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_21.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_22.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_22.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_23.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_23.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_24.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_24.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_25.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_25.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_26.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_26.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_27.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_27.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_28.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_28.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_29.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_29.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_3.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_3.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_30.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_30.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_31.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_31.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_32.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_32.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_33.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_33.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_34.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_34.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_35.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_35.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_36.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_36.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_37.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_37.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_38.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_38.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_39.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_39.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_4.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_4.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_40.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_40.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_41.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_41.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_42.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_42.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_43.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_43.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_44.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_44.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_45.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_45.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_46.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_46.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_47.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_47.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_48.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_48.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_49.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_49.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_5.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_5.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_50.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_50.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_51.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_51.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_52.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_52.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_53.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_53.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_54.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_54.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_55.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_55.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_56.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_56.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_57.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_57.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_58.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_58.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_59.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_59.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_6.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_6.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_60.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_60.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_61.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_61.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_62.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_62.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_63.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_63.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_64.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_64.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_65.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_65.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_66.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_66.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_67.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_67.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_68.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_68.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_69.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_69.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_7.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_7.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_70.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_70.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_71.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_71.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_72.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_72.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_73.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_73.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_74.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_74.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_75.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_75.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_76.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_76.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_77.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_77.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_78.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_78.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_79.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_79.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_8.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_8.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_80.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_80.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_81.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_81.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_82.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_82.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_83.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_83.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_84.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_84.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_85.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_85.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_86.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_86.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_87.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_87.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_88.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_88.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_89.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_89.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_9.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_9.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_90.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_90.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_91.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_91.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_92.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_92.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_93.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_93.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_94.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_94.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_95.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_95.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/universe_96.py` & `comet_toolbox-0.3.5/tutorials/multiverse/universe_96.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/results/forking_paths.pkl` & `comet_toolbox-0.3.5/tutorials/multiverse/results/forking_paths.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/results/multiverse_summary.csv` & `comet_toolbox-0.3.5/tutorials/multiverse/results/multiverse_summary.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/tutorials/multiverse/results/pipelines.csv` & `comet_toolbox-0.3.5/tutorials/multiverse/results/pipelines.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/.gitignore` & `comet_toolbox-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/LICENSE` & `comet_toolbox-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/README.md` & `comet_toolbox-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.4/pyproject.toml` & `comet_toolbox-0.3.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comet-toolbox"
-version = "0.3.4"
+version = "0.3.5"
 authors = [
   {name="Micha Burkhardt", email="micha.burkhardt@uol.de"},
 ]
 description = "Dynamic functional connectivity toolbox for multiverse analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -23,15 +23,14 @@
   "pandas >=2.1.3",
   "pycwt >=0.4.0b0",
   "bctpy >=0.6.1",
   "joblib >=1.3.2",
   "jinja2 >=3.1.2",
   "tqdm >=4.66.1",
   "numba >=0.58.1",
-  "pyqt5-tools>=5.15",
   "PyQt6-tools >=6.4.2",
   "qdarkstyle >=3.2.3",
   "seaborn >=0.13.0",
   "networkx >=3.2.1",
   "pydfc >=1.0.4",
   "ipykernel >=6.29.3",
   "notebook >=7.0.6"
```

### Comparing `comet_toolbox-0.3.4/PKG-INFO` & `comet_toolbox-0.3.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: comet-toolbox
-Version: 0.3.4
+Version: 0.3.5
 Summary: Dynamic functional connectivity toolbox for multiverse analysis
 Project-URL: Homepage, https://github.com/mibur1/dfc-multiverse
 Project-URL: Issues, https://github.com/mibur1/dfc-multiverse/issues
 Author-email: Micha Burkhardt <micha.burkhardt@uol.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,15 +20,14 @@
 Requires-Dist: nilearn>=0.10.2
 Requires-Dist: notebook>=7.0.6
 Requires-Dist: numba>=0.58.1
 Requires-Dist: numpy>=1.26.2
 Requires-Dist: pandas>=2.1.3
 Requires-Dist: pycwt>=0.4.0b0
 Requires-Dist: pydfc>=1.0.4
-Requires-Dist: pyqt5-tools>=5.15
 Requires-Dist: pyqt6-tools>=6.4.2
 Requires-Dist: qdarkstyle>=3.2.3
 Requires-Dist: scikit-learn>=1.3.2
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: seaborn>=0.13.0
 Requires-Dist: statsmodels>=0.14.0
 Requires-Dist: tqdm>=4.66.1
```

