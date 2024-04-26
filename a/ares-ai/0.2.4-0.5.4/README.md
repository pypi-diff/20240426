# Comparing `tmp/ares_ai-0.2.4.tar.gz` & `tmp/ares_ai-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ares_ai-0.2.4.tar", last modified: Fri Apr 26 10:13:58 2024, max compression
+gzip compressed data, was "ares_ai-0.5.4.tar", last modified: Fri Apr 26 09:47:50 2024, max compression
```

## Comparing `ares_ai-0.2.4.tar` & `ares_ai-0.5.4.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:13:58.171701 ares_ai-0.2.4/
--rw-rw-rw-   0 manihani (23549) future   (20099)     4591 2024-04-24 11:52:46.000000 ares_ai-0.2.4/.gitignore
--rw-rw-rw-   0 manihani (23549) future   (20099)      268 2024-04-22 03:39:34.000000 ares_ai-0.2.4/CHANGELOG.md
--rw-rw-rw-   0 manihani (23549) future   (20099)    11357 2024-01-08 23:19:52.000000 ares_ai-0.2.4/LICENSE
--rw-rw-rw-   0 manihani (23549) future   (20099)       51 2024-04-25 23:18:28.000000 ares_ai-0.2.4/MANIFEST.in
--rw-r--r--   0 manihani (23549) future   (20099)    26407 2024-04-26 10:13:58.170701 ares_ai-0.2.4/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)    10868 2024-04-26 10:12:51.000000 ares_ai-0.2.4/README.md
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:13:58.000709 ares_ai-0.2.4/ares/
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:13:58.014708 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/
--rw-rw-rw-   0 manihani (23549) future   (20099)     6952 2024-04-26 08:46:18.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    29589 2024-04-26 09:47:00.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    25648 2024-04-26 09:23:11.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    17172 2024-04-26 08:52:43.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__init__.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:13:58.040707 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)     4441 2024-04-26 08:48:35.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     9876 2024-03-23 04:28:17.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    16631 2024-04-26 09:51:49.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    39678 2024-03-23 04:28:17.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    11077 2024-04-26 09:25:16.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    24854 2024-03-25 00:41:32.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9237 2024-04-26 08:55:30.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    18100 2024-03-23 04:28:17.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      159 2024-04-24 01:00:10.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      175 2024-03-23 04:28:12.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2243 2024-04-24 05:41:16.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2109 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:13:58.059706 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/
--rw-rw-rw-   0 manihani (23549) future   (20099)    33610 2024-04-25 19:02:45.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    42944 2024-04-25 18:44:17.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)       36 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    18046 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     7064 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     8000 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__init__.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:13:58.091705 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)    11001 2024-04-25 19:45:00.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    11341 2024-03-25 23:25:08.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    22313 2024-04-25 18:46:20.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    39551 2024-03-23 04:28:19.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     7856 2024-04-24 01:01:09.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    19694 2024-03-23 04:31:25.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     4238 2024-04-24 01:01:09.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     9481 2024-03-23 04:31:25.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      158 2024-04-24 01:01:00.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      169 2024-02-08 01:18:18.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     5437 2024-01-20 22:01:06.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     8966 2024-04-24 01:01:00.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    19175 2024-03-23 04:28:19.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      494 2024-01-20 21:58:30.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/ppi.py
--rw-rw-rw-   0 manihani (23549) future   (20099)       22 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/__init__.py
--rw-r--r--   0 manihani (23549) future   (20099)      152 2024-03-25 00:40:39.000000 ares_ai-0.2.4/ares/__init__.pyc
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:13:58.126703 ares_ai-0.2.4/ares/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)      166 2024-04-24 01:00:10.000000 ares_ai-0.2.4/ares/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      196 2024-03-23 04:28:12.000000 ares_ai-0.2.4/ares/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     7504 2024-04-24 11:55:06.000000 ares_ai-0.2.4/ares/__pycache__/ares.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     9734 2024-03-25 23:24:58.000000 ares_ai-0.2.4/ares/__pycache__/ares.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     4163 2024-04-24 11:55:12.000000 ares_ai-0.2.4/ares/__pycache__/binary_classifier.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     3676 2024-03-23 04:28:17.000000 ares_ai-0.2.4/ares/__pycache__/binary_classifier.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      371 2024-04-24 01:01:09.000000 ares_ai-0.2.4/ares/__pycache__/kilt_filter.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      469 2024-03-23 04:31:25.000000 ares_ai-0.2.4/ares/__pycache__/kilt_filter.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2294 2024-04-24 11:55:14.000000 ares_ai-0.2.4/ares/__pycache__/rag_scoring.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     2495 2024-03-23 04:28:19.000000 ares_ai-0.2.4/ares/__pycache__/rag_scoring.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      356 2024-04-24 01:01:09.000000 ares_ai-0.2.4/ares/__pycache__/superglue_filter.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)      442 2024-03-23 04:31:25.000000 ares_ai-0.2.4/ares/__pycache__/superglue_filter.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2419 2024-04-26 07:58:28.000000 ares_ai-0.2.4/ares/__pycache__/synthetic_generator.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     3600 2024-03-23 04:28:12.000000 ares_ai-0.2.4/ares/__pycache__/synthetic_generator.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     4840 2024-04-24 11:55:15.000000 ares_ai-0.2.4/ares/__pycache__/ues_idp.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     5858 2024-03-25 23:25:08.000000 ares_ai-0.2.4/ares/__pycache__/ues_idp.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    11651 2024-04-24 11:48:03.000000 ares_ai-0.2.4/ares/ares.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:13:58.139702 ares_ai-0.2.4/ares/ares_ai.egg-info/
--rw-r--r--   0 manihani (23549) future   (20099)    26304 2024-04-05 05:20:31.000000 ares_ai-0.2.4/ares/ares_ai.egg-info/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-05 05:20:31.000000 ares_ai-0.2.4/ares/ares_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 05:20:31.000000 ares_ai-0.2.4/ares/ares_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 05:20:31.000000 ares_ai-0.2.4/ares/ares_ai.egg-info/entry_points.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)      627 2024-04-05 05:20:31.000000 ares_ai-0.2.4/ares/ares_ai.egg-info/requires.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 05:20:31.000000 ares_ai-0.2.4/ares/ares_ai.egg-info/top_level.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)     8082 2024-04-24 11:17:32.000000 ares_ai-0.2.4/ares/binary_classifier.py
--rw-rw-rw-   0 manihani (23549) future   (20099)      154 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/kilt_filter.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:13:58.145702 ares_ai-0.2.4/ares/ppi/
--rw-rw-rw-   0 manihani (23549) future   (20099)     6148 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/ppi/.DS_Store
--rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/ppi/ppi.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     9196 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/ppi/ppi_testing.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     6085 2024-04-24 11:39:44.000000 ares_ai-0.2.4/ares/rag_scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)      134 2024-04-22 03:39:34.000000 ares_ai-0.2.4/ares/superglue_filter.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     4332 2024-04-26 07:54:48.000000 ares_ai-0.2.4/ares/synthetic_generator.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    10206 2024-04-24 11:36:32.000000 ares_ai-0.2.4/ares/ues_idp.py
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:13:58.167701 ares_ai-0.2.4/ares_ai.egg-info/
--rw-r--r--   0 manihani (23549) future   (20099)    26407 2024-04-26 10:13:52.000000 ares_ai-0.2.4/ares_ai.egg-info/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)     4221 2024-04-26 10:13:57.000000 ares_ai-0.2.4/ares_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-26 10:13:52.000000 ares_ai-0.2.4/ares_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-26 10:13:52.000000 ares_ai-0.2.4/ares_ai.egg-info/entry_points.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)      682 2024-04-26 10:13:52.000000 ares_ai-0.2.4/ares_ai.egg-info/requires.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-26 10:13:52.000000 ares_ai-0.2.4/ares_ai.egg-info/top_level.txt
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:13:58.163701 ares_ai-0.2.4/checkpoints/
--rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:34.000000 ares_ai-0.2.4/checkpoints/.gitignore
--rw-rw-rw-   0 manihani (23549) future   (20099)     2905 2024-04-26 10:13:26.000000 ares_ai-0.2.4/pyproject.toml
--rw-rw-rw-   0 manihani (23549) future   (20099)     5066 2024-04-26 03:07:42.000000 ares_ai-0.2.4/requirements.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       93 2024-04-26 10:13:58.173701 ares_ai-0.2.4/setup.cfg
-drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 10:13:58.165701 ares_ai-0.2.4/tests/
--rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:53.000000 ares_ai-0.2.4/tests/.gitignore
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 09:47:50.483091 ares_ai-0.5.4/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4591 2024-04-24 11:52:46.000000 ares_ai-0.5.4/.gitignore
+-rw-rw-rw-   0 manihani (23549) future   (20099)      268 2024-04-22 03:39:34.000000 ares_ai-0.5.4/CHANGELOG.md
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11357 2024-01-08 23:19:52.000000 ares_ai-0.5.4/LICENSE
+-rw-rw-rw-   0 manihani (23549) future   (20099)       51 2024-04-25 23:18:28.000000 ares_ai-0.5.4/MANIFEST.in
+-rw-r--r--   0 manihani (23549) future   (20099)    26423 2024-04-26 09:47:50.482091 ares_ai-0.5.4/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10884 2024-04-26 09:28:53.000000 ares_ai-0.5.4/README.md
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 09:47:50.318098 ares_ai-0.5.4/ares/
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 09:47:50.331098 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     6952 2024-04-26 08:46:18.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    29589 2024-04-26 09:47:00.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    25648 2024-04-26 09:23:11.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    17172 2024-04-26 08:52:43.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__init__.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 09:47:50.356097 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4441 2024-04-26 08:48:35.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     9876 2024-03-23 04:28:17.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    16446 2024-04-24 11:55:12.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    39678 2024-03-23 04:28:17.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11077 2024-04-26 09:25:16.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    24854 2024-03-25 00:41:32.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9237 2024-04-26 08:55:30.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    18100 2024-03-23 04:28:17.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      159 2024-04-24 01:00:10.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      175 2024-03-23 04:28:12.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2243 2024-04-24 05:41:16.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2109 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 09:47:50.373096 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    33610 2024-04-25 19:02:45.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    42944 2024-04-25 18:44:17.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)       36 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    18046 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7064 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8000 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__init__.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 09:47:50.404095 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11001 2024-04-25 19:45:00.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    11341 2024-03-25 23:25:08.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    22313 2024-04-25 18:46:20.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    39551 2024-03-23 04:28:19.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7856 2024-04-24 01:01:09.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    19694 2024-03-23 04:31:25.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4238 2024-04-24 01:01:09.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     9481 2024-03-23 04:31:25.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      158 2024-04-24 01:01:00.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      169 2024-02-08 01:18:18.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5437 2024-01-20 22:01:06.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8966 2024-04-24 01:01:00.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    19175 2024-03-23 04:28:19.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      494 2024-01-20 21:58:30.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/ppi.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)       22 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/__init__.py
+-rw-r--r--   0 manihani (23549) future   (20099)      152 2024-03-25 00:40:39.000000 ares_ai-0.5.4/ares/__init__.pyc
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 09:47:50.438093 ares_ai-0.5.4/ares/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)      166 2024-04-24 01:00:10.000000 ares_ai-0.5.4/ares/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      196 2024-03-23 04:28:12.000000 ares_ai-0.5.4/ares/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7504 2024-04-24 11:55:06.000000 ares_ai-0.5.4/ares/__pycache__/ares.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     9734 2024-03-25 23:24:58.000000 ares_ai-0.5.4/ares/__pycache__/ares.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4163 2024-04-24 11:55:12.000000 ares_ai-0.5.4/ares/__pycache__/binary_classifier.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     3676 2024-03-23 04:28:17.000000 ares_ai-0.5.4/ares/__pycache__/binary_classifier.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      371 2024-04-24 01:01:09.000000 ares_ai-0.5.4/ares/__pycache__/kilt_filter.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      469 2024-03-23 04:31:25.000000 ares_ai-0.5.4/ares/__pycache__/kilt_filter.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2294 2024-04-24 11:55:14.000000 ares_ai-0.5.4/ares/__pycache__/rag_scoring.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     2495 2024-03-23 04:28:19.000000 ares_ai-0.5.4/ares/__pycache__/rag_scoring.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      356 2024-04-24 01:01:09.000000 ares_ai-0.5.4/ares/__pycache__/superglue_filter.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)      442 2024-03-23 04:31:25.000000 ares_ai-0.5.4/ares/__pycache__/superglue_filter.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2419 2024-04-26 07:58:28.000000 ares_ai-0.5.4/ares/__pycache__/synthetic_generator.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     3600 2024-03-23 04:28:12.000000 ares_ai-0.5.4/ares/__pycache__/synthetic_generator.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4840 2024-04-24 11:55:15.000000 ares_ai-0.5.4/ares/__pycache__/ues_idp.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     5858 2024-03-25 23:25:08.000000 ares_ai-0.5.4/ares/__pycache__/ues_idp.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11651 2024-04-24 11:48:03.000000 ares_ai-0.5.4/ares/ares.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 09:47:50.450092 ares_ai-0.5.4/ares/ares_ai.egg-info/
+-rw-r--r--   0 manihani (23549) future   (20099)    26304 2024-04-05 05:20:31.000000 ares_ai-0.5.4/ares/ares_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-05 05:20:31.000000 ares_ai-0.5.4/ares/ares_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 05:20:31.000000 ares_ai-0.5.4/ares/ares_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 05:20:31.000000 ares_ai-0.5.4/ares/ares_ai.egg-info/entry_points.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)      627 2024-04-05 05:20:31.000000 ares_ai-0.5.4/ares/ares_ai.egg-info/requires.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 05:20:31.000000 ares_ai-0.5.4/ares/ares_ai.egg-info/top_level.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8082 2024-04-24 11:17:32.000000 ares_ai-0.5.4/ares/binary_classifier.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)      154 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/kilt_filter.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 09:47:50.456092 ares_ai-0.5.4/ares/ppi/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     6148 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/ppi/.DS_Store
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9054 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/ppi/ppi.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9196 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/ppi/ppi_testing.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     6085 2024-04-24 11:39:44.000000 ares_ai-0.5.4/ares/rag_scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)      134 2024-04-22 03:39:34.000000 ares_ai-0.5.4/ares/superglue_filter.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4332 2024-04-26 07:54:48.000000 ares_ai-0.5.4/ares/synthetic_generator.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10206 2024-04-24 11:36:32.000000 ares_ai-0.5.4/ares/ues_idp.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 09:47:50.477091 ares_ai-0.5.4/ares_ai.egg-info/
+-rw-r--r--   0 manihani (23549) future   (20099)    26423 2024-04-26 09:47:43.000000 ares_ai-0.5.4/ares_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4221 2024-04-26 09:47:50.000000 ares_ai-0.5.4/ares_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-26 09:47:43.000000 ares_ai-0.5.4/ares_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-26 09:47:43.000000 ares_ai-0.5.4/ares_ai.egg-info/entry_points.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)      682 2024-04-26 09:47:43.000000 ares_ai-0.5.4/ares_ai.egg-info/requires.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-26 09:47:43.000000 ares_ai-0.5.4/ares_ai.egg-info/top_level.txt
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 09:47:50.474091 ares_ai-0.5.4/checkpoints/
+-rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:34.000000 ares_ai-0.5.4/checkpoints/.gitignore
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2905 2024-04-26 09:47:29.000000 ares_ai-0.5.4/pyproject.toml
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5066 2024-04-26 03:07:42.000000 ares_ai-0.5.4/requirements.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       93 2024-04-26 09:47:50.485091 ares_ai-0.5.4/setup.cfg
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-04-26 09:47:50.476091 ares_ai-0.5.4/tests/
+-rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:53.000000 ares_ai-0.5.4/tests/.gitignore
```

### Comparing `ares_ai-0.2.4/.gitignore` & `ares_ai-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/LICENSE` & `ares_ai-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/PKG-INFO` & `ares_ai-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.2.4
+Version: 0.5.4
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -362,15 +362,15 @@
 OPTIONAL: You can run the following command to get the full NQ dataset! (347 MB)
 ```python
 from ares import ARES
 ares = ARES() 
 ares.KILT_dataset("nq")
 
 # Fetches NQ datasets with ratios including 0.5, 0.6, 0.7, etc.
-# For purposes of our quick start guide, we rename nq_ratio_0.5 to nq_unlabeled_output and nq_labeled_output.
+# For purposes of our quick start guide, we rename nq_ratio_0.5 to nq_unlabeled_output and nq_ratio_0.6 to nq_labeled_output.
 ```
 <hr>
 
 ### 🚀 Quick Start - #1
 
 <hr>
```

### Comparing `ares_ai-0.2.4/README.md` & `ares_ai-0.5.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 OPTIONAL: You can run the following command to get the full NQ dataset! (347 MB)
 ```python
 from ares import ARES
 ares = ARES() 
 ares.KILT_dataset("nq")
 
 # Fetches NQ datasets with ratios including 0.5, 0.6, 0.7, etc.
-# For purposes of our quick start guide, we rename nq_ratio_0.5 to nq_unlabeled_output and nq_labeled_output.
+# For purposes of our quick start guide, we rename nq_ratio_0.5 to nq_unlabeled_output and nq_ratio_0.6 to nq_labeled_output.
 ```
 <hr>
 
 ### 🚀 Quick Start - #1
 
 <hr>
```

#### html2text {}

```diff
@@ -56,15 +56,15 @@
 raw.githubusercontent.com/stanford-futuredata/ARES/main/datasets/example_files/
 nq_labeled_output.tsv wget https://raw.githubusercontent.com/stanford-
 futuredata/ARES/main/datasets/example_files/nq_unlabeled_output.tsv ```
 OPTIONAL: You can run the following command to get the full NQ dataset! (347
 MB) ```python from ares import ARES ares = ARES() ares.KILT_dataset("nq") #
 Fetches NQ datasets with ratios including 0.5, 0.6, 0.7, etc. # For purposes of
 our quick start guide, we rename nq_ratio_0.5 to nq_unlabeled_output and
-nq_labeled_output. ```
+nq_ratio_0.6 to nq_labeled_output. ```
 ===============================================================================
 ### ð Quick Start - #1
 ===============================================================================
 To get started with ARES's PPI, you'll need to set up your configuration. Below
 is an example of a configuration for ARES! Just copy-paste as you go to see
 ARES in action! Step 1) Run the following to retrive the UES/IDP scores with
 GPT3.5! ```python from ares import ARES ues_idp_config =
```

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Apr 26 09:47:00 2024 UTC, .py size: 29589 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 1478 2b66 9573 0000  o........x+f.s..
+00000000: 6f0d 0d0a 0000 0000 6dee 2866 a672 0000  o.......m.(f.r..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 dc02 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 c602 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c02 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 0100 6400 6401 6c0a 5a0b 6400  m.Z...d.d.l.Z.d.
 00000070: 6401 6c0c 5a0d 6400 6401 6c0e 5a0e 6400  d.l.Z.d.d.l.Z.d.
 00000080: 6401 6c0f 5a0f 6400 6404 6c0f 6d10 5a10  d.l.Z.d.d.l.m.Z.
 00000090: 0100 6400 6405 6c02 6d11 5a11 6d12 5a12  ..d.d.l.m.Z.m.Z.
@@ -15,1026 +15,1014 @@
 000000e0: 6d1f 5a1f 0100 6400 6401 6c20 5a20 6400  m.Z...d.d.l Z d.
 000000f0: 6409 6c21 6d22 5a22 0100 6400 6401 6c23  d.l!m"Z"..d.d.l#
 00000100: 5a23 6400 6401 6c24 5a24 6400 6401 6c25  Z#d.d.l$Z$d.d.l%
 00000110: 5a26 6400 6401 6c27 5a27 6400 640a 6c28  Z&d.d.l'Z'd.d.l(
 00000120: 6d29 5a29 0100 6400 6401 6c2a 5a2a 6400  m)Z)..d.d.l*Z*d.
 00000130: 6401 6c2b 5a2b 6400 6401 6c2c 5a2c 6400  d.l+Z+d.d.l,Z,d.
 00000140: 6401 6c2d 5a2d 6400 640b 6c22 6d22 5a22  d.l-Z-d.d.l"m"Z"
