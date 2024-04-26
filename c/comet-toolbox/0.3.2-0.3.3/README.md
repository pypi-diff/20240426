# Comparing `tmp/comet_toolbox-0.3.2.tar.gz` & `tmp/comet_toolbox-0.3.3.tar.gz`

## Comparing `comet_toolbox-0.3.2.tar` & `comet_toolbox-0.3.3.tar`

### file list

```diff
@@ -1,233 +1,248 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/.gitattributes
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/adj.mat
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/adj_bin.mat
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/simulation.txt
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/__init__.py
--rwxr-xr-x   0        0        0     3821 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/cifti.py
--rwxr-xr-x   0        0        0     3968 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/data.py
--rw-r--r--   0        0        0    29936 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/graph.py
--rw-r--r--   0        0        0   135519 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/gui.py
--rwxr-xr-x   0        0        0    47496 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/methods.py
--rwxr-xr-x   0        0        0    26011 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/multiverse.py
--rw-r--r--   0        0        0    96617 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/simulation.pkl
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/simulation.txt
--rw-r--r--   0        0        0   192811 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/single_state.txt
--rwxr-xr-x   0        0        0  1038952 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii
--rwxr-xr-x   0        0        0      531 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/atlas/README.md
--rwxr-xr-x   0        0        0  1029992 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii
--rwxr-xr-x   0        0        0   655904 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii
--rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat
--rw-r--r--   0        0        0    40910 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/img/content.drawio
--rw-r--r--   0        0        0   175918 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/img/content.png
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/img/doi.svg
--rw-r--r--   0        0        0   202431 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/img/gui.png
--rw-r--r--   0        0        0   724684 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/img/logo.png
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/src/comet/resources/img/pypi.svg
--rw-r--r--   0        0        0   185059 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_analysis.ipynb
--rw-r--r--   0        0        0   450982 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_dfc.ipynb
--rw-r--r--   0        0        0  1311678 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_graph.ipynb
--rw-r--r--   0        0        0   114703 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_multiverse.ipynb
--rw-r--r--   0        0        0   804479 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_data/abide_50008.txt
--rw-r--r--   0        0        0   969955 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_data/aomic_multi.pkl
--rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_data/simulation.txt
--rw-r--r--   0        0        0  1564386 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/example_data/xcpd.tsv
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_1.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_10.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_11.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_12.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_13.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_14.py
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_15.py
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_16.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_17.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_18.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_19.py
--rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_2.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_20.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_21.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_22.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_23.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_24.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_25.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_26.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_27.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_28.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_29.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_3.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_30.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_31.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_32.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_33.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_34.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_35.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_36.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_37.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_38.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_39.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_4.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_40.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_41.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_42.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_43.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_44.py
--rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_45.py
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_46.py
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_47.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_48.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_49.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_5.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_50.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_51.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_52.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_53.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_54.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_55.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_56.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_57.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_58.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_59.py
--rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_6.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_60.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_61.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_62.py
--rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_63.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_64.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_65.py
--rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_66.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_67.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_68.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_69.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_7.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_70.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_71.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_72.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_73.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_74.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_75.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_76.py
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_77.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_78.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_79.py
--rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_8.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_80.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_81.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_82.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_83.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_84.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_85.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_86.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_87.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_88.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_89.py
--rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_9.py
--rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_90.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_91.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_92.py
--rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_93.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_94.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_95.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/universe_96.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/forking_paths.pkl
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/multiverse_summary.csv
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/pipelines.csv
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_1.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_10.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_11.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_12.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_13.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_14.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_15.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_16.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_17.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_18.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_19.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_2.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_20.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_21.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_22.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_23.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_24.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_25.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_26.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_27.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_28.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_29.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_3.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_30.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_31.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_32.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_33.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_34.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_35.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_36.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_37.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_38.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_39.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_4.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_40.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_41.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_42.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_43.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_44.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_45.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_46.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_47.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_48.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_49.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_5.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_50.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_51.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_52.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_53.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_54.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_55.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_56.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_57.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_58.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_59.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_6.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_60.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_61.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_62.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_63.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_64.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_65.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_66.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_67.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_68.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_69.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_7.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_70.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_71.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_72.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_73.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_74.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_75.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_76.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_77.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_78.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_79.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_8.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_80.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_81.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_82.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_83.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_84.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_85.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_86.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_87.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_88.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_89.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_9.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_90.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_91.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_92.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_93.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_94.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_95.pkl
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/tutorials/multiverse/results/universe_96.pkl
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/LICENSE
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/README.md
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 comet_toolbox-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/.gitattributes
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/adj.mat
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/adj_bin.mat
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/simulation.txt
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/test_template.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/universe_1.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/universe_10.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/universe_11.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/universe_12.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/universe_2.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/universe_3.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/universe_4.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/universe_5.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/universe_6.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/universe_7.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/universe_8.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/universe_9.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/results/forking_paths.pkl
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/example_multiverse/results/multiverse_summary.csv
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/__init__.py
+-rwxr-xr-x   0        0        0     3821 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/cifti.py
+-rwxr-xr-x   0        0        0     4027 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/data.py
+-rw-r--r--   0        0        0    29936 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/graph.py
+-rw-r--r--   0        0        0   137181 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/gui.py
+-rwxr-xr-x   0        0        0    47496 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/methods.py
+-rwxr-xr-x   0        0        0    25135 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/multiverse.py
+-rw-r--r--   0        0        0    96617 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/simulation.pkl
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/simulation.txt
+-rw-r--r--   0        0        0   192811 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/single_state.txt
+-rwxr-xr-x   0        0        0  1038952 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii
+-rwxr-xr-x   0        0        0      531 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/atlas/README.md
+-rwxr-xr-x   0        0        0  1029992 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii
+-rwxr-xr-x   0        0        0   655904 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii
+-rwxr-xr-x   0        0        0     1047 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat
+-rw-r--r--   0        0        0    40910 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/img/content.drawio
+-rw-r--r--   0        0        0   175918 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/img/content.png
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/img/doi.svg
+-rw-r--r--   0        0        0   202431 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/img/gui.png
+-rw-r--r--   0        0        0   724684 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/img/logo.png
+-rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/src/comet/resources/img/pypi.svg
+-rw-r--r--   0        0        0   185059 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/example_analysis.ipynb
+-rw-r--r--   0        0        0   450982 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/example_dfc.ipynb
+-rw-r--r--   0        0        0  1311678 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/example_graph.ipynb
+-rw-r--r--   0        0        0   114703 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/example_multiverse.ipynb
+-rw-r--r--   0        0        0   804479 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/example_data/abide_50008.txt
+-rw-r--r--   0        0        0   969955 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/example_data/aomic_multi.pkl
+-rw-r--r--   0        0        0   193093 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/example_data/simulation.txt
+-rw-r--r--   0        0        0  1564386 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/example_data/xcpd.tsv
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_1.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_10.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_11.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_12.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_13.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_14.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_15.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_16.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_17.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_18.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_19.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_2.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_20.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_21.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_22.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_23.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_24.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_25.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_26.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_27.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_28.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_29.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_3.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_30.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_31.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_32.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_33.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_34.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_35.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_36.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_37.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_38.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_39.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_4.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_40.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_41.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_42.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_43.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_44.py
+-rw-r--r--   0        0        0     4664 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_45.py
+-rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_46.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_47.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_48.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_49.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_5.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_50.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_51.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_52.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_53.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_54.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_55.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_56.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_57.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_58.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_59.py
+-rw-r--r--   0        0        0     4686 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_6.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_60.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_61.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_62.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_63.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_64.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_65.py
+-rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_66.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_67.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_68.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_69.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_7.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_70.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_71.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_72.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_73.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_74.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_75.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_76.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_77.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_78.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_79.py
+-rw-r--r--   0        0        0     4687 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_8.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_80.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_81.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_82.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_83.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_84.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_85.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_86.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_87.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_88.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_89.py
+-rw-r--r--   0        0        0     4689 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_9.py
+-rw-r--r--   0        0        0     4695 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_90.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_91.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_92.py
+-rw-r--r--   0        0        0     4699 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_93.py
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_94.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_95.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/universe_96.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/forking_paths.pkl
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/multiverse_summary.csv
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/pipelines.csv
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_1.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_10.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_11.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_12.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_13.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_14.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_15.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_16.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_17.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_18.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_19.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_2.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_20.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_21.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_22.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_23.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_24.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_25.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_26.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_27.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_28.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_29.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_3.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_30.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_31.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_32.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_33.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_34.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_35.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_36.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_37.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_38.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_39.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_4.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_40.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_41.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_42.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_43.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_44.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_45.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_46.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_47.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_48.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_49.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_5.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_50.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_51.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_52.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_53.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_54.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_55.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_56.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_57.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_58.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_59.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_6.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_60.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_61.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_62.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_63.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_64.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_65.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_66.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_67.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_68.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_69.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_7.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_70.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_71.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_72.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_73.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_74.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_75.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_76.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_77.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_78.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_79.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_8.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_80.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_81.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_82.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_83.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_84.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_85.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_86.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_87.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_88.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_89.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_9.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_90.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_91.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_92.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_93.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_94.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_95.pkl
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/tutorials/multiverse/results/universe_96.pkl
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/README.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     5004 2020-02-02 00:00:00.000000 comet_toolbox-0.3.3/PKG-INFO
```

