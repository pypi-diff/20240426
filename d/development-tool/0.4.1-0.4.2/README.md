# Comparing `tmp/development-tool-0.4.1.tar.gz` & `tmp/development-tool-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "development-tool-0.4.1.tar", last modified: Wed Apr 24 14:31:08 2024, max compression
+gzip compressed data, was "dist/development-tool-0.4.2.tar", last modified: Fri Apr 26 14:51:41 2024, max compression
```

## Comparing `development-tool-0.4.1.tar` & `development-tool-0.4.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-24 14:31:08.965313 development-tool-0.4.1/
--rwx------   0 alex       (501) staff       (20)        0 2024-03-26 13:20:44.000000 development-tool-0.4.1/License.txt
--rw-r--r--   0 alex       (501) staff       (20)      167 2024-04-24 14:31:08.964524 development-tool-0.4.1/PKG-INFO
--rwx------   0 alex       (501) staff       (20)        9 2024-03-26 13:20:44.000000 development-tool-0.4.1/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-24 14:31:08.808533 development-tool-0.4.1/development_tool.egg-info/
--rwx------   0 alex       (501) staff       (20)      167 2024-04-24 14:31:08.000000 development-tool-0.4.1/development_tool.egg-info/PKG-INFO
--rwx------   0 alex       (501) staff       (20)     5336 2024-04-24 14:31:08.000000 development-tool-0.4.1/development_tool.egg-info/SOURCES.txt
--rwx------   0 alex       (501) staff       (20)        1 2024-04-24 14:31:08.000000 development-tool-0.4.1/development_tool.egg-info/dependency_links.txt
--rwx------   0 alex       (501) staff       (20)       75 2024-04-24 14:31:08.000000 development-tool-0.4.1/development_tool.egg-info/entry_points.txt
--rwx------   0 alex       (501) staff       (20)       14 2024-04-24 14:31:08.000000 development-tool-0.4.1/development_tool.egg-info/namespace_packages.txt
--rwx------   0 alex       (501) staff       (20)        6 2024-04-24 14:31:08.000000 development-tool-0.4.1/development_tool.egg-info/requires.txt
--rwx------   0 alex       (501) staff       (20)       14 2024-04-24 14:31:08.000000 development-tool-0.4.1/development_tool.egg-info/top_level.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-24 14:31:08.809319 development-tool-0.4.1/orangecontrib/
--rwx------   0 alex       (501) staff       (20)       55 2024-03-26 13:20:44.000000 development-tool-0.4.1/orangecontrib/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-24 14:31:08.810065 development-tool-0.4.1/orangecontrib/development_tool/
--rwx------   0 alex       (501) staff       (20)        0 2024-03-26 13:20:44.000000 development-tool-0.4.1/orangecontrib/development_tool/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-24 14:31:08.827417 development-tool-0.4.1/orangecontrib/development_tool/widgets/
--rwx------   0 alex       (501) staff       (20)      799 2024-03-26 13:20:44.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/Gpt4AllManagement.py
--rwx------   0 alex       (501) staff       (20)    14328 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/MetManagement.py
--rwx------   0 alex       (501) staff       (20)     4882 2024-03-26 13:20:44.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/VarManagement.py
--rwx------   0 alex       (501) staff       (20)     2087 2024-03-26 13:20:44.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/WrapMessageBox.py
--rwx------   0 alex       (501) staff       (20)      324 2024-03-26 13:20:44.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/__init__.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-24 14:31:08.832201 development-tool-0.4.1/orangecontrib/development_tool/widgets/dataset_devellopper/
--rwx------   0 alex       (501) staff       (20)       87 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/dataset_devellopper/fake_input.csv
--rwx------   0 alex       (501) staff       (20)        0 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/dataset_devellopper/fakeows.ows
--rwx------   0 alex       (501) staff       (20)       49 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/dataset_devellopper/readme.txt
--rw-r--r--   0 alex       (501) staff       (20)     7815 2024-04-24 14:29:59.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/document_eater.py
--rwx------   0 alex       (501) staff       (20)    20858 2024-03-26 13:20:44.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/goto.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-24 14:31:08.931169 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/
--rwx------   0 alex       (501) staff       (20)   269355 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Emblem_of_Napoleon_Bonaparte.svg
--rwx------   0 alex       (501) staff       (20)     4161 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Logo_HKH.svg
--rwx------   0 alex       (501) staff       (20)     4259 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Logo_HKH_4.svg
--rwx------   0 alex       (501) staff       (20)     6129 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Logo_HKH_4_jc.svg
--rwx------   0 alex       (501) staff       (20)  1310135 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Napoleon2.svg
--rwx------   0 alex       (501) staff       (20)    82296 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Pikachu SVG File.svg
--rwx------   0 alex       (501) staff       (20)     1364 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Workflow.svg
--rwx------   0 alex       (501) staff       (20)      506 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/category.svg
--rwx------   0 alex       (501) staff       (20)    17140 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/chat-bot.png
--rwx------   0 alex       (501) staff       (20)     9815 2024-03-27 16:51:28.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/data-integration.png
--rwx------   0 alex       (501) staff       (20)     6493 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/database.svg
--rwx------   0 alex       (501) staff       (20)    16824 2024-03-13 15:23:26.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/documents.png
--rwx------   0 alex       (501) staff       (20)     1402 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/download-svgrepo-com.svg
--rwx------   0 alex       (501) staff       (20)    10205 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/duplicate.png
--rwx------   0 alex       (501) staff       (20)    40437 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/ecriture.svg
--rwx------   0 alex       (501) staff       (20)    24354 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/file-transfer.png
--rwx------   0 alex       (501) staff       (20)    21756 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/goto.png
--rwx------   0 alex       (501) staff       (20)    38778 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/icon_surrogate_learner.png
--rwx------   0 alex       (501) staff       (20)    40434 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/icon_surrogate_predict.png
--rwx------   0 alex       (501) staff       (20)    16844 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/input.png
--rwx------   0 alex       (501) staff       (20)     4781 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/interrupteur.svg
--rwx------   0 alex       (501) staff       (20)    29352 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/jcm_export_score.png
--rwx------   0 alex       (501) staff       (20)    20371 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/jcm_open_file_resize_alpha_channel.png
--rwx------   0 alex       (501) staff       (20)    30017 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/jcm_optuna_parameters_setting.png
--rwx------   0 alex       (501) staff       (20)    12060 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/jcm_output_table.png
--rwx------   0 alex       (501) staff       (20)     1801 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/label.svg
--rwx------   0 alex       (501) staff       (20)    10741 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/lecture.svg
--rwx------   0 alex       (501) staff       (20)      631 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/mywidget.svg
--rwx------   0 alex       (501) staff       (20)     1738 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/openai.svg
--rwx------   0 alex       (501) staff       (20)     3945 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/optuna.svg
--rwx------   0 alex       (501) staff       (20)    16483 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/output.png
--rwx------   0 alex       (501) staff       (20)     3591 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/tank-canon-svgrepo-com.svg
--rwx------   0 alex       (501) staff       (20)    23619 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/tool.png
--rwx------   0 alex       (501) staff       (20)     2880 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/tutoriel_bouton.svg
--rwx------   0 alex       (501) staff       (20)      394 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/upload-svgrepo-com.svg
--rwx------   0 alex       (501) staff       (20)     2516 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/variable_editor.svg
--rwx------   0 alex       (501) staff       (20)    24762 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/war-svgrepo-com.png
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-24 14:31:08.944606 development-tool-0.4.1/orangecontrib/development_tool/widgets/img/
--rwx------   0 alex       (501) staff       (20)    15981 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/img/bandeau_pour_orange.png
--rwx------   0 alex       (501) staff       (20)     9070 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_18px.png
--rwx------   0 alex       (501) staff       (20)    15224 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_30px.png
--rwx------   0 alex       (501) staff       (20)     2746 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/img/interrupteur_ferme.svg
--rwx------   0 alex       (501) staff       (20)     3530 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/img/interrupteur_ouvert.svg
--rwx------   0 alex       (501) staff       (20)     9329 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/img/khk_label_explanation.svg
--rwx------   0 alex       (501) staff       (20)     2597 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/img/refresh.svg
--rwx------   0 alex       (501) staff       (20)     2598 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/img/refresh2.svg
--rwx------   0 alex       (501) staff       (20)     2606 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/img/refresh_with_txt.svg
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-24 14:31:08.952850 development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/
--rwx------   0 alex       (501) staff       (20)    19522 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/Table_management.py
--rwx------   0 alex       (501) staff       (20)     2136 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/Utils_box.py
--rwx------   0 alex       (501) staff       (20)      982 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis.tab
--rwx------   0 alex       (501) staff       (20)      982 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis_permutation_tototo.tab
--rwx------   0 alex       (501) staff       (20)      982 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/zoubida.dada
--rwx------   0 alex       (501) staff       (20)     1082 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/zoubida2.dada
--rwx------   0 alex       (501) staff       (20)     3610 2024-03-26 13:20:44.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/llm.py
--rwx------   0 alex       (501) staff       (20)     3928 2024-03-26 15:12:50.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/load_workflow.py
--rwx------   0 alex       (501) staff       (20)    15322 2024-03-26 13:20:44.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/orange_sub_workflow.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-24 14:31:08.961917 development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/
--rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example1.ows
--rwx------   0 alex       (501) staff       (20)      642 2024-03-26 13:33:44.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example1.txt
--rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example2.ows
--rwx------   0 alex       (501) staff       (20)      695 2024-03-26 13:33:34.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example2.txt
--rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example3.ows
--rwx------   0 alex       (501) staff       (20)      703 2024-03-26 13:33:28.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example3.txt
--rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example4.ows
--rwx------   0 alex       (501) staff       (20)      787 2024-03-26 13:33:14.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example4.txt
--rwx------   0 alex       (501) staff       (20)     6790 2024-03-26 13:20:44.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/shared_functions.py
--rwx------   0 alex       (501) staff       (20)      682 2024-03-26 13:20:46.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/shared_variables.py
--rwx------   0 alex       (501) staff       (20)    33276 2024-03-26 13:20:44.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/subworkflow_input.py
--rwx------   0 alex       (501) staff       (20)     3987 2024-03-26 13:20:44.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/subworkflow_output.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-24 14:31:08.963010 development-tool-0.4.1/orangecontrib/development_tool/widgets/widget_designer/
--rw-r--r--   0 alex       (501) staff       (20)     1861 2024-04-19 07:01:27.000000 development-tool-0.4.1/orangecontrib/development_tool/widgets/widget_designer/document_eater.ui
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-24 14:31:08.965578 development-tool-0.4.1/setup.cfg
--rwx------   0 alex       (501) staff       (20)     1904 2024-04-24 14:31:04.000000 development-tool-0.4.1/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:41.000000 development-tool-0.4.2/
+-rwx------   0 alex       (501) staff       (20)        0 2024-03-26 13:20:44.000000 development-tool-0.4.2/License.txt
+-rw-r--r--   0 alex       (501) staff       (20)      237 2024-04-26 14:51:41.000000 development-tool-0.4.2/PKG-INFO
+-rwx------   0 alex       (501) staff       (20)        9 2024-03-26 13:20:44.000000 development-tool-0.4.2/README.md
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/
+-rwx------   0 alex       (501) staff       (20)      237 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/PKG-INFO
+-rwx------   0 alex       (501) staff       (20)     5336 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/SOURCES.txt
+-rwx------   0 alex       (501) staff       (20)        1 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/dependency_links.txt
+-rwx------   0 alex       (501) staff       (20)       76 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/entry_points.txt
+-rwx------   0 alex       (501) staff       (20)       14 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/namespace_packages.txt
+-rwx------   0 alex       (501) staff       (20)        6 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/requires.txt
+-rwx------   0 alex       (501) staff       (20)       14 2024-04-26 14:51:40.000000 development-tool-0.4.2/development_tool.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/
+-rwx------   0 alex       (501) staff       (20)       55 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/development_tool/
+-rwx------   0 alex       (501) staff       (20)        0 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/
+-rwx------   0 alex       (501) staff       (20)      799 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/Gpt4AllManagement.py
+-rwx------   0 alex       (501) staff       (20)    14328 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/MetManagement.py
+-rwx------   0 alex       (501) staff       (20)     4882 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/VarManagement.py
+-rwx------   0 alex       (501) staff       (20)     2087 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/WrapMessageBox.py
+-rwx------   0 alex       (501) staff       (20)      324 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/__init__.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/dataset_devellopper/
+-rwx------   0 alex       (501) staff       (20)       87 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/dataset_devellopper/fake_input.csv
+-rwx------   0 alex       (501) staff       (20)        0 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/dataset_devellopper/fakeows.ows
+-rwx------   0 alex       (501) staff       (20)       49 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/dataset_devellopper/readme.txt
+-rw-r--r--   0 alex       (501) staff       (20)     9163 2024-04-26 14:50:42.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/document_eater.py
+-rwx------   0 alex       (501) staff       (20)    20858 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/goto.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/
+-rwx------   0 alex       (501) staff       (20)   269355 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Emblem_of_Napoleon_Bonaparte.svg
+-rwx------   0 alex       (501) staff       (20)     4161 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Logo_HKH.svg
+-rwx------   0 alex       (501) staff       (20)     4259 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Logo_HKH_4.svg
+-rwx------   0 alex       (501) staff       (20)     6129 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Logo_HKH_4_jc.svg
+-rwx------   0 alex       (501) staff       (20)  1310135 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Napoleon2.svg
+-rwx------   0 alex       (501) staff       (20)    82296 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Pikachu SVG File.svg
+-rwx------   0 alex       (501) staff       (20)     1364 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Workflow.svg
+-rwx------   0 alex       (501) staff       (20)      506 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/category.svg
+-rwx------   0 alex       (501) staff       (20)    17140 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/chat-bot.png
+-rwx------   0 alex       (501) staff       (20)     9815 2024-03-27 16:51:28.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/data-integration.png
+-rwx------   0 alex       (501) staff       (20)     6493 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/database.svg
+-rwx------   0 alex       (501) staff       (20)    16824 2024-03-13 15:23:26.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/documents.png
+-rwx------   0 alex       (501) staff       (20)     1402 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/download-svgrepo-com.svg
+-rwx------   0 alex       (501) staff       (20)    10205 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/duplicate.png
+-rwx------   0 alex       (501) staff       (20)    40437 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/ecriture.svg
+-rwx------   0 alex       (501) staff       (20)    24354 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/file-transfer.png
+-rwx------   0 alex       (501) staff       (20)    21756 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/goto.png
+-rwx------   0 alex       (501) staff       (20)    38778 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/icon_surrogate_learner.png
+-rwx------   0 alex       (501) staff       (20)    40434 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/icon_surrogate_predict.png
+-rwx------   0 alex       (501) staff       (20)    16844 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/input.png
+-rwx------   0 alex       (501) staff       (20)     4781 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/interrupteur.svg
+-rwx------   0 alex       (501) staff       (20)    29352 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_export_score.png
+-rwx------   0 alex       (501) staff       (20)    20371 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_open_file_resize_alpha_channel.png
+-rwx------   0 alex       (501) staff       (20)    30017 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_optuna_parameters_setting.png
+-rwx------   0 alex       (501) staff       (20)    12060 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_output_table.png
+-rwx------   0 alex       (501) staff       (20)     1801 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/label.svg
+-rwx------   0 alex       (501) staff       (20)    10741 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/lecture.svg
+-rwx------   0 alex       (501) staff       (20)      631 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/mywidget.svg
+-rwx------   0 alex       (501) staff       (20)     1738 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/openai.svg
+-rwx------   0 alex       (501) staff       (20)     3945 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/optuna.svg
+-rwx------   0 alex       (501) staff       (20)    16483 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/output.png
+-rwx------   0 alex       (501) staff       (20)     3591 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/tank-canon-svgrepo-com.svg
+-rwx------   0 alex       (501) staff       (20)    23619 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/tool.png
+-rwx------   0 alex       (501) staff       (20)     2880 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/tutoriel_bouton.svg
+-rwx------   0 alex       (501) staff       (20)      394 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/upload-svgrepo-com.svg
+-rwx------   0 alex       (501) staff       (20)     2516 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/variable_editor.svg
+-rwx------   0 alex       (501) staff       (20)    24762 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/war-svgrepo-com.png
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/
+-rwx------   0 alex       (501) staff       (20)    15981 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/bandeau_pour_orange.png
+-rwx------   0 alex       (501) staff       (20)     9070 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_18px.png
+-rwx------   0 alex       (501) staff       (20)    15224 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_30px.png
+-rwx------   0 alex       (501) staff       (20)     2746 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/interrupteur_ferme.svg
+-rwx------   0 alex       (501) staff       (20)     3530 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/interrupteur_ouvert.svg
+-rwx------   0 alex       (501) staff       (20)     9329 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/khk_label_explanation.svg
+-rwx------   0 alex       (501) staff       (20)     2597 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/refresh.svg
+-rwx------   0 alex       (501) staff       (20)     2598 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/refresh2.svg
+-rwx------   0 alex       (501) staff       (20)     2606 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/img/refresh_with_txt.svg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:40.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/
+-rwx------   0 alex       (501) staff       (20)    19522 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/Table_management.py
+-rwx------   0 alex       (501) staff       (20)     2136 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/Utils_box.py
+-rwx------   0 alex       (501) staff       (20)      982 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis.tab
+-rwx------   0 alex       (501) staff       (20)      982 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis_permutation_tototo.tab
+-rwx------   0 alex       (501) staff       (20)      982 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/zoubida.dada
+-rwx------   0 alex       (501) staff       (20)     1082 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/zoubida2.dada
+-rwx------   0 alex       (501) staff       (20)     3610 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/llm.py
+-rwx------   0 alex       (501) staff       (20)     3928 2024-03-26 15:12:50.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/load_workflow.py
+-rwx------   0 alex       (501) staff       (20)    15322 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/orange_sub_workflow.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:41.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/
+-rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example1.ows
+-rwx------   0 alex       (501) staff       (20)      642 2024-03-26 13:33:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example1.txt
+-rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example2.ows
+-rwx------   0 alex       (501) staff       (20)      695 2024-03-26 13:33:34.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example2.txt
+-rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example3.ows
+-rwx------   0 alex       (501) staff       (20)      703 2024-03-26 13:33:28.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example3.txt
+-rwx------   0 alex       (501) staff       (20)      935 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example4.ows
+-rwx------   0 alex       (501) staff       (20)      787 2024-03-26 13:33:14.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example4.txt
+-rwx------   0 alex       (501) staff       (20)     6790 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/shared_functions.py
+-rwx------   0 alex       (501) staff       (20)      682 2024-03-26 13:20:46.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/shared_variables.py
+-rwx------   0 alex       (501) staff       (20)    33276 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/subworkflow_input.py
+-rwx------   0 alex       (501) staff       (20)     3987 2024-03-26 13:20:44.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/subworkflow_output.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-04-26 14:51:41.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/widget_designer/
+-rw-r--r--   0 alex       (501) staff       (20)     2625 2024-04-26 14:51:03.000000 development-tool-0.4.2/orangecontrib/development_tool/widgets/widget_designer/document_eater.ui
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-04-26 14:51:41.000000 development-tool-0.4.2/setup.cfg
+-rwx------   0 alex       (501) staff       (20)     1904 2024-04-26 14:51:31.000000 development-tool-0.4.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `development-tool-0.4.1/development_tool.egg-info/SOURCES.txt` & `development-tool-0.4.2/development_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/Gpt4AllManagement.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/Gpt4AllManagement.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/MetManagement.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/MetManagement.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/VarManagement.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/VarManagement.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/WrapMessageBox.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/WrapMessageBox.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/document_eater.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/document_eater.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,50 +10,74 @@
 from AnyQt.QtCore import Qt, QObject, pyqtSignal
 
 from langchain.embeddings import HuggingFaceEmbeddings
 from langchain.docstore.document import Document
 from sentence_transformers import SentenceTransformer
 from PyQt5.QtWidgets import QFileDialog, QMessageBox, QPushButton
 from PyQt5 import QtCore
+import copy
+from Orange.data import Domain, StringVariable, ContinuousVariable, Table
+from PyQt5.QtCore import QThread, pyqtSignal
 
+from PyQt5.QtWidgets import QComboBox, QProgressBar
 class DocumentEater(widget.OWWidget):
     name = "DocumentEater"
     description = "Documents ingestion to generate embeddings and store it in db and add it to input file"
     icon = "icons/data-integration.png"
     want_control_area = False
 
     dossier_du_script = os.path.dirname(os.path.abspath(__file__))
     input_data = None
     working_dir = os.path.dirname(os.path.abspath(__file__) + '/tests/')
     model_dir = os.path.join(working_dir, "Models")
     data_dir = os.path.join(working_dir, "Data")
     db_dir = os.path.join(data_dir, "db")
 
     auto_send = False  # Variable de classe pour suivre l'état de la case à cocher
-
+    model_name = None
     dataChanged = pyqtSignal()
 
+    embeddings_generated = False
+
+    progressBar = None
+
     class Inputs:
         input_data = Input("Data", Orange.data.Table)
 
     class Outputs:
         data_out = Output("Data", Orange.data.Table)
 
     @Inputs.input_data
     def set_data(self, input_data):
         self.input_data = input_data
         print("new input data")
         if self.auto_send:  # Si auto_send est activé
             self.generate_embeddings()  # Appeler generate_embeddings automatiquement
 
+        # Réinitialise la barre de progression à 0 si input_data est None
+        if input_data is None:
+                self.progressBar.setValue(0)
+
+
+        # Mettre à jour la combobox avec les noms des colonnes de métadonnées
+        if input_data is not None:
+            meta_columns = [var.name for var in input_data.domain.metas]
+            self.metaComboBox.clear()
+            self.metaComboBox.addItems(meta_columns)
+            # Sélectionne la colonne "content" par défaut si elle existe, sinon sélectionne la première colonne disponible
+            default_column_index = meta_columns.index("content") if "content" in meta_columns else 0
+            self.metaComboBox.setCurrentIndex(default_column_index)
+
     def __init__(self):
         super().__init__()
 
         self.setFixedWidth(470)
         self.setFixedHeight(300)
+
+        self.embeddings_generated = False
         # QT Management
         uic.loadUi(self.dossier_du_script + '/widget_designer/document_eater.ui', self)
 
         self.selectFolderButton = self.findChild(QPushButton, 'push')
         # Connexion du clic du bouton à la méthode pour ouvrir le sélecteur de fichier
         self.selectFolderButton.clicked.connect(self.select_folder)
 
@@ -65,18 +89,29 @@
         self.modelPathLabel.setText("Model Folder Path: Not selected")  # Définir le texte initial
 
         self.generateCheckBox = self.findChild(QtWidgets.QCheckBox,
                                                'checkBox')  # Récupérer le QCheckBox à partir du fichier .ui
         self.generateCheckBox.stateChanged.connect(self.toggle_auto_send)  # Connecter le signal stateChanged
         self.generate.setEnabled(not self.generateCheckBox.isChecked())  # Désactiver le bouton de génération
 
+        # Ajoute cette ligne dans ta méthode __init__ après avoir chargé le fichier UI
+        self.metaComboBox = self.findChild(QComboBox, 'comboBox')
+
+        # Initialise la barre de progression à 0%
+        self.progressBar.setValue(0)
+
     def toggle_auto_send(self, state):
         self.auto_send = state == QtCore.Qt.Checked
         if self.auto_send and self.input_data is not None:
-            self.generate_embeddings()
+            # Vérifie si les embeddings ont déjà été générés
+            if not self.embeddings_generated:
+                self.generate_embeddings()
+        else:
+            # Si auto_send est désactivé ou s'il n'y a pas de données d'entrée, réinitialise la barre de progression à 0
+            self.progressBar.setValue(0)
 
     def select_folder(self):
         # Ouvrir la boîte de dialogue pour sélectionner un dossier
         folder_path = QFileDialog.getExistingDirectory(self, 'Select Folder')
         # Si un dossier a été sélectionné
         if folder_path:
             # Récupérer la liste des fichiers dans le dossier
@@ -86,75 +121,74 @@
                 # Sélectionner le premier fichier dans la liste (peu importe lequel)
                 file_name = files[0]
                 # Construire le chemin complet du fichier en utilisant le chemin du dossier et le nom du fichier
                 model_name = os.path.join(folder_path, file_name)
                 # Mettre à jour self.model_name avec le chemin complet du fichier
                 self.model_name = folder_path
                 self.label.setText(f"Model Folder Path: {folder_path}")
-                # Imprimer le chemin complet du dossier et le nom du fichier
-                print("Chemin du dossier sélectionné:", folder_path)
-                print("Nom du fichier dans le dossier:", file_name)
-                print("Chemin complet du fichier:", self.model_name)
             else:
                 print("Le dossier sélectionné est vide.")
         else:
             print("Aucun dossier sélectionné.")
 
     def generate_embeddings(self):
         try:
             if self.input_data is None:
-                self.Outputs.data_out.send(None)  # Envoyer None si input_data est None
-                return
-
-            data = self.input_data
-
-            df = table_to_frame(data)
-
-            # Initialisation du modèle Sentence Transformers
-            # Ajout repertoire pour aller chercher
-            model_name = getattr(self, 'model_name', None)  # Obtient self.model_name s'il est défini, sinon None
-            if model_name is None:  # or model_name not in SentenceTransformer.available_models():
-                # Utilise "all-mini-lm-6-v2" comme valeur par défaut si self.model_name n'est pas défini ou inconnu
-                model_name = "all-MiniLM-L6-v2"
-                print("Using default model:", model_name)
-
-            model = SentenceTransformer(model_name)
-
-            # Génération des embeddings pour chaque contenu dans la colonne "content"
-            embeddings = []
-
-            # Copie de la table d'entrée + génération des colonnes d'embeddings
-            # Création d'un DataFrame à partir de la datatable
-            data_dict = {}
-            for col in data.domain.variables + data.domain.metas:
-                data_dict[col.name] = []
-
-            for row in data:
-                for col in data.domain.variables + data.domain.metas:
-                    data_dict[col.name].append(row[col].value)
-
-            df = pd.DataFrame(data_dict)
-
-            # Génération des embeddings pour chaque contenu dans la colonne "content"
-            embeddings = []
-            for content in df["content"]:
-                embedding = model.encode(content)
-                embeddings.append(embedding)
-
-            # Création d'un DataFrame pour stocker les embeddings
-            df_embeddings = pd.DataFrame(embeddings, columns=[f'embedding_{i}' for i in range(len(embeddings[0]))])
-
-            # Concaténation du DataFrame des embeddings avec le DataFrame original
-            df_concat = pd.concat([df, df_embeddings], axis=1)
-
-            # Convertir les embeddings en un tableau numpy
-            embeddings = np.array(df[[col for col in df.columns if col.startswith("embedding_")]].values.tolist())
-
-            out_data = table_from_frame(df_concat)
-            print('df_concat', df_concat.columns)
+                out_data = None
+            else:
+                # Initialisation du modèle Sentence Transformers
+                model_name = getattr(self, 'model_name', None)
+                if model_name is None:
+                    model_name = "all-MiniLM-L6-v2"
+                    print("Using default model:", model_name)
+
+                model = SentenceTransformer(model_name)
+
+                # Copy of input data
+                data = copy.deepcopy(self.input_data)
+                attr_dom = list(data.domain.attributes)
+                metas_dom = list(data.domain.metas)
+
+                # Initialisation du modèle Sentence Transformers
+                selected_column_index = self.metaComboBox.currentIndex()
+                selected_column_name = self.input_data.domain.metas[selected_column_index].name
+
+                print("col name:", selected_column_name)
+                # Initialize progress bar
+                self.progressBar.setMaximum(len(data))
+                self.progressBar.setValue(0)
+
+                embeddings = []
+
+                for i, row in enumerate(data):
+                    # Update progress bar value
+                    self.progressBar.setValue(i + 1)
+                    # Generate embeddings for the current row
+                    embeddings.append(model.encode(str(row[selected_column_name])))
+                # Create new metas domains for embeddings
+
+                #embeddings = [model.encode(str(row["content"])) for row in data]
+                n_columns = len(embeddings[0])
+                new_metas_dom = [StringVariable("embedding" + f"_{selected_column_name}" + f"_{i}") for i in range(n_columns)]
+
+                # Create the new updated Domain
+                domain = Domain(attr_dom, metas=metas_dom + new_metas_dom)
+                rows = []
+
+                n = len(data)
+                for i in range(n):
+                    features = list(data[i])
+
+                    metas = list(data.metas[i])
+                    metas += list(embeddings[i])
+                    rows.append(features + metas)
+
+                out_data = Table.from_list(domain, rows=rows)
+                # Met à jour le statut embeddings_generated à True après avoir généré les embeddings avec succès
+                self.embeddings_generated = True
             self.Outputs.data_out.send(out_data)
         except Exception as e:
             print("An error occurred during embeddings processing:", str(e))
 
     def load_input_data(self):
         print("self.data", self.input_data.domain)
```

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/goto.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/goto.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Emblem_of_Napoleon_Bonaparte.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Emblem_of_Napoleon_Bonaparte.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Logo_HKH.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Logo_HKH.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Logo_HKH_4.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Logo_HKH_4.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Logo_HKH_4_jc.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Logo_HKH_4_jc.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Napoleon2.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Napoleon2.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Pikachu SVG File.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Pikachu SVG File.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/Workflow.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/Workflow.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/chat-bot.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/chat-bot.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/data-integration.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/data-integration.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/database.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/database.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/documents.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/documents.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/download-svgrepo-com.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/download-svgrepo-com.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/duplicate.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/duplicate.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/ecriture.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/ecriture.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/file-transfer.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/file-transfer.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/goto.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/goto.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/icon_surrogate_learner.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/icon_surrogate_learner.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/icon_surrogate_predict.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/icon_surrogate_predict.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/input.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/input.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/interrupteur.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/interrupteur.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/jcm_export_score.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_export_score.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/jcm_open_file_resize_alpha_channel.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_open_file_resize_alpha_channel.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/jcm_optuna_parameters_setting.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_optuna_parameters_setting.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/jcm_output_table.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/jcm_output_table.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/label.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/label.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/lecture.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/lecture.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/mywidget.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/mywidget.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/openai.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/openai.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/optuna.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/optuna.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/output.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/output.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/tank-canon-svgrepo-com.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/tank-canon-svgrepo-com.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/tool.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/tool.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/tutoriel_bouton.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/tutoriel_bouton.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/variable_editor.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/variable_editor.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/icons/war-svgrepo-com.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/icons/war-svgrepo-com.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/img/bandeau_pour_orange.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/bandeau_pour_orange.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_18px.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_18px.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_30px.png` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/bandeau_pour_orange_30px.png`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/img/interrupteur_ferme.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/interrupteur_ferme.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/img/interrupteur_ouvert.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/interrupteur_ouvert.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/img/khk_label_explanation.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/khk_label_explanation.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/img/refresh.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/refresh.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/img/refresh2.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/refresh2.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/img/refresh_with_txt.svg` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/img/refresh_with_txt.svg`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/Table_management.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/Table_management.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/Utils_box.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/Utils_box.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis.tab` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis.tab`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis_permutation_tototo.tab` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/supp_moi_bis_permutation_tototo.tab`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/zoubida.dada` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/zoubida.dada`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/kernel_function/zoubida2.dada` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/kernel_function/zoubida2.dada`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/llm.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/llm.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/load_workflow.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/load_workflow.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/orange_sub_workflow.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/orange_sub_workflow.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example1.ows` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example1.ows`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example1.txt` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example1.txt`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example2.ows` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example2.ows`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example2.txt` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example2.txt`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example3.ows` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example3.ows`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example3.txt` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example3.txt`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example4.ows` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example4.ows`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/ows_example/example4.txt` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/ows_example/example4.txt`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/shared_functions.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/shared_functions.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/shared_variables.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/shared_variables.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/subworkflow_input.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/subworkflow_input.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/subworkflow_output.py` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/subworkflow_output.py`

 * *Files identical despite different names*

### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/widget_designer/document_eater.ui` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/widget_designer/document_eater.ui`

 * *Files 18% similar despite different names*

#### Comparing `development-tool-0.4.1/orangecontrib/development_tool/widgets/widget_designer/document_eater.ui` & `development-tool-0.4.2/orangecontrib/development_tool/widgets/widget_designer/document_eater.ui`

```diff
@@ -2,65 +2,65 @@
 <ui version="4.0">
   <class>Form</class>
   <widget class="QWidget" name="Form">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>463</width>
-        <height>299</height>
+        <width>549</width>
+        <height>305</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>Form</string>
     </property>
     <widget class="QPushButton" name="push">
       <property name="geometry">
         <rect>
           <x>30</x>
-          <y>20</y>
+          <y>40</y>
           <width>161</width>
           <height>51</height>
         </rect>
       </property>
       <property name="text">
         <string>Select a model folder</string>
       </property>
     </widget>
     <widget class="QPushButton" name="generate">
       <property name="geometry">
         <rect>
-          <x>250</x>
-          <y>140</y>
+          <x>280</x>
+          <y>200</y>
           <width>141</width>
-          <height>51</height>
+          <height>31</height>
         </rect>
       </property>
       <property name="text">
         <string>Generate embeddings</string>
       </property>
     </widget>
     <widget class="QLabel" name="label">
       <property name="geometry">
         <rect>
-          <x>40</x>
-          <y>80</y>
+          <x>30</x>
+          <y>0</y>
           <width>681</width>
           <height>41</height>
         </rect>
       </property>
       <property name="text">
         <string>Model:</string>
       </property>
     </widget>
     <widget class="QCheckBox" name="checkBox">
       <property name="geometry">
         <rect>
-          <x>40</x>
-          <y>140</y>
+          <x>50</x>
+          <y>200</y>
           <width>221</width>
           <height>41</height>
         </rect>
       </property>
       <property name="text">
         <string>Compute/Send automatically</string>
       </property>
@@ -74,11 +74,47 @@
           <height>16</height>
         </rect>
       </property>
       <property name="text">
         <string>Your input_data requires a &quot;content&quot; column in order to generate embeddings !</string>
       </property>
     </widget>
+    <widget class="QProgressBar" name="progressBar">
+      <property name="geometry">
+        <rect>
+          <x>40</x>
+          <y>110</y>
+          <width>401</width>
+          <height>23</height>
+        </rect>
+      </property>
+      <property name="value">
+        <number>24</number>
+      </property>
+    </widget>
+    <widget class="QComboBox" name="comboBox">
+      <property name="geometry">
+        <rect>
+          <x>290</x>
+          <y>40</y>
+          <width>131</width>
+          <height>41</height>
+        </rect>
+      </property>
+    </widget>
+    <widget class="QLabel" name="label_3">
+      <property name="geometry">
+        <rect>
+          <x>300</x>
+          <y>10</y>
+          <width>141</width>
+          <height>16</height>
+        </rect>
+      </property>
+      <property name="text">
+        <string>Data for embedding</string>
+      </property>
+    </widget>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `development-tool-0.4.1/setup.py` & `development-tool-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI ('pip install development-tool')
 NAME = "development-tool"
 
 # Version du package PyPI
-VERSION = "0.4.1" # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.4.2" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = "alex_hkh"
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = "Library of developed widgets"
 LICENSE = ""
```