-00000150: 6d2e 5a2e 0100 6400 6401 6c2f 5a2f 652f  m.Z...d.d.l/Z/e/
-00000160: 6a30 640c 640d 640e 8d02 0100 6441 640f  j0d.d.d.....dAd.
-00000170: 6531 6410 6531 6604 6411 6412 8405 5a32  e1d.e1f.d.d...Z2
-00000180: 6413 6531 6410 6531 6604 6414 6415 8404  d.e1d.e1f.d.d...
-00000190: 5a33 6416 5a34 650d 6a2b a035 6534 a101  Z3d.Z4e.j+.5e4..
-000001a0: 0100 652b a035 6534 a101 0100 6520 a036  ..e+.5e4....e .6
-000001b0: 6534 a101 0100 6531 6534 8301 6527 6a37  e4....e1e4..e'j7
-000001c0: 6417 3c00 6418 6419 8400 5a38 4700 641a  d.<.d.d...Z8G.d.
-000001d0: 641b 8400 641b 6501 6a39 8303 5a3a 641c  d...d.e.j9..Z:d.
-000001e0: 641d 8400 5a3b 641e 641f 8400 5a3c 6420  d...Z;d.d...Z<d 
-000001f0: 6421 8400 5a3d 6422 6423 8400 5a3e 6424  d!..Z=d"d#..Z>d$
-00000200: 6425 8400 5a3f 6426 6427 8400 5a40 6428  d%..Z?d&d'..Z@d(
-00000210: 6429 8400 5a41 642a 642b 8400 5a42 642c  d)..ZAd*d+..ZBd,
-00000220: 642d 8400 5a43 642e 642f 8400 5a44 6430  d-..ZCd.d/..ZDd0
-00000230: 6431 8400 5a45 6432 6433 8400 5a46 6547  d1..ZEd2d3..ZFeG
-00000240: 6434 6b02 9001 726c 652d a048 a100 5a49  d4k...rle-.H..ZI
-00000250: 6549 6a4a 6435 6531 6436 6437 8d03 0100  eIjJd5e1d6d7....
-00000260: 6549 6a4a 6438 6531 6436 6437 8d03 0100  eIjJd8e1d6d7....
-00000270: 6549 6a4a 6439 6531 6436 6437 8d03 0100  eIjJd9e1d6d7....
-00000280: 6549 6a4a 643a 654b 6436 6437 8d03 0100  eIjJd:eKd6d7....
-00000290: 6549 6a4a 643b 654b 6436 6437 8d03 0100  eIjJd;eKd6d7....
-000002a0: 6549 6a4a 643c 654c 6436 6437 8d03 0100  eIjJd<eLd6d7....
-000002b0: 6549 a04d a100 5a4e 654e 6a4f 6701 5a50  eI.M..ZNeNjOg.ZP
-000002c0: 654e 6a51 5a51 654e 6a52 5a52 654e 6a53  eNjQZQeNjRZReNjS
-000002d0: 5a53 654e 6a54 5a54 654e 6a55 6701 5a56  ZSeNjTZTeNjUg.ZV
-000002e0: 643d 5a57 6520 a057 6557 a101 5a57 6436  d=ZWe .WeW..ZWd6
-000002f0: 5a58 643e 5a59 643f 5a5a 643e 5a5b 6440  ZXd>ZYd?ZZd>Z[d@
-00000300: 5a5c 6401 5300 6401 5300 2942 e900 0000  Z\d.S.d.S.)B....
-00000310: 004e 2903 da0b 5435 546f 6b65 6e69 7a65  .N)...T5Tokenize
-00000320: 72da 0e54 3545 6e63 6f64 6572 4d6f 6465  r..T5EncoderMode
-00000330: 6cda 1a54 3546 6f72 436f 6e64 6974 696f  l..T5ForConditio
-00000340: 6e61 6c47 656e 6572 6174 696f 6e29 04da  nalGeneration)..
-00000350: 0942 6572 744d 6f64 656c da0d 4175 746f  .BertModel..Auto
-00000360: 546f 6b65 6e69 7a65 72da 0941 7574 6f4d  Tokenizer..AutoM
-00000370: 6f64 656c da0d 4750 5432 546f 6b65 6e69  odel..GPT2Tokeni
-00000380: 7a65 7229 01da 0b6c 6f61 645f 6d65 7472  zer)...load_metr
-00000390: 6963 2902 da11 5472 6169 6e69 6e67 4172  ic)...TrainingAr
-000003a0: 6775 6d65 6e74 73da 0754 7261 696e 6572  guments..Trainer
-000003b0: 2901 da04 4164 616d 2901 da0a 4461 7461  )...Adam)...Data
-000003c0: 4c6f 6164 6572 2904 da0d 6765 745f 7363  Loader)...get_sc
-000003d0: 6865 6475 6c65 72da 1441 7574 6f4d 6f64  heduler..AutoMod
-000003e0: 656c 466f 7243 6175 7361 6c4c 4dda 0a41  elForCausalLM..A
-000003f0: 7574 6f43 6f6e 6669 67da 2241 7574 6f4d  utoConfig."AutoM
-00000400: 6f64 656c 466f 7253 6571 7565 6e63 6543  odelForSequenceC
-00000410: 6c61 7373 6966 6963 6174 696f 6e29 01da  lassification)..
-00000420: 0474 7164 6d29 01da 1074 7261 696e 5f74  .tqdm)...train_t
-00000430: 6573 745f 7370 6c69 7429 0272 1200 0000  est_split).r....
-00000440: da0b 7471 646d 5f70 616e 6461 73da 0669  ..tqdm_pandas..i
-00000450: 676e 6f72 657a 9654 6865 2073 656e 7465  gnorez.The sente
-00000460: 6e63 6570 6965 6365 2074 6f6b 656e 697a  ncepiece tokeniz
-00000470: 6572 2074 6861 7420 796f 7520 6172 6520  er that you are 
-00000480: 636f 6e76 6572 7469 6e67 2074 6f20 6120  converting to a 
-00000490: 6661 7374 2074 6f6b 656e 697a 6572 2075  fast tokenizer u
-000004a0: 7365 7320 7468 6520 6279 7465 2066 616c  ses the byte fal
-000004b0: 6c62 6163 6b20 6f70 7469 6f6e 2077 6869  lback option whi
-000004c0: 6368 2069 7320 6e6f 7420 696d 706c 656d  ch is not implem
-000004d0: 656e 7465 6420 696e 2074 6865 2066 6173  ented in the fas
-000004e0: 7420 746f 6b65 6e69 7a65 7273 2e29 01da  t tokenizers.)..
-000004f0: 076d 6573 7361 6765 da05 7175 6572 79da  .message..query.
-00000500: 0864 6f63 756d 656e 7463 0300 0000 0000  .documentc......
-00000510: 0000 0000 0000 0400 0000 0800 0000 4300  ..............C.
-00000520: 0000 731e 0100 0074 00a0 0164 0164 027c  ..s....t...d.d.|
-00000530: 01a0 0264 0364 04a1 02a0 0264 0564 04a1  ...d.d.....d.d..
-00000540: 02a1 03a0 03a1 007d 037c 03a0 0264 0664  .......}.|...d.d
-00000550: 04a1 02a0 0264 0764 04a1 027d 0374 00a0  .....d.d...}.t..
-00000560: 0164 0864 047c 03a1 03a0 03a1 007d 0364  .d.d.|.......}.d
-00000570: 04a0 047c 03a0 0564 04a1 0164 0064 0985  ...|...d...d.d..
-00000580: 0219 00a1 017d 0374 067c 00a0 0564 04a1  .....}.t.|...d..
-00000590: 0183 0164 0a6b 0472 4564 04a0 047c 00a0  ...d.k.rEd...|..
-000005a0: 0564 04a1 0164 0064 0b85 0219 00a1 017d  .d...d.d.......}
-000005b0: 007c 0264 0075 0072 4f7c 0064 0c17 007c  .|.d.u.rO|.d...|
-000005c0: 0317 0053 007a 0b7c 0064 0c17 007c 0317  ...S.z.|.d...|..
-000005d0: 0064 0c17 007c 0217 0057 0053 0001 0001  .d...|...W.S....
-000005e0: 0001 0074 0783 0001 0074 0864 0d83 0101  ...t.....t.d....
-000005f0: 0074 0864 0e74 097c 0083 0117 0083 0101  .t.d.t.|........
-00000600: 0074 0864 0f74 097c 0383 0117 0083 0101  .t.d.t.|........
-00000610: 0074 0864 1074 097c 0283 0117 0083 0101  .t.d.t.|........
-00000620: 0074 097c 0083 0164 0c17 0074 097c 0383  .t.|...d...t.|..
-00000630: 0117 0064 0c17 0074 097c 0283 0117 0006  ...d...t.|......
-00000640: 0059 0053 0029 114e fa03 5c6e 2bda 010a  .Y.S.).N..\n+...
-00000650: fa01 0dda 0120 fa01 09da 013d da01 2dfa  ..... .....=..-.
-00000660: 035c 732b e900 0200 00e9 6400 0000 e91e  .\s+......d.....
-00000670: 0000 007a 0320 7c20 7a21 4572 726f 7220  ...z. | z!Error 
-00000680: 7769 7468 2063 6f6d 6269 6e65 5f71 7565  with combine_que
-00000690: 7279 5f64 6f63 756d 656e 747a 0751 7565  ry_documentz.Que
-000006a0: 7279 3a20 7a12 436c 6561 6e65 6420 446f  ry: z.Cleaned Do
-000006b0: 6375 6d65 6e74 3a20 7a08 416e 7377 6572  cument: z.Answer
-000006c0: 3a20 290a da02 7265 da03 7375 62da 0772  : )...re..sub..r
-000006d0: 6570 6c61 6365 da05 7374 7269 70da 046a  eplace..strip..j
-000006e0: 6f69 6eda 0573 706c 6974 da03 6c65 6eda  oin..split..len.
-000006f0: 0a62 7265 616b 706f 696e 74da 0570 7269  .breakpoint..pri
-00000700: 6e74 da03 7374 7229 0472 1700 0000 7218  nt..str).r....r.
-00000710: 0000 00da 0661 6e73 7765 72da 1063 6c65  .....answer..cle
-00000720: 616e 6564 5f64 6f63 756d 656e 74a9 0072  aned_document..r
-00000730: 3000 0000 fa53 2f66 7574 7572 652f 752f  0....S/future/u/
-00000740: 6d61 6e69 6861 6e69 2f41 5245 532f 6172  manihani/ARES/ar
-00000750: 6573 2f4c 4c4d 5f61 735f 615f 4a75 6467  es/LLM_as_a_Judg
-00000760: 655f 4164 6170 7461 7469 6f6e 2f47 656e  e_Adaptation/Gen
-00000770: 6572 616c 5f42 696e 6172 795f 436c 6173  eral_Binary_Clas
-00000780: 7369 6669 6572 2e70 79da 1663 6f6d 6269  sifier.py..combi
-00000790: 6e65 5f71 7565 7279 5f64 6f63 756d 656e  ne_query_documen
-000007a0: 742b 0000 0073 2200 0000 2201 1401 1201  t+...s"...".....
-000007b0: 1801 1202 1801 0802 0c01 0202 1601 0601  ................
-000007c0: 0601 0801 1001 1001 1001 2401 7232 0000  ..........$.r2..
-000007d0: 00da 0871 7565 7374 696f 6e63 0200 0000  ...questionc....
-000007e0: 0000 0000 0000 0000 0400 0000 0800 0000  ................
-000007f0: 4300 0000 73a0 0000 0064 017d 027c 0264  C...s....d.}.|.d
-00000800: 0237 007d 0274 00a0 0164 0364 047c 01a0  .7.}.t...d.d.|..
-00000810: 0264 0564 06a1 02a0 0264 0764 06a1 02a1  .d.d.....d.d....
-00000820: 03a0 03a1 007d 037c 03a0 0264 0864 06a1  .....}.|...d.d..
-00000830: 02a0 0264 0964 06a1 027d 0374 00a0 0164  ...d.d...}.t...d
-00000840: 0a64 067c 03a1 03a0 03a1 007d 0364 06a0  .d.|.......}.d..
-00000850: 047c 03a0 0564 06a1 0164 0064 0b85 0219  .|...d...d.d....
-00000860: 00a1 017d 037c 0264 0c37 007d 027c 0264  ...}.|.d.7.}.|.d
-00000870: 0d7c 0017 0064 0417 0037 007d 027c 0264  .|...d...7.}.|.d
-00000880: 0e7c 0317 0064 0417 0037 007d 027c 0264  .|...d...7.}.|.d
-00000890: 0f37 007d 027c 0253 0029 104e 7a43 596f  .7.}.|.S.).NzCYo
-000008a0: 7520 6172 6520 616e 2065 7870 6572 7420  u are an expert 
-000008b0: 6a75 6467 6520 666f 7220 6576 616c 7561  judge for evalua
-000008c0: 7469 6e67 2071 7565 7374 696f 6e20 616e  ting question an
-000008d0: 7377 6572 696e 6720 7379 7374 656d 732e  swering systems.
-000008e0: 207a 9747 6976 656e 2074 6865 2066 6f6c   z.Given the fol
-000008f0: 6c6f 7769 6e67 2071 7565 7374 696f 6e20  lowing question 
-00000900: 616e 6420 646f 6375 6d65 6e74 2c20 796f  and document, yo
-00000910: 7520 6d75 7374 2061 6e61 6c79 7a65 2074  u must analyze t
-00000920: 6865 2070 726f 7669 6465 6420 646f 6375  he provided docu
-00000930: 6d65 6e74 2061 6e64 2064 6574 6572 6d69  ment and determi
-00000940: 6e65 2077 6865 7468 6572 2069 7420 6973  ne whether it is
-00000950: 2073 7566 6669 6369 656e 7420 666f 7220   sufficient for 
-00000960: 616e 7377 6572 696e 6720 7468 6520 7175  answering the qu
-00000970: 6573 7469 6f6e 2e20 0a0a 7219 0000 0072  estion. ..r....r
-00000980: 1a00 0000 721b 0000 0072 1c00 0000 721d  ....r....r....r.
-00000990: 0000 0072 1e00 0000 721f 0000 0072 2000  ...r....r....r .
-000009a0: 0000 7221 0000 007a 1123 2323 2049 6e73  ..r!...z.### Ins
-000009b0: 7472 7563 7469 6f6e 3a0a 7a0a 5175 6573  truction:.z.Ques
-000009c0: 7469 6f6e 3a20 7a0a 446f 6375 6d65 6e74  tion: z.Document
-000009d0: 3a20 7a0e 2323 2320 5265 7370 6f6e 7365  : z.### Response
-000009e0: 3a0a 2906 7224 0000 0072 2500 0000 7226  :.).r$...r%...r&
-000009f0: 0000 0072 2700 0000 7228 0000 0072 2900  ...r'...r(...r).
-00000a00: 0000 2904 7233 0000 0072 1800 0000 da0b  ..).r3...r......
-00000a10: 696e 7374 7275 6374 696f 6e72 2f00 0000  instructionr/...
-00000a20: 7230 0000 0072 3000 0000 7231 0000 00da  r0...r0...r1....
-00000a30: 4566 6f72 6d61 745f 7465 7874 5f66 6f72  Eformat_text_for
-00000a40: 5f66 696e 655f 7475 6e69 6e67 5f63 6f6e  _fine_tuning_con
-00000a50: 7465 6e74 5f72 656c 6576 616e 6365 5f73  tent_relevance_s
-00000a60: 6571 7565 6e63 655f 636c 6173 7369 6669  equence_classifi
-00000a70: 6361 7469 6f6e 4100 0000 7316 0000 0004  cationA...s.....
-00000a80: 0108 0122 0214 0112 0118 0108 0210 0110  ..."............
-00000a90: 0108 0104 0272 3500 0000 e92a 0000 005a  .....r5....*...Z
-00000aa0: 0e50 5954 484f 4e48 4153 4853 4545 4463  .PYTHONHASHSEEDc
-00000ab0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00000ac0: 0400 0000 4300 0000 7344 0000 0064 017d  ....C...sD...d.}
-00000ad0: 0074 00a0 017c 00a0 02a1 00a1 01a0 0364  .t...|.........d
-00000ae0: 02a1 01a0 0264 03a1 0164 0064 0485 0219  .....d...d.d....
-00000af0: 0064 0564 0085 0219 007d 0164 0664 0784  .d.d.....}.d.d..
-00000b00: 0074 047c 0183 0144 0083 017d 027c 0253  .t.|...D...}.|.S
-00000b10: 0029 084e 7a2f 6e76 6964 6961 2d73 6d69  .).Nz/nvidia-smi
-00000b20: 202d 2d71 7565 7279 2d67 7075 3d6d 656d   --query-gpu=mem
-00000b30: 6f72 792e 6672 6565 202d 2d66 6f72 6d61  ory.free --forma
-00000b40: 743d 6373 76da 0561 7363 6969 721a 0000  t=csv..asciir...
-00000b50: 00e9 ffff ffff e901 0000 0063 0100 0000  ...........c....
-00000b60: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-00000b70: 5300 0000 7320 0000 0067 007c 005d 0c5c  S...s ...g.|.].\
-00000b80: 027d 017d 0274 007c 02a0 01a1 0064 0019  .}.}.t.|.....d..
-00000b90: 0083 0191 0271 0253 0029 0172 0100 0000  .....q.S.).r....
-00000ba0: 2902 da03 696e 7472 2900 0000 2903 da02  )...intr)...)...
-00000bb0: 2e30 da01 69da 0178 7230 0000 0072 3000  .0..i..xr0...r0.
-00000bc0: 0000 7231 0000 00da 0a3c 6c69 7374 636f  ..r1.....<listco
-00000bd0: 6d70 3e5f 0000 0073 0200 0000 2000 7a22  mp>_...s.... .z"
-00000be0: 6765 745f 6770 755f 6d65 6d6f 7279 2e3c  get_gpu_memory.<
-00000bf0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00000c00: 703e 2905 da02 7370 da0c 6368 6563 6b5f  p>)...sp..check_
-00000c10: 6f75 7470 7574 7229 0000 00da 0664 6563  outputr).....dec
-00000c20: 6f64 65da 0965 6e75 6d65 7261 7465 2903  ode..enumerate).
-00000c30: da07 636f 6d6d 616e 645a 106d 656d 6f72  ..commandZ.memor
-00000c40: 795f 6672 6565 5f69 6e66 6f5a 126d 656d  y_free_infoZ.mem
-00000c50: 6f72 795f 6672 6565 5f76 616c 7565 7372  ory_free_valuesr
-00000c60: 3000 0000 7230 0000 0072 3100 0000 da0e  0...r0...r1.....
-00000c70: 6765 745f 6770 755f 6d65 6d6f 7279 5c00  get_gpu_memory\.
-00000c80: 0000 7308 0000 0004 012a 0112 0104 0172  ..s......*.....r
-00000c90: 4400 0000 6300 0000 0000 0000 0000 0000  D...c...........
-00000ca0: 0000 0000 0003 0000 0000 0000 0073 2600  .............s&.
-00000cb0: 0000 6500 5a01 6400 5a02 8700 6601 6401  ..e.Z.d.Z...f.d.
-00000cc0: 6402 8408 5a03 6406 6404 6405 8401 5a04  d...Z.d.d.d...Z.
-00000cd0: 8700 0400 5a05 5300 2907 da0f 4375 7374  ....Z.S.)...Cust
-00000ce0: 6f6d 4245 5254 4d6f 6465 6c63 0300 0000  omBERTModelc....
-00000cf0: 0000 0000 0000 0000 0600 0000 0700 0000  ................
-00000d00: 0300 0000 7316 0100 007c 027c 005f 0074  ....s....|.|._.t
-00000d10: 0174 027c 0083 02a0 03a1 0001 007c 0264  .t.|.........|.d
-00000d20: 0176 0072 2f74 046a 057c 0264 0264 038d  .v.r/t.j.|.d.d..
-00000d30: 027d 0364 047c 036a 0664 053c 0074 077c  .}.d.|.j.d.<.t.|
-00000d40: 035f 0874 096a 057c 027c 0374 0a6a 0b64  ._.t.j.|.|.t.j.d
-00000d50: 0264 0264 068d 057d 0464 077d 057c 046a  .d.d...}.d.}.|.j
-00000d60: 0c7c 005f 0d6e 487c 0264 0876 0072 4074  .|._.nH|.d.v.r@t
-00000d70: 0e6a 0564 0964 0264 038d 027d 0464 0a7d  .j.d.d.d...}.d.}
-00000d80: 057c 047c 005f 0d6e 377c 0264 0b76 0072  .|.|._.n7|.d.v.r
-00000d90: 4f74 0fa0 057c 02a1 017d 0464 0c7d 057c  Ot...|...}.d.}.|
-00000da0: 047c 005f 0d6e 287c 0264 0d76 0072 5e74  .|._.n(|.d.v.r^t
-00000db0: 10a0 057c 02a1 017d 0464 0c7d 057c 047c  ...|...}.d.}.|.|
-00000dc0: 005f 0d6e 197c 0264 0e76 0072 6d74 10a0  ._.n.|.d.v.rmt..
-00000dd0: 057c 02a1 017d 0464 0f7d 057c 047c 005f  .|...}.d.}.|.|._
-00000de0: 0d6e 0a74 10a0 057c 02a1 017d 0464 107d  .n.t...|...}.d.}
-00000df0: 057c 047c 005f 0d74 11a0 1274 11a0 137c  .|.|._.t...t...|
-00000e00: 0564 11a1 0274 11a0 1364 117c 01a1 02a1  .d...t...d.|....
-00000e10: 027c 005f 147c 057c 005f 1564 0053 0029  .|._.|.|._.d.S.)
-00000e20: 124e 2902 7a18 6d6f 7361 6963 6d6c 2f6d  .N).z.mosaicml/m
-00000e30: 7074 2d37 622d 696e 7374 7275 6374 7a0f  pt-7b-instructz.
-00000e40: 6d6f 7361 6963 6d6c 2f6d 7074 2d37 6254  mosaicml/mpt-7bT
-00000e50: a901 da11 7472 7573 745f 7265 6d6f 7465  ....trust_remote
-00000e60: 5f63 6f64 65da 0674 7269 746f 6e5a 0961  _code..tritonZ.a
-00000e70: 7474 6e5f 696d 706c 2904 da06 636f 6e66  ttn_impl)...conf
-00000e80: 6967 da0b 746f 7263 685f 6474 7970 6572  ig..torch_dtyper
-00000e90: 4700 0000 da0e 7573 655f 6175 7468 5f74  G.....use_auth_t
-00000ea0: 6f6b 656e 6900 1000 00a9 01fa 1e6d 6f73  okeni........mos
-00000eb0: 6169 636d 6c2f 6d70 742d 3162 2d72 6564  aicml/mpt-1b-red
-00000ec0: 7061 6a61 6d61 2d32 3030 6272 4d00 0000  pajama-200brM...
-00000ed0: e900 0800 0029 02fa 1867 6f6f 676c 652f  .....)...google/
-00000ee0: 7435 2d6c 6172 6765 2d6c 6d2d 6164 6170  t5-large-lm-adap
-00000ef0: 74fa 1567 6f6f 676c 652f 7435 2d78 6c2d  t..google/t5-xl-
-00000f00: 6c6d 2d61 6461 7074 6900 0400 0029 027a  lm-adapti....).z
-00000f10: 0d72 6f62 6572 7461 2d6c 6172 6765 7a1a  .roberta-largez.
-00000f20: 6d69 6372 6f73 6f66 742f 6465 6265 7274  microsoft/debert
-00000f30: 612d 7633 2d6c 6172 6765 2902 7a1b 6d69  a-v3-large).z.mi
-00000f40: 6372 6f73 6f66 742f 6465 6265 7274 612d  crosoft/deberta-
-00000f50: 7632 2d78 6c61 7267 657a 1c6d 6963 726f  v2-xlargez.micro
-00000f60: 736f 6674 2f64 6562 6572 7461 2d76 322d  soft/deberta-v2-
-00000f70: 7878 6c61 7267 6569 0006 0000 6900 0300  xxlargei....i...
-00000f80: 00e9 0001 0000 2916 da0c 6d6f 6465 6c5f  ......)...model_
-00000f90: 6368 6f69 6365 da05 7375 7065 7272 4500  choice..superrE.
-00000fa0: 0000 da08 5f5f 696e 6974 5f5f 7210 0000  ....__init__r...
-00000fb0: 00da 0f66 726f 6d5f 7072 6574 7261 696e  ...from_pretrain
-00000fc0: 6564 5a0b 6174 746e 5f63 6f6e 6669 67da  edZ.attn_config.
-00000fd0: 106d 6178 5f74 6f6b 656e 5f6c 656e 6774  .max_token_lengt
-00000fe0: 68da 0b6d 6178 5f73 6571 5f6c 656e 720f  h..max_seq_lenr.
-00000ff0: 0000 00da 0574 6f72 6368 da08 6266 6c6f  .....torch..bflo
-00001000: 6174 3136 da0b 7472 616e 7366 6f72 6d65  at16..transforme
-00001010: 72da 0c65 6e63 6f64 6572 4d6f 6465 6cda  r..encoderModel.
-00001020: 1c4d 7074 466f 7253 6571 7565 6e63 6543  .MptForSequenceC
-00001030: 6c61 7373 6966 6963 6174 696f 6e72 1100  lassificationr..
-00001040: 0000 7207 0000 00da 026e 6eda 0a53 6571  ..r......nn..Seq
-00001050: 7565 6e74 6961 6cda 064c 696e 6561 72da  uential..Linear.
-00001060: 0a63 6c61 7373 6966 6965 72da 0e65 6d62  .classifier..emb
-00001070: 6564 6469 6e67 5f73 697a 6529 06da 0473  edding_size)...s
-00001080: 656c 66da 106e 756d 6265 725f 6f66 5f6c  elf..number_of_l
-00001090: 6162 656c 7372 5200 0000 7249 0000 005a  abelsrR...rI...Z
-000010a0: 0e6d 6f64 656c 5f65 6e63 6f64 696e 6772  .model_encodingr
-000010b0: 6100 0000 a901 da09 5f5f 636c 6173 735f  a.......__class_
-000010c0: 5f72 3000 0000 7231 0000 0072 5400 0000  _r0...r1...rT...
-000010d0: 6500 0000 7348 0000 0006 010e 0108 010e  e...sH..........
-000010e0: 020a 0106 0104 0202 0102 0104 0202 0102  ................
-000010f0: 0106 fa04 080a 0108 020e 0404 0108 0108  ................
-00001100: 020a 0204 0108 0108 020a 0204 0108 0108  ................
-00001110: 020a 0204 0108 010a 0404 0106 011e 040a  ................
-00001120: 017a 1843 7573 746f 6d42 4552 544d 6f64  .z.CustomBERTMod
-00001130: 656c 2e5f 5f69 6e69 745f 5f4e 6305 0000  el.__init__Nc...
-00001140: 0000 0000 0000 0000 000a 0000 0005 0000  ................
-00001150: 0043 0000 0073 6800 0000 7c00 6a00 7d05  .C...sh...|.j.}.
-00001160: 7c05 6401 7600 7212 7c00 6a01 7c01 7c02  |.d.v.r.|.j.|.|.
-00001170: 6402 8d02 7d06 7c06 6403 1900 5300 7c00  d...}.|.d...S.|.
-00001180: 6a01 7c01 7c02 6404 8d02 7d06 7c06 6405  j.|.|.d...}.|.d.
-00001190: 1900 7d07 7c07 6400 6400 8502 6406 6400  ..}.|.d.d...d.d.
-000011a0: 6400 8502 6603 1900 a002 6407 7c00 6a03  d...f.....d.|.j.
-000011b0: a102 7d08 7c00 a004 7c08 a101 7d09 7c09  ..}.|...|...}.|.
-000011c0: 5300 2908 4e29 04fa 0874 352d 736d 616c  S.).N)...t5-smal
-000011d0: 6c72 5000 0000 724f 0000 0072 4d00 0000  lrP...rO...rM...
-000011e0: 2902 da09 696e 7075 745f 6964 73da 0e61  )...input_ids..a
-000011f0: 7474 656e 7469 6f6e 5f6d 6173 6bda 066c  ttention_mask..l
-00001200: 6f67 6974 7329 0172 6800 0000 5a11 6c61  ogits).rh...Z.la
-00001210: 7374 5f68 6964 6465 6e5f 7374 6174 6572  st_hidden_stater
-00001220: 0100 0000 7238 0000 0029 0572 5200 0000  ....r8...).rR...
-00001230: 725b 0000 00da 0476 6965 7772 6100 0000  r[.....viewra...
-00001240: 7260 0000 0029 0a72 6200 0000 da03 6964  r`...).rb.....id
-00001250: 73da 046d 6173 6bda 066c 6162 656c 73da  s..mask..labels.
-00001260: 1164 6563 6f64 6572 5f69 6e70 7574 5f69  .decoder_input_i
-00001270: 6473 7252 0000 005a 0c74 6f74 616c 5f6f  dsrR...Z.total_o
-00001280: 7574 7075 745a 0f73 6571 7565 6e63 655f  utputZ.sequence_
-00001290: 6f75 7470 7574 5a1b 6c61 7374 5f68 6964  outputZ.last_hid
-000012a0: 6465 6e5f 7374 6174 655f 666f 726d 6174  den_state_format
-000012b0: 7465 645a 0e6c 696e 6561 7232 5f6f 7574  tedZ.linear2_out
-000012c0: 7075 7472 3000 0000 7230 0000 0072 3100  putr0...r0...r1.
-000012d0: 0000 da07 666f 7277 6172 64a0 0000 0073  ....forward....s
-000012e0: 1200 0000 0601 0801 0e01 0801 0e02 0801  ................
-000012f0: 2002 0a01 0402 7a17 4375 7374 6f6d 4245   .....z.CustomBE
-00001300: 5254 4d6f 6465 6c2e 666f 7277 6172 6429  RTModel.forward)
-00001310: 024e 4e29 06da 085f 5f6e 616d 655f 5fda  .NN)...__name__.
-00001320: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00001330: 7561 6c6e 616d 655f 5f72 5400 0000 726f  ualname__rT...ro
-00001340: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00001350: 5f5f 7230 0000 0072 3000 0000 7264 0000  __r0...r0...rd..
-00001360: 0072 3100 0000 7245 0000 0064 0000 0073  .r1...rE...d...s
-00001370: 0600 0000 0800 0c01 123b 7245 0000 0063  .........;rE...c
-00001380: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00001390: 0500 0000 4300 0000 7312 0000 007c 007c  ....C...s....|.|
-000013a0: 0164 0119 0064 0264 0364 048d 0353 0029  .d...d.d.d...S.)
-000013b0: 054e da04 7465 7874 da0a 6d61 785f 6c65  .N..text..max_le
-000013c0: 6e67 7468 5429 02da 0770 6164 6469 6e67  ngthT)...padding
-000013d0: da0a 7472 756e 6361 7469 6f6e 7230 0000  ..truncationr0..
-000013e0: 0029 02da 0974 6f6b 656e 697a 6572 da08  .)...tokenizer..
-000013f0: 6578 616d 706c 6573 7230 0000 0072 3000  examplesr0...r0.
-00001400: 0000 7231 0000 00da 1174 6f6b 656e 697a  ..r1.....tokeniz
-00001410: 655f 6675 6e63 7469 6f6e b000 0000 7302  e_function....s.
-00001420: 0000 0012 0172 7a00 0000 6302 0000 0000  .....rz...c.....
-00001430: 0000 0000 0000 0005 0000 000a 0000 0043  ...............C
-00001440: 0000 0073 b200 0000 6401 7d02 7400 6a01  ...s....d.}.t.j.
-00001450: a002 7c02 a101 730d 7400 a003 7c02 a101  ..|...s.t...|...
-00001460: 0100 6401 7c01 a004 6402 6403 a102 1700  ..d.|...d.d.....
-00001470: 7d03 7400 6a01 a002 7c03 a101 7326 7405  }.t.j...|...s&t.
-00001480: 6404 7c03 1700 8301 0100 7400 a003 7c03  d.|.......t...|.
-00001490: a101 0100 7406 4400 5d2e 7d04 7a13 7400  ....t.D.].}.z.t.
-000014a0: a003 7c03 6402 1700 7c04 a004 6405 6406  ..|.d...|...d.d.
-000014b0: a102 a004 6402 6403 a102 1700 a101 0100  ....d.d.........
-000014c0: 5700 7128 0100 0100 0100 7405 6407 8301  W.q(......t.d...
-000014d0: 0100 7405 7c03 6402 1700 7c04 a004 6405  ..t.|.d...|...d.
-000014e0: 6406 a102 a004 6402 6403 a102 1700 8301  d.....d.d.......
-000014f0: 0100 5900 7128 6400 5300 2908 4efa 0c63  ..Y.q(d.S.).N..c
-00001500: 6865 636b 706f 696e 7473 2ffa 012f 721f  heckpoints/../r.
-00001510: 0000 007a 1143 7265 6174 696e 6720 666f  ...z.Creating fo
-00001520: 6c64 6572 3a20 7a03 2e2e 2fda 007a 0e41  lder: z.../..z.A
-00001530: 6c72 6561 6479 2065 7869 7374 7329 07da  lready exists)..
-00001540: 026f 73da 0470 6174 68da 0569 7364 6972  .os..path..isdir
-00001550: da05 6d6b 6469 7272 2600 0000 722c 0000  ..mkdirr&...r,..
-00001560: 00da 1763 6c61 7373 6966 6963 6174 696f  ...classificatio
-00001570: 6e5f 6461 7461 7365 7473 2905 da16 636c  n_datasets)...cl
-00001580: 6173 7369 6669 6361 7469 6f6e 5f64 6174  assification_dat
-00001590: 6173 6574 7252 0000 005a 1763 6865 636b  asetrR...Z.check
-000015a0: 706f 696e 7473 5f66 6f6c 6465 725f 7061  points_folder_pa
-000015b0: 7468 5a13 6461 7461 7365 745f 666f 6c64  thZ.dataset_fold
-000015c0: 6572 5f70 6174 68da 0764 6174 6173 6574  er_path..dataset
-000015d0: 7230 0000 0072 3000 0000 7231 0000 00da  r0...r0...r1....
-000015e0: 0b63 6865 636b 706f 696e 7473 b500 0000  .checkpoints....
-000015f0: 731c 0000 0004 010c 010a 0110 020c 010c  s...............
-00001600: 010a 0108 0202 0126 0106 0108 0124 0104  .......&.....$..
-00001610: fb72 8500 0000 6301 0000 0000 0000 0000  .r....c.........
-00001620: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-00001630: 1a00 0000 6401 7d01 7400 6a01 7c00 7c01  ....d.}.t.j.|.|.
-00001640: 6402 8d02 7d02 7c02 7c01 6602 5300 2903  d...}.|.|.f.S.).
-00001650: 4e72 4e00 0000 2901 da10 6d6f 6465 6c5f  NrN...)...model_
-00001660: 6d61 785f 6c65 6e67 7468 2902 7206 0000  max_length).r...
-00001670: 0072 5500 0000 2903 7252 0000 0072 5600  .rU...).rR...rV.
-00001680: 0000 7278 0000 0072 3000 0000 7230 0000  ..rx...r0...r0..
-00001690: 0072 3100 0000 da0a 6c6f 6164 5f6d 6f64  .r1.....load_mod
-000016a0: 656c c800 0000 7306 0000 0004 010e 0108  el....s.........
-000016b0: 0272 8700 0000 630e 0000 0000 0000 0000  .r....c.........
-000016c0: 0000 0012 0000 0006 0000 0043 0000 0073  ...........C...s
-000016d0: 2201 0000 7400 6401 8301 0100 7400 6402  "...t.d.....t.d.
-000016e0: 7401 7c02 8301 1700 8301 0100 7400 6401  t.|.........t.d.
-000016f0: 8301 0100 6403 6400 6c02 7d0e 7c0e 6a02  ....d.d.l.}.|.j.
-00001700: a003 a100 a004 6404 a101 7d0f 6405 7c03  ......d...}.d.|.
-00001710: a005 6406 6407 a102 1700 6406 1700 7c06  ..d.d.....d...|.
-00001720: 1700 6408 1700 7401 7c07 a006 6406 a101  ..d...t.|...d...
-00001730: 6409 1900 a005 640a 640b a102 8301 1700  d.....d.d.......
-00001740: 6408 1700 7c0f 1700 640c 1700 7d10 7407  d...|...d...}.t.
-00001750: a007 a100 7d11 7400 640d 7c00 1700 8301  ....}.t.d.|.....
-00001760: 0100 7400 640e 7c03 1700 8301 0100 7400  ..t.d.|.......t.
-00001770: 640f 7c07 1700 8301 0100 7400 6410 7401  d.|.......t.d.t.
-00001780: 7c04 8301 1700 8301 0100 7400 6411 7401  |.........t.d.t.
-00001790: 7c02 8301 1700 8301 0100 7400 6412 7c10  |.........t.d.|.
-000017a0: 1700 8301 0100 7400 6413 7401 7c08 8301  ......t.d.t.|...
-000017b0: 1700 8301 0100 7400 6414 7401 7c05 8301  ......t.d.t.|...
-000017c0: 1700 8301 0100 7400 6415 7401 7c09 8301  ......t.d.t.|...
-000017d0: 1700 8301 0100 7400 6416 7401 7c0a 8301  ......t.d.t.|...
-000017e0: 1700 8301 0100 7400 6401 8301 0100 7c10  ......t.d.....|.
-000017f0: 7c08 6602 5300 2917 4e7a 4a2d 2d2d 2d2d  |.f.S.).NzJ-----
-00001800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001840: 2d2d 2d2d 2d7a 1c53 7461 7274 696e 6720  -----z.Starting 
-00001850: 6e65 7720 6c65 6172 6e69 6e67 2072 6174  new learning rat
-00001860: 653a 2072 0100 0000 7a11 2559 2d25 6d2d  e: r....z.%Y-%m-
-00001870: 2564 5f25 483a 254d 3a25 5372 7b00 0000  %d_%H:%M:%Sr{...
-00001880: 727c 0000 0072 1f00 0000 da01 5f72 3800  r|...r......_r8.
-00001890: 0000 7a04 2e74 7376 727d 0000 007a 032e  ..z..tsvr}...z..
-000018a0: 7074 7a09 4461 7461 7365 743a 207a 074d  ptz.Dataset: z.M
-000018b0: 6f64 656c 3a20 7a14 5465 7374 2053 6574  odel: z.Test Set
-000018c0: 2053 656c 6563 7469 6f6e 3a20 7a10 4e75   Selection: z.Nu
-000018d0: 6d62 6572 206f 6620 5275 6e73 3a20 7a0f  mber of Runs: z.
-000018e0: 4c65 6172 6e69 6e67 2052 6174 653a 20fa  Learning Rate: .
-000018f0: 1143 6865 636b 706f 696e 7420 5061 7468  .Checkpoint Path
-00001900: 3a20 7a0a 5061 7469 656e 6365 3a20 7a17  : z.Patience: z.
-00001910: 5661 6c69 6461 7469 6f6e 2053 6574 2043  Validation Set C
-00001920: 686f 6963 653a 207a 124e 756d 6265 7220  hoice: z.Number 
-00001930: 6f66 2045 706f 6368 733a 207a 184e 756d  of Epochs: z.Num
-00001940: 6265 7220 6f66 2077 6172 6d75 7020 7374  ber of warmup st
-00001950: 6570 733a 2029 0872 2c00 0000 722d 0000  eps: ).r,...r-..
-00001960: 00da 0864 6174 6574 696d 65da 036e 6f77  ...datetime..now
-00001970: da08 7374 7266 7469 6d65 7226 0000 0072  ..strftimer&...r
-00001980: 2900 0000 da04 7469 6d65 2912 7284 0000  ).....time).r...
-00001990: 00da 156c 6561 726e 696e 675f 7261 7465  ...learning_rate
-000019a0: 5f63 686f 6963 6573 da14 6368 6f73 656e  _choices..chosen
-000019b0: 5f6c 6561 726e 696e 675f 7261 7465 7252  _learning_raterR
-000019c0: 0000 00da 0e6e 756d 6265 725f 6f66 5f72  .....number_of_r
-000019d0: 756e 73da 1676 616c 6964 6174 696f 6e5f  uns..validation_
-000019e0: 7365 745f 7363 6f72 696e 67da 0c6c 6162  set_scoring..lab
-000019f0: 656c 5f63 6f6c 756d 6eda 0e76 616c 6964  el_column..valid
-00001a00: 6174 696f 6e5f 7365 74da 0e70 6174 6965  ation_set..patie
-00001a10: 6e63 655f 7661 6c75 65da 0a6e 756d 5f65  nce_value..num_e
-00001a20: 706f 6368 73da 106e 756d 5f77 6172 6d75  pochs..num_warmu
-00001a30: 705f 7374 6570 73da 2067 7261 6469 656e  p_steps. gradien
-00001a40: 745f 6163 6375 6d75 6c61 7469 6f6e 5f6d  t_accumulation_m
-00001a50: 756c 7469 706c 6965 72da 1361 7373 6967  ultiplier..assig
-00001a60: 6e65 645f 6261 7463 685f 7369 7a65 7278  ned_batch_sizerx
-00001a70: 0000 0072 8a00 0000 5a10 6375 7272 656e  ...r....Z.curren
-00001a80: 745f 6461 7465 7469 6d65 da0f 6368 6563  t_datetime..chec
-00001a90: 6b70 6f69 6e74 5f70 6174 685a 0f65 7865  kpoint_pathZ.exe
-00001aa0: 6375 7469 6f6e 5f73 7461 7274 7230 0000  cution_startr0..
-00001ab0: 0072 3000 0000 7231 0000 00da 1670 7265  .r0...r1.....pre
-00001ac0: 7061 7265 5f61 6e64 5f63 6c65 616e 5f64  pare_and_clean_d
-00001ad0: 6174 61d0 0000 0073 2600 0000 0806 1001  ata....s&.......
-00001ae0: 0801 0802 1002 4202 0808 0c02 0c01 0c01  ......B.........
-00001af0: 1001 1001 0c01 1001 1001 1001 1001 0801  ................
-00001b00: 0802 729a 0000 0063 0400 0000 0000 0000  ..r....c........
-00001b10: 0000 0000 0400 0000 0500 0000 0300 0000  ................
-00001b20: 7324 0100 0074 006a 017c 0064 0164 028d  s$...t.j.|.d.d..
-00001b30: 0289 0064 037c 0076 0072 1d88 0064 0419  ...d.|.v.r...d..
-00001b40: 0088 0064 053c 0088 0064 0619 0088 0064  ...d.<...d.....d
-00001b50: 073c 0088 0064 0819 0088 0064 093c 0088  .<...d.....d.<..
-00001b60: 0088 007c 0119 0064 0a6b 0319 0089 0088  ...|...d.k......
-00001b70: 0088 0064 0519 00a0 02a1 0019 0089 0088  ...d............
-00001b80: 0088 0064 0919 00a0 02a1 0019 0089 0088  ...d............
-00001b90: 0088 0064 0719 00a0 02a1 0019 0089 0088  ...d............
-00001ba0: 0088 007c 0119 00a0 02a1 0019 0089 0088  ...|............
-00001bb0: 006a 0374 0488 0083 0164 0b64 0c8d 0289  .j.t.....d.d....
-00001bc0: 0064 0d7c 0176 0072 6287 0066 0164 0e64  .d.|.v.rb..f.d.d
-00001bd0: 0f84 0874 0574 0488 0083 0183 0144 0083  ...t.t.......D..
-00001be0: 0188 0064 103c 006e 0f87 0066 0164 1164  ...d.<.n...f.d.d
-00001bf0: 0f84 0874 0574 0488 0083 0183 0144 0083  ...t.t.......D..
-00001c00: 0188 0064 103c 0087 0166 0164 1264 0f84  ...d.<...f.d.d..
-00001c10: 0874 0688 0064 1019 0064 1364 148d 0244  .t...d...d.d...D
-00001c20: 0083 0188 0064 153c 0088 00a0 0764 1067  .....d.<.....d.g
-00001c30: 01a1 0189 0088 0088 0064 1519 0064 166b  .........d...d.k
-00001c40: 0119 0089 0088 0053 0029 174e 721d 0000  .......S.).Nr...
-00001c50: 00a9 01da 0373 6570 da0e 6e71 5f72 6566  .....sep..nq_ref
-00001c60: 6f72 6d61 7474 6564 da05 5175 6572 79da  ormatted..Query.
-00001c70: 0f73 796e 7468 6574 6963 5f71 7565 7279  .synthetic_query
-00001c80: da06 416e 7377 6572 da10 6765 6e65 7261  ..Answer..genera
-00001c90: 7465 645f 616e 7377 6572 da08 446f 6375  ted_answer..Docu
-00001ca0: 6d65 6e74 7218 0000 00da 034e 614e 7236  mentr......NaNr6
-00001cb0: 0000 0029 02da 016e da0c 7261 6e64 6f6d  ...)...n..random
-00001cc0: 5f73 7461 7465 da07 436f 6e74 6578 7463  _state..Contextc
-00001cd0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001ce0: 0600 0000 1300 0000 f32a 0000 0067 007c  .........*...g.|
-00001cf0: 005d 117d 0174 0088 006a 017c 0119 0064  .].}.t...j.|...d
-00001d00: 0019 0088 006a 017c 0119 0064 0119 0083  .....j.|...d....
-00001d10: 0291 0271 0253 0029 0272 9f00 0000 7218  ...q.S.).r....r.
-00001d20: 0000 00a9 0272 3200 0000 da04 696c 6f63  .....r2.....iloc
-00001d30: a902 723b 0000 0072 3c00 0000 a901 da0d  ..r;...r<.......
-00001d40: 7379 6e74 685f 7175 6572 6965 7372 3000  synth_queriesr0.
-00001d50: 0000 7231 0000 0072 3e00 0000 1601 0000  ..r1...r>.......
-00001d60: f302 0000 002a 007a 2b61 6e61 6c79 7a65  .....*.z+analyze
-00001d70: 5f61 6e64 5f72 6570 6f72 745f 6461 7461  _and_report_data
-00001d80: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00001d90: 6f6d 703e da0b 636f 6e63 6174 5f74 6578  omp>..concat_tex
-00001da0: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
-00001db0: 0000 0700 0000 1300 0000 f336 0000 0067  ...........6...g
-00001dc0: 007c 005d 177d 0174 0088 006a 017c 0119  .|.].}.t...j.|..
-00001dd0: 0064 0019 0088 006a 017c 0119 0064 0119  .d.....j.|...d..
-00001de0: 0088 006a 017c 0119 0064 0219 0083 0391  ...j.|...d......
-00001df0: 0271 0253 0029 0372 9f00 0000 7218 0000  .q.S.).r....r...
-00001e00: 0072 a100 0000 72a8 0000 0072 aa00 0000  .r....r....r....
-00001e10: 72ab 0000 0072 3000 0000 7231 0000 0072  r....r0...r1...r
-00001e20: 3e00 0000 1801 0000 f302 0000 0036 0063  >............6.c
-00001e30: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001e40: 0700 0000 1300 0000 7322 0000 0067 007c  ........s"...g.|
-00001e50: 005d 0d7d 0174 0088 006a 017c 0164 0064  .].}.t...j.|.d.d
-00001e60: 018d 0264 0219 0083 0191 0271 0253 0029  ...d.......q.S.)
-00001e70: 03da 0270 7429 01da 0e72 6574 7572 6e5f  ...pt)...return_
-00001e80: 7465 6e73 6f72 7372 0100 0000 2902 722a  tensorsr....).r*
-00001e90: 0000 00da 0665 6e63 6f64 6529 0272 3b00  .....encode).r;.
-00001ea0: 0000 7274 0000 00a9 0172 7800 0000 7230  ..rt.....rx...r0
-00001eb0: 0000 0072 3100 0000 723e 0000 0019 0100  ...r1...r>......
-00001ec0: 0073 0200 0000 2200 5a0a 546f 6b65 6e69  .s....".Z.Tokeni
-00001ed0: 7a69 6e67 2901 da04 6465 7363 5a0c 746f  zing)...descZ.to
-00001ee0: 6b65 6e5f 6c65 6e67 7468 724e 0000 0029  ken_lengthrN...)
-00001ef0: 08da 0270 64da 0872 6561 645f 6373 76da  ...pd..read_csv.
-00001f00: 056e 6f74 6e61 da06 7361 6d70 6c65 722a  .notna..sampler*
-00001f10: 0000 00da 0572 616e 6765 7212 0000 00da  .....ranger.....
-00001f20: 0f64 726f 705f 6475 706c 6963 6174 6573  .drop_duplicates
-00001f30: 2904 7284 0000 0072 9200 0000 7278 0000  ).r....r....rx..
-00001f40: 0072 5600 0000 7230 0000 0029 0272 ac00  .rV...r0...).r..
-00001f50: 0000 7278 0000 0072 3100 0000 da17 616e  ..rx...r1.....an
-00001f60: 616c 797a 655f 616e 645f 7265 706f 7274  alyze_and_report
-00001f70: 5f64 6174 61f8 0000 0073 2400 0000 0e02  _data....s$.....
-00001f80: 0802 0c01 0c01 0c01 1007 1001 1001 1001  ................
-00001f90: 1001 1201 080a 2001 1e02 2201 0c01 1007  ...... ...".....
-00001fa0: 0402 72bc 0000 0063 0300 0000 0000 0000  ..r....c........
-00001fb0: 0000 0000 0500 0000 0600 0000 0300 0000  ................
-00001fc0: 7360 0100 007c 007d 0374 006a 017c 0164  s`...|.}.t.j.|.d
-00001fd0: 0164 028d 0289 0088 0064 0319 0088 0064  .d.......d.....d
-00001fe0: 043c 0088 0064 0519 006a 02a0 03a1 0088  .<...d...j......
-00001ff0: 0064 053c 0088 0088 0064 0519 006a 02a0  .d.<.....d...j..
-00002000: 04a1 0064 066b 0419 0089 0088 0088 007c  ...d.k.........|
-00002010: 0219 00a0 05a1 0019 0089 007c 0364 0719  ...........|.d..
-00002020: 00a0 0674 02a1 016a 02a0 03a1 007c 0364  ...t...j.....|.d
-00002030: 073c 007c 037c 0364 0719 006a 02a0 04a1  .<.|.|.d...j....
-00002040: 0064 066b 0419 007d 037c 037c 037c 0219  .d.k...}.|.|.|..
-00002050: 00a0 05a1 0019 007d 0364 087c 0276 0072  .......}.d.|.v.r
-00002060: 5e87 0066 0164 0964 0a84 0874 0774 0488  ^..f.d.d...t.t..
-00002070: 0083 0183 0144 0083 0188 0064 0b3c 006e  .....D.....d.<.n
-00002080: 0f87 0066 0164 0c64 0a84 0874 0774 0488  ...f.d.d...t.t..
-00002090: 0083 0183 0144 0083 0188 0064 0b3c 007c  .....D.....d.<.|
-000020a0: 03a0 0864 0b67 01a1 017d 0388 00a0 0864  ...d.g...}.....d
-000020b0: 0b67 01a1 0189 0064 0d7c 0276 0072 ac74  .g.....d.|.v.r.t
-000020c0: 0964 0e83 0101 007c 037c 0364 0f19 00a0  .d.....|.|.d....
-000020d0: 05a1 0019 007d 037c 037c 0364 1019 00a0  .....}.|.|.d....
-000020e0: 05a1 0019 007d 0367 0064 11a2 017d 047c  .....}.g.d...}.|
-000020f0: 0364 1219 00a0 0674 02a1 017c 0364 123c  .d.....t...|.d.<
-00002100: 007c 037c 0364 1219 006a 02a0 0a64 13a0  .|.|.d...j...d..
-00002110: 0b7c 04a1 01a1 010f 0019 007d 037c 0388  .|.........}.|..
-00002120: 0066 0253 0029 144e 721d 0000 0072 9b00  .f.S.).Nr....r..
-00002130: 0000 729e 0000 00da 0851 7565 7374 696f  ..r......Questio
-00002140: 6e72 a200 0000 7222 0000 0072 1800 0000  nr....r"...r....
-00002150: 72a6 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00002160: 0000 0200 0000 0600 0000 1300 0000 72a7  ..............r.
-00002170: 0000 0029 0272 bd00 0000 72a2 0000 0072  ...).r....r....r
-00002180: a800 0000 72aa 0000 00a9 01da 0874 6573  ....r........tes
-00002190: 745f 7365 7472 3000 0000 7231 0000 0072  t_setr0...r1...r
-000021a0: 3e00 0000 3601 0000 72ad 0000 007a 2274  >...6...r....z"t
-000021b0: 7261 6e73 666f 726d 5f64 6174 612e 3c6c  ransform_data.<l
-000021c0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-000021d0: 3e72 ae00 0000 6301 0000 0000 0000 0000  >r....c.........
-000021e0: 0000 0002 0000 0007 0000 0013 0000 0072  ...............r
-000021f0: af00 0000 2903 72bd 0000 0072 a200 0000  ....).r....r....
-00002200: 72a0 0000 0072 a800 0000 72aa 0000 0072  r....r....r....r
-00002210: be00 0000 7230 0000 0072 3100 0000 723e  ....r0...r1...r>
-00002220: 0000 0038 0100 0072 b000 0000 5a05 4661  ...8...r....Z.Fa
-00002230: 6974 687a 3552 6566 696e 696e 6720 6461  ithz5Refining da
-00002240: 7461 2066 6f72 2041 6e73 7765 725f 4661  ta for Answer_Fa
-00002250: 6974 6866 756c 6e65 7373 2063 6c61 7373  ithfulness class
-00002260: 6966 6963 6174 696f 6e21 da17 436f 6e74  ification!..Cont
-00002270: 6578 745f 5265 6c65 7661 6e63 655f 4c61  ext_Relevance_La
-00002280: 6265 6cda 1941 6e73 7765 725f 4661 6974  bel..Answer_Fait
-00002290: 6866 756c 6e65 7373 5f4c 6162 656c 290a  hfulness_Label).
-000022a0: 722e 0000 005a 0763 6f6e 7472 6164 da05  r....Z.contrad..
-000022b0: 6661 6c73 655a 0b69 6e66 6f72 6d61 7469  falseZ.informati
-000022c0: 6f6e 5a08 756e 616e 7377 6572 72a0 0000  onZ.unanswerr...
-000022d0: 005a 0743 6f6e 7472 6164 da05 4661 6c73  .Z.Contrad..Fals
-000022e0: 655a 0b49 6e66 6f72 6d61 7469 6f6e 5a08  eZ.InformationZ.
-000022f0: 556e 616e 7377 6572 72a1 0000 00da 017c  Unanswerr......|
-00002300: 290c 72b6 0000 0072 b700 0000 722d 0000  ).r....r....r-..
-00002310: 0072 2700 0000 722a 0000 0072 b800 0000  .r'...r*...r....
-00002320: da06 6173 7479 7065 72ba 0000 0072 bb00  ..astyper....r..
-00002330: 0000 722c 0000 00da 0863 6f6e 7461 696e  ..r,.....contain
-00002340: 7372 2800 0000 2905 72ac 0000 0072 9300  sr(...).r....r..
-00002350: 0000 7292 0000 00da 0874 7261 696e 5f64  ..r......train_d
-00002360: 665a 0d65 7272 6f72 5f73 7472 696e 6773  fZ.error_strings
-00002370: 7230 0000 0072 be00 0000 7231 0000 00da  r0...r....r1....
-00002380: 0e74 7261 6e73 666f 726d 5f64 6174 6127  .transform_data'
-00002390: 0100 0073 2c00 0000 0402 0e02 0c01 1201  ...s,...........
-000023a0: 1601 1001 1802 1601 1001 0802 2001 1e02  ............ ...
-000023b0: 0c02 0c01 0802 0801 1001 1001 0801 1201  ................
-000023c0: 1c01 0802 72c8 0000 0063 0400 0000 0000  ....r....c......
-000023d0: 0000 0000 0000 0b00 0000 0700 0000 0300  ................
-000023e0: 0000 7306 0100 0064 0164 0264 039c 0289  ..s....d.d.d....
-000023f0: 0087 0366 0164 0464 0584 0874 0074 0188  ...f.d.d...t.t..
-00002400: 0383 0183 0144 0083 017d 0464 067c 0176  .....D...}.d.|.v
-00002410: 0172 2687 0087 0187 0366 0364 0764 0584  .r&......f.d.d..
-00002420: 0874 0074 0188 0383 0183 0144 0083 017d  .t.t.......D...}
-00002430: 056e 0e87 0187 0366 0264 0864 0584 0874  .n.....f.d.d...t
-00002440: 0074 0188 0383 0183 0144 0083 017d 0587  .t.......D...}..
-00002450: 0266 0164 0964 0584 0874 0074 0188 0283  .f.d.d...t.t....
-00002460: 0183 0144 0083 017d 0687 0187 0266 0264  ...D...}.....f.d
-00002470: 0a64 0584 0874 0074 0188 0283 0183 0144  .d...t.t.......D
-00002480: 0083 017d 0787 0266 0164 0b64 0584 0874  ...}...f.d.d...t
-00002490: 0074 0188 0283 0183 0144 0083 017d 0887  .t.......D...}..
-000024a0: 0187 0266 0264 0c64 0584 0874 0074 0188  ...f.d.d...t.t..
-000024b0: 0283 0183 0144 0083 017d 0974 0264 0d83  .....D...}.t.d..
-000024c0: 0101 0074 0374 0474 057c 057c 0717 007c  ...t.t.t.|.|...|
-000024d0: 0917 0083 0183 0183 017d 0a7c 047c 057c  .........}.|.|.|
-000024e0: 067c 077c 087c 097c 0a66 0753 0029 0e4e  .|.|.|.|.f.S.).N
-000024f0: 7239 0000 0072 0100 0000 2902 da03 5965  r9...r....)...Ye
-00002500: 73da 024e 6f63 0100 0000 0000 0000 0000  s..Noc..........
-00002510: 0000 0200 0000 0400 0000 1300 0000 f31a  ................
-00002520: 0000 0067 007c 005d 097d 0188 006a 007c  ...g.|.].}...j.|
-00002530: 0119 0064 0019 0091 0271 0253 00a9 0172  ...d.....q.S...r
-00002540: ae00 0000 a901 72a9 0000 0072 aa00 0000  ......r....r....
-00002550: 2901 72c7 0000 0072 3000 0000 7231 0000  ).r....r0...r1..
-00002560: 0072 3e00 0000 4b01 0000 f302 0000 001a  .r>...K.........
-00002570: 007a 2173 706c 6974 5f64 6174 6173 6574  .z!split_dataset
-00002580: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00002590: 6f6d 703e 729d 0000 0063 0100 0000 0000  omp>r....c......
-000025a0: 0000 0000 0000 0200 0000 0500 0000 1300  ................
-000025b0: 0000 731e 0000 0067 007c 005d 0b7d 0188  ..s....g.|.].}..
-000025c0: 0088 026a 007c 0119 0088 0119 0019 0091  ...j.|..........
-000025d0: 0271 0253 0072 3000 0000 72cd 0000 0072  .q.S.r0...r....r
-000025e0: aa00 0000 2903 da0f 636f 6e76 6572 7369  ....)...conversi
-000025f0: 6f6e 5f64 6963 7472 9200 0000 72c7 0000  on_dictr....r...
-00002600: 0072 3000 0000 7231 0000 0072 3e00 0000  .r0...r1...r>...
-00002610: 4d01 0000 f302 0000 001e 0063 0100 0000  M..........c....
-00002620: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00002630: 1300 0000 f31e 0000 0067 007c 005d 0b7d  .........g.|.].}
-00002640: 0174 0088 016a 017c 0119 0088 0019 0083  .t...j.|........
-00002650: 0191 0271 0253 0072 3000 0000 a902 723a  ...q.S.r0.....r:
-00002660: 0000 0072 a900 0000 72aa 0000 0029 0272  ...r....r....).r
-00002670: 9200 0000 72c7 0000 0072 3000 0000 7231  ....r....r0...r1
-00002680: 0000 0072 3e00 0000 4f01 0000 72d0 0000  ...r>...O...r...
-00002690: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-000026a0: 0000 0400 0000 1300 0000 72cb 0000 0072  ..........r....r
-000026b0: cc00 0000 72cd 0000 0072 aa00 0000 72be  ....r....r....r.
-000026c0: 0000 0072 3000 0000 7231 0000 0072 3e00  ...r0...r1...r>.
-000026d0: 0000 5301 0000 72ce 0000 0063 0100 0000  ..S...r....c....
-000026e0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-000026f0: 1300 0000 72d1 0000 0072 3000 0000 72d2  ....r....r0...r.
-00002700: 0000 0072 aa00 0000 a902 7292 0000 0072  ...r......r....r
-00002710: bf00 0000 7230 0000 0072 3100 0000 723e  ....r0...r1...r>
-00002720: 0000 0054 0100 0072 d000 0000 6301 0000  ...T...r....c...
-00002730: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00002740: 0013 0000 0072 cb00 0000 72cc 0000 0072  .....r....r....r
-00002750: cd00 0000 72aa 0000 0072 be00 0000 7230  ....r....r....r0
-00002760: 0000 0072 3100 0000 723e 0000 0058 0100  ...r1...r>...X..
-00002770: 0072 ce00 0000 6301 0000 0000 0000 0000  .r....c.........
-00002780: 0000 0002 0000 0005 0000 0013 0000 0072  ...............r
-00002790: d100 0000 7230 0000 0072 d200 0000 72aa  ....r0...r....r.
-000027a0: 0000 0072 d300 0000 7230 0000 0072 3100  ...r....r0...r1.
-000027b0: 0000 723e 0000 0059 0100 0072 d000 0000  ..r>...Y...r....
-000027c0: 7a33 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  z3--------------
-000027d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000027e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000027f0: 2d2d 2d2d 2d29 0672 ba00 0000 722a 0000  -----).r....r*..
-00002800: 0072 2c00 0000 da06 736f 7274 6564 da04  .r,.....sorted..
-00002810: 6c69 7374 da03 7365 7429 0b72 c700 0000  list..set).r....
-00002820: 7284 0000 0072 bf00 0000 7292 0000 00da  r....r....r.....
-00002830: 0e74 7261 696e 5f73 6574 5f74 6578 74da  .train_set_text.
-00002840: 0f74 7261 696e 5f73 6574 5f6c 6162 656c  .train_set_label
-00002850: da0c 6465 765f 7365 745f 7465 7874 da0d  ..dev_set_text..
-00002860: 6465 765f 7365 745f 6c61 6265 6cda 0d74  dev_set_label..t
-00002870: 6573 745f 7365 745f 7465 7874 da0e 7465  est_set_text..te
-00002880: 7374 5f73 6574 5f6c 6162 656c da0b 6c61  st_set_label..la
-00002890: 6265 6c73 5f6c 6973 7472 3000 0000 2904  bels_listr0...).
-000028a0: 72cf 0000 0072 9200 0000 72bf 0000 0072  r....r....r....r
-000028b0: c700 0000 7231 0000 00da 0d73 706c 6974  ....r1.....split
-000028c0: 5f64 6174 6173 6574 4901 0000 7318 0000  _datasetI...s...
-000028d0: 000a 011a 0108 0120 011c 021a 041c 011a  ....... ........
-000028e0: 041c 0108 0218 0b12 0872 de00 0000 6305  .........r....c.
-000028f0: 0000 0000 0000 0000 0000 000b 0000 0005  ................
-00002900: 0000 0043 0000 0073 fc00 0000 7c00 6401  ...C...s....|.d.
-00002910: 6b02 723e 7400 a001 7c01 7c02 6402 9c02  k.r>t...|.|.d...
-00002920: a101 7d05 7402 6a03 a004 7c05 a101 7d06  ..}.t.j...|...}.
-00002930: 7405 a006 7c06 a101 7d06 7400 a001 7c03  t...|...}.t...|.
-00002940: 7c04 6402 9c02 a101 7d07 7402 6a03 a004  |.d.....}.t.j...
-00002950: 7c07 a101 7d08 7405 a006 7c08 a101 7d08  |...}.t...|...}.
-00002960: 7400 a001 7c03 7c04 6402 9c02 a101 7d09  t...|.|.d.....}.
-00002970: 7402 6a03 a004 7c09 a101 7d0a 7405 a006  t.j...|...}.t...
-00002980: 7c0a a101 7d0a 6e39 7400 a001 7c01 7c02  |...}.n9t...|.|.
-00002990: 6402 9c02 a101 7d05 7402 6a03 a004 7c05  d.....}.t.j...|.
-000029a0: a101 7d06 7405 a006 7c06 a101 7d06 7400  ..}.t...|...}.t.
-000029b0: a001 7c03 7c04 6402 9c02 a101 7d07 7402  ..|.|.d.....}.t.
-000029c0: 6a03 a004 7c07 a101 7d08 7405 a006 7c08  j...|...}.t...|.
-000029d0: a101 7d08 7400 a001 7407 7408 6402 9c02  ..}.t...t.t.d...
-000029e0: a101 7d09 7402 6a03 a004 7c09 a101 7d0a  ..}.t.j...|...}.
-000029f0: 7405 a006 7c0a a101 7d0a 7c05 7c06 7c08  t...|...}.|.|.|.
-00002a00: 7c0a 7c09 6605 5300 2903 4e54 2902 da05  |.|.f.S.).NT)...
-00002a10: 6c61 6265 6c72 7400 0000 2909 72b6 0000  labelrt...).r...
-00002a20: 00da 0944 6174 6146 7261 6d65 da02 7061  ...DataFrame..pa
-00002a30: da05 5461 626c 65da 0b66 726f 6d5f 7061  ..Table..from_pa
-00002a40: 6e64 6173 da08 6461 7461 7365 7473 da07  ndas..datasets..
-00002a50: 4461 7461 7365 7472 dc00 0000 72db 0000  Datasetr....r...
-00002a60: 0029 0b72 9100 0000 72d8 0000 0072 d700  .).r....r....r..
-00002a70: 0000 72da 0000 0072 d900 0000 da17 7472  ..r....r......tr
-00002a80: 6169 6e69 6e67 5f64 6174 6173 6574 5f70  aining_dataset_p
-00002a90: 616e 6461 73da 1674 7261 696e 696e 675f  andas..training_
-00002aa0: 6461 7461 7365 745f 6172 726f 775a 1976  dataset_arrowZ.v
-00002ab0: 616c 6964 6174 696f 6e5f 6461 7461 7365  alidation_datase
-00002ac0: 745f 7061 6e64 6173 da18 7661 6c69 6461  t_pandas..valida
-00002ad0: 7469 6f6e 5f64 6174 6173 6574 5f61 7272  tion_dataset_arr
-00002ae0: 6f77 da13 7465 7374 5f64 6174 6173 6574  ow..test_dataset
-00002af0: 5f70 616e 6461 73da 1274 6573 745f 6461  _pandas..test_da
-00002b00: 7461 7365 745f 6172 726f 7772 3000 0000  taset_arrowr0...
-00002b10: 7230 0000 0072 3100 0000 da0f 7072 6570  r0...r1.....prep
-00002b20: 6172 655f 6461 7461 7365 7472 0100 0073  are_datasetr...s
-00002b30: 2800 0000 0801 1002 0c01 0a01 1002 0c01  (...............
-00002b40: 0a01 1002 0c01 0c01 1004 0c01 0a01 1002  ................
-00002b50: 0c01 0a01 1002 0c01 0a01 0e02 72eb 0000  ............r...
-00002b60: 0063 0400 0000 0000 0000 0000 0000 0600  .c..............
-00002b70: 0000 0600 0000 0300 0000 734e 0000 0074  ..........sN...t
-00002b80: 00a0 017c 017c 027c 0364 019c 03a1 017d  ...|.|.|.d.....}
-00002b90: 047c 046a 0287 0066 0164 0264 0384 0864  .|.j...f.d.d...d
-00002ba0: 0464 058d 027d 057c 05a0 0364 0667 01a1  .d...}.|...d.g..
-00002bb0: 017d 057c 05a0 0464 0764 08a1 027d 057c  .}.|...d.d...}.|
-00002bc0: 05a0 0564 09a1 0101 007c 0553 0029 0a4e  ...d.....|.S.).N
-00002bd0: 2903 da05 7472 6169 6eda 0a76 616c 6964  )...train..valid
-00002be0: 6174 696f 6eda 0474 6573 7463 0100 0000  ation..testc....
-00002bf0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00002c00: 1300 0000 730a 0000 0074 0088 007c 0083  ....s....t...|..
-00002c10: 0253 00a9 014e 2901 727a 0000 0029 0172  .S...N).rz...).r
-00002c20: 7900 0000 72b4 0000 0072 3000 0000 7231  y...r....r0...r1
-00002c30: 0000 00da 083c 6c61 6d62 6461 3e98 0100  .....<lambda>...
-00002c40: 0073 0200 0000 0a00 7a34 696e 6974 616c  .s......z4inital
-00002c50: 697a 655f 6461 7461 7365 745f 666f 725f  ize_dataset_for_
-00002c60: 746f 6b65 6e69 7a61 7469 6f6e 2e3c 6c6f  tokenization.<lo
-00002c70: 6361 6c73 3e2e 3c6c 616d 6264 613e 5429  cals>.<lambda>T)
-00002c80: 01da 0762 6174 6368 6564 7274 0000 0072  ...batchedrt...r
-00002c90: df00 0000 726d 0000 0072 5800 0000 2906  ....rm...rX...).
-00002ca0: 72e4 0000 00da 0b44 6174 6173 6574 4469  r......DatasetDi
-00002cb0: 6374 da03 6d61 70da 0e72 656d 6f76 655f  ct..map..remove_
-00002cc0: 636f 6c75 6d6e 73da 0d72 656e 616d 655f  columns..rename_
-00002cd0: 636f 6c75 6d6e da0a 7365 745f 666f 726d  column..set_form
-00002ce0: 6174 2906 7278 0000 0072 e700 0000 72e8  at).rx...r....r.
-00002cf0: 0000 0072 ea00 0000 7283 0000 00da 1274  ...r....r......t
-00002d00: 6f6b 656e 697a 6564 5f64 6174 6173 6574  okenized_dataset
-00002d10: 7372 3000 0000 72b4 0000 0072 3100 0000  sr0...r....r1...
-00002d20: da22 696e 6974 616c 697a 655f 6461 7461  ."initalize_data
-00002d30: 7365 745f 666f 725f 746f 6b65 6e69 7a61  set_for_tokeniza
-00002d40: 7469 6f6e 9201 0000 7312 0000 0006 0202  tion....s.......
-00002d50: 0102 0108 fe16 040c 020c 010a 0104 0272  ...............r
-00002d60: f800 0000 630c 0000 0000 0000 0000 0000  ....c...........
-00002d70: 002b 0000 000b 0000 0043 0000 0073 ac03  .+.......C...s..
-00002d80: 0000 6700 7d0c 6700 7d0d 6700 7d0e 7400  ..g.}.g.}.g.}.t.
-00002d90: 6401 7c00 8302 4400 9001 5dc7 7d0f 7401  d.|...D...].}.t.
-00002da0: a001 a100 7d10 7402 6402 8301 0100 7403  ....}.t.d.....t.
-00002db0: 7c01 6403 1900 7c02 6404 8d02 7d11 7403  |.d...|.d...}.t.
-00002dc0: 7c01 6405 1900 7c02 6404 8d02 7d12 7403  |.d...|.d...}.t.
-00002dd0: 7c01 6406 1900 7c02 6404 8d02 7d13 7404  |.d...|.d...}.t.
-00002de0: 7405 7406 7c03 8301 8301 7c04 8302 7d14  t.t.|.....|...}.
-00002df0: 7c14 a007 7c06 a101 0100 7408 a009 a100  |...|.....t.....
-00002e00: 7d15 740a 7c14 a00b a100 7c05 6407 8d02  }.t.|.....|.d...
-00002e10: 7d16 7c09 7405 7c11 8301 1400 7d17 740c  }.|.t.|.....}.t.
-00002e20: 6408 7c16 7c0a 7c17 6409 8d04 7d18 6700  d.|.|.|.d...}.g.
-00002e30: 7d19 6700 7d1a 6700 7d1b 6700 7d1c 6401  }.g.}.g.}.g.}.d.
-00002e40: 640a 6c0d 6d0e 7d1d 0100 7c1d 7c08 640b  d.l.m.}...|.|.d.
-00002e50: 7c07 640c 8d03 7d1e 7402 640d 7c07 1700  |.d...}.t.d.|...
-00002e60: 8301 0100 7402 640e 8301 0100 6401 7d1f  ....t.d.....d.}.
-00002e70: 7400 7c09 8301 4400 9001 5d4e 7d20 7c1f  t.|...D...]N} |.
-00002e80: 640f 3700 7d1f 7402 6410 740f 7c20 8301  d.7.}.t.d.t.| ..
-00002e90: 1700 8301 0100 7410 7400 7405 7c11 8301  ......t.t.t.|...
-00002ea0: 8301 8301 7d21 6401 7d22 7c14 a011 a100  ....}!d.}"|.....
-00002eb0: 0100 7c11 4400 5d5e 7d23 7c04 6411 7600  ..|.D.]^}#|.d.v.
-00002ec0: 72b2 7c23 6412 1900 a007 7c06 a101 7c23  r.|#d.....|...|#
-00002ed0: 6413 1900 a012 a100 a007 7c06 a101 6414  d.........|...d.
-00002ee0: 9c02 7d24 6e0f 7c23 6412 1900 a007 7c06  ..}$n.|#d.....|.
-00002ef0: a101 7c23 6413 1900 a007 7c06 a101 6414  ..|#d.....|...d.
-00002f00: 9c02 7d24 7c14 6421 6900 7c24 a401 8e01  ..}$|.d!i.|$....
-00002f10: 7d25 7c15 7c25 7c23 6415 1900 a007 7c06  }%|.|%|#d.....|.
-00002f20: a101 8302 7d26 7c26 a013 a100 0100 7c22  ....}&|&......|"
-00002f30: 640f 3700 7d22 7c22 7c0b 1600 6401 6b02  d.7.}"|"|...d.k.
-00002f40: 72ec 7c16 a014 a100 0100 7c18 a014 a100  r.|.......|.....
-00002f50: 0100 7c16 a015 a100 0100 7c21 a016 640f  ..|.......|!..d.
-00002f60: a101 0100 7c19 a017 7c26 a018 a100 a101  ....|...|&......
-00002f70: 0100 719a 7410 7400 7405 7c12 8301 8301  ..q.t.t.t.|.....
-00002f80: 8301 7d21 7c14 a019 a100 0100 7c12 4400  ..}!|.......|.D.
-00002f90: 5d73 7d23 741a a01b a100 8f63 0100 7c04  ]s}#t......c..|.
-00002fa0: 6411 7600 9001 7225 7c23 6412 1900 a007  d.v...r%|#d.....
-00002fb0: 7c06 a101 7c23 6413 1900 a012 a100 a007  |...|#d.........
-00002fc0: 7c06 a101 6414 9c02 7d24 6e0f 7c23 6412  |...d...}$n.|#d.
-00002fd0: 1900 a007 7c06 a101 7c23 6413 1900 a007  ....|...|#d.....
-00002fe0: 7c06 a101 6414 9c02 7d24 7c04 6416 7600  |...d...}$|.d.v.
-00002ff0: 9001 724c 7c23 6415 1900 a01c 7c23 6415  ..rL|#d.....|#d.
-00003000: 1900 6a1d 6401 1900 640f a102 a007 7c06  ..j.d...d.....|.
-00003010: a101 6601 7c24 6417 3c00 7c14 6421 6900  ..f.|$d.<.|.d!i.
-00003020: 7c24 a401 8e01 7d25 7c15 7c25 7c23 6415  |$....}%|.|%|#d.
-00003030: 1900 a007 7c06 a101 8302 7d26 7c21 a016  ....|.....}&|!..
-00003040: 640f a101 0100 7c1a a017 7c26 a018 a100  d.....|...|&....
-00003050: a101 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00003060: 6e09 3100 9001 7374 7701 0100 0100 0100  n.1...stw.......
-00003070: 5900 0100 9001 7107 741e a01f 7c19 a101  Y.....q.t...|...
-00003080: 7d27 741e a01f 7c1a a101 7d28 7c1b a017  }'t...|...}(|...
-00003090: 7c27 a101 0100 7c1c a017 7c28 a101 0100  |'....|...|(....
-000030a0: 7405 740f 7c09 8301 8301 7d29 6418 7c20  t.t.|.....})d.| 
-000030b0: 6419 7c29 9b00 9d02 9b04 641a 7c09 6419  d.|)......d.|.d.
-000030c0: 7c29 9b00 9d02 9b04 641b 9d05 641c 7c27  |)......d...d.|'
-000030d0: 641d 9b04 641e 9d03 1700 641f 7c28 641d  d...d.....d.|(d.
-000030e0: 9b04 9d02 1700 7d2a 7402 7c2a 8301 0100  ......}*t.|*....
-000030f0: 6700 7d19 6700 7d1a 7c1e 7c28 7c14 8302  g.}.g.}.|.|(|...
-00003100: 0100 7c1e 6a20 9001 72ca 7402 6420 8301  ..|.j ..r.t.d ..
-00003110: 0100 0100 6e01 717b 7c14 7c1b 7c1c 7c13  ....n.q{|.|.|.|.
-00003120: 7c0e 6605 0200 0100 5300 6400 5300 2922  |.f.....S.d.S.)"
-00003130: 4e72 0100 0000 7a0d 4c6f 6164 696e 6720  Nr....z.Loading 
-00003140: 4d6f 6465 6c72 ec00 0000 2901 da0a 6261  Modelr....)...ba
-00003150: 7463 685f 7369 7a65 72ed 0000 0072 ee00  tch_sizer....r..
-00003160: 0000 2901 da02 6c72 da06 6c69 6e65 6172  ..)...lr..linear
-00003170: 2904 da04 6e61 6d65 da09 6f70 7469 6d69  )...name..optimi
-00003180: 7a65 7272 9600 0000 da12 6e75 6d5f 7472  zerr......num_tr
-00003190: 6169 6e69 6e67 5f73 7465 7073 2901 da0d  aining_steps)...
-000031a0: 4561 726c 7953 746f 7070 696e 6754 2903  EarlyStoppingT).
-000031b0: da08 7061 7469 656e 6365 da07 7665 7262  ..patience..verb
-000031c0: 6f73 6572 7f00 0000 7289 0000 007a 1242  oser....r....z.B
-000031d0: 6567 696e 6e69 6e67 2054 7261 696e 696e  eginning Trainin
-000031e0: 6772 3900 0000 7a0f 4375 7272 656e 7420  gr9...z.Current 
-000031f0: 4570 6f63 683a 2072 4c00 0000 7267 0000  Epoch: rL...rg..
-00003200: 0072 6800 0000 a902 726b 0000 0072 6c00  .rh.....rk...rl.
-00003210: 0000 726d 0000 00a9 0372 6600 0000 7250  ..rm.....rf...rP
-00003220: 0000 0072 4f00 0000 726e 0000 00da 015b  ...rO...rn.....[
-00003230: da01 3e72 7c00 0000 7a02 5d20 7a0c 7472  ..>r|...z.] z.tr
-00003240: 6169 6e5f 6c6f 7373 3a20 7a03 2e35 6672  ain_loss: z..5fr
-00003250: 1c00 0000 7a0c 7661 6c69 645f 6c6f 7373  ....z.valid_loss
-00003260: 3a20 7a0e 4561 726c 7920 7374 6f70 7069  : z.Early stoppi
-00003270: 6e67 7230 0000 0029 2172 ba00 0000 728d  ngr0...)!r....r.
-00003280: 0000 0072 2c00 0000 720d 0000 0072 4500  ...r,...r....rE.
-00003290: 0000 722a 0000 0072 d600 0000 da02 746f  ..r*...r......to
-000032a0: 725d 0000 00da 1043 726f 7373 456e 7472  r].....CrossEntr
-000032b0: 6f70 794c 6f73 7372 0c00 0000 da0a 7061  opyLossr......pa
-000032c0: 7261 6d65 7465 7273 720e 0000 005a 2b61  rametersr....Z+a
-000032d0: 7265 732e 4c4c 4d5f 6173 5f61 5f4a 7564  res.LLM_as_a_Jud
-000032e0: 6765 5f41 6461 7074 6174 696f 6e2e 7079  ge_Adaptation.py
-000032f0: 746f 7263 6874 6f6f 6c73 72ff 0000 0072  torchtoolsr....r
-00003300: 2d00 0000 7212 0000 0072 ec00 0000 da04  -...r....r......
-00003310: 626f 6f6c da08 6261 636b 7761 7264 da04  bool..backward..
-00003320: 7374 6570 da09 7a65 726f 5f67 7261 64da  step..zero_grad.
-00003330: 0675 7064 6174 65da 0661 7070 656e 64da  .update..append.
-00003340: 0469 7465 6dda 0465 7661 6c72 5800 0000  .item..evalrX...
-00003350: da07 6e6f 5f67 7261 64da 0772 6573 6861  ..no_grad..resha
-00003360: 7065 da05 7368 6170 65da 026e 70da 0761  pe..shape..np..a
-00003370: 7665 7261 6765 5a0a 6561 726c 795f 7374  verageZ.early_st
-00003380: 6f70 292b 7290 0000 0072 f700 0000 7298  op)+r....r....r.
-00003390: 0000 0072 d800 0000 7252 0000 0072 8f00  ...r....rR...r..
-000033a0: 0000 da06 6465 7669 6365 7299 0000 0072  ....devicer....r
-000033b0: 9400 0000 7295 0000 0072 9600 0000 7297  ....r....r....r.
-000033c0: 0000 005a 0e6d 6963 726f 5f61 7665 7261  ...Z.micro_avera
-000033d0: 6765 735a 0e6d 6163 726f 5f61 7665 7261  gesZ.macro_avera
-000033e0: 6765 73da 0f69 6e66 6572 656e 6365 5f74  ges..inference_t
-000033f0: 696d 6573 723c 0000 005a 0972 756e 5f73  imesr<...Z.run_s
-00003400: 7461 7274 5a10 7472 6169 6e5f 6461 7461  tartZ.train_data
-00003410: 6c6f 6164 6572 5a15 7661 6c69 6461 7469  loaderZ.validati
-00003420: 6f6e 5f64 6174 616c 6f61 6465 72da 0f65  on_dataloader..e
-00003430: 7661 6c5f 6461 7461 6c6f 6164 6572 da05  val_dataloader..
-00003440: 6d6f 6465 6c5a 0963 7269 7465 7269 6f6e  modelZ.criterion
-00003450: 72fd 0000 0072 fe00 0000 da0c 6c72 5f73  r....r......lr_s
-00003460: 6368 6564 756c 6572 5a0c 7472 6169 6e5f  chedulerZ.train_
-00003470: 6c6f 7373 6573 5a0c 7661 6c69 645f 6c6f  lossesZ.valid_lo
-00003480: 7373 6573 da10 6176 675f 7472 6169 6e5f  sses..avg_train_
-00003490: 6c6f 7373 6573 da10 6176 675f 7661 6c69  losses..avg_vali
-000034a0: 645f 6c6f 7373 6573 72ff 0000 00da 0e65  d_lossesr......e
-000034b0: 6172 6c79 5f73 746f 7070 696e 675a 1674  arly_stoppingZ.t
-000034c0: 6f74 616c 5f65 706f 6368 735f 7065 7266  otal_epochs_perf
-000034d0: 6f72 6d65 64da 0565 706f 6368 da0c 7072  ormed..epoch..pr
-000034e0: 6f67 7265 7373 5f62 6172 5a1b 6772 6164  ogress_barZ.grad
-000034f0: 6965 6e74 5f61 6363 756d 756c 6174 696f  ient_accumulatio
-00003500: 6e5f 636f 756e 74da 0562 6174 6368 da09  n_count..batch..
-00003510: 6e65 775f 6261 7463 68da 076f 7574 7075  new_batch..outpu
-00003520: 7473 da04 6c6f 7373 5a0a 7472 6169 6e5f  ts..lossZ.train_
-00003530: 6c6f 7373 5a0a 7661 6c69 645f 6c6f 7373  lossZ.valid_loss
-00003540: 5a09 6570 6f63 685f 6c65 6e5a 0970 7269  Z.epoch_lenZ.pri
-00003550: 6e74 5f6d 7367 7230 0000 0072 3000 0000  nt_msgr0...r0...
-00003560: 7231 0000 00da 1874 7261 696e 5f61 6e64  r1.....train_and
-00003570: 5f65 7661 6c75 6174 655f 6d6f 6465 6ca2  _evaluate_model.
-00003580: 0100 0073 a400 0000 0403 0401 0401 1002  ...s............
-00003590: 0802 0802 1002 1001 1001 1206 0a02 0804  ................
-000035a0: 1001 0c02 0202 0801 06ff 0407 0402 0402  ................
-000035b0: 0402 0c03 0e03 0c03 0802 0402 0e02 0802  ................
-000035c0: 1002 1002 0402 0802 0801 0802 2401 1e02  ............$...
-000035d0: 0e02 1402 0802 0802 0c01 0801 0801 0801  ................
-000035e0: 0a02 1001 1004 0802 0801 0a02 0a02 2401  ..............$.
-000035f0: 1e02 0a02 2601 0e02 1402 0a01 1002 1ef1  ....&...........
-00003600: 0480 0a13 0a01 0a01 0a01 0c02 2002 0c01  ............ ...
-00003610: 02ff 0a02 04fe 0804 0403 0401 0a04 0802  ................
-00003620: 0801 0401 02fe 1204 0081 04f6 7224 0100  ............r$..
-00003630: 0063 0600 0000 0000 0000 0000 0000 1200  .c..............
-00003640: 0000 0900 0000 4300 0000 7398 0100 0074  ......C...s....t
-00003650: 0064 0183 0101 007c 00a0 0174 02a0 037c  .d.....|...t...|
-00003660: 02a1 01a1 0101 0074 0064 0283 0101 0074  .......t.d.....t
-00003670: 0464 0383 017d 0674 02a0 0567 00a1 01a0  .d...}.t...g....
-00003680: 067c 03a1 017d 0774 02a0 0567 00a1 01a0  .|...}.t...g....
-00003690: 067c 03a1 017d 0874 07a0 07a1 007d 0974  .|...}.t.....}.t
-000036a0: 0874 0974 0a7c 0483 0183 0183 017d 0a7c  .t.t.|.......}.|
-000036b0: 0444 005d 877d 0b74 02a0 0ba1 008f 7901  .D.].}.t......y.
-000036c0: 007c 0164 0476 0072 4f7c 0b64 0519 00a0  .|.d.v.rO|.d....
-000036d0: 067c 03a1 017c 0b64 0619 00a0 0ca1 00a0  .|...|.d........
-000036e0: 067c 03a1 0164 079c 027d 0c6e 0f7c 0b64  .|...d...}.n.|.d
-000036f0: 0519 00a0 067c 03a1 017c 0b64 0619 00a0  .....|...|.d....
-00003700: 067c 03a1 0164 079c 027d 0c7c 0164 0876  .|...d...}.|.d.v
-00003710: 0072 747c 0b64 0919 00a0 0d7c 0b64 0919  .rt|.d.....|.d..
-00003720: 006a 0e64 0a19 0064 0ba1 02a0 067c 03a1  .j.d...d.....|..
-00003730: 017c 0c64 0c3c 007c 0064 1069 007c 0ca4  .|.d.<.|.d.i.|..
-00003740: 018e 017d 0d7c 0d7d 0e74 026a 0f7c 0e64  ...}.|.}.t.j.|.d
-00003750: 0d64 0e8d 027d 0f7c 066a 107c 0f7c 0b64  .d...}.|.j.|.|.d
-00003760: 0919 00a0 067c 03a1 0164 0f8d 0201 0074  .....|...d.....t
-00003770: 02a0 117c 077c 0f66 0264 0aa1 027d 0774  ...|.|.f.d...}.t
-00003780: 02a0 117c 087c 0b64 0919 00a0 067c 03a1  ...|.|.d.....|..
-00003790: 0166 0264 0aa1 027d 087c 0aa0 1264 0ba1  .f.d...}.|...d..
-000037a0: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-000037b0: 0831 0073 b477 0101 0001 0001 0059 0001  .1.s.w.......Y..
-000037c0: 0071 3274 07a0 07a1 007d 107c 107c 0918  .q2t.....}.|.|..
-000037d0: 007d 117c 05a0 137c 11a1 0101 007c 077c  .}.|...|.....|.|
-000037e0: 087c 0666 0353 0029 114e 7a16 4c6f 6164  .|.f.S.).Nz.Load
-000037f0: 696e 6720 7468 6520 4265 7374 204d 6f64  ing the Best Mod
-00003800: 656c 7a14 4265 6769 6e6e 696e 6720 4576  elz.Beginning Ev
-00003810: 616c 7561 7469 6f6e da08 6163 6375 7261  aluation..accura
-00003820: 6379 724c 0000 0072 6700 0000 7268 0000  cyrL...rg...rh..
-00003830: 0072 0201 0000 7203 0100 0072 6d00 0000  .r....r....rm...
-00003840: 7201 0000 0072 3900 0000 726e 0000 0072  r....r9...rn...r
-00003850: 3800 0000 2901 da03 6469 6d29 02da 0b70  8...)...dim)...p
-00003860: 7265 6469 6374 696f 6e73 da0a 7265 6665  redictions..refe
-00003870: 7265 6e63 6573 7230 0000 0029 1472 2c00  rencesr0...).r,.
-00003880: 0000 da0f 6c6f 6164 5f73 7461 7465 5f64  ....load_state_d
-00003890: 6963 7472 5800 0000 da04 6c6f 6164 7209  ictrX.....loadr.
-000038a0: 0000 00da 0b46 6c6f 6174 5465 6e73 6f72  .....FloatTensor
-000038b0: 7206 0100 0072 8d00 0000 7212 0000 0072  r....r....r....r
-000038c0: ba00 0000 722a 0000 0072 1101 0000 7209  ....r*...r....r.
-000038d0: 0100 0072 1201 0000 7213 0100 00da 0661  ...r....r......a
-000038e0: 7267 6d61 78da 0961 6464 5f62 6174 6368  rgmax..add_batch
-000038f0: da03 6361 7472 0d01 0000 720e 0100 0029  ..catr....r....)
-00003900: 1272 1901 0000 7252 0000 0072 9900 0000  .r....rR...r....
-00003910: 7216 0100 0072 1801 0000 7217 0100 00da  r....r....r.....
-00003920: 066d 6574 7269 63da 1174 6f74 616c 5f70  .metric..total_p
-00003930: 7265 6469 6374 696f 6e73 da10 746f 7461  redictions..tota
-00003940: 6c5f 7265 6665 7265 6e63 6573 5a0f 696e  l_referencesZ.in
-00003950: 6665 7265 6e63 655f 7374 6172 7472 1f01  ference_startr..
-00003960: 0000 7220 0100 0072 2101 0000 7222 0100  ..r ...r!...r"..
-00003970: 0072 6900 0000 7227 0100 005a 0d69 6e66  .ri...r'...Z.inf
-00003980: 6572 656e 6365 5f65 6e64 5a14 746f 7461  erence_endZ.tota
-00003990: 6c5f 696e 6665 7265 6e63 655f 7469 6d65  l_inference_time
-000039a0: 7230 0000 0072 3000 0000 7231 0000 00da  r0...r0...r1....
-000039b0: 0e65 7661 6c75 6174 655f 6d6f 6465 6c36  .evaluate_model6
-000039c0: 0200 0073 3800 0000 0802 1002 0804 0802  ...s8...........
-000039d0: 1002 1001 0802 1004 0801 0a02 0802 2401  ..............$.
-000039e0: 1e02 0802 2401 0e02 0402 0e01 1801 1002  ....$...........
-000039f0: 1a01 0c02 1ced 0280 0817 0801 0a01 0a02  ................
-00003a00: 7232 0100 0063 0400 0000 0000 0000 0000  r2...c..........
-00003a10: 0000 0800 0000 0800 0000 4300 0000 73e2  ..........C...s.
-00003a20: 0000 0074 0064 0183 0101 0074 0064 0283  ...t.d.....t.d..
-00003a30: 0101 0074 007c 006a 0183 0101 0074 007c  ...t.|.j.....t.|
-00003a40: 016a 0183 0101 007c 036a 027c 017c 0064  .j.....|.j.|.|.d
-00003a50: 038d 027d 0474 0064 0474 037c 0464 0519  ...}.t.d.t.|.d..
-00003a60: 0083 0117 0083 0101 0074 0464 0664 0764  .........t.d.d.d
-00003a70: 088d 027d 057c 056a 0264 097c 017c 0064  ...}.|.j.d.|.|.d
-00003a80: 0a8d 037d 0674 0064 0b74 037c 0664 0619  ...}.t.d.t.|.d..
-00003a90: 0064 0c14 0083 0117 0083 0101 007c 056a  .d...........|.j
-00003aa0: 0264 0d7c 017c 0064 0a8d 037d 0774 0064  .d.|.|.d...}.t.d
-00003ab0: 0e74 037c 0764 0619 0064 0c14 0083 0117  .t.|.d...d......
-00003ac0: 0083 0101 0074 0064 0f74 0374 057c 01a0  .....t.d.t.t.|..
-00003ad0: 06a1 00a0 0764 10a1 0174 087c 01a0 06a1  .....d...t.|....
-00003ae0: 0083 011b 0064 1183 0283 0117 0083 0101  .....d..........
-00003af0: 0074 0064 1274 037c 0283 0117 0083 0101  .t.d.t.|........
-00003b00: 0064 0053 0029 134e 7a1a 2d2d 2d2d 2d2d  .d.S.).Nz.------
-00003b10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003b20: 2d2d 2d2d 7a20 5072 6564 6963 7469 6f6e  ----z Prediction
-00003b30: 7320 616e 6420 5265 6665 7265 6e63 6520  s and Reference 
-00003b40: 5368 6170 6573 2902 7228 0100 0072 2701  Shapes).r(...r'.
-00003b50: 0000 7a17 4163 6375 7261 6379 2066 6f72  ..z.Accuracy for
-00003b60: 2054 6573 7420 5365 743a 2072 2501 0000   Test Set: r%...
-00003b70: da02 6631 5472 4600 0000 da05 6d61 6372  ..f1TrF.....macr
-00003b80: 6f29 0372 1501 0000 7228 0100 0072 2701  o).r....r(...r'.
-00003b90: 0000 7a17 4d61 6372 6f20 4631 2066 6f72  ..z.Macro F1 for
-00003ba0: 2054 6573 7420 5365 743a 2072 2200 0000   Test Set: r"...
-00003bb0: da05 6d69 6372 6f7a 174d 6963 726f 2046  ..microz.Micro F
-00003bc0: 3120 666f 7220 5465 7374 2053 6574 3a20  1 for Test Set: 
-00003bd0: 7a25 506f 7369 7469 7665 202f 204e 6567  z%Positive / Neg
-00003be0: 6174 6976 6520 5265 6665 7265 6e63 6520  ative Reference 
-00003bf0: 5261 7469 6f3a 2072 3900 0000 e903 0000  Ratio: r9.......
-00003c00: 007a 2453 6176 6564 2063 6c61 7373 6966  .z$Saved classif
-00003c10: 6963 6174 696f 6e20 6368 6563 6b70 6f69  ication checkpoi
-00003c20: 6e74 2074 6f3a 2029 0972 2c00 0000 7213  nt to: ).r,...r.
-00003c30: 0100 00da 0763 6f6d 7075 7465 722d 0000  .....computer-..
-00003c40: 0072 0900 0000 da05 726f 756e 64da 0674  .r......round..t
-00003c50: 6f6c 6973 74da 0563 6f75 6e74 722a 0000  olist..countr*..
-00003c60: 0029 0872 3001 0000 7231 0100 0072 9900  .).r0...r1...r..
-00003c70: 0000 722f 0100 00da 0772 6573 756c 7473  ..r/.....results
-00003c80: 5a0a 665f 315f 6d65 7472 6963 5a11 6d61  Z.f_1_metricZ.ma
-00003c90: 6372 6f5f 665f 315f 7265 7375 6c74 735a  cro_f_1_resultsZ
-00003ca0: 116d 6963 726f 5f66 5f31 5f72 6573 756c  .micro_f_1_resul
-00003cb0: 7473 7230 0000 0072 3000 0000 7231 0000  tsr0...r0...r1..
-00003cc0: 00da 1470 7269 6e74 5f61 6e64 5f73 6176  ...print_and_sav
-00003cd0: 655f 6d6f 6465 6c6b 0200 0073 1a00 0000  e_modelk...s....
-00003ce0: 0801 0801 0a01 0a01 0e02 1401 0c02 1001  ................
-00003cf0: 1801 1001 1801 2c02 1402 723c 0100 00da  ......,...r<....
-00003d00: 085f 5f6d 6169 6e5f 5f7a 182d 2d63 6c61  .__main__z.--cla
-00003d10: 7373 6966 6963 6174 696f 6e5f 6461 7461  ssification_data
-00003d20: 7365 7454 2902 da04 7479 7065 da08 7265  setT)...type..re
-00003d30: 7175 6972 6564 7a14 2d2d 7465 7374 5f73  quiredz.--test_s
-00003d40: 6574 5f73 656c 6563 7469 6f6e 7a0e 2d2d  et_selectionz.--
-00003d50: 6c61 6265 6c5f 636f 6c75 6d6e 7a0c 2d2d  label_columnz.--
-00003d60: 6e75 6d5f 6570 6f63 6873 7a10 2d2d 7061  num_epochsz.--pa
-00003d70: 7469 656e 6365 5f76 616c 7565 7a0f 2d2d  tience_valuez.--
-00003d80: 6c65 6172 6e69 6e67 5f72 6174 657a 0663  learning_ratez.c
-00003d90: 7564 613a 3072 3900 0000 e920 0000 0072  uda:0r9.... ...r
-00003da0: 2200 0000 72ef 0000 0029 5dda 0874 6f72  "...r....)]..tor
-00003db0: 6368 2e6e 6e72 5d00 0000 da0c 7472 616e  ch.nnr].....tran
-00003dc0: 7366 6f72 6d65 7273 7202 0000 0072 0300  sformersr....r..
-00003dd0: 0000 7204 0000 0072 0500 0000 7206 0000  ..r....r....r...
-00003de0: 0072 0700 0000 7208 0000 00da 0670 616e  .r....r......pan
-00003df0: 6461 7372 b600 0000 da05 6e75 6d70 7972  dasr......numpyr
-00003e00: 1401 0000 da03 6173 7472 e400 0000 7209  ......astr....r.
-00003e10: 0000 0072 0a00 0000 720b 0000 00da 0770  ...r....r......p
-00003e20: 7961 7272 6f77 72e1 0000 00da 0f70 7961  yarrowr......pya
-00003e30: 7272 6f77 2e64 6174 6173 6574 7284 0000  rrow.datasetr...
-00003e40: 00da 0264 735a 0b74 6f72 6368 2e6f 7074  ...dsZ.torch.opt
-00003e50: 696d 720c 0000 00da 1074 6f72 6368 2e75  imr......torch.u
-00003e60: 7469 6c73 2e64 6174 6172 0d00 0000 720e  tils.datar....r.
-00003e70: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
-00003e80: 0000 7258 0000 00da 0974 7164 6d2e 6175  ..rX.....tqdm.au
-00003e90: 746f 7212 0000 00da 0a73 7461 7469 7374  tor......statist
-00003ea0: 6963 7372 8d00 0000 da0a 7375 6270 726f  icsr......subpro
-00003eb0: 6365 7373 723f 0000 0072 7e00 0000 da17  cessr?...r~.....
-00003ec0: 736b 6c65 6172 6e2e 6d6f 6465 6c5f 7365  sklearn.model_se
-00003ed0: 6c65 6374 696f 6e72 1300 0000 da04 6a73  lectionr......js
-00003ee0: 6f6e da06 7261 6e64 6f6d 7224 0000 00da  on..randomr$....
-00003ef0: 0861 7267 7061 7273 6572 1400 0000 da08  .argparser......
-00003f00: 7761 726e 696e 6773 da0e 6669 6c74 6572  warnings..filter
-00003f10: 7761 726e 696e 6773 722d 0000 0072 3200  warningsr-...r2.
-00003f20: 0000 7235 0000 0072 a500 0000 da04 7365  ..r5...r......se
-00003f30: 6564 da0b 6d61 6e75 616c 5f73 6565 64da  ed..manual_seed.
-00003f40: 0765 6e76 6972 6f6e 7244 0000 00da 064d  .environrD.....M
-00003f50: 6f64 756c 6572 4500 0000 727a 0000 0072  odulerE...rz...r
-00003f60: 8500 0000 7287 0000 0072 9a00 0000 72bc  ....r....r....r.
-00003f70: 0000 0072 c800 0000 72de 0000 0072 eb00  ...r....r....r..
-00003f80: 0000 72f8 0000 0072 2401 0000 7232 0100  ..r....r$...r2..
-00003f90: 0072 3c01 0000 7270 0000 00da 0e41 7267  .r<...rp.....Arg
-00003fa0: 756d 656e 7450 6172 7365 72da 0670 6172  umentParser..par
-00003fb0: 7365 72da 0c61 6464 5f61 7267 756d 656e  ser..add_argumen
-00003fc0: 7472 3a00 0000 da05 666c 6f61 74da 0a70  tr:.....float..p
-00003fd0: 6172 7365 5f61 7267 73da 0461 7267 7372  arse_args..argsr
-00003fe0: 8300 0000 7282 0000 005a 1274 6573 745f  ....r....Z.test_
-00003ff0: 7365 745f 7365 6c65 6374 696f 6e72 9200  set_selectionr..
-00004000: 0000 7295 0000 0072 9400 0000 da0d 6c65  ..r....r......le
-00004010: 6172 6e69 6e67 5f72 6174 6572 8e00 0000  arning_rater....
-00004020: 7216 0100 0072 9100 0000 7298 0000 0072  r....r....r....r
-00004030: 9700 0000 7290 0000 0072 9600 0000 7230  ....r....r....r0
-00004040: 0000 0072 3000 0000 7230 0000 0072 3100  ...r0...r0...r1.
-00004050: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00004060: 7392 0000 000c 0214 0118 0108 0308 0108  s...............
-00004070: 0108 010c 0110 0108 020c 010c 020c 0118  ................
-00004080: 0108 020c 0108 0108 0108 0208 010c 0208  ................
-00004090: 0108 0108 0208 0110 0208 020e 0114 0312  ................
-000040a0: 1604 120c 020a 010a 010e 0108 0412 0808  ................
-000040b0: 4c08 0508 1308 0808 2808 2f08 2208 2908  L.......(./.".).
-000040c0: 2008 1000 7f08 1508 350a 1408 0210 0210   .......5.......
-000040d0: 0110 0110 0110 0110 0108 0208 0206 0106  ................
-000040e0: 0106 0106 0108 0104 040a 0104 0204 0104  ................
-000040f0: 0104 0208 0104 e2                        .......
+00000150: 6d2e 5a2e 0100 643e 640c 652f 640d 652f  m.Z...d>d.e/d.e/
+00000160: 6604 640e 640f 8405 5a30 6410 652f 640d  f.d.d...Z0d.e/d.
+00000170: 652f 6604 6411 6412 8404 5a31 6413 5a32  e/f.d.d...Z1d.Z2
+00000180: 650d 6a2b a033 6532 a101 0100 652b a033  e.j+.3e2....e+.3
+00000190: 6532 a101 0100 6520 a034 6532 a101 0100  e2....e .4e2....
+000001a0: 652f 6532 8301 6527 6a35 6414 3c00 6415  e/e2..e'j5d.<.d.
+000001b0: 6416 8400 5a36 4700 6417 6418 8400 6418  d...Z6G.d.d...d.
+000001c0: 6501 6a37 8303 5a38 6419 641a 8400 5a39  e.j7..Z8d.d...Z9
+000001d0: 641b 641c 8400 5a3a 641d 641e 8400 5a3b  d.d...Z:d.d...Z;
+000001e0: 641f 6420 8400 5a3c 6421 6422 8400 5a3d  d.d ..Z<d!d"..Z=
+000001f0: 6423 6424 8400 5a3e 6425 6426 8400 5a3f  d#d$..Z>d%d&..Z?
+00000200: 6427 6428 8400 5a40 6429 642a 8400 5a41  d'd(..Z@d)d*..ZA
+00000210: 642b 642c 8400 5a42 642d 642e 8400 5a43  d+d,..ZBd-d...ZC
+00000220: 642f 6430 8400 5a44 6545 6431 6b02 9001  d/d0..ZDeEd1k...
+00000230: 7261 652d a046 a100 5a47 6547 6a48 6432  rae-.F..ZGeGjHd2
+00000240: 652f 6433 6434 8d03 0100 6547 6a48 6435  e/d3d4....eGjHd5
+00000250: 652f 6433 6434 8d03 0100 6547 6a48 6436  e/d3d4....eGjHd6
+00000260: 652f 6433 6434 8d03 0100 6547 6a48 6437  e/d3d4....eGjHd7
+00000270: 6549 6433 6434 8d03 0100 6547 6a48 6438  eId3d4....eGjHd8
+00000280: 6549 6433 6434 8d03 0100 6547 6a48 6439  eId3d4....eGjHd9
+00000290: 654a 6433 6434 8d03 0100 6547 a04b a100  eJd3d4....eG.K..
+000002a0: 5a4c 654c 6a4d 6701 5a4e 654c 6a4f 5a4f  ZLeLjMg.ZNeLjOZO
+000002b0: 654c 6a50 5a50 654c 6a51 5a51 654c 6a52  eLjPZPeLjQZQeLjR
+000002c0: 5a52 654c 6a53 6701 5a54 643a 5a55 6520  ZReLjSg.ZTd:ZUe 
+000002d0: a055 6555 a101 5a55 6433 5a56 643b 5a57  .UeU..ZUd3ZVd;ZW
+000002e0: 643c 5a58 643b 5a59 643d 5a5a 6401 5300  d<ZXd;ZYd=ZZd.S.
+000002f0: 6401 5300 293f e900 0000 004e 2903 da0b  d.S.)?.....N)...
+00000300: 5435 546f 6b65 6e69 7a65 72da 0e54 3545  T5Tokenizer..T5E
+00000310: 6e63 6f64 6572 4d6f 6465 6cda 1a54 3546  ncoderModel..T5F
+00000320: 6f72 436f 6e64 6974 696f 6e61 6c47 656e  orConditionalGen
+00000330: 6572 6174 696f 6e29 04da 0942 6572 744d  eration)...BertM
+00000340: 6f64 656c da0d 4175 746f 546f 6b65 6e69  odel..AutoTokeni
+00000350: 7a65 72da 0941 7574 6f4d 6f64 656c da0d  zer..AutoModel..
+00000360: 4750 5432 546f 6b65 6e69 7a65 7229 01da  GPT2Tokenizer)..
+00000370: 0b6c 6f61 645f 6d65 7472 6963 2902 da11  .load_metric)...
+00000380: 5472 6169 6e69 6e67 4172 6775 6d65 6e74  TrainingArgument
+00000390: 73da 0754 7261 696e 6572 2901 da04 4164  s..Trainer)...Ad
+000003a0: 616d 2901 da0a 4461 7461 4c6f 6164 6572  am)...DataLoader
+000003b0: 2904 da0d 6765 745f 7363 6865 6475 6c65  )...get_schedule
+000003c0: 72da 1441 7574 6f4d 6f64 656c 466f 7243  r..AutoModelForC
+000003d0: 6175 7361 6c4c 4dda 0a41 7574 6f43 6f6e  ausalLM..AutoCon
+000003e0: 6669 67da 2241 7574 6f4d 6f64 656c 466f  fig."AutoModelFo
+000003f0: 7253 6571 7565 6e63 6543 6c61 7373 6966  rSequenceClassif
+00000400: 6963 6174 696f 6e29 01da 0474 7164 6d29  ication)...tqdm)
+00000410: 01da 1074 7261 696e 5f74 6573 745f 7370  ...train_test_sp
+00000420: 6c69 7429 0272 1200 0000 da0b 7471 646d  lit).r......tqdm
+00000430: 5f70 616e 6461 73da 0571 7565 7279 da08  _pandas..query..
+00000440: 646f 6375 6d65 6e74 6303 0000 0000 0000  documentc.......
+00000450: 0000 0000 0004 0000 0008 0000 0043 0000  .............C..
+00000460: 0073 1e01 0000 7400 a001 6401 6402 7c01  .s....t...d.d.|.
+00000470: a002 6403 6404 a102 a002 6405 6404 a102  ..d.d.....d.d...
+00000480: a103 a003 a100 7d03 7c03 a002 6406 6404  ......}.|...d.d.
+00000490: a102 a002 6407 6404 a102 7d03 7400 a001  ....d.d...}.t...
+000004a0: 6408 6404 7c03 a103 a003 a100 7d03 6404  d.d.|.......}.d.
+000004b0: a004 7c03 a005 6404 a101 6400 6409 8502  ..|...d...d.d...
+000004c0: 1900 a101 7d03 7406 7c00 a005 6404 a101  ....}.t.|...d...
+000004d0: 8301 640a 6b04 7245 6404 a004 7c00 a005  ..d.k.rEd...|...
+000004e0: 6404 a101 6400 640b 8502 1900 a101 7d00  d...d.d.......}.
+000004f0: 7c02 6400 7500 724f 7c00 640c 1700 7c03  |.d.u.rO|.d...|.
+00000500: 1700 5300 7a0b 7c00 640c 1700 7c03 1700  ..S.z.|.d...|...
+00000510: 640c 1700 7c02 1700 5700 5300 0100 0100  d...|...W.S.....
+00000520: 0100 7407 8300 0100 7408 640d 8301 0100  ..t.....t.d.....
+00000530: 7408 640e 7409 7c00 8301 1700 8301 0100  t.d.t.|.........
+00000540: 7408 640f 7409 7c03 8301 1700 8301 0100  t.d.t.|.........
+00000550: 7408 6410 7409 7c02 8301 1700 8301 0100  t.d.t.|.........
+00000560: 7409 7c00 8301 640c 1700 7409 7c03 8301  t.|...d...t.|...
+00000570: 1700 640c 1700 7409 7c02 8301 1700 0600  ..d...t.|.......
+00000580: 5900 5300 2911 4efa 035c 6e2b da01 0afa  Y.S.).N..\n+....
+00000590: 010d da01 20fa 0109 da01 3dda 012d fa03  .... .....=..-..
+000005a0: 5c73 2be9 0002 0000 e964 0000 00e9 1e00  \s+......d......
+000005b0: 0000 7a03 207c 207a 2145 7272 6f72 2077  ..z. | z!Error w
+000005c0: 6974 6820 636f 6d62 696e 655f 7175 6572  ith combine_quer
+000005d0: 795f 646f 6375 6d65 6e74 7a07 5175 6572  y_documentz.Quer
+000005e0: 793a 207a 1243 6c65 616e 6564 2044 6f63  y: z.Cleaned Doc
+000005f0: 756d 656e 743a 207a 0841 6e73 7765 723a  ument: z.Answer:
+00000600: 2029 0ada 0272 65da 0373 7562 da07 7265   )...re..sub..re
+00000610: 706c 6163 65da 0573 7472 6970 da04 6a6f  place..strip..jo
+00000620: 696e da05 7370 6c69 74da 036c 656e da0a  in..split..len..
+00000630: 6272 6561 6b70 6f69 6e74 da05 7072 696e  breakpoint..prin
+00000640: 74da 0373 7472 2904 7215 0000 0072 1600  t..str).r....r..
+00000650: 0000 da06 616e 7377 6572 da10 636c 6561  ....answer..clea
+00000660: 6e65 645f 646f 6375 6d65 6e74 a900 722e  ned_document..r.
+00000670: 0000 00fa 532f 6675 7475 7265 2f75 2f6d  ....S/future/u/m
+00000680: 616e 6968 616e 692f 4152 4553 2f61 7265  anihani/ARES/are
+00000690: 732f 4c4c 4d5f 6173 5f61 5f4a 7564 6765  s/LLM_as_a_Judge
+000006a0: 5f41 6461 7074 6174 696f 6e2f 4765 6e65  _Adaptation/Gene
+000006b0: 7261 6c5f 4269 6e61 7279 5f43 6c61 7373  ral_Binary_Class
+000006c0: 6966 6965 722e 7079 da16 636f 6d62 696e  ifier.py..combin
+000006d0: 655f 7175 6572 795f 646f 6375 6d65 6e74  e_query_document
+000006e0: 2800 0000 7322 0000 0022 0114 0112 0118  (...s"..."......
+000006f0: 0112 0218 0108 020c 0102 0216 0106 0106  ................
+00000700: 0108 0110 0110 0110 0124 0172 3000 0000  .........$.r0...
+00000710: da08 7175 6573 7469 6f6e 6302 0000 0000  ..questionc.....
+00000720: 0000 0000 0000 0004 0000 0008 0000 0043  ...............C
+00000730: 0000 0073 a000 0000 6401 7d02 7c02 6402  ...s....d.}.|.d.
+00000740: 3700 7d02 7400 a001 6403 6404 7c01 a002  7.}.t...d.d.|...
+00000750: 6405 6406 a102 a002 6407 6406 a102 a103  d.d.....d.d.....
+00000760: a003 a100 7d03 7c03 a002 6408 6406 a102  ....}.|...d.d...
+00000770: a002 6409 6406 a102 7d03 7400 a001 640a  ..d.d...}.t...d.
+00000780: 6406 7c03 a103 a003 a100 7d03 6406 a004  d.|.......}.d...
+00000790: 7c03 a005 6406 a101 6400 640b 8502 1900  |...d...d.d.....
+000007a0: a101 7d03 7c02 640c 3700 7d02 7c02 640d  ..}.|.d.7.}.|.d.
+000007b0: 7c00 1700 6404 1700 3700 7d02 7c02 640e  |...d...7.}.|.d.
+000007c0: 7c03 1700 6404 1700 3700 7d02 7c02 640f  |...d...7.}.|.d.
+000007d0: 3700 7d02 7c02 5300 2910 4e7a 4359 6f75  7.}.|.S.).NzCYou
+000007e0: 2061 7265 2061 6e20 6578 7065 7274 206a   are an expert j
+000007f0: 7564 6765 2066 6f72 2065 7661 6c75 6174  udge for evaluat
+00000800: 696e 6720 7175 6573 7469 6f6e 2061 6e73  ing question ans
+00000810: 7765 7269 6e67 2073 7973 7465 6d73 2e20  wering systems. 
+00000820: 7a97 4769 7665 6e20 7468 6520 666f 6c6c  z.Given the foll
+00000830: 6f77 696e 6720 7175 6573 7469 6f6e 2061  owing question a
+00000840: 6e64 2064 6f63 756d 656e 742c 2079 6f75  nd document, you
+00000850: 206d 7573 7420 616e 616c 797a 6520 7468   must analyze th
+00000860: 6520 7072 6f76 6964 6564 2064 6f63 756d  e provided docum
+00000870: 656e 7420 616e 6420 6465 7465 726d 696e  ent and determin
+00000880: 6520 7768 6574 6865 7220 6974 2069 7320  e whether it is 
+00000890: 7375 6666 6963 6965 6e74 2066 6f72 2061  sufficient for a
+000008a0: 6e73 7765 7269 6e67 2074 6865 2071 7565  nswering the que
+000008b0: 7374 696f 6e2e 200a 0a72 1700 0000 7218  stion. ..r....r.
+000008c0: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
+000008d0: 0000 721c 0000 0072 1d00 0000 721e 0000  ..r....r....r...
+000008e0: 0072 1f00 0000 7a11 2323 2320 496e 7374  .r....z.### Inst
+000008f0: 7275 6374 696f 6e3a 0a7a 0a51 7565 7374  ruction:.z.Quest
+00000900: 696f 6e3a 207a 0a44 6f63 756d 656e 743a  ion: z.Document:
+00000910: 207a 0e23 2323 2052 6573 706f 6e73 653a   z.### Response:
+00000920: 0a29 0672 2200 0000 7223 0000 0072 2400  .).r"...r#...r$.
+00000930: 0000 7225 0000 0072 2600 0000 7227 0000  ..r%...r&...r'..
+00000940: 0029 0472 3100 0000 7216 0000 00da 0b69  .).r1...r......i
+00000950: 6e73 7472 7563 7469 6f6e 722d 0000 0072  nstructionr-...r
+00000960: 2e00 0000 722e 0000 0072 2f00 0000 da45  ....r....r/....E
+00000970: 666f 726d 6174 5f74 6578 745f 666f 725f  format_text_for_
+00000980: 6669 6e65 5f74 756e 696e 675f 636f 6e74  fine_tuning_cont
+00000990: 656e 745f 7265 6c65 7661 6e63 655f 7365  ent_relevance_se
+000009a0: 7175 656e 6365 5f63 6c61 7373 6966 6963  quence_classific
+000009b0: 6174 696f 6e3e 0000 0073 1600 0000 0401  ation>...s......
+000009c0: 0801 2202 1401 1201 1801 0802 1001 1001  ..".............
+000009d0: 0801 0402 7233 0000 00e9 2a00 0000 5a0e  ....r3....*...Z.
+000009e0: 5059 5448 4f4e 4841 5348 5345 4544 6300  PYTHONHASHSEEDc.
+000009f0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00000a00: 0000 0043 0000 0073 4400 0000 6401 7d00  ...C...sD...d.}.
+00000a10: 7400 a001 7c00 a002 a100 a101 a003 6402  t...|.........d.
+00000a20: a101 a002 6403 a101 6400 6404 8502 1900  ....d...d.d.....
+00000a30: 6405 6400 8502 1900 7d01 6406 6407 8400  d.d.....}.d.d...
+00000a40: 7404 7c01 8301 4400 8301 7d02 7c02 5300  t.|...D...}.|.S.
+00000a50: 2908 4e7a 2f6e 7669 6469 612d 736d 6920  ).Nz/nvidia-smi 
+00000a60: 2d2d 7175 6572 792d 6770 753d 6d65 6d6f  --query-gpu=memo
+00000a70: 7279 2e66 7265 6520 2d2d 666f 726d 6174  ry.free --format
+00000a80: 3d63 7376 da05 6173 6369 6972 1800 0000  =csv..asciir....
+00000a90: e9ff ffff ffe9 0100 0000 6301 0000 0000  ..........c.....
+00000aa0: 0000 0000 0000 0003 0000 0005 0000 0053  ...............S
+00000ab0: 0000 0073 2000 0000 6700 7c00 5d0c 5c02  ...s ...g.|.].\.
+00000ac0: 7d01 7d02 7400 7c02 a001 a100 6400 1900  }.}.t.|.....d...
+00000ad0: 8301 9102 7102 5300 2901 7201 0000 0029  ....q.S.).r....)
+00000ae0: 02da 0369 6e74 7227 0000 0029 03da 022e  ...intr'...)....
+00000af0: 30da 0169 da01 7872 2e00 0000 722e 0000  0..i..xr....r...
+00000b00: 0072 2f00 0000 da0a 3c6c 6973 7463 6f6d  .r/.....<listcom
+00000b10: 703e 5c00 0000 7302 0000 0020 007a 2267  p>\...s.... .z"g
+00000b20: 6574 5f67 7075 5f6d 656d 6f72 792e 3c6c  et_gpu_memory.<l
+00000b30: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000b40: 3e29 05da 0273 70da 0c63 6865 636b 5f6f  >)...sp..check_o
+00000b50: 7574 7075 7472 2700 0000 da06 6465 636f  utputr'.....deco
+00000b60: 6465 da09 656e 756d 6572 6174 6529 03da  de..enumerate)..
+00000b70: 0763 6f6d 6d61 6e64 5a10 6d65 6d6f 7279  .commandZ.memory
+00000b80: 5f66 7265 655f 696e 666f 5a12 6d65 6d6f  _free_infoZ.memo
+00000b90: 7279 5f66 7265 655f 7661 6c75 6573 722e  ry_free_valuesr.
+00000ba0: 0000 0072 2e00 0000 722f 0000 00da 0e67  ...r....r/.....g
+00000bb0: 6574 5f67 7075 5f6d 656d 6f72 7959 0000  et_gpu_memoryY..
+00000bc0: 0073 0800 0000 0401 2a01 1201 0401 7242  .s......*.....rB
+00000bd0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000be0: 0000 0000 0300 0000 0000 0000 7326 0000  ............s&..
+00000bf0: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
+00000c00: 0284 085a 0364 0664 0464 0584 015a 0487  ...Z.d.d.d...Z..
+00000c10: 0004 005a 0553 0029 07da 0f43 7573 746f  ...Z.S.)...Custo
+00000c20: 6d42 4552 544d 6f64 656c 6303 0000 0000  mBERTModelc.....
+00000c30: 0000 0000 0000 0006 0000 0007 0000 0003  ................
+00000c40: 0000 0073 1601 0000 7c02 7c00 5f00 7401  ...s....|.|._.t.
+00000c50: 7402 7c00 8302 a003 a100 0100 7c02 6401  t.|.........|.d.
+00000c60: 7600 722f 7404 6a05 7c02 6402 6403 8d02  v.r/t.j.|.d.d...
+00000c70: 7d03 6404 7c03 6a06 6405 3c00 7407 7c03  }.d.|.j.d.<.t.|.
+00000c80: 5f08 7409 6a05 7c02 7c03 740a 6a0b 6402  _.t.j.|.|.t.j.d.
+00000c90: 6402 6406 8d05 7d04 6407 7d05 7c04 6a0c  d.d...}.d.}.|.j.
+00000ca0: 7c00 5f0d 6e48 7c02 6408 7600 7240 740e  |._.nH|.d.v.r@t.
+00000cb0: 6a05 6409 6402 6403 8d02 7d04 640a 7d05  j.d.d.d...}.d.}.
+00000cc0: 7c04 7c00 5f0d 6e37 7c02 640b 7600 724f  |.|._.n7|.d.v.rO
+00000cd0: 740f a005 7c02 a101 7d04 640c 7d05 7c04  t...|...}.d.}.|.
+00000ce0: 7c00 5f0d 6e28 7c02 640d 7600 725e 7410  |._.n(|.d.v.r^t.
+00000cf0: a005 7c02 a101 7d04 640c 7d05 7c04 7c00  ..|...}.d.}.|.|.
+00000d00: 5f0d 6e19 7c02 640e 7600 726d 7410 a005  _.n.|.d.v.rmt...
+00000d10: 7c02 a101 7d04 640f 7d05 7c04 7c00 5f0d  |...}.d.}.|.|._.
+00000d20: 6e0a 7410 a005 7c02 a101 7d04 6410 7d05  n.t...|...}.d.}.
+00000d30: 7c04 7c00 5f0d 7411 a012 7411 a013 7c05  |.|._.t...t...|.
+00000d40: 6411 a102 7411 a013 6411 7c01 a102 a102  d...t...d.|.....
+00000d50: 7c00 5f14 7c05 7c00 5f15 6400 5300 2912  |._.|.|._.d.S.).
+00000d60: 4e29 027a 186d 6f73 6169 636d 6c2f 6d70  N).z.mosaicml/mp
+00000d70: 742d 3762 2d69 6e73 7472 7563 747a 0f6d  t-7b-instructz.m
+00000d80: 6f73 6169 636d 6c2f 6d70 742d 3762 5429  osaicml/mpt-7bT)
+00000d90: 01da 1174 7275 7374 5f72 656d 6f74 655f  ...trust_remote_
+00000da0: 636f 6465 5a06 7472 6974 6f6e 5a09 6174  codeZ.tritonZ.at
+00000db0: 746e 5f69 6d70 6c29 04da 0663 6f6e 6669  tn_impl)...confi
+00000dc0: 67da 0b74 6f72 6368 5f64 7479 7065 7244  g..torch_dtyperD
+00000dd0: 0000 00da 0e75 7365 5f61 7574 685f 746f  .....use_auth_to
+00000de0: 6b65 6e69 0010 0000 a901 fa1e 6d6f 7361  keni........mosa
+00000df0: 6963 6d6c 2f6d 7074 2d31 622d 7265 6470  icml/mpt-1b-redp
+00000e00: 616a 616d 612d 3230 3062 7249 0000 00e9  ajama-200brI....
+00000e10: 0008 0000 2902 fa18 676f 6f67 6c65 2f74  ....)...google/t
+00000e20: 352d 6c61 7267 652d 6c6d 2d61 6461 7074  5-large-lm-adapt
+00000e30: fa15 676f 6f67 6c65 2f74 352d 786c 2d6c  ..google/t5-xl-l
+00000e40: 6d2d 6164 6170 7469 0004 0000 2902 7a0d  m-adapti....).z.
+00000e50: 726f 6265 7274 612d 6c61 7267 657a 1a6d  roberta-largez.m
+00000e60: 6963 726f 736f 6674 2f64 6562 6572 7461  icrosoft/deberta
+00000e70: 2d76 332d 6c61 7267 6529 027a 1b6d 6963  -v3-large).z.mic
+00000e80: 726f 736f 6674 2f64 6562 6572 7461 2d76  rosoft/deberta-v
+00000e90: 322d 786c 6172 6765 7a1c 6d69 6372 6f73  2-xlargez.micros
+00000ea0: 6f66 742f 6465 6265 7274 612d 7632 2d78  oft/deberta-v2-x
+00000eb0: 786c 6172 6765 6900 0600 0069 0003 0000  xlargei....i....
+00000ec0: e900 0100 0029 16da 0c6d 6f64 656c 5f63  .....)...model_c
+00000ed0: 686f 6963 65da 0573 7570 6572 7243 0000  hoice..superrC..
+00000ee0: 00da 085f 5f69 6e69 745f 5f72 1000 0000  ...__init__r....
+00000ef0: da0f 6672 6f6d 5f70 7265 7472 6169 6e65  ..from_pretraine
+00000f00: 645a 0b61 7474 6e5f 636f 6e66 6967 da10  dZ.attn_config..
+00000f10: 6d61 785f 746f 6b65 6e5f 6c65 6e67 7468  max_token_length
+00000f20: 5a0b 6d61 785f 7365 715f 6c65 6e72 0f00  Z.max_seq_lenr..
+00000f30: 0000 da05 746f 7263 68da 0862 666c 6f61  ....torch..bfloa
+00000f40: 7431 36da 0b74 7261 6e73 666f 726d 6572  t16..transformer
+00000f50: da0c 656e 636f 6465 724d 6f64 656c da1c  ..encoderModel..
+00000f60: 4d70 7446 6f72 5365 7175 656e 6365 436c  MptForSequenceCl
+00000f70: 6173 7369 6669 6361 7469 6f6e 7211 0000  assificationr...
+00000f80: 0072 0700 0000 da02 6e6e da0a 5365 7175  .r......nn..Sequ
+00000f90: 656e 7469 616c da06 4c69 6e65 6172 da0a  ential..Linear..
+00000fa0: 636c 6173 7369 6669 6572 da0e 656d 6265  classifier..embe
+00000fb0: 6464 696e 675f 7369 7a65 2906 da04 7365  dding_size)...se
+00000fc0: 6c66 da10 6e75 6d62 6572 5f6f 665f 6c61  lf..number_of_la
+00000fd0: 6265 6c73 724e 0000 0072 4500 0000 5a0e  belsrN...rE...Z.
+00000fe0: 6d6f 6465 6c5f 656e 636f 6469 6e67 725c  model_encodingr\
+00000ff0: 0000 00a9 01da 095f 5f63 6c61 7373 5f5f  .......__class__
+00001000: 722e 0000 0072 2f00 0000 7250 0000 0062  r....r/...rP...b
+00001010: 0000 0073 4800 0000 0601 0e01 0801 0e02  ...sH...........
+00001020: 0a01 0601 0402 0201 0201 0402 0201 0201  ................
+00001030: 06fa 0408 0a01 0802 0e04 0401 0801 0802  ................
+00001040: 0a02 0401 0801 0802 0a02 0401 0801 0802  ................
+00001050: 0a02 0401 0801 0a04 0401 0601 1e04 0a01  ................
+00001060: 7a18 4375 7374 6f6d 4245 5254 4d6f 6465  z.CustomBERTMode
+00001070: 6c2e 5f5f 696e 6974 5f5f 4e63 0500 0000  l.__init__Nc....
+00001080: 0000 0000 0000 0000 0a00 0000 0500 0000  ................
+00001090: 4300 0000 7368 0000 007c 006a 007d 057c  C...sh...|.j.}.|
+000010a0: 0564 0176 0072 127c 006a 017c 017c 0264  .d.v.r.|.j.|.|.d
+000010b0: 028d 027d 067c 0664 0319 0053 007c 006a  ...}.|.d...S.|.j
+000010c0: 017c 017c 0264 048d 027d 067c 0664 0519  .|.|.d...}.|.d..
+000010d0: 007d 077c 0764 0064 0085 0264 0664 0064  .}.|.d.d...d.d.d
+000010e0: 0085 0266 0319 00a0 0264 077c 006a 03a1  ...f.....d.|.j..
+000010f0: 027d 087c 00a0 047c 08a1 017d 097c 0953  .}.|...|...}.|.S
+00001100: 0029 084e 2904 fa08 7435 2d73 6d61 6c6c  .).N)...t5-small
+00001110: 724c 0000 0072 4b00 0000 7249 0000 0029  rL...rK...rI...)
+00001120: 02da 0969 6e70 7574 5f69 6473 da0e 6174  ...input_ids..at
+00001130: 7465 6e74 696f 6e5f 6d61 736b da06 6c6f  tention_mask..lo
+00001140: 6769 7473 2901 7263 0000 005a 116c 6173  gits).rc...Z.las
+00001150: 745f 6869 6464 656e 5f73 7461 7465 7201  t_hidden_stater.
+00001160: 0000 0072 3600 0000 2905 724e 0000 0072  ...r6...).rN...r
+00001170: 5600 0000 da04 7669 6577 725c 0000 0072  V.....viewr\...r
+00001180: 5b00 0000 290a 725d 0000 00da 0369 6473  [...).r].....ids
+00001190: da04 6d61 736b da06 6c61 6265 6c73 da11  ..mask..labels..
+000011a0: 6465 636f 6465 725f 696e 7075 745f 6964  decoder_input_id
+000011b0: 7372 4e00 0000 5a0c 746f 7461 6c5f 6f75  srN...Z.total_ou
+000011c0: 7470 7574 5a0f 7365 7175 656e 6365 5f6f  tputZ.sequence_o
+000011d0: 7574 7075 745a 1b6c 6173 745f 6869 6464  utputZ.last_hidd
+000011e0: 656e 5f73 7461 7465 5f66 6f72 6d61 7474  en_state_formatt
+000011f0: 6564 5a0e 6c69 6e65 6172 325f 6f75 7470  edZ.linear2_outp
+00001200: 7574 722e 0000 0072 2e00 0000 722f 0000  utr....r....r/..
+00001210: 00da 0766 6f72 7761 7264 9d00 0000 7312  ...forward....s.
+00001220: 0000 0006 0108 010e 0108 010e 0208 0120  ............... 
+00001230: 020a 0104 027a 1743 7573 746f 6d42 4552  .....z.CustomBER
+00001240: 544d 6f64 656c 2e66 6f72 7761 7264 2902  TModel.forward).
+00001250: 4e4e 2906 da08 5f5f 6e61 6d65 5f5f da0a  NN)...__name__..
+00001260: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00001270: 616c 6e61 6d65 5f5f 7250 0000 0072 6a00  alname__rP...rj.
+00001280: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
+00001290: 5f72 2e00 0000 722e 0000 0072 5f00 0000  _r....r....r_...
+000012a0: 722f 0000 0072 4300 0000 6100 0000 7306  r/...rC...a...s.
+000012b0: 0000 0008 000c 0112 3b72 4300 0000 6302  ........;rC...c.
+000012c0: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+000012d0: 0000 0043 0000 0073 1200 0000 7c00 7c01  ...C...s....|.|.
+000012e0: 6401 1900 6402 6403 6404 8d03 5300 2905  d...d.d.d...S.).
+000012f0: 4eda 0474 6578 74da 0a6d 6178 5f6c 656e  N..text..max_len
+00001300: 6774 6854 2902 da07 7061 6464 696e 67da  gthT)...padding.
+00001310: 0a74 7275 6e63 6174 696f 6e72 2e00 0000  .truncationr....
+00001320: 2902 da09 746f 6b65 6e69 7a65 72da 0865  )...tokenizer..e
+00001330: 7861 6d70 6c65 7372 2e00 0000 722e 0000  xamplesr....r...
+00001340: 0072 2f00 0000 da11 746f 6b65 6e69 7a65  .r/.....tokenize
+00001350: 5f66 756e 6374 696f 6ead 0000 0073 0200  _function....s..
+00001360: 0000 1201 7275 0000 0063 0200 0000 0000  ....ru...c......
+00001370: 0000 0000 0000 0500 0000 0a00 0000 4300  ..............C.
+00001380: 0000 73b2 0000 0064 017d 0274 006a 01a0  ..s....d.}.t.j..
+00001390: 027c 02a1 0173 0d74 00a0 037c 02a1 0101  .|...s.t...|....
+000013a0: 0064 017c 01a0 0464 0264 03a1 0217 007d  .d.|...d.d.....}
+000013b0: 0374 006a 01a0 027c 03a1 0173 2674 0564  .t.j...|...s&t.d
+000013c0: 047c 0317 0083 0101 0074 00a0 037c 03a1  .|.......t...|..
+000013d0: 0101 0074 0644 005d 2e7d 047a 1374 00a0  ...t.D.].}.z.t..
+000013e0: 037c 0364 0217 007c 04a0 0464 0564 06a1  .|.d...|...d.d..
+000013f0: 02a0 0464 0264 03a1 0217 00a1 0101 0057  ...d.d.........W
+00001400: 0071 2801 0001 0001 0074 0564 0783 0101  .q(......t.d....
+00001410: 0074 057c 0364 0217 007c 04a0 0464 0564  .t.|.d...|...d.d
+00001420: 06a1 02a0 0464 0264 03a1 0217 0083 0101  .....d.d........
+00001430: 0059 0071 2864 0053 0029 084e fa0c 6368  .Y.q(d.S.).N..ch
+00001440: 6563 6b70 6f69 6e74 732f fa01 2f72 1d00  eckpoints/../r..
+00001450: 0000 7a11 4372 6561 7469 6e67 2066 6f6c  ..z.Creating fol
+00001460: 6465 723a 207a 032e 2e2f da00 7a0e 416c  der: z.../..z.Al
+00001470: 7265 6164 7920 6578 6973 7473 2907 da02  ready exists)...
+00001480: 6f73 da04 7061 7468 da05 6973 6469 72da  os..path..isdir.
+00001490: 056d 6b64 6972 7224 0000 0072 2a00 0000  .mkdirr$...r*...
+000014a0: da17 636c 6173 7369 6669 6361 7469 6f6e  ..classification
+000014b0: 5f64 6174 6173 6574 7329 05da 1663 6c61  _datasets)...cla
+000014c0: 7373 6966 6963 6174 696f 6e5f 6461 7461  ssification_data
+000014d0: 7365 7472 4e00 0000 5a17 6368 6563 6b70  setrN...Z.checkp
+000014e0: 6f69 6e74 735f 666f 6c64 6572 5f70 6174  oints_folder_pat
+000014f0: 685a 1364 6174 6173 6574 5f66 6f6c 6465  hZ.dataset_folde
+00001500: 725f 7061 7468 da07 6461 7461 7365 7472  r_path..datasetr
+00001510: 2e00 0000 722e 0000 0072 2f00 0000 da0b  ....r....r/.....
+00001520: 6368 6563 6b70 6f69 6e74 73b2 0000 0073  checkpoints....s
+00001530: 1c00 0000 0401 0c01 0a01 1002 0c01 0c01  ................
+00001540: 0a01 0802 0201 2601 0601 0801 2401 04fb  ......&.....$...
+00001550: 7280 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00001560: 0000 0300 0000 0400 0000 4300 0000 731a  ..........C...s.
+00001570: 0000 0064 017d 0174 006a 017c 007c 0164  ...d.}.t.j.|.|.d
+00001580: 028d 027d 027c 027c 0166 0253 0029 034e  ...}.|.|.f.S.).N
+00001590: 724a 0000 0029 01da 106d 6f64 656c 5f6d  rJ...)...model_m
+000015a0: 6178 5f6c 656e 6774 6829 0272 0600 0000  ax_length).r....
+000015b0: 7251 0000 0029 0372 4e00 0000 7252 0000  rQ...).rN...rR..
+000015c0: 0072 7300 0000 722e 0000 0072 2e00 0000  .rs...r....r....
+000015d0: 722f 0000 00da 0a6c 6f61 645f 6d6f 6465  r/.....load_mode
+000015e0: 6cc5 0000 0073 0600 0000 0401 0e01 0802  l....s..........
+000015f0: 7282 0000 0063 0e00 0000 0000 0000 0000  r....c..........
+00001600: 0000 1200 0000 0600 0000 4300 0000 7322  ..........C...s"
+00001610: 0100 0074 0064 0183 0101 0074 0064 0274  ...t.d.....t.d.t
+00001620: 017c 0283 0117 0083 0101 0074 0064 0183  .|.........t.d..
+00001630: 0101 0064 0364 006c 027d 0e7c 0e6a 02a0  ...d.d.l.}.|.j..
+00001640: 03a1 00a0 0464 04a1 017d 0f64 057c 03a0  .....d...}.d.|..
+00001650: 0564 0664 07a1 0217 0064 0617 007c 0617  .d.d.....d...|..
+00001660: 0064 0817 0074 017c 07a0 0664 06a1 0164  .d...t.|...d...d
+00001670: 0919 00a0 0564 0a64 0ba1 0283 0117 0064  .....d.d.......d
+00001680: 0817 007c 0f17 0064 0c17 007d 1074 07a0  ...|...d...}.t..
+00001690: 07a1 007d 1174 0064 0d7c 0017 0083 0101  ...}.t.d.|......
+000016a0: 0074 0064 0e7c 0317 0083 0101 0074 0064  .t.d.|.......t.d
+000016b0: 0f7c 0717 0083 0101 0074 0064 1074 017c  .|.......t.d.t.|
+000016c0: 0483 0117 0083 0101 0074 0064 1174 017c  .........t.d.t.|
+000016d0: 0283 0117 0083 0101 0074 0064 127c 1017  .........t.d.|..
+000016e0: 0083 0101 0074 0064 1374 017c 0883 0117  .....t.d.t.|....
+000016f0: 0083 0101 0074 0064 1474 017c 0583 0117  .....t.d.t.|....
+00001700: 0083 0101 0074 0064 1574 017c 0983 0117  .....t.d.t.|....
+00001710: 0083 0101 0074 0064 1674 017c 0a83 0117  .....t.d.t.|....
+00001720: 0083 0101 0074 0064 0183 0101 007c 107c  .....t.d.....|.|
+00001730: 0866 0253 0029 174e 7a4a 2d2d 2d2d 2d2d  .f.S.).NzJ------
+00001740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001780: 2d2d 2d2d 7a1c 5374 6172 7469 6e67 206e  ----z.Starting n
+00001790: 6577 206c 6561 726e 696e 6720 7261 7465  ew learning rate
+000017a0: 3a20 7201 0000 007a 1125 592d 256d 2d25  : r....z.%Y-%m-%
+000017b0: 645f 2548 3a25 4d3a 2553 7276 0000 0072  d_%H:%M:%Srv...r
+000017c0: 7700 0000 721d 0000 00da 015f 7236 0000  w...r......_r6..
+000017d0: 007a 042e 7473 7672 7800 0000 7a03 2e70  .z..tsvrx...z..p
+000017e0: 747a 0944 6174 6173 6574 3a20 7a07 4d6f  tz.Dataset: z.Mo
+000017f0: 6465 6c3a 207a 1454 6573 7420 5365 7420  del: z.Test Set 
+00001800: 5365 6c65 6374 696f 6e3a 207a 104e 756d  Selection: z.Num
+00001810: 6265 7220 6f66 2052 756e 733a 207a 0f4c  ber of Runs: z.L
+00001820: 6561 726e 696e 6720 5261 7465 3a20 fa11  earning Rate: ..
+00001830: 4368 6563 6b70 6f69 6e74 2050 6174 683a  Checkpoint Path:
+00001840: 207a 0a50 6174 6965 6e63 653a 207a 1756   z.Patience: z.V
+00001850: 616c 6964 6174 696f 6e20 5365 7420 4368  alidation Set Ch
+00001860: 6f69 6365 3a20 7a12 4e75 6d62 6572 206f  oice: z.Number o
+00001870: 6620 4570 6f63 6873 3a20 7a18 4e75 6d62  f Epochs: z.Numb
+00001880: 6572 206f 6620 7761 726d 7570 2073 7465  er of warmup ste
+00001890: 7073 3a20 2908 722a 0000 0072 2b00 0000  ps: ).r*...r+...
+000018a0: da08 6461 7465 7469 6d65 da03 6e6f 77da  ..datetime..now.
+000018b0: 0873 7472 6674 696d 6572 2400 0000 7227  .strftimer$...r'
+000018c0: 0000 00da 0474 696d 6529 1272 7f00 0000  .....time).r....
+000018d0: da15 6c65 6172 6e69 6e67 5f72 6174 655f  ..learning_rate_
+000018e0: 6368 6f69 6365 73da 1463 686f 7365 6e5f  choices..chosen_
+000018f0: 6c65 6172 6e69 6e67 5f72 6174 6572 4e00  learning_raterN.
+00001900: 0000 da0e 6e75 6d62 6572 5f6f 665f 7275  ....number_of_ru
+00001910: 6e73 da16 7661 6c69 6461 7469 6f6e 5f73  ns..validation_s
+00001920: 6574 5f73 636f 7269 6e67 da0c 6c61 6265  et_scoring..labe
+00001930: 6c5f 636f 6c75 6d6e da0e 7661 6c69 6461  l_column..valida
+00001940: 7469 6f6e 5f73 6574 da0e 7061 7469 656e  tion_set..patien
+00001950: 6365 5f76 616c 7565 da0a 6e75 6d5f 6570  ce_value..num_ep
+00001960: 6f63 6873 da10 6e75 6d5f 7761 726d 7570  ochs..num_warmup
+00001970: 5f73 7465 7073 da20 6772 6164 6965 6e74  _steps. gradient
+00001980: 5f61 6363 756d 756c 6174 696f 6e5f 6d75  _accumulation_mu
+00001990: 6c74 6970 6c69 6572 da13 6173 7369 676e  ltiplier..assign
+000019a0: 6564 5f62 6174 6368 5f73 697a 6572 7300  ed_batch_sizers.
+000019b0: 0000 7285 0000 005a 1063 7572 7265 6e74  ..r....Z.current
+000019c0: 5f64 6174 6574 696d 65da 0f63 6865 636b  _datetime..check
+000019d0: 706f 696e 745f 7061 7468 5a0f 6578 6563  point_pathZ.exec
+000019e0: 7574 696f 6e5f 7374 6172 7472 2e00 0000  ution_startr....
+000019f0: 722e 0000 0072 2f00 0000 da16 7072 6570  r....r/.....prep
+00001a00: 6172 655f 616e 645f 636c 6561 6e5f 6461  are_and_clean_da
+00001a10: 7461 cd00 0000 7326 0000 0008 0610 0108  ta....s&........
+00001a20: 0108 0210 0242 0208 080c 020c 010c 0110  .....B..........
+00001a30: 0110 010c 0110 0110 0110 0110 0108 0108  ................
+00001a40: 0272 9500 0000 6304 0000 0000 0000 0000  .r....c.........
+00001a50: 0000 0004 0000 0005 0000 0003 0000 0073  ...............s
+00001a60: 2401 0000 7400 6a01 7c00 6401 6402 8d02  $...t.j.|.d.d...
+00001a70: 8900 6403 7c00 7600 721d 8800 6404 1900  ..d.|.v.r...d...
+00001a80: 8800 6405 3c00 8800 6406 1900 8800 6407  ..d.<...d.....d.
+00001a90: 3c00 8800 6408 1900 8800 6409 3c00 8800  <...d.....d.<...
+00001aa0: 8800 7c01 1900 640a 6b03 1900 8900 8800  ..|...d.k.......
+00001ab0: 8800 6405 1900 a002 a100 1900 8900 8800  ..d.............
+00001ac0: 8800 6409 1900 a002 a100 1900 8900 8800  ..d.............
+00001ad0: 8800 6407 1900 a002 a100 1900 8900 8800  ..d.............
+00001ae0: 8800 7c01 1900 a002 a100 1900 8900 8800  ..|.............
+00001af0: 6a03 7404 8800 8301 640b 640c 8d02 8900  j.t.....d.d.....
+00001b00: 640d 7c01 7600 7262 8700 6601 640e 640f  d.|.v.rb..f.d.d.
+00001b10: 8408 7405 7404 8800 8301 8301 4400 8301  ..t.t.......D...
+00001b20: 8800 6410 3c00 6e0f 8700 6601 6411 640f  ..d.<.n...f.d.d.
+00001b30: 8408 7405 7404 8800 8301 8301 4400 8301  ..t.t.......D...
+00001b40: 8800 6410 3c00 8701 6601 6412 640f 8408  ..d.<...f.d.d...
+00001b50: 7406 8800 6410 1900 6413 6414 8d02 4400  t...d...d.d...D.
+00001b60: 8301 8800 6415 3c00 8800 a007 6410 6701  ....d.<.....d.g.
+00001b70: a101 8900 8800 8800 6415 1900 6416 6b01  ........d...d.k.
+00001b80: 1900 8900 8800 5300 2917 4e72 1b00 0000  ......S.).Nr....
+00001b90: a901 da03 7365 70da 0e6e 715f 7265 666f  ....sep..nq_refo
+00001ba0: 726d 6174 7465 64da 0551 7565 7279 da0f  rmatted..Query..
+00001bb0: 7379 6e74 6865 7469 635f 7175 6572 79da  synthetic_query.
+00001bc0: 0641 6e73 7765 72da 1067 656e 6572 6174  .Answer..generat
+00001bd0: 6564 5f61 6e73 7765 72da 0844 6f63 756d  ed_answer..Docum
+00001be0: 656e 7472 1600 0000 da03 4e61 4e72 3400  entr......NaNr4.
+00001bf0: 0000 2902 da01 6eda 0c72 616e 646f 6d5f  ..)...n..random_
+00001c00: 7374 6174 65da 0743 6f6e 7465 7874 6301  state..Contextc.
+00001c10: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00001c20: 0000 0013 0000 00f3 2a00 0000 6700 7c00  ........*...g.|.
+00001c30: 5d11 7d01 7400 8800 6a01 7c01 1900 6400  ].}.t...j.|...d.
+00001c40: 1900 8800 6a01 7c01 1900 6401 1900 8302  ....j.|...d.....
+00001c50: 9102 7102 5300 2902 729a 0000 0072 1600  ..q.S.).r....r..
+00001c60: 0000 a902 7230 0000 00da 0469 6c6f 63a9  ....r0.....iloc.
+00001c70: 0272 3900 0000 723a 0000 00a9 01da 0d73  .r9...r:.......s
+00001c80: 796e 7468 5f71 7565 7269 6573 722e 0000  ynth_queriesr...
+00001c90: 0072 2f00 0000 723c 0000 0013 0100 00f3  .r/...r<........
+00001ca0: 0200 0000 2a00 7a2b 616e 616c 797a 655f  ....*.z+analyze_
+00001cb0: 616e 645f 7265 706f 7274 5f64 6174 612e  and_report_data.
+00001cc0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00001cd0: 6d70 3eda 0b63 6f6e 6361 745f 7465 7874  mp>..concat_text
+00001ce0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001cf0: 0007 0000 0013 0000 00f3 3600 0000 6700  ..........6...g.
+00001d00: 7c00 5d17 7d01 7400 8800 6a01 7c01 1900  |.].}.t...j.|...
+00001d10: 6400 1900 8800 6a01 7c01 1900 6401 1900  d.....j.|...d...
+00001d20: 8800 6a01 7c01 1900 6402 1900 8303 9102  ..j.|...d.......
+00001d30: 7102 5300 2903 729a 0000 0072 1600 0000  q.S.).r....r....
+00001d40: 729c 0000 0072 a300 0000 72a5 0000 0072  r....r....r....r
+00001d50: a600 0000 722e 0000 0072 2f00 0000 723c  ....r....r/...r<
+00001d60: 0000 0015 0100 00f3 0200 0000 3600 6301  ............6.c.
+00001d70: 0000 0000 0000 0000 0000 0002 0000 0007  ................
+00001d80: 0000 0013 0000 0073 2200 0000 6700 7c00  .......s"...g.|.
+00001d90: 5d0d 7d01 7400 8800 6a01 7c01 6400 6401  ].}.t...j.|.d.d.
+00001da0: 8d02 6402 1900 8301 9102 7102 5300 2903  ..d.......q.S.).
+00001db0: da02 7074 2901 da0e 7265 7475 726e 5f74  ..pt)...return_t
+00001dc0: 656e 736f 7273 7201 0000 0029 0272 2800  ensorsr....).r(.
+00001dd0: 0000 da06 656e 636f 6465 2902 7239 0000  ....encode).r9..
+00001de0: 0072 6f00 0000 a901 7273 0000 0072 2e00  .ro.....rs...r..
+00001df0: 0000 722f 0000 0072 3c00 0000 1601 0000  ..r/...r<.......
+00001e00: 7302 0000 0022 005a 0a54 6f6b 656e 697a  s....".Z.Tokeniz
+00001e10: 696e 6729 01da 0464 6573 635a 0c74 6f6b  ing)...descZ.tok
+00001e20: 656e 5f6c 656e 6774 6872 4a00 0000 2908  en_lengthrJ...).
+00001e30: da02 7064 da08 7265 6164 5f63 7376 da05  ..pd..read_csv..
+00001e40: 6e6f 746e 61da 0673 616d 706c 6572 2800  notna..sampler(.
+00001e50: 0000 da05 7261 6e67 6572 1200 0000 da0f  ....ranger......
+00001e60: 6472 6f70 5f64 7570 6c69 6361 7465 7329  drop_duplicates)
+00001e70: 0472 7f00 0000 728d 0000 0072 7300 0000  .r....r....rs...
+00001e80: 7252 0000 0072 2e00 0000 2902 72a7 0000  rR...r....).r...
+00001e90: 0072 7300 0000 722f 0000 00da 1761 6e61  .rs...r/.....ana
+00001ea0: 6c79 7a65 5f61 6e64 5f72 6570 6f72 745f  lyze_and_report_
+00001eb0: 6461 7461 f500 0000 7324 0000 000e 0208  data....s$......
+00001ec0: 020c 010c 010c 0110 0710 0110 0110 0110  ................
+00001ed0: 0112 0108 0a20 011e 0222 010c 0110 0704  ..... ..."......
+00001ee0: 0272 b700 0000 6303 0000 0000 0000 0000  .r....c.........
+00001ef0: 0000 0005 0000 0006 0000 0003 0000 0073  ...............s
+00001f00: 6001 0000 7c00 7d03 7400 6a01 7c01 6401  `...|.}.t.j.|.d.
+00001f10: 6402 8d02 8900 8800 6403 1900 8800 6404  d.......d.....d.
+00001f20: 3c00 8800 6405 1900 6a02 a003 a100 8800  <...d...j.......
+00001f30: 6405 3c00 8800 8800 6405 1900 6a02 a004  d.<.....d...j...
+00001f40: a100 6406 6b04 1900 8900 8800 8800 7c02  ..d.k.........|.
+00001f50: 1900 a005 a100 1900 8900 7c03 6407 1900  ..........|.d...
+00001f60: a006 7402 a101 6a02 a003 a100 7c03 6407  ..t...j.....|.d.
+00001f70: 3c00 7c03 7c03 6407 1900 6a02 a004 a100  <.|.|.d...j.....
+00001f80: 6406 6b04 1900 7d03 7c03 7c03 7c02 1900  d.k...}.|.|.|...
+00001f90: a005 a100 1900 7d03 6408 7c02 7600 725e  ......}.d.|.v.r^
+00001fa0: 8700 6601 6409 640a 8408 7407 7404 8800  ..f.d.d...t.t...
+00001fb0: 8301 8301 4400 8301 8800 640b 3c00 6e0f  ....D.....d.<.n.
+00001fc0: 8700 6601 640c 640a 8408 7407 7404 8800  ..f.d.d...t.t...
+00001fd0: 8301 8301 4400 8301 8800 640b 3c00 7c03  ....D.....d.<.|.
+00001fe0: a008 640b 6701 a101 7d03 8800 a008 640b  ..d.g...}.....d.
+00001ff0: 6701 a101 8900 640d 7c02 7600 72ac 7409  g.....d.|.v.r.t.
+00002000: 640e 8301 0100 7c03 7c03 640f 1900 a005  d.....|.|.d.....
+00002010: a100 1900 7d03 7c03 7c03 6410 1900 a005  ....}.|.|.d.....
+00002020: a100 1900 7d03 6700 6411 a201 7d04 7c03  ....}.g.d...}.|.
+00002030: 6412 1900 a006 7402 a101 7c03 6412 3c00  d.....t...|.d.<.
+00002040: 7c03 7c03 6412 1900 6a02 a00a 6413 a00b  |.|.d...j...d...
+00002050: 7c04 a101 a101 0f00 1900 7d03 7c03 8800  |.........}.|...
+00002060: 6602 5300 2914 4e72 1b00 0000 7296 0000  f.S.).Nr....r...
+00002070: 0072 9900 0000 da08 5175 6573 7469 6f6e  .r......Question
+00002080: 729d 0000 0072 2000 0000 7216 0000 0072  r....r ...r....r
+00002090: a100 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000020a0: 0002 0000 0006 0000 0013 0000 0072 a200  .............r..
+000020b0: 0000 2902 72b8 0000 0072 9d00 0000 72a3  ..).r....r....r.
+000020c0: 0000 0072 a500 0000 a901 da08 7465 7374  ...r........test
+000020d0: 5f73 6574 722e 0000 0072 2f00 0000 723c  _setr....r/...r<
+000020e0: 0000 0033 0100 0072 a800 0000 7a22 7472  ...3...r....z"tr
+000020f0: 616e 7366 6f72 6d5f 6461 7461 2e3c 6c6f  ansform_data.<lo
+00002100: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00002110: 72a9 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00002120: 0000 0200 0000 0700 0000 1300 0000 72aa  ..............r.
+00002130: 0000 0029 0372 b800 0000 729d 0000 0072  ...).r....r....r
+00002140: 9b00 0000 72a3 0000 0072 a500 0000 72b9  ....r....r....r.
+00002150: 0000 0072 2e00 0000 722f 0000 0072 3c00  ...r....r/...r<.
+00002160: 0000 3501 0000 72ab 0000 005a 0546 6169  ..5...r....Z.Fai
+00002170: 7468 7a35 5265 6669 6e69 6e67 2064 6174  thz5Refining dat
+00002180: 6120 666f 7220 416e 7377 6572 5f46 6169  a for Answer_Fai
+00002190: 7468 6675 6c6e 6573 7320 636c 6173 7369  thfulness classi
+000021a0: 6669 6361 7469 6f6e 21da 1743 6f6e 7465  fication!..Conte
+000021b0: 7874 5f52 656c 6576 616e 6365 5f4c 6162  xt_Relevance_Lab
+000021c0: 656c da19 416e 7377 6572 5f46 6169 7468  el..Answer_Faith
+000021d0: 6675 6c6e 6573 735f 4c61 6265 6c29 0a72  fulness_Label).r
+000021e0: 2c00 0000 5a07 636f 6e74 7261 64da 0566  ,...Z.contrad..f
+000021f0: 616c 7365 da0b 696e 666f 726d 6174 696f  alse..informatio
+00002200: 6e5a 0875 6e61 6e73 7765 7272 9b00 0000  nZ.unanswerr....
+00002210: 5a07 436f 6e74 7261 64da 0546 616c 7365  Z.Contrad..False
+00002220: 5a0b 496e 666f 726d 6174 696f 6e5a 0855  Z.InformationZ.U
+00002230: 6e61 6e73 7765 7272 9c00 0000 da01 7c29  nanswerr......|)
+00002240: 0c72 b100 0000 72b2 0000 0072 2b00 0000  .r....r....r+...
+00002250: 7225 0000 0072 2800 0000 72b3 0000 00da  r%...r(...r.....
+00002260: 0661 7374 7970 6572 b500 0000 72b6 0000  .astyper....r...
+00002270: 0072 2a00 0000 da08 636f 6e74 6169 6e73  .r*.....contains
+00002280: 7226 0000 0029 0572 a700 0000 728e 0000  r&...).r....r...
+00002290: 0072 8d00 0000 da08 7472 6169 6e5f 6466  .r......train_df
+000022a0: 5a0d 6572 726f 725f 7374 7269 6e67 7372  Z.error_stringsr
+000022b0: 2e00 0000 72b9 0000 0072 2f00 0000 da0e  ....r....r/.....
+000022c0: 7472 616e 7366 6f72 6d5f 6461 7461 2401  transform_data$.
+000022d0: 0000 732c 0000 0004 020e 020c 0112 0116  ..s,............
+000022e0: 0110 0118 0216 0110 0108 0220 011e 020c  ........... ....
+000022f0: 020c 0108 0208 0110 0110 0108 0112 011c  ................
+00002300: 0108 0272 c400 0000 6304 0000 0000 0000  ...r....c.......
+00002310: 0000 0000 000b 0000 0007 0000 0003 0000  ................
+00002320: 0073 0601 0000 6401 6402 6403 9c02 8900  .s....d.d.d.....
+00002330: 8703 6601 6404 6405 8408 7400 7401 8803  ..f.d.d...t.t...
+00002340: 8301 8301 4400 8301 7d04 6406 7c01 7601  ....D...}.d.|.v.
+00002350: 7226 8700 8701 8703 6603 6407 6405 8408  r&......f.d.d...
+00002360: 7400 7401 8803 8301 8301 4400 8301 7d05  t.t.......D...}.
+00002370: 6e0e 8701 8703 6602 6408 6405 8408 7400  n.....f.d.d...t.
+00002380: 7401 8803 8301 8301 4400 8301 7d05 8702  t.......D...}...
+00002390: 6601 6409 6405 8408 7400 7401 8802 8301  f.d.d...t.t.....
+000023a0: 8301 4400 8301 7d06 8701 8702 6602 640a  ..D...}.....f.d.
+000023b0: 6405 8408 7400 7401 8802 8301 8301 4400  d...t.t.......D.
+000023c0: 8301 7d07 8702 6601 640b 6405 8408 7400  ..}...f.d.d...t.
+000023d0: 7401 8802 8301 8301 4400 8301 7d08 8701  t.......D...}...
+000023e0: 8702 6602 640c 6405 8408 7400 7401 8802  ..f.d.d...t.t...
+000023f0: 8301 8301 4400 8301 7d09 7402 640d 8301  ....D...}.t.d...
+00002400: 0100 7403 7404 7405 7c05 7c07 1700 7c09  ..t.t.t.|.|...|.
+00002410: 1700 8301 8301 8301 7d0a 7c04 7c05 7c06  ........}.|.|.|.
+00002420: 7c07 7c08 7c09 7c0a 6607 5300 290e 4e72  |.|.|.|.f.S.).Nr
+00002430: 3700 0000 7201 0000 0029 02da 0359 6573  7...r....)...Yes
+00002440: da02 4e6f 6301 0000 0000 0000 0000 0000  ..Noc...........
+00002450: 0002 0000 0004 0000 0013 0000 00f3 1a00  ................
+00002460: 0000 6700 7c00 5d09 7d01 8800 6a00 7c01  ..g.|.].}...j.|.
+00002470: 1900 6400 1900 9102 7102 5300 a901 72a9  ..d.....q.S...r.
+00002480: 0000 00a9 0172 a400 0000 72a5 0000 0029  .....r....r....)
+00002490: 0172 c300 0000 722e 0000 0072 2f00 0000  .r....r....r/...
+000024a0: 723c 0000 0048 0100 00f3 0200 0000 1a00  r<...H..........
+000024b0: 7a21 7370 6c69 745f 6461 7461 7365 742e  z!split_dataset.
+000024c0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+000024d0: 6d70 3e72 9800 0000 6301 0000 0000 0000  mp>r....c.......
+000024e0: 0000 0000 0002 0000 0005 0000 0013 0000  ................
+000024f0: 0073 1e00 0000 6700 7c00 5d0b 7d01 8800  .s....g.|.].}...
+00002500: 8802 6a00 7c01 1900 8801 1900 1900 9102  ..j.|...........
+00002510: 7102 5300 722e 0000 0072 c900 0000 72a5  q.S.r....r....r.
+00002520: 0000 0029 03da 0f63 6f6e 7665 7273 696f  ...)...conversio
+00002530: 6e5f 6469 6374 728d 0000 0072 c300 0000  n_dictr....r....
+00002540: 722e 0000 0072 2f00 0000 723c 0000 004a  r....r/...r<...J
+00002550: 0100 00f3 0200 0000 1e00 6301 0000 0000  ..........c.....
+00002560: 0000 0000 0000 0002 0000 0005 0000 0013  ................
+00002570: 0000 00f3 1e00 0000 6700 7c00 5d0b 7d01  ........g.|.].}.
+00002580: 7400 8801 6a01 7c01 1900 8800 1900 8301  t...j.|.........
+00002590: 9102 7102 5300 722e 0000 00a9 0272 3800  ..q.S.r......r8.
+000025a0: 0000 72a4 0000 0072 a500 0000 2902 728d  ..r....r....).r.
+000025b0: 0000 0072 c300 0000 722e 0000 0072 2f00  ...r....r....r/.
+000025c0: 0000 723c 0000 004c 0100 0072 cc00 0000  ..r<...L...r....
+000025d0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000025e0: 0004 0000 0013 0000 0072 c700 0000 72c8  .........r....r.
+000025f0: 0000 0072 c900 0000 72a5 0000 0072 b900  ...r....r....r..
+00002600: 0000 722e 0000 0072 2f00 0000 723c 0000  ..r....r/...r<..
+00002610: 0050 0100 0072 ca00 0000 6301 0000 0000  .P...r....c.....
+00002620: 0000 0000 0000 0002 0000 0005 0000 0013  ................
+00002630: 0000 0072 cd00 0000 722e 0000 0072 ce00  ...r....r....r..
+00002640: 0000 72a5 0000 00a9 0272 8d00 0000 72ba  ..r......r....r.
+00002650: 0000 0072 2e00 0000 722f 0000 0072 3c00  ...r....r/...r<.
+00002660: 0000 5101 0000 72cc 0000 0063 0100 0000  ..Q...r....c....
+00002670: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00002680: 1300 0000 72c7 0000 0072 c800 0000 72c9  ....r....r....r.
+00002690: 0000 0072 a500 0000 72b9 0000 0072 2e00  ...r....r....r..
+000026a0: 0000 722f 0000 0072 3c00 0000 5501 0000  ..r/...r<...U...
+000026b0: 72ca 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000026c0: 0000 0200 0000 0500 0000 1300 0000 72cd  ..............r.
+000026d0: 0000 0072 2e00 0000 72ce 0000 0072 a500  ...r....r....r..
+000026e0: 0000 72cf 0000 0072 2e00 0000 722f 0000  ..r....r....r/..
+000026f0: 0072 3c00 0000 5601 0000 72cc 0000 007a  .r<...V...r....z
+00002700: 332d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  3---------------
+00002710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002720: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002730: 2d2d 2d2d 2906 72b5 0000 0072 2800 0000  ----).r....r(...
+00002740: 722a 0000 00da 0673 6f72 7465 64da 046c  r*.....sorted..l
+00002750: 6973 74da 0373 6574 290b 72c3 0000 0072  ist..set).r....r
+00002760: 7f00 0000 72ba 0000 0072 8d00 0000 da0e  ....r....r......
+00002770: 7472 6169 6e5f 7365 745f 7465 7874 da0f  train_set_text..
+00002780: 7472 6169 6e5f 7365 745f 6c61 6265 6cda  train_set_label.
+00002790: 0c64 6576 5f73 6574 5f74 6578 74da 0d64  .dev_set_text..d
+000027a0: 6576 5f73 6574 5f6c 6162 656c da0d 7465  ev_set_label..te
+000027b0: 7374 5f73 6574 5f74 6578 74da 0e74 6573  st_set_text..tes
+000027c0: 745f 7365 745f 6c61 6265 6cda 0b6c 6162  t_set_label..lab
+000027d0: 656c 735f 6c69 7374 722e 0000 0029 0472  els_listr....).r
+000027e0: cb00 0000 728d 0000 0072 ba00 0000 72c3  ....r....r....r.
+000027f0: 0000 0072 2f00 0000 da0d 7370 6c69 745f  ...r/.....split_
+00002800: 6461 7461 7365 7446 0100 0073 1800 0000  datasetF...s....
+00002810: 0a01 1a01 0801 2001 1c02 1a04 1c01 1a04  ...... .........
+00002820: 1c01 0802 180b 1208 72da 0000 0063 0500  ........r....c..
+00002830: 0000 0000 0000 0000 0000 0b00 0000 0500  ................
+00002840: 0000 4300 0000 73fc 0000 007c 0064 016b  ..C...s....|.d.k
+00002850: 0272 3e74 00a0 017c 017c 0264 029c 02a1  .r>t...|.|.d....
+00002860: 017d 0574 026a 03a0 047c 05a1 017d 0674  .}.t.j...|...}.t
+00002870: 05a0 067c 06a1 017d 0674 00a0 017c 037c  ...|...}.t...|.|
+00002880: 0464 029c 02a1 017d 0774 026a 03a0 047c  .d.....}.t.j...|
+00002890: 07a1 017d 0874 05a0 067c 08a1 017d 0874  ...}.t...|...}.t
+000028a0: 00a0 017c 037c 0464 029c 02a1 017d 0974  ...|.|.d.....}.t
+000028b0: 026a 03a0 047c 09a1 017d 0a74 05a0 067c  .j...|...}.t...|
+000028c0: 0aa1 017d 0a6e 3974 00a0 017c 017c 0264  ...}.n9t...|.|.d
+000028d0: 029c 02a1 017d 0574 026a 03a0 047c 05a1  .....}.t.j...|..
+000028e0: 017d 0674 05a0 067c 06a1 017d 0674 00a0  .}.t...|...}.t..
+000028f0: 017c 037c 0464 029c 02a1 017d 0774 026a  .|.|.d.....}.t.j
+00002900: 03a0 047c 07a1 017d 0874 05a0 067c 08a1  ...|...}.t...|..
+00002910: 017d 0874 00a0 0174 0774 0864 029c 02a1  .}.t...t.t.d....
+00002920: 017d 0974 026a 03a0 047c 09a1 017d 0a74  .}.t.j...|...}.t
+00002930: 05a0 067c 0aa1 017d 0a7c 057c 067c 087c  ...|...}.|.|.|.|
+00002940: 0a7c 0966 0553 0029 034e 5429 02da 056c  .|.f.S.).NT)...l
+00002950: 6162 656c 726f 0000 0029 0972 b100 0000  abelro...).r....
+00002960: da09 4461 7461 4672 616d 65da 0270 61da  ..DataFrame..pa.
+00002970: 0554 6162 6c65 da0b 6672 6f6d 5f70 616e  .Table..from_pan
+00002980: 6461 73da 0864 6174 6173 6574 73da 0744  das..datasets..D
+00002990: 6174 6173 6574 72d8 0000 0072 d700 0000  atasetr....r....
+000029a0: 290b 728c 0000 0072 d400 0000 72d3 0000  ).r....r....r...
+000029b0: 0072 d600 0000 72d5 0000 00da 1774 7261  .r....r......tra
+000029c0: 696e 696e 675f 6461 7461 7365 745f 7061  ining_dataset_pa
+000029d0: 6e64 6173 da16 7472 6169 6e69 6e67 5f64  ndas..training_d
+000029e0: 6174 6173 6574 5f61 7272 6f77 5a19 7661  ataset_arrowZ.va
+000029f0: 6c69 6461 7469 6f6e 5f64 6174 6173 6574  lidation_dataset
+00002a00: 5f70 616e 6461 73da 1876 616c 6964 6174  _pandas..validat
+00002a10: 696f 6e5f 6461 7461 7365 745f 6172 726f  ion_dataset_arro
+00002a20: 77da 1374 6573 745f 6461 7461 7365 745f  w..test_dataset_
+00002a30: 7061 6e64 6173 da12 7465 7374 5f64 6174  pandas..test_dat
+00002a40: 6173 6574 5f61 7272 6f77 722e 0000 0072  aset_arrowr....r
+00002a50: 2e00 0000 722f 0000 00da 0f70 7265 7061  ....r/.....prepa
+00002a60: 7265 5f64 6174 6173 6574 6f01 0000 7328  re_dataseto...s(
+00002a70: 0000 0008 0110 020c 010a 0110 020c 010a  ................
+00002a80: 0110 020c 010c 0110 040c 010a 0110 020c  ................
+00002a90: 010a 0110 020c 010a 010e 0272 e700 0000  ...........r....
+00002aa0: 6304 0000 0000 0000 0000 0000 0006 0000  c...............
+00002ab0: 0006 0000 0003 0000 0073 4e00 0000 7400  .........sN...t.
+00002ac0: a001 7c01 7c02 7c03 6401 9c03 a101 7d04  ..|.|.|.d.....}.
+00002ad0: 7c04 6a02 8700 6601 6402 6403 8408 6404  |.j...f.d.d...d.
+00002ae0: 6405 8d02 7d05 7c05 a003 6406 6701 a101  d...}.|...d.g...
+00002af0: 7d05 7c05 a004 6407 6408 a102 7d05 7c05  }.|...d.d...}.|.
+00002b00: a005 6409 a101 0100 7c05 5300 290a 4e29  ..d.....|.S.).N)
+00002b10: 03da 0574 7261 696e da0a 7661 6c69 6461  ...train..valida
+00002b20: 7469 6f6e da04 7465 7374 6301 0000 0000  tion..testc.....
+00002b30: 0000 0000 0000 0001 0000 0003 0000 0013  ................
+00002b40: 0000 0073 0a00 0000 7400 8800 7c00 8302  ...s....t...|...
+00002b50: 5300 a901 4e29 0172 7500 0000 2901 7274  S...N).ru...).rt
+00002b60: 0000 0072 af00 0000 722e 0000 0072 2f00  ...r....r....r/.
+00002b70: 0000 da08 3c6c 616d 6264 613e 9501 0000  ....<lambda>....
+00002b80: 7302 0000 000a 007a 3469 6e69 7461 6c69  s......z4initali
+00002b90: 7a65 5f64 6174 6173 6574 5f66 6f72 5f74  ze_dataset_for_t
+00002ba0: 6f6b 656e 697a 6174 696f 6e2e 3c6c 6f63  okenization.<loc
+00002bb0: 616c 733e 2e3c 6c61 6d62 6461 3e54 2901  als>.<lambda>T).
+00002bc0: da07 6261 7463 6865 6472 6f00 0000 72db  ..batchedro...r.
+00002bd0: 0000 0072 6800 0000 7253 0000 0029 0672  ...rh...rS...).r
+00002be0: e000 0000 da0b 4461 7461 7365 7444 6963  ......DatasetDic
+00002bf0: 74da 036d 6170 da0e 7265 6d6f 7665 5f63  t..map..remove_c
+00002c00: 6f6c 756d 6e73 da0d 7265 6e61 6d65 5f63  olumns..rename_c
+00002c10: 6f6c 756d 6eda 0a73 6574 5f66 6f72 6d61  olumn..set_forma
+00002c20: 7429 0672 7300 0000 72e3 0000 0072 e400  t).rs...r....r..
+00002c30: 0000 72e6 0000 0072 7e00 0000 da12 746f  ..r....r~.....to
+00002c40: 6b65 6e69 7a65 645f 6461 7461 7365 7473  kenized_datasets
+00002c50: 722e 0000 0072 af00 0000 722f 0000 00da  r....r....r/....
+00002c60: 2269 6e69 7461 6c69 7a65 5f64 6174 6173  "initalize_datas
+00002c70: 6574 5f66 6f72 5f74 6f6b 656e 697a 6174  et_for_tokenizat
+00002c80: 696f 6e8f 0100 0073 1200 0000 0602 0201  ion....s........
+00002c90: 0201 08fe 1604 0c02 0c01 0a01 0402 72f4  ..............r.
+00002ca0: 0000 0063 0c00 0000 0000 0000 0000 0000  ...c............
+00002cb0: 2b00 0000 0b00 0000 4300 0000 73c6 0300  +.......C...s...
+00002cc0: 0067 007d 0c67 007d 0d67 007d 0e74 0064  .g.}.g.}.g.}.t.d
+00002cd0: 017c 0083 0244 0090 015d d47d 0f74 01a0  .|...D...].}.t..
+00002ce0: 01a1 007d 1074 0264 0283 0101 0074 037c  ...}.t.d.....t.|
+00002cf0: 0164 0319 007c 0264 048d 027d 1174 037c  .d...|.d...}.t.|
+00002d00: 0164 0519 007c 0264 048d 027d 1274 037c  .d...|.d...}.t.|
+00002d10: 0164 0619 007c 0264 048d 027d 1374 0264  .d...|.d...}.t.d
+00002d20: 0774 0474 0574 067c 0383 0183 0183 0117  .t.t.t.|........
+00002d30: 0083 0101 0074 0774 0574 067c 0383 0183  .....t.t.t.|....
+00002d40: 017c 0483 027d 147c 14a0 087c 06a1 0101  .|...}.|...|....
+00002d50: 0074 09a0 0aa1 007d 1574 0b7c 14a0 0ca1  .t.....}.t.|....
+00002d60: 007c 0564 088d 027d 167c 0974 057c 1183  .|.d...}.|.t.|..
+00002d70: 0114 007d 1774 0d64 097c 167c 0a7c 1764  ...}.t.d.|.|.|.d
+00002d80: 0a8d 047d 1867 007d 1967 007d 1a67 007d  ...}.g.}.g.}.g.}
+00002d90: 1b67 007d 1c64 0164 0b6c 0e6d 0f7d 1d01  .g.}.d.d.l.m.}..
+00002da0: 007c 1d7c 0864 0c7c 0764 0d8d 037d 1e74  .|.|.d.|.d...}.t
+00002db0: 0264 0e7c 0717 0083 0101 0074 0264 0f83  .d.|.......t.d..
+00002dc0: 0101 0064 017d 1f74 007c 0983 0144 0090  ...d.}.t.|...D..
+00002dd0: 015d 4f7d 207c 1f64 1037 007d 1f74 0264  .]O} |.d.7.}.t.d
+00002de0: 1174 047c 2083 0117 0083 0101 0074 1074  .t.| ........t.t
+00002df0: 0074 057c 1183 0183 0183 017d 2164 017d  .t.|.......}!d.}
+00002e00: 227c 14a0 11a1 0001 007c 1144 005d 5e7d  "|.......|.D.]^}
+00002e10: 237c 0464 1276 0072 be7c 2364 1319 00a0  #|.d.v.r.|#d....
+00002e20: 087c 06a1 017c 2364 1419 00a0 12a1 00a0  .|...|#d........
+00002e30: 087c 06a1 0164 159c 027d 246e 0f7c 2364  .|...d...}$n.|#d
+00002e40: 1319 00a0 087c 06a1 017c 2364 1419 00a0  .....|...|#d....
+00002e50: 087c 06a1 0164 159c 027d 247c 1464 2269  .|...d...}$|.d"i
+00002e60: 007c 24a4 018e 017d 257c 157c 257c 2364  .|$....}%|.|%|#d
+00002e70: 1619 00a0 087c 06a1 0183 027d 267c 26a0  .....|.....}&|&.
+00002e80: 13a1 0001 007c 2264 1037 007d 227c 227c  .....|"d.7.}"|"|
+00002e90: 0b16 0064 016b 0272 f87c 16a0 14a1 0001  ...d.k.r.|......
+00002ea0: 007c 18a0 14a1 0001 007c 16a0 15a1 0001  .|.......|......
+00002eb0: 007c 21a0 1664 10a1 0101 007c 19a0 177c  .|!..d.....|...|
+00002ec0: 26a0 18a1 00a1 0101 0071 a674 1074 0074  &........q.t.t.t
+00002ed0: 057c 1283 0183 0183 017d 217c 14a0 19a1  .|.......}!|....
+00002ee0: 0001 007c 1244 005d 737d 2374 1aa0 1ba1  ...|.D.]s}#t....
+00002ef0: 008f 6301 007c 0464 1276 0090 0172 317c  ..c..|.d.v...r1|
+00002f00: 2364 1319 00a0 087c 06a1 017c 2364 1419  #d.....|...|#d..
+00002f10: 00a0 12a1 00a0 087c 06a1 0164 159c 027d  .......|...d...}
+00002f20: 246e 0f7c 2364 1319 00a0 087c 06a1 017c  $n.|#d.....|...|
+00002f30: 2364 1419 00a0 087c 06a1 0164 159c 027d  #d.....|...d...}
+00002f40: 247c 0464 1776 0090 0172 587c 2364 1619  $|.d.v...rX|#d..
+00002f50: 00a0 1c7c 2364 1619 006a 1d64 0119 0064  ...|#d...j.d...d
+00002f60: 10a1 02a0 087c 06a1 0166 017c 2464 183c  .....|...f.|$d.<
+00002f70: 007c 1464 2269 007c 24a4 018e 017d 257c  .|.d"i.|$....}%|
+00002f80: 157c 257c 2364 1619 00a0 087c 06a1 0183  .|%|#d.....|....
+00002f90: 027d 267c 21a0 1664 10a1 0101 007c 1aa0  .}&|!..d.....|..
+00002fa0: 177c 26a0 18a1 00a1 0101 0057 0064 0004  .|&........W.d..
+00002fb0: 0004 0083 0301 006e 0931 0090 0173 8077  .......n.1...s.w
+00002fc0: 0101 0001 0001 0059 0001 0090 0171 1374  .......Y.....q.t
+00002fd0: 1ea0 1f7c 19a1 017d 2774 1ea0 1f7c 1aa1  ...|...}'t...|..
+00002fe0: 017d 287c 1ba0 177c 27a1 0101 007c 1ca0  .}(|...|'....|..
+00002ff0: 177c 28a1 0101 0074 0574 047c 0983 0183  .|(....t.t.|....
+00003000: 017d 2964 197c 2064 1a7c 299b 009d 029b  .})d.| d.|).....
+00003010: 0464 1b7c 0964 1a7c 299b 009d 029b 0464  .d.|.d.|)......d
+00003020: 1c9d 0564 1d7c 2764 1e9b 0464 1f9d 0317  ...d.|'d...d....
+00003030: 0064 207c 2864 1e9b 049d 0217 007d 2a74  .d |(d.......}*t
+00003040: 027c 2a83 0101 0067 007d 1967 007d 1a7c  .|*....g.}.g.}.|
+00003050: 1e7c 287c 1483 0201 007c 1e6a 2090 0172  .|(|.....|.j ..r
+00003060: d774 0264 2183 0101 0001 0090 0171 d871  .t.d!........q.q
+00003070: 877c 147c 1b7c 1c7c 137c 0e66 0502 0001  .|.|.|.|.|.f....
+00003080: 0053 0064 0053 0029 234e 7201 0000 007a  .S.d.S.)#Nr....z
+00003090: 0d4c 6f61 6469 6e67 204d 6f64 656c 72e8  .Loading Modelr.
+000030a0: 0000 0029 01da 0a62 6174 6368 5f73 697a  ...)...batch_siz
+000030b0: 6572 e900 0000 72ea 0000 007a 124e 756d  er....r....z.Num
+000030c0: 6265 7220 6f66 206c 6162 656c 733a 2029  ber of labels: )
+000030d0: 01da 026c 72da 066c 696e 6561 7229 04da  ...lr..linear)..
+000030e0: 046e 616d 65da 096f 7074 696d 697a 6572  .name..optimizer
+000030f0: 7291 0000 00da 126e 756d 5f74 7261 696e  r......num_train
+00003100: 696e 675f 7374 6570 7329 01da 0d45 6172  ing_steps)...Ear
+00003110: 6c79 5374 6f70 7069 6e67 5429 03da 0870  lyStoppingT)...p
+00003120: 6174 6965 6e63 65da 0776 6572 626f 7365  atience..verbose
+00003130: 727a 0000 0072 8400 0000 7a12 4265 6769  rz...r....z.Begi
+00003140: 6e6e 696e 6720 5472 6169 6e69 6e67 7237  nning Trainingr7
+00003150: 0000 007a 0f43 7572 7265 6e74 2045 706f  ...z.Current Epo
+00003160: 6368 3a20 7248 0000 0072 6200 0000 7263  ch: rH...rb...rc
+00003170: 0000 00a9 0272 6600 0000 7267 0000 0072  .....rf...rg...r
+00003180: 6800 0000 a903 7261 0000 0072 4c00 0000  h.....ra...rL...
+00003190: 724b 0000 0072 6900 0000 da01 5bda 013e  rK...ri.....[..>
+000031a0: 7277 0000 007a 025d 207a 0c74 7261 696e  rw...z.] z.train
+000031b0: 5f6c 6f73 733a 207a 032e 3566 721a 0000  _loss: z..5fr...
+000031c0: 007a 0c76 616c 6964 5f6c 6f73 733a 207a  .z.valid_loss: z
+000031d0: 0e45 6172 6c79 2073 746f 7070 696e 6772  .Early stoppingr
+000031e0: 2e00 0000 2921 72b5 0000 0072 8800 0000  ....)!r....r....
+000031f0: 722a 0000 0072 0d00 0000 722b 0000 0072  r*...r....r+...r
+00003200: 2800 0000 72d2 0000 0072 4300 0000 da02  (...r....rC.....
+00003210: 746f 7258 0000 00da 1043 726f 7373 456e  torX.....CrossEn
+00003220: 7472 6f70 794c 6f73 7372 0c00 0000 da0a  tropyLossr......
+00003230: 7061 7261 6d65 7465 7273 720e 0000 005a  parametersr....Z
+00003240: 2b61 7265 732e 4c4c 4d5f 6173 5f61 5f4a  +ares.LLM_as_a_J
+00003250: 7564 6765 5f41 6461 7074 6174 696f 6e2e  udge_Adaptation.
+00003260: 7079 746f 7263 6874 6f6f 6c73 72fb 0000  pytorchtoolsr...
+00003270: 0072 1200 0000 72e8 0000 00da 0462 6f6f  .r....r......boo
+00003280: 6cda 0862 6163 6b77 6172 64da 0473 7465  l..backward..ste
+00003290: 70da 097a 6572 6f5f 6772 6164 da06 7570  p..zero_grad..up
+000032a0: 6461 7465 da06 6170 7065 6e64 da04 6974  date..append..it
+000032b0: 656d da04 6576 616c 7253 0000 00da 076e  em..evalrS.....n
+000032c0: 6f5f 6772 6164 da07 7265 7368 6170 65da  o_grad..reshape.
+000032d0: 0573 6861 7065 da02 6e70 da07 6176 6572  .shape..np..aver
+000032e0: 6167 655a 0a65 6172 6c79 5f73 746f 7029  ageZ.early_stop)
+000032f0: 2b72 8b00 0000 72f3 0000 0072 9300 0000  +r....r....r....
+00003300: 72d4 0000 0072 4e00 0000 728a 0000 00da  r....rN...r.....
+00003310: 0664 6576 6963 6572 9400 0000 728f 0000  .devicer....r...
+00003320: 0072 9000 0000 7291 0000 0072 9200 0000  .r....r....r....
+00003330: 5a0e 6d69 6372 6f5f 6176 6572 6167 6573  Z.micro_averages
+00003340: 5a0e 6d61 6372 6f5f 6176 6572 6167 6573  Z.macro_averages
+00003350: da0f 696e 6665 7265 6e63 655f 7469 6d65  ..inference_time
+00003360: 7372 3a00 0000 5a09 7275 6e5f 7374 6172  sr:...Z.run_star
+00003370: 745a 1074 7261 696e 5f64 6174 616c 6f61  tZ.train_dataloa
+00003380: 6465 725a 1576 616c 6964 6174 696f 6e5f  derZ.validation_
+00003390: 6461 7461 6c6f 6164 6572 da0f 6576 616c  dataloader..eval
+000033a0: 5f64 6174 616c 6f61 6465 72da 056d 6f64  _dataloader..mod
+000033b0: 656c 5a09 6372 6974 6572 696f 6e72 f900  elZ.criterionr..
+000033c0: 0000 72fa 0000 00da 0c6c 725f 7363 6865  ..r......lr_sche
+000033d0: 6475 6c65 725a 0c74 7261 696e 5f6c 6f73  dulerZ.train_los
+000033e0: 7365 735a 0c76 616c 6964 5f6c 6f73 7365  sesZ.valid_losse
+000033f0: 73da 1061 7667 5f74 7261 696e 5f6c 6f73  s..avg_train_los
+00003400: 7365 73da 1061 7667 5f76 616c 6964 5f6c  ses..avg_valid_l
+00003410: 6f73 7365 7372 fb00 0000 da0e 6561 726c  ossesr......earl
+00003420: 795f 7374 6f70 7069 6e67 5a16 746f 7461  y_stoppingZ.tota
+00003430: 6c5f 6570 6f63 6873 5f70 6572 666f 726d  l_epochs_perform
+00003440: 6564 da05 6570 6f63 68da 0c70 726f 6772  ed..epoch..progr
+00003450: 6573 735f 6261 725a 1b67 7261 6469 656e  ess_barZ.gradien
+00003460: 745f 6163 6375 6d75 6c61 7469 6f6e 5f63  t_accumulation_c
+00003470: 6f75 6e74 da05 6261 7463 68da 096e 6577  ount..batch..new
+00003480: 5f62 6174 6368 da07 6f75 7470 7574 73da  _batch..outputs.
+00003490: 046c 6f73 735a 0a74 7261 696e 5f6c 6f73  .lossZ.train_los
+000034a0: 735a 0a76 616c 6964 5f6c 6f73 735a 0965  sZ.valid_lossZ.e
+000034b0: 706f 6368 5f6c 656e 5a09 7072 696e 745f  poch_lenZ.print_
+000034c0: 6d73 6772 2e00 0000 722e 0000 0072 2f00  msgr....r....r/.
+000034d0: 0000 da18 7472 6169 6e5f 616e 645f 6576  ....train_and_ev
+000034e0: 616c 7561 7465 5f6d 6f64 656c 9f01 0000  aluate_model....
+000034f0: 73a6 0000 0004 0304 0104 0110 0208 0208  s...............
+00003500: 0210 0210 0110 0118 0212 040a 0208 0410  ................
+00003510: 010c 0202 0208 0106 ff04 0704 0204 0204  ................
+00003520: 020c 030e 030c 0308 0204 020e 0208 0210  ................
+00003530: 0210 0204 0208 0208 0108 0224 011e 020e  ...........$....
+00003540: 0214 0208 0208 020c 0108 0108 0108 010a  ................
+00003550: 0210 0110 0408 0208 010a 020a 0224 011e  .............$..
+00003560: 020a 0226 010e 0214 020a 0110 021e f104  ...&............
+00003570: 800a 130a 010a 010a 010c 0220 020c 0102  ........... ....
+00003580: ff0a 0204 fe08 0404 0304 010a 0408 0208  ................
+00003590: 0106 0102 fe12 0400 8104 f672 2001 0000  ...........r ...
+000035a0: 6306 0000 0000 0000 0000 0000 0012 0000  c...............
+000035b0: 0009 0000 0043 0000 0073 9801 0000 7400  .....C...s....t.
+000035c0: 6401 8301 0100 7c00 a001 7402 a003 7c02  d.....|...t...|.
+000035d0: a101 a101 0100 7400 6402 8301 0100 7404  ......t.d.....t.
+000035e0: 6403 8301 7d06 7402 a005 6700 a101 a006  d...}.t...g.....
+000035f0: 7c03 a101 7d07 7402 a005 6700 a101 a006  |...}.t...g.....
+00003600: 7c03 a101 7d08 7407 a007 a100 7d09 7408  |...}.t.....}.t.
+00003610: 7409 740a 7c04 8301 8301 8301 7d0a 7c04  t.t.|.......}.|.
+00003620: 4400 5d87 7d0b 7402 a00b a100 8f79 0100  D.].}.t......y..
+00003630: 7c01 6404 7600 724f 7c0b 6405 1900 a006  |.d.v.rO|.d.....
+00003640: 7c03 a101 7c0b 6406 1900 a00c a100 a006  |...|.d.........
+00003650: 7c03 a101 6407 9c02 7d0c 6e0f 7c0b 6405  |...d...}.n.|.d.
+00003660: 1900 a006 7c03 a101 7c0b 6406 1900 a006  ....|...|.d.....
+00003670: 7c03 a101 6407 9c02 7d0c 7c01 6408 7600  |...d...}.|.d.v.
+00003680: 7274 7c0b 6409 1900 a00d 7c0b 6409 1900  rt|.d.....|.d...
+00003690: 6a0e 640a 1900 640b a102 a006 7c03 a101  j.d...d.....|...
+000036a0: 7c0c 640c 3c00 7c00 6410 6900 7c0c a401  |.d.<.|.d.i.|...
+000036b0: 8e01 7d0d 7c0d 7d0e 7402 6a0f 7c0e 640d  ..}.|.}.t.j.|.d.
+000036c0: 640e 8d02 7d0f 7c06 6a10 7c0f 7c0b 6409  d...}.|.j.|.|.d.
+000036d0: 1900 a006 7c03 a101 640f 8d02 0100 7402  ....|...d.....t.
+000036e0: a011 7c07 7c0f 6602 640a a102 7d07 7402  ..|.|.f.d...}.t.
+000036f0: a011 7c08 7c0b 6409 1900 a006 7c03 a101  ..|.|.d.....|...
+00003700: 6602 640a a102 7d08 7c0a a012 640b a101  f.d...}.|...d...
+00003710: 0100 5700 6400 0400 0400 8303 0100 6e08  ..W.d.........n.
+00003720: 3100 73b4 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
+00003730: 7132 7407 a007 a100 7d10 7c10 7c09 1800  q2t.....}.|.|...
+00003740: 7d11 7c05 a013 7c11 a101 0100 7c07 7c08  }.|...|.....|.|.
+00003750: 7c06 6603 5300 2911 4e7a 164c 6f61 6469  |.f.S.).Nz.Loadi
+00003760: 6e67 2074 6865 2042 6573 7420 4d6f 6465  ng the Best Mode
+00003770: 6c7a 1442 6567 696e 6e69 6e67 2045 7661  lz.Beginning Eva
+00003780: 6c75 6174 696f 6eda 0861 6363 7572 6163  luation..accurac
+00003790: 7972 4800 0000 7262 0000 0072 6300 0000  yrH...rb...rc...
+000037a0: 72fe 0000 0072 ff00 0000 7268 0000 0072  r....r....rh...r
+000037b0: 0100 0000 7237 0000 0072 6900 0000 7236  ....r7...ri...r6
+000037c0: 0000 0029 01da 0364 696d 2902 da0b 7072  ...)...dim)...pr
+000037d0: 6564 6963 7469 6f6e 73da 0a72 6566 6572  edictions..refer
+000037e0: 656e 6365 7372 2e00 0000 2914 722a 0000  encesr....).r*..
+000037f0: 00da 0f6c 6f61 645f 7374 6174 655f 6469  ...load_state_di
+00003800: 6374 7253 0000 00da 046c 6f61 6472 0900  ctrS.....loadr..
+00003810: 0000 da0b 466c 6f61 7454 656e 736f 7272  ....FloatTensorr
+00003820: 0201 0000 7288 0000 0072 1200 0000 72b5  ....r....r....r.
+00003830: 0000 0072 2800 0000 720d 0100 0072 0501  ...r(...r....r..
+00003840: 0000 720e 0100 0072 0f01 0000 da06 6172  ..r....r......ar
+00003850: 676d 6178 da09 6164 645f 6261 7463 68da  gmax..add_batch.
+00003860: 0363 6174 7209 0100 0072 0a01 0000 2912  .catr....r....).
+00003870: 7215 0100 0072 4e00 0000 7294 0000 0072  r....rN...r....r
+00003880: 1201 0000 7214 0100 0072 1301 0000 da06  ....r....r......
+00003890: 6d65 7472 6963 da11 746f 7461 6c5f 7072  metric..total_pr
+000038a0: 6564 6963 7469 6f6e 73da 1074 6f74 616c  edictions..total
+000038b0: 5f72 6566 6572 656e 6365 735a 0f69 6e66  _referencesZ.inf
+000038c0: 6572 656e 6365 5f73 7461 7274 721b 0100  erence_startr...
+000038d0: 0072 1c01 0000 721d 0100 0072 1e01 0000  .r....r....r....
+000038e0: 7264 0000 0072 2301 0000 5a0d 696e 6665  rd...r#...Z.infe
+000038f0: 7265 6e63 655f 656e 645a 1474 6f74 616c  rence_endZ.total
+00003900: 5f69 6e66 6572 656e 6365 5f74 696d 6572  _inference_timer
+00003910: 2e00 0000 722e 0000 0072 2f00 0000 da0e  ....r....r/.....
+00003920: 6576 616c 7561 7465 5f6d 6f64 656c 3302  evaluate_model3.
+00003930: 0000 7338 0000 0008 0210 0208 0408 0210  ..s8............
+00003940: 0210 0108 0210 0408 010a 0208 0224 011e  .............$..
+00003950: 0208 0224 010e 0204 020e 0118 0110 021a  ...$............
+00003960: 010c 021c ed02 8008 1708 010a 010a 0272  ...............r
+00003970: 2e01 0000 6304 0000 0000 0000 0000 0000  ....c...........
+00003980: 0008 0000 0008 0000 0043 0000 0073 de00  .........C...s..
+00003990: 0000 7400 6401 8301 0100 7400 6402 8301  ..t.d.....t.d...
+000039a0: 0100 7400 7c00 6a01 8301 0100 7400 7c01  ..t.|.j.....t.|.
+000039b0: 6a01 8301 0100 7c03 6a02 7c01 7c00 6403  j.....|.j.|.|.d.
+000039c0: 8d02 7d04 7400 6404 7403 7c04 6405 1900  ..}.t.d.t.|.d...
+000039d0: 8301 1700 8301 0100 7404 6406 8301 7d05  ........t.d...}.
+000039e0: 7c05 6a02 6407 7c01 7c00 6408 8d03 7d06  |.j.d.|.|.d...}.
+000039f0: 7400 6409 7403 7c06 6406 1900 640a 1400  t.d.t.|.d...d...
+00003a00: 8301 1700 8301 0100 7c05 6a02 640b 7c01  ........|.j.d.|.
+00003a10: 7c00 6408 8d03 7d07 7400 640c 7403 7c07  |.d...}.t.d.t.|.
+00003a20: 6406 1900 640a 1400 8301 1700 8301 0100  d...d...........
+00003a30: 7400 640d 7403 7405 7c01 a006 a100 a007  t.d.t.t.|.......
+00003a40: 640e a101 7408 7c01 a006 a100 8301 1b00  d...t.|.........
+00003a50: 640f 8302 8301 1700 8301 0100 7400 6410  d...........t.d.
+00003a60: 7403 7c02 8301 1700 8301 0100 6400 5300  t.|.........d.S.
+00003a70: 2911 4e7a 1a2d 2d2d 2d2d 2d2d 2d2d 2d2d  ).Nz.-----------
+00003a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7a  ---------------z
+00003a90: 2050 7265 6469 6374 696f 6e73 2061 6e64   Predictions and
+00003aa0: 2052 6566 6572 656e 6365 2053 6861 7065   Reference Shape
+00003ab0: 7329 0272 2401 0000 7223 0100 007a 1741  s).r$...r#...z.A
+00003ac0: 6363 7572 6163 7920 666f 7220 5465 7374  ccuracy for Test
+00003ad0: 2053 6574 3a20 7221 0100 00da 0266 31da   Set: r!.....f1.
+00003ae0: 056d 6163 726f 2903 7211 0100 0072 2401  .macro).r....r$.
+00003af0: 0000 7223 0100 007a 174d 6163 726f 2046  ..r#...z.Macro F
+00003b00: 3120 666f 7220 5465 7374 2053 6574 3a20  1 for Test Set: 
+00003b10: 7220 0000 00da 056d 6963 726f 7a17 4d69  r .....microz.Mi
+00003b20: 6372 6f20 4631 2066 6f72 2054 6573 7420  cro F1 for Test 
+00003b30: 5365 743a 207a 2550 6f73 6974 6976 6520  Set: z%Positive 
+00003b40: 2f20 4e65 6761 7469 7665 2052 6566 6572  / Negative Refer
+00003b50: 656e 6365 2052 6174 696f 3a20 7237 0000  ence Ratio: r7..
+00003b60: 00e9 0300 0000 7a24 5361 7665 6420 636c  ......z$Saved cl
+00003b70: 6173 7369 6669 6361 7469 6f6e 2063 6865  assification che
+00003b80: 636b 706f 696e 7420 746f 3a20 2909 722a  ckpoint to: ).r*
+00003b90: 0000 0072 0f01 0000 da07 636f 6d70 7574  ...r......comput
+00003ba0: 6572 2b00 0000 7209 0000 00da 0572 6f75  er+...r......rou
+00003bb0: 6e64 da06 746f 6c69 7374 da05 636f 756e  nd..tolist..coun
+00003bc0: 7472 2800 0000 2908 722c 0100 0072 2d01  tr(...).r,...r-.
+00003bd0: 0000 7294 0000 0072 2b01 0000 da07 7265  ..r....r+.....re
+00003be0: 7375 6c74 735a 0a66 5f31 5f6d 6574 7269  sultsZ.f_1_metri
+00003bf0: 635a 116d 6163 726f 5f66 5f31 5f72 6573  cZ.macro_f_1_res
+00003c00: 756c 7473 5a11 6d69 6372 6f5f 665f 315f  ultsZ.micro_f_1_
+00003c10: 7265 7375 6c74 7372 2e00 0000 722e 0000  resultsr....r...
+00003c20: 0072 2f00 0000 da14 7072 696e 745f 616e  .r/.....print_an
+00003c30: 645f 7361 7665 5f6d 6f64 656c 6802 0000  d_save_modelh...
+00003c40: 731a 0000 0008 0108 010a 010a 010e 0214  s...............
+00003c50: 0108 0210 0118 0110 0118 012c 0214 0272  ...........,...r
+00003c60: 3801 0000 da08 5f5f 6d61 696e 5f5f 7a18  8.....__main__z.
+00003c70: 2d2d 636c 6173 7369 6669 6361 7469 6f6e  --classification
+00003c80: 5f64 6174 6173 6574 5429 02da 0474 7970  _datasetT)...typ
+00003c90: 65da 0872 6571 7569 7265 647a 142d 2d74  e..requiredz.--t
+00003ca0: 6573 745f 7365 745f 7365 6c65 6374 696f  est_set_selectio
+00003cb0: 6e7a 0e2d 2d6c 6162 656c 5f63 6f6c 756d  nz.--label_colum
+00003cc0: 6e7a 0c2d 2d6e 756d 5f65 706f 6368 737a  nz.--num_epochsz
+00003cd0: 102d 2d70 6174 6965 6e63 655f 7661 6c75  .--patience_valu
+00003ce0: 657a 0f2d 2d6c 6561 726e 696e 675f 7261  ez.--learning_ra
+00003cf0: 7465 7a06 6375 6461 3a30 7237 0000 00e9  tez.cuda:0r7....
+00003d00: 2000 0000 7220 0000 0072 eb00 0000 295b   ...r ...r....)[
+00003d10: da08 746f 7263 682e 6e6e 7258 0000 00da  ..torch.nnrX....
+00003d20: 0c74 7261 6e73 666f 726d 6572 7372 0200  .transformersr..
+00003d30: 0000 7203 0000 0072 0400 0000 7205 0000  ..r....r....r...
+00003d40: 0072 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
+00003d50: da06 7061 6e64 6173 72b1 0000 00da 056e  ..pandasr......n
+00003d60: 756d 7079 7210 0100 00da 0361 7374 72e0  umpyr......astr.
+00003d70: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
+00003d80: 0000 da07 7079 6172 726f 7772 dd00 0000  ....pyarrowr....
+00003d90: da0f 7079 6172 726f 772e 6461 7461 7365  ..pyarrow.datase
+00003da0: 7472 7f00 0000 da02 6473 5a0b 746f 7263  tr......dsZ.torc
+00003db0: 682e 6f70 7469 6d72 0c00 0000 da10 746f  h.optimr......to
+00003dc0: 7263 682e 7574 696c 732e 6461 7461 720d  rch.utils.datar.
+00003dd0: 0000 0072 0e00 0000 720f 0000 0072 1000  ...r....r....r..
+00003de0: 0000 7211 0000 0072 5300 0000 da09 7471  ..r....rS.....tq
+00003df0: 646d 2e61 7574 6f72 1200 0000 da0a 7374  dm.autor......st
+00003e00: 6174 6973 7469 6373 7288 0000 00da 0a73  atisticsr......s
+00003e10: 7562 7072 6f63 6573 7372 3d00 0000 7279  ubprocessr=...ry
+00003e20: 0000 00da 1773 6b6c 6561 726e 2e6d 6f64  .....sklearn.mod
+00003e30: 656c 5f73 656c 6563 7469 6f6e 7213 0000  el_selectionr...
+00003e40: 00da 046a 736f 6eda 0672 616e 646f 6d72  ...json..randomr
+00003e50: 2200 0000 da08 6172 6770 6172 7365 7214  ".....argparser.
+00003e60: 0000 0072 2b00 0000 7230 0000 0072 3300  ...r+...r0...r3.
+00003e70: 0000 72a0 0000 00da 0473 6565 64da 0b6d  ..r......seed..m
+00003e80: 616e 7561 6c5f 7365 6564 da07 656e 7669  anual_seed..envi
+00003e90: 726f 6e72 4200 0000 da06 4d6f 6475 6c65  ronrB.....Module
+00003ea0: 7243 0000 0072 7500 0000 7280 0000 0072  rC...ru...r....r
+00003eb0: 8200 0000 7295 0000 0072 b700 0000 72c4  ....r....r....r.
+00003ec0: 0000 0072 da00 0000 72e7 0000 0072 f400  ...r....r....r..
+00003ed0: 0000 7220 0100 0072 2e01 0000 7238 0100  ..r ...r....r8..
+00003ee0: 0072 6b00 0000 da0e 4172 6775 6d65 6e74  .rk.....Argument
+00003ef0: 5061 7273 6572 da06 7061 7273 6572 da0c  Parser..parser..
+00003f00: 6164 645f 6172 6775 6d65 6e74 7238 0000  add_argumentr8..
+00003f10: 00da 0566 6c6f 6174 da0a 7061 7273 655f  ...float..parse_
+00003f20: 6172 6773 da04 6172 6773 727e 0000 0072  args..argsr~...r
+00003f30: 7d00 0000 5a12 7465 7374 5f73 6574 5f73  }...Z.test_set_s
+00003f40: 656c 6563 7469 6f6e 728d 0000 0072 9000  electionr....r..
+00003f50: 0000 728f 0000 00da 0d6c 6561 726e 696e  ..r......learnin
+00003f60: 675f 7261 7465 7289 0000 0072 1201 0000  g_rater....r....
+00003f70: 728c 0000 0072 9300 0000 7292 0000 0072  r....r....r....r
+00003f80: 8b00 0000 7291 0000 0072 2e00 0000 722e  ....r....r....r.
+00003f90: 0000 0072 2e00 0000 722f 0000 00da 083c  ...r....r/.....<
+00003fa0: 6d6f 6475 6c65 3e01 0000 0073 8e00 0000  module>....s....
+00003fb0: 0c02 1401 1801 0803 0801 0801 0801 0c01  ................
+00003fc0: 1001 0802 0c01 0c02 0c01 1801 0802 0c01  ................
+00003fd0: 0801 0801 0802 0801 0c02 0801 0801 0802  ................
+00003fe0: 0801 1002 1403 1216 0412 0c02 0a01 0a01  ................
+00003ff0: 0e01 0804 1208 084c 0805 0813 0808 0828  .......L.......(
+00004000: 082f 0822 0829 0820 0810 007f 0815 0835  ./.".). .......5
+00004010: 0a14 0802 1002 1001 1001 1001 1001 1001  ................
+00004020: 0802 0802 0601 0601 0601 0601 0801 0404  ................
+00004030: 0a01 0402 0401 0401 0402 0801 04e2       ..............
```

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py` & `ares_ai-0.5.4/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/RAGAS_Scoring.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/RAG_Automatic_Evaluation/ppi.py` & `ares_ai-0.5.4/ares/RAG_Automatic_Evaluation/ppi.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/__pycache__/ares.cpython-310.pyc` & `ares_ai-0.5.4/ares/__pycache__/ares.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/__pycache__/ares.cpython-311.pyc` & `ares_ai-0.5.4/ares/__pycache__/ares.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/__pycache__/binary_classifier.cpython-310.pyc` & `ares_ai-0.5.4/ares/__pycache__/binary_classifier.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/__pycache__/binary_classifier.cpython-311.pyc` & `ares_ai-0.5.4/ares/__pycache__/binary_classifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/__pycache__/rag_scoring.cpython-310.pyc` & `ares_ai-0.5.4/ares/__pycache__/rag_scoring.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/__pycache__/rag_scoring.cpython-311.pyc` & `ares_ai-0.5.4/ares/__pycache__/rag_scoring.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/__pycache__/synthetic_generator.cpython-310.pyc` & `ares_ai-0.5.4/ares/__pycache__/synthetic_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/__pycache__/synthetic_generator.cpython-311.pyc` & `ares_ai-0.5.4/ares/__pycache__/synthetic_generator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/__pycache__/ues_idp.cpython-310.pyc` & `ares_ai-0.5.4/ares/__pycache__/ues_idp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/__pycache__/ues_idp.cpython-311.pyc` & `ares_ai-0.5.4/ares/__pycache__/ues_idp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/ares.py` & `ares_ai-0.5.4/ares/ares.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/ares_ai.egg-info/PKG-INFO` & `ares_ai-0.5.4/ares/ares_ai.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/ares_ai.egg-info/requires.txt` & `ares_ai-0.5.4/ares/ares_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/binary_classifier.py` & `ares_ai-0.5.4/ares/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/ppi/.DS_Store` & `ares_ai-0.5.4/ares/ppi/.DS_Store`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/ppi/ppi.py` & `ares_ai-0.5.4/ares/ppi/ppi.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/ppi/ppi_testing.py` & `ares_ai-0.5.4/ares/ppi/ppi_testing.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/rag_scoring.py` & `ares_ai-0.5.4/ares/rag_scoring.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/synthetic_generator.py` & `ares_ai-0.5.4/ares/synthetic_generator.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares/ues_idp.py` & `ares_ai-0.5.4/ares/ues_idp.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares_ai.egg-info/PKG-INFO` & `ares_ai-0.5.4/ares_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.2.4
+Version: 0.5.4
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -362,15 +362,15 @@
 OPTIONAL: You can run the following command to get the full NQ dataset! (347 MB)
 ```python
 from ares import ARES
 ares = ARES() 
 ares.KILT_dataset("nq")
 
 # Fetches NQ datasets with ratios including 0.5, 0.6, 0.7, etc.
-# For purposes of our quick start guide, we rename nq_ratio_0.5 to nq_unlabeled_output and nq_labeled_output.
+# For purposes of our quick start guide, we rename nq_ratio_0.5 to nq_unlabeled_output and nq_ratio_0.6 to nq_labeled_output.
 ```
 <hr>
 
 ### 🚀 Quick Start - #1
 
 <hr>
```

### Comparing `ares_ai-0.2.4/ares_ai.egg-info/SOURCES.txt` & `ares_ai-0.5.4/ares_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/ares_ai.egg-info/requires.txt` & `ares_ai-0.5.4/ares_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ares_ai-0.2.4/pyproject.toml` & `ares_ai-0.5.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ares-ai"
-version = "0.2.4"
+version = "0.5.4"
 description = """ 
 ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 utilizing fine-tuned classifiers and synthetic data to assess performance efficiently. It streamlines 
 the evaluation of context relevance, answer faithfulness, and answer relevance with minimal human annotations.
 """
 readme = "README.md"
 authors = [
```

### Comparing `ares_ai-0.2.4/requirements.txt` & `ares_ai-0.5.4/requirements.txt`

 * *Files identical despite different names*