### Comparing `comet_toolbox-0.3.2/adj.mat` & `comet_toolbox-0.3.3/adj.mat`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/adj_bin.mat` & `comet_toolbox-0.3.3/adj_bin.mat`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/simulation.txt` & `comet_toolbox-0.3.3/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/cifti.py` & `comet_toolbox-0.3.3/src/comet/cifti.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/data.py` & `comet_toolbox-0.3.3/src/comet/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 
         # Update header_list if rois exist
         rois = rois.to_list() if rois is not None else None
 
     else:
         raise ValueError("Unsupported file format")
     
-    return data, rois
+    if rois is not None:
+        return data, rois
+    else:
+        return data
 
 def load_example(type=None):
     """
     Load simulated time series data with two randomly changing connectivity states
     """
     if type == "pkl":
         with pkg_resources.path("comet.resources", "simulation.pkl") as file_path:
```

### Comparing `comet_toolbox-0.3.2/src/comet/graph.py` & `comet_toolbox-0.3.3/src/comet/graph.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/gui.py` & `comet_toolbox-0.3.3/src/comet/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import re
 import sys
 import copy
 import json
 import pickle
 import inspect
+import subprocess
 import numpy as np
 import pandas as pd
 import nibabel as nib
 from scipy.io import loadmat, savemat
 from dataclasses import dataclass, field
 from importlib import resources as pkg_resources
-from typing import Any, Dict, get_type_hints, get_origin, get_args, Literal, Union
+from typing import Any, Dict, get_type_hints, get_origin, Literal
 
 # Plotting imports
 from matplotlib.image import imread
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from matplotlib.figure import Figure
 from matplotlib.ticker import FuncFormatter
@@ -811,18 +812,17 @@
 
         # Add the horizontal layout to the main left layout
         leftLayout.addLayout(loadLayout)
 
         # Connect the button to the method that handles file loading
         loadScriptButton.clicked.connect(self.loadScript)
 
-        executeButton = QPushButton('Run multiverse analysis')
-        leftLayout.addWidget(executeButton)
-        executeButton.clicked.connect(self.executeScript)
-
+        runButton = QPushButton('Run multiverse analysis')
+        leftLayout.addWidget(runButton)
+        runButton.clicked.connect(self.runScript)
 
         ################################
         #  Right section for plotting  #
         ################################
         rightLayout = QVBoxLayout()
 
         # Creating a tab widget for different purposes
@@ -1252,14 +1252,20 @@
         buttonLayoutIndex = layout.indexOf(buttonLayout)
         layout.insertWidget(buttonLayoutIndex, newDecisionWidget)
 
         return
 
     # Add option to a decision
     def addOption(self, functionComboBox, parameterContainer, nameInputField, optionsInputField):
+        # Name for the decision must be provided
+        name = nameInputField.text().strip()
+        if not name:
+            QMessageBox.warning(self, "Input Error", "Please ensure a name is provided for the decision.")
+            return
+        
         # Retrieve the selected function key and determine its module prefix
         func_key = functionComboBox.currentData()
 
         try:
             method_name = self.connectivityMethods[func_key]
         except:
             method_name = self.graphOptions[func_key]
@@ -1365,14 +1371,15 @@
         # No key means the decision widget is empty, so clear and delete everything
         if key == "":
             if decisionWidget.layout():
                 self.clearLayout(decisionWidget.layout())
                 decisionWidget.deleteLater()
                 optionsInputField.clear()
                 self.data.mv_containers.remove(decisionWidget)
+                self.generateScript()
                 return
             
         if key in self.data.forking_paths:
             options = self.data.forking_paths[key]
 
             # Remove the last option and update the input field
             if options:
@@ -1463,21 +1470,31 @@
                 "\nmultiverse = Multiverse(name=\"example_multiverse\")\n"
                 "multiverse.create(analysis_template, forking_paths)\n"
                 "multiverse.summary()\n"
                 "#multiverse.run()\n"
             )
 
         self.scriptDisplay.setText(script_content)
+        self.scriptDisplay.setReadOnly(True)
 
     # Loads a multiverse script
     def loadScript(self):
         fileName, _ = QFileDialog.getOpenFileName(self, "Load Script", "", "Python Files (*.py);;All Files (*)")
         if fileName:
             self.loadedScriptDisplay.setText(f"Loaded: {fileName}")
             self.loadedScriptPath = fileName
+            
+            # Read the content of the file
+            try:
+                with open(fileName, 'r', encoding='utf-8') as file:
+                    scriptContent = file.read()
+                    self.scriptDisplay.setText(scriptContent)
+                    self.scriptDisplay.setReadOnly(False)
+            except Exception as e:
+                QMessageBox.critical(self, "Error", f"Failed to read the file: {str(e)}")
 
     # Saves the current template script
     def saveScript(self):
         script_text = self.scriptDisplay.toPlainText()
         fileName, _ = QFileDialog.getSaveFileName(self, "Save Script", "", "Python Files (*.py);;All Files (*)")
 
         if fileName:
@@ -1485,21 +1502,26 @@
             if not fileName.endswith('.py'):
                 fileName += '.py'
             
             with open(fileName, 'w') as file:
                 file.write(script_text)
 
     # Runs the script/multiverse analysis
-    def executeScript(self):
+    def runScript(self):
         if hasattr(self, 'loadedScriptPath') and self.loadedScriptPath:
-            with open(self.loadedScriptPath, "r") as file:
-                exec(file.read(), {})
-            QMessageBox.information(self, "Execution", "Script executed successfully.")
+            try:
+                # Run the script
+                subprocess.run(['python', self.loadedScriptPath], check=True)
+                QMessageBox.information(self, "Multiverse Analysis", "Multiverse ran successfully!")
+            except subprocess.CalledProcessError:
+                QMessageBox.warning(self, "Multiverse Analysis", "Multiverse failed!")
+            except Exception as e:
+                QMessageBox.warning(self, "Multiverse Analysis", f"Multiverse failed!\n{str(e)}")
         else:
-            QMessageBox.warning(self, "Load Script", "No script file is loaded.")
+            QMessageBox.warning(self, "Multiverse Analysis", "No script was loaded to run.")
 
     """
     I/O and data related functions
     """
     # dFC tab
     def loadConnectivityFile(self):
         fileFilter = "All Supported Files (*.mat *.txt *.npy *.pkl *.tsv *.dtseries.nii *.ptseries.nii);;MAT files (*.mat);;Text files (*.txt);;NumPy files (*.npy);;Pickle files (*.pkl);;TSV files (*.tsv);;CIFTI files (*.dtseries.nii *.ptseries.nii)"
@@ -1701,14 +1723,20 @@
         elif file_path.endswith('.npy'):
             self.data.graph_data = np.load(file_path)
       
         else:
             self.data.graph_data = None
             self.time_series_textbox.setText("Unsupported file format")
 
+        # Check if data is square
+        if self.data.graph_data.ndim != 2 or self.data.graph_data.shape[0] != self.data.graph_data.shape[1]:
+            QMessageBox.warning(self, "Data Error", "The loaded data is not a square matrix.")
+            self.data.graph_data = None
+            return
+
         self.data.graph_raw = self.data.graph_data
         self.graphFileNameLabel.setText(f"Loaded {self.data.graph_file} with shape {self.data.graph_data.shape}")
         
         self.plotGraph()
         self.onGraphCombobox()
 
     def saveGraphFile(self):
@@ -1760,15 +1788,22 @@
             return
 
     def takeCurrentData(self):
         if self.data.dfc_data is None:
             QMessageBox.warning(self, "Output Error", "No current dFC data available.")
             return
         
-        self.data.graph_data = self.data.dfc_data[:,:,self.currentSliderValue]
+        if len(self.data.dfc_data.shape) == 3:
+            self.data.graph_data = self.data.dfc_data[:,:,self.currentSliderValue]
+        elif len(self.data.dfc_data.shape) == 2:
+            self.data.graph_data = self.data.dfc_data
+        else:
+            QMessageBox.warning(self, "Output Error", "FC data seems to have the wrong shape.")
+            return
+        
         self.data.graph_raw = self.data.graph_data
         
         print(f"Used current dFC data with shape {self.data.graph_data.shape}")
         self.graphFileNameLabel.setText(f"Used current dFC data with shape {self.data.graph_data.shape}")
         self.data.graph_file = f"dfC from {self.data.file_name}" #with {self.data.dfc_name} at t={self.currentSliderValue}"
         self.plotGraph()
         self.onGraphCombobox()
```

### Comparing `comet_toolbox-0.3.2/src/comet/methods.py` & `comet_toolbox-0.3.3/src/comet/methods.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/multiverse.py` & `comet_toolbox-0.3.3/src/comet/multiverse.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,41 +274,31 @@
         else:
             raise TypeError(f"Unsupported type for {value} which is of type {type(value)}")
 
     # Handle the decision points that require class/function imports
     def handle_dict(self, value):
         function_call = ""
 
-        if "connectivity" in value.keys():
-            dfc_class = value["connectivity"]
-            input_data = value["input_data"]
-            dfc_args = value["args"]
-            function_call = f"comet.methods.{dfc_class}({input_data}, **{dfc_args}).connectivity()"
-        
-        if "graph" in value.keys():
-            graph_function = value["graph"]
-            input_data = value["input_data"]
-            
-            # If we have args, we need to handle them for indviduak 
-            try:
-                graph_args = value["args"].copy()  # Copy to avoid mutating the original
-
-                # Measures that need a community affiliation vector
-                if graph_function in("bct.participation_coef", "bct.participation_coef_sparse", "bct.participation_coef_sign", \
-                                    "bct.agreement_wei", "bct.diversity_coef_sign", "bct.gateway_coef_sign", "bct.module_degree_zscore"):
-                    ci = graph_args["ci"]
-                    del graph_args["ci"]
-                    function_call = f"{graph_function}({input_data}, ci={ci}[0], **{graph_args})"
-                # Measures that have additional numerical or string arguments
-                else:
-                    function_call = f"{graph_function}({input_data}, **{graph_args})"
-            
-            # Measures that only need an adjacency matrix as input
-            except KeyError:
-                function_call = f"{graph_function}({input_data})"
+        func = value["func"]
+        args = value["args"].copy()
+        del args["Option"]
+
+        first_arg = next(iter(args))
+        input_data = args[first_arg]
+        del args[first_arg]
+
+        if value["func"].startswith("comet.methods"):
+            function_call = f"{func}({input_data}, **{args}).connectivity()"
+        else:
+            if "ci" in args:
+                ci = args["ci"]
+                del args["ci"]
+                function_call = f"{func}({input_data}, ci={ci}[0], **{args})"
+            else:
+                function_call = f"{func}({input_data}, **{args})"
 
         return function_call
 
     # Create CSV file with the parameters of all universes
     def create_csv(self, csv_path, all_universes, keys):
         # Generate CSV file with the parameters of all universes
         with open(f"{csv_path}/multiverse_summary.csv", "w", newline='') as csvfile:
```

### Comparing `comet_toolbox-0.3.2/src/comet/resources/simulation.pkl` & `comet_toolbox-0.3.3/src/comet/resources/simulation.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/simulation.txt` & `comet_toolbox-0.3.3/src/comet/resources/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/single_state.txt` & `comet_toolbox-0.3.3/src/comet/resources/single_state.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii` & `comet_toolbox-0.3.3/src/comet/resources/atlas/Q1-Q6_RelatedValidation210.CorticalAreas_dil_Final_Final_Areas_Group_Colors_with_Atlas_ROIs2.32k_fs_LR.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/atlas/README.md` & `comet_toolbox-0.3.3/src/comet/resources/atlas/README.md`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii` & `comet_toolbox-0.3.3/src/comet/resources/atlas/Schaefer2018_200Parcels_17Networks_order_Tian_Subcortex_S4.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii` & `comet_toolbox-0.3.3/src/comet/resources/atlas/Schaefer2018_200Parcels_Kong2022_17Networks_order.dlabel.nii`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat` & `comet_toolbox-0.3.3/src/comet/resources/atlas/fs_LR_32k_medial_mask.mat`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/img/content.drawio` & `comet_toolbox-0.3.3/src/comet/resources/img/content.drawio`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/img/content.png` & `comet_toolbox-0.3.3/src/comet/resources/img/content.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/img/doi.svg` & `comet_toolbox-0.3.3/src/comet/resources/img/doi.svg`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/img/gui.png` & `comet_toolbox-0.3.3/src/comet/resources/img/gui.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/img/logo.png` & `comet_toolbox-0.3.3/src/comet/resources/img/logo.png`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/src/comet/resources/img/pypi.svg` & `comet_toolbox-0.3.3/src/comet/resources/img/pypi.svg`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/example_analysis.ipynb` & `comet_toolbox-0.3.3/tutorials/example_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/example_dfc.ipynb` & `comet_toolbox-0.3.3/tutorials/example_dfc.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/example_graph.ipynb` & `comet_toolbox-0.3.3/tutorials/example_graph.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/example_multiverse.ipynb` & `comet_toolbox-0.3.3/tutorials/example_multiverse.ipynb`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/example_data/abide_50008.txt` & `comet_toolbox-0.3.3/tutorials/example_data/abide_50008.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/example_data/aomic_multi.pkl` & `comet_toolbox-0.3.3/tutorials/example_data/aomic_multi.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/example_data/simulation.txt` & `comet_toolbox-0.3.3/tutorials/example_data/simulation.txt`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/example_data/xcpd.tsv` & `comet_toolbox-0.3.3/tutorials/example_data/xcpd.tsv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_1.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_1.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_10.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_10.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_11.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_11.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_12.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_12.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_13.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_13.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_14.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_14.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_15.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_15.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_16.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_16.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_17.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_17.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_18.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_18.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_19.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_19.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_2.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_2.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_20.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_20.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_21.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_21.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_22.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_22.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_23.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_23.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_24.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_24.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_25.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_25.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_26.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_26.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_27.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_27.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_28.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_28.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_29.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_29.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_3.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_3.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_30.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_30.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_31.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_31.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_32.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_32.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_33.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_33.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_34.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_34.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_35.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_35.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_36.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_36.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_37.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_37.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_38.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_38.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_39.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_39.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_4.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_4.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_40.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_40.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_41.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_41.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_42.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_42.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_43.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_43.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_44.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_44.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_45.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_45.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_46.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_46.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_47.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_47.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_48.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_48.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_49.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_49.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_5.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_5.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_50.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_50.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_51.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_51.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_52.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_52.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_53.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_53.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_54.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_54.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_55.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_55.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_56.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_56.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_57.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_57.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_58.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_58.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_59.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_59.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_6.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_6.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_60.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_60.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_61.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_61.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_62.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_62.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_63.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_63.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_64.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_64.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_65.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_65.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_66.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_66.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_67.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_67.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_68.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_68.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_69.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_69.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_7.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_7.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_70.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_70.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_71.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_71.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_72.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_72.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_73.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_73.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_74.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_74.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_75.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_75.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_76.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_76.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_77.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_77.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_78.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_78.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_79.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_79.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_8.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_8.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_80.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_80.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_81.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_81.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_82.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_82.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_83.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_83.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_84.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_84.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_85.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_85.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_86.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_86.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_87.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_87.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_88.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_88.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_89.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_89.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_9.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_9.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_90.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_90.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_91.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_91.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_92.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_92.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_93.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_93.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_94.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_94.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_95.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_95.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/universe_96.py` & `comet_toolbox-0.3.3/tutorials/multiverse/universe_96.py`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/results/forking_paths.pkl` & `comet_toolbox-0.3.3/tutorials/multiverse/results/forking_paths.pkl`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/results/multiverse_summary.csv` & `comet_toolbox-0.3.3/tutorials/multiverse/results/multiverse_summary.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/tutorials/multiverse/results/pipelines.csv` & `comet_toolbox-0.3.3/tutorials/multiverse/results/pipelines.csv`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/.gitignore` & `comet_toolbox-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/LICENSE` & `comet_toolbox-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/README.md` & `comet_toolbox-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `comet_toolbox-0.3.2/pyproject.toml` & `comet_toolbox-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comet-toolbox"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   {name="Micha Burkhardt", email="micha.burkhardt@uol.de"},
 ]
 description = "Dynamic functional connectivity toolbox for multiverse analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `comet_toolbox-0.3.2/PKG-INFO` & `comet_toolbox-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: comet-toolbox
-Version: 0.3.2
+Version: 0.3.3
 Summary: Dynamic functional connectivity toolbox for multiverse analysis
 Project-URL: Homepage, https://github.com/mibur1/dfc-multiverse
 Project-URL: Issues, https://github.com/mibur1/dfc-multiverse/issues
 Author-email: Micha Burkhardt <micha.burkhardt@uol.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

