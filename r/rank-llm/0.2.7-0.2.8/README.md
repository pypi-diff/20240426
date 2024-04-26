# Comparing `tmp/rank-llm-0.2.7.tar.gz` & `tmp/rank-llm-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rank-llm-0.2.7.tar", last modified: Wed Feb  7 23:07:42 2024, max compression
+gzip compressed data, was "rank-llm-0.2.8.tar", last modified: Tue Feb 13 03:18:48 2024, max compression
```

## Comparing `rank-llm-0.2.7.tar` & `rank-llm-0.2.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 s8sharif  (1032) s8sharif  (1033)        0 2024-02-07 23:07:42.942552 rank-llm-0.2.7/
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     1064 2024-02-03 23:49:03.000000 rank-llm-0.2.7/CONTRIBUTING.md
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)    10766 2024-01-24 23:20:29.000000 rank-llm-0.2.7/LICENSE
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)       53 2024-01-24 23:20:29.000000 rank-llm-0.2.7/MANIFEST.in
--rw-r--r--   0 s8sharif  (1032) s8sharif  (1033)    16908 2024-02-07 23:07:42.942552 rank-llm-0.2.7/PKG-INFO
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)      841 2024-02-07 23:06:37.000000 rank-llm-0.2.7/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     3718 2024-02-07 23:07:22.000000 rank-llm-0.2.7/README.md
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     1459 2024-02-07 23:07:22.000000 rank-llm-0.2.7/pyproject.toml
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)      160 2024-02-03 23:49:03.000000 rank-llm-0.2.7/requirements.txt
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)       38 2024-02-07 23:07:42.942552 rank-llm-0.2.7/setup.cfg
-drwxrwxr-x   0 s8sharif  (1032) s8sharif  (1033)        0 2024-02-07 23:07:42.930553 rank-llm-0.2.7/src/
-drwxrwxr-x   0 s8sharif  (1032) s8sharif  (1033)        0 2024-02-07 23:07:42.930553 rank-llm-0.2.7/src/rank_llm/
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)        0 2024-01-24 23:20:29.000000 rank-llm-0.2.7/src/rank_llm/__init__.py
-drwxrwxr-x   0 s8sharif  (1032) s8sharif  (1033)        0 2024-02-07 23:07:42.938552 rank-llm-0.2.7/src/rank_llm/analysis/
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)        0 2024-01-24 23:20:29.000000 rank-llm-0.2.7/src/rank_llm/analysis/__init__.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)      186 2024-02-03 23:49:03.000000 rank-llm-0.2.7/src/rank_llm/analysis/estimate_costs.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     7564 2024-02-07 23:06:37.000000 rank-llm-0.2.7/src/rank_llm/analysis/response_analysis.py
-drwxrwxr-x   0 s8sharif  (1032) s8sharif  (1033)        0 2024-02-07 23:07:42.938552 rank-llm-0.2.7/src/rank_llm/evaluation/
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)        0 2024-01-24 23:20:29.000000 rank-llm-0.2.7/src/rank_llm/evaluation/__init__.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     6440 2024-02-07 23:06:37.000000 rank-llm-0.2.7/src/rank_llm/evaluation/trec_eval.py
-drwxrwxr-x   0 s8sharif  (1032) s8sharif  (1033)        0 2024-02-07 23:07:42.938552 rank-llm-0.2.7/src/rank_llm/rerank/
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)        0 2024-01-24 23:20:29.000000 rank-llm-0.2.7/src/rank_llm/rerank/__init__.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)      621 2024-02-03 23:49:03.000000 rank-llm-0.2.7/src/rank_llm/rerank/api_keys.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)    13969 2024-02-04 03:42:30.000000 rank-llm-0.2.7/src/rank_llm/rerank/rank_gpt.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     9009 2024-02-04 14:57:16.000000 rank-llm-0.2.7/src/rank_llm/rerank/rank_listwise_os_llm.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)    13113 2024-02-03 23:49:03.000000 rank-llm-0.2.7/src/rank_llm/rerank/rankllm.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     5530 2024-02-03 23:49:03.000000 rank-llm-0.2.7/src/rank_llm/rerank/reranker.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     2591 2024-02-03 04:29:37.000000 rank-llm-0.2.7/src/rank_llm/rerank/vicuna_reranker.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     2695 2024-02-03 04:29:37.000000 rank-llm-0.2.7/src/rank_llm/rerank/zephyr_reranker.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     1983 2024-02-03 23:49:03.000000 rank-llm-0.2.7/src/rank_llm/result.py
-drwxrwxr-x   0 s8sharif  (1032) s8sharif  (1033)        0 2024-02-07 23:07:42.942552 rank-llm-0.2.7/src/rank_llm/retrieve/
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)        0 2024-01-24 23:20:29.000000 rank-llm-0.2.7/src/rank_llm/retrieve/__init__.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     3169 2024-02-03 23:49:03.000000 rank-llm-0.2.7/src/rank_llm/retrieve/indices_dict.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)    13546 2024-02-04 14:57:22.000000 rank-llm-0.2.7/src/rank_llm/retrieve/pyserini_retriever.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)    11992 2024-02-04 14:57:22.000000 rank-llm-0.2.7/src/rank_llm/retrieve/retriever.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     1161 2024-01-24 23:20:29.000000 rank-llm-0.2.7/src/rank_llm/retrieve/topics_dict.py
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     5208 2024-02-03 23:49:03.000000 rank-llm-0.2.7/src/rank_llm/retrieve_and_rerank.py
-drwxrwxr-x   0 s8sharif  (1032) s8sharif  (1033)        0 2024-02-07 23:07:42.942552 rank-llm-0.2.7/src/rank_llm.egg-info/
--rw-r--r--   0 s8sharif  (1032) s8sharif  (1033)    16908 2024-02-07 23:07:42.000000 rank-llm-0.2.7/src/rank_llm.egg-info/PKG-INFO
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)     1024 2024-02-07 23:07:42.000000 rank-llm-0.2.7/src/rank_llm.egg-info/SOURCES.txt
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)        1 2024-02-07 23:07:42.000000 rank-llm-0.2.7/src/rank_llm.egg-info/dependency_links.txt
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)      160 2024-02-07 23:07:42.000000 rank-llm-0.2.7/src/rank_llm.egg-info/requires.txt
--rw-rw-r--   0 s8sharif  (1032) s8sharif  (1033)        9 2024-02-07 23:07:42.000000 rank-llm-0.2.7/src/rank_llm.egg-info/top_level.txt
+drwxr-xr-x   0 s8sharif (11119) jimmylin (11153)        0 2024-02-13 03:18:48.618915 rank-llm-0.2.8/
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     1064 2024-02-13 02:45:10.000000 rank-llm-0.2.8/CONTRIBUTING.md
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)    10766 2024-01-23 16:32:12.000000 rank-llm-0.2.8/LICENSE
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)       53 2024-01-23 16:32:12.000000 rank-llm-0.2.8/MANIFEST.in
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)    17115 2024-02-13 03:18:48.614915 rank-llm-0.2.8/PKG-INFO
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)      841 2024-02-13 02:45:10.000000 rank-llm-0.2.8/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     3925 2024-02-13 03:18:02.000000 rank-llm-0.2.8/README.md
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     1459 2024-02-13 03:18:02.000000 rank-llm-0.2.8/pyproject.toml
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)      160 2024-02-13 02:45:10.000000 rank-llm-0.2.8/requirements.txt
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)       38 2024-02-13 03:18:48.618915 rank-llm-0.2.8/setup.cfg
+drwxr-xr-x   0 s8sharif (11119) jimmylin (11153)        0 2024-02-13 03:18:48.586916 rank-llm-0.2.8/src/
+drwxr-xr-x   0 s8sharif (11119) jimmylin (11153)        0 2024-02-13 03:18:48.594915 rank-llm-0.2.8/src/rank_llm/
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)        0 2024-01-23 16:32:12.000000 rank-llm-0.2.8/src/rank_llm/__init__.py
+drwxr-xr-x   0 s8sharif (11119) jimmylin (11153)        0 2024-02-13 03:18:48.602915 rank-llm-0.2.8/src/rank_llm/analysis/
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)        0 2024-01-23 16:32:12.000000 rank-llm-0.2.8/src/rank_llm/analysis/__init__.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)      186 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/analysis/estimate_costs.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     7564 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/analysis/response_analysis.py
+drwxr-xr-x   0 s8sharif (11119) jimmylin (11153)        0 2024-02-13 03:18:48.602915 rank-llm-0.2.8/src/rank_llm/evaluation/
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)        0 2024-01-23 16:32:12.000000 rank-llm-0.2.8/src/rank_llm/evaluation/__init__.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     6440 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/evaluation/trec_eval.py
+drwxr-xr-x   0 s8sharif (11119) jimmylin (11153)        0 2024-02-13 03:18:48.610915 rank-llm-0.2.8/src/rank_llm/rerank/
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)        0 2024-01-23 16:32:12.000000 rank-llm-0.2.8/src/rank_llm/rerank/__init__.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)      621 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/rerank/api_keys.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)    13969 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/rerank/rank_gpt.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     9009 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/rerank/rank_listwise_os_llm.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)    13113 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/rerank/rankllm.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     5530 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/rerank/reranker.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     2591 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/rerank/vicuna_reranker.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     2695 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/rerank/zephyr_reranker.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     1983 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/result.py
+drwxr-xr-x   0 s8sharif (11119) jimmylin (11153)        0 2024-02-13 03:18:48.614915 rank-llm-0.2.8/src/rank_llm/retrieve/
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)        0 2024-01-23 16:32:12.000000 rank-llm-0.2.8/src/rank_llm/retrieve/__init__.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     3169 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/retrieve/indices_dict.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)    13546 2024-02-13 02:45:10.000000 rank-llm-0.2.8/src/rank_llm/retrieve/pyserini_retriever.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)    11993 2024-02-13 02:45:53.000000 rank-llm-0.2.8/src/rank_llm/retrieve/retriever.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     1161 2024-01-23 16:32:12.000000 rank-llm-0.2.8/src/rank_llm/retrieve/topics_dict.py
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     5209 2024-02-13 02:47:47.000000 rank-llm-0.2.8/src/rank_llm/retrieve_and_rerank.py
+drwxr-xr-x   0 s8sharif (11119) jimmylin (11153)        0 2024-02-13 03:18:48.614915 rank-llm-0.2.8/src/rank_llm.egg-info/
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)    17115 2024-02-13 03:18:48.000000 rank-llm-0.2.8/src/rank_llm.egg-info/PKG-INFO
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)     1024 2024-02-13 03:18:48.000000 rank-llm-0.2.8/src/rank_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)        1 2024-02-13 03:18:48.000000 rank-llm-0.2.8/src/rank_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)      160 2024-02-13 03:18:48.000000 rank-llm-0.2.8/src/rank_llm.egg-info/requires.txt
+-rw-r--r--   0 s8sharif (11119) jimmylin (11153)        9 2024-02-13 03:18:48.000000 rank-llm-0.2.8/src/rank_llm.egg-info/top_level.txt
```

### Comparing `rank-llm-0.2.7/CONTRIBUTING.md` & `rank-llm-0.2.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/LICENSE` & `rank-llm-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/PKG-INFO` & `rank-llm-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rank-llm
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Package for running prompt decoders like RankVicuna
 Author-email: Sahel Sharifymoghaddam <sahel.sharifymoghaddam@uwaterloo.ca>, Ronak Pradeep <rpradeep@uwaterloo.ca>, Jimmy Lin <jimmylin@uwaterloo.ca>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -216,18 +216,18 @@
 [![PyPI](https://img.shields.io/pypi/v/rank-llm?color=brightgreen)](https://pypi.org/project/rank-llm/)
 [![Downloads](https://static.pepy.tech/personalized-badge/rank-llm?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads)](https://pepy.tech/project/rank-llm)
 [![Downloads](https://static.pepy.tech/personalized-badge/rank-llm?period=week&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads/week)](https://pepy.tech/project/rank-llm)
 [![Generic badge](https://img.shields.io/badge/arXiv-2309.15088-red.svg)](https://arxiv.org/abs/2309.15088)
 [![LICENSE](https://img.shields.io/badge/license-Apache-blue.svg?style=flat)](https://www.apache.org/licenses/LICENSE-2.0)
 
 
-We offer a suite of prompt decoders, albeit with a current focus on RankVicuna. Some of the code in this repository is borrowed from [RankGPT](https://github.com/sunnweiwei/RankGPT)!
+We offer a suite of prompt-decoders, albeit with focus on open source LLMs compatible with [FastChat](https://github.com/lm-sys/FastChat?tab=readme-ov-file#supported-models) (e.g., Vicuna, Zephyr, etc.). Some of the code in this repository is borrowed from [RankGPT](https://github.com/sunnweiwei/RankGPT)!
 
 # Releases
-current_version = 0.2.7
+current_version = 0.2.8
 
 ## 📟 Instructions
 
 ### Create Conda Environment
 
 ```bash
 conda create -n rankllm python=3.10
@@ -270,30 +270,35 @@
 
 ## ✨ References
 
 If you use RankLLM, please cite the following relevant papers: 
 
 [[2309.15088] RankVicuna: Zero-Shot Listwise Document Reranking with Open-Source Large Language Models](https://arxiv.org/abs/2309.15088)
 
+<!-- {% raw %} -->
 ```
 @ARTICLE{pradeep2023rankvicuna,
   title   = {{RankVicuna}: Zero-Shot Listwise Document Reranking with Open-Source Large Language Models},
   author  = {Ronak Pradeep and Sahel Sharifymoghaddam and Jimmy Lin},
   year    = {2023},
   journal = {arXiv:2309.15088}
 }
 ```
+<!-- {% endraw %} -->
+
 
 [[2312.02724] RankZephyr: Effective and Robust Zero-Shot Listwise Reranking is a Breeze!](https://arxiv.org/abs/2312.02724)
 
+<!-- {% raw %} -->
 ```
 @ARTICLE{pradeep2023rankzephyr,
   title   = {{RankZephyr}: Effective and Robust Zero-Shot Listwise Reranking is a Breeze!},
   author  = {Ronak Pradeep and Sahel Sharifymoghaddam and Jimmy Lin},
   year    = {2023},
   journal = {arXiv:2312.02724}
 }
 ```
+<!-- {% endraw %} -->
 
 ## 🙏 Acknowledgments
 
 This research is supported in part by the Natural Sciences and Engineering Research Council (NSERC) of Canada.
```

### Comparing `rank-llm-0.2.7/PULL_REQUEST_TEMPLATE.md` & `rank-llm-0.2.8/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/README.md` & `rank-llm-0.2.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 [![PyPI](https://img.shields.io/pypi/v/rank-llm?color=brightgreen)](https://pypi.org/project/rank-llm/)
 [![Downloads](https://static.pepy.tech/personalized-badge/rank-llm?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads)](https://pepy.tech/project/rank-llm)
 [![Downloads](https://static.pepy.tech/personalized-badge/rank-llm?period=week&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads/week)](https://pepy.tech/project/rank-llm)
 [![Generic badge](https://img.shields.io/badge/arXiv-2309.15088-red.svg)](https://arxiv.org/abs/2309.15088)
 [![LICENSE](https://img.shields.io/badge/license-Apache-blue.svg?style=flat)](https://www.apache.org/licenses/LICENSE-2.0)
 
 
-We offer a suite of prompt decoders, albeit with a current focus on RankVicuna. Some of the code in this repository is borrowed from [RankGPT](https://github.com/sunnweiwei/RankGPT)!
+We offer a suite of prompt-decoders, albeit with focus on open source LLMs compatible with [FastChat](https://github.com/lm-sys/FastChat?tab=readme-ov-file#supported-models) (e.g., Vicuna, Zephyr, etc.). Some of the code in this repository is borrowed from [RankGPT](https://github.com/sunnweiwei/RankGPT)!
 
 # Releases
-current_version = 0.2.7
+current_version = 0.2.8
 
 ## 📟 Instructions
 
 ### Create Conda Environment
 
 ```bash
 conda create -n rankllm python=3.10
@@ -57,30 +57,35 @@
 
 ## ✨ References
 
 If you use RankLLM, please cite the following relevant papers: 
 
 [[2309.15088] RankVicuna: Zero-Shot Listwise Document Reranking with Open-Source Large Language Models](https://arxiv.org/abs/2309.15088)
 
+<!-- {% raw %} -->
 ```
 @ARTICLE{pradeep2023rankvicuna,
   title   = {{RankVicuna}: Zero-Shot Listwise Document Reranking with Open-Source Large Language Models},
   author  = {Ronak Pradeep and Sahel Sharifymoghaddam and Jimmy Lin},
   year    = {2023},
   journal = {arXiv:2309.15088}
 }
 ```
+<!-- {% endraw %} -->
+
 
 [[2312.02724] RankZephyr: Effective and Robust Zero-Shot Listwise Reranking is a Breeze!](https://arxiv.org/abs/2312.02724)
 
+<!-- {% raw %} -->
 ```
 @ARTICLE{pradeep2023rankzephyr,
   title   = {{RankZephyr}: Effective and Robust Zero-Shot Listwise Reranking is a Breeze!},
   author  = {Ronak Pradeep and Sahel Sharifymoghaddam and Jimmy Lin},
   year    = {2023},
   journal = {arXiv:2312.02724}
 }
 ```
+<!-- {% endraw %} -->
 
 ## 🙏 Acknowledgments
 
 This research is supported in part by the Natural Sciences and Engineering Research Council (NSERC) of Canada.
```

### Comparing `rank-llm-0.2.7/pyproject.toml` & `rank-llm-0.2.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rank-llm"
-version = "0.2.7"
+version = "0.2.8"
 description = "A Package for running prompt decoders like RankVicuna"
 readme = "README.md"
 authors = [
     { name = "Sahel Sharifymoghaddam", email = "sahel.sharifymoghaddam@uwaterloo.ca" },
     { name = "Ronak Pradeep", email = "rpradeep@uwaterloo.ca" },
     { name = "Jimmy Lin", email = "jimmylin@uwaterloo.ca" },
 ]
@@ -26,15 +26,15 @@
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.urls]
 Homepage = "https://github.com/castorini/rank_llm"
 
 [tool.bumpver]
-current_version = "0.2.7"
+current_version = "0.2.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
```

### Comparing `rank-llm-0.2.7/src/rank_llm/analysis/response_analysis.py` & `rank-llm-0.2.8/src/rank_llm/analysis/response_analysis.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/evaluation/trec_eval.py` & `rank-llm-0.2.8/src/rank_llm/evaluation/trec_eval.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/rerank/api_keys.py` & `rank-llm-0.2.8/src/rank_llm/rerank/api_keys.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/rerank/rank_gpt.py` & `rank-llm-0.2.8/src/rank_llm/rerank/rank_gpt.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/rerank/rank_listwise_os_llm.py` & `rank-llm-0.2.8/src/rank_llm/rerank/rank_listwise_os_llm.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/rerank/rankllm.py` & `rank-llm-0.2.8/src/rank_llm/rerank/rankllm.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/rerank/reranker.py` & `rank-llm-0.2.8/src/rank_llm/rerank/reranker.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/rerank/vicuna_reranker.py` & `rank-llm-0.2.8/src/rank_llm/rerank/vicuna_reranker.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/rerank/zephyr_reranker.py` & `rank-llm-0.2.8/src/rank_llm/rerank/zephyr_reranker.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/result.py` & `rank-llm-0.2.8/src/rank_llm/result.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/retrieve/indices_dict.py` & `rank-llm-0.2.8/src/rank_llm/retrieve/indices_dict.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/retrieve/pyserini_retriever.py` & `rank-llm-0.2.8/src/rank_llm/retrieve/pyserini_retriever.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/retrieve/retriever.py` & `rank-llm-0.2.8/src/rank_llm/retrieve/retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         if not hits:
             raise ValueError("Please provide a non-empty list of hits.")
 
         retriever = Retriever(RetrievalMode.QUERY_AND_HITS, dataset=hits, query=query)
         return retriever.retrieve()
 
     @staticmethod
-    def from_dataset_with_prebuit_index(
+    def from_dataset_with_prebuilt_index(
         dataset_name: str,
         retrieval_method: RetrievalMethod = RetrievalMethod.BM25,
         k: int = 100,
     ):
         """
         Creates a Retriever instance for a dataset with a prebuilt index.
```

### Comparing `rank-llm-0.2.7/src/rank_llm/retrieve/topics_dict.py` & `rank-llm-0.2.8/src/rank_llm/retrieve/topics_dict.py`

 * *Files identical despite different names*

### Comparing `rank-llm-0.2.7/src/rank_llm/retrieve_and_rerank.py` & `rank-llm-0.2.8/src/rank_llm/retrieve_and_rerank.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         )
     else:
         raise ValueError(f"Unsupported model: {model_path}")
 
     # Retrieve
     print("Retrieving:")
     if retrieval_mode == RetrievalMode.DATASET:
-        retrieved_results = Retriever.from_dataset_with_prebuit_index(
+        retrieved_results = Retriever.from_dataset_with_prebuilt_index(
             dataset_name=dataset, retrieval_method=retrieval_method
         )
     elif retrieval_mode == RetrievalMode.QUERY_AND_DOCUMENTS:
         retrieved_results = Retriever.from_inline_documents(
             query=query, documents=dataset
         )
     elif retrieval_mode == RetrievalMode.QUERY_AND_HITS:
```

### Comparing `rank-llm-0.2.7/src/rank_llm.egg-info/PKG-INFO` & `rank-llm-0.2.8/src/rank_llm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rank-llm
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Package for running prompt decoders like RankVicuna
 Author-email: Sahel Sharifymoghaddam <sahel.sharifymoghaddam@uwaterloo.ca>, Ronak Pradeep <rpradeep@uwaterloo.ca>, Jimmy Lin <jimmylin@uwaterloo.ca>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -216,18 +216,18 @@
 [![PyPI](https://img.shields.io/pypi/v/rank-llm?color=brightgreen)](https://pypi.org/project/rank-llm/)
 [![Downloads](https://static.pepy.tech/personalized-badge/rank-llm?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads)](https://pepy.tech/project/rank-llm)
 [![Downloads](https://static.pepy.tech/personalized-badge/rank-llm?period=week&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads/week)](https://pepy.tech/project/rank-llm)
 [![Generic badge](https://img.shields.io/badge/arXiv-2309.15088-red.svg)](https://arxiv.org/abs/2309.15088)
 [![LICENSE](https://img.shields.io/badge/license-Apache-blue.svg?style=flat)](https://www.apache.org/licenses/LICENSE-2.0)
 
 
-We offer a suite of prompt decoders, albeit with a current focus on RankVicuna. Some of the code in this repository is borrowed from [RankGPT](https://github.com/sunnweiwei/RankGPT)!
+We offer a suite of prompt-decoders, albeit with focus on open source LLMs compatible with [FastChat](https://github.com/lm-sys/FastChat?tab=readme-ov-file#supported-models) (e.g., Vicuna, Zephyr, etc.). Some of the code in this repository is borrowed from [RankGPT](https://github.com/sunnweiwei/RankGPT)!
 
 # Releases
-current_version = 0.2.7
+current_version = 0.2.8
 
 ## 📟 Instructions
 
 ### Create Conda Environment
 
 ```bash
 conda create -n rankllm python=3.10
@@ -270,30 +270,35 @@
 
 ## ✨ References
 
 If you use RankLLM, please cite the following relevant papers: 
 
 [[2309.15088] RankVicuna: Zero-Shot Listwise Document Reranking with Open-Source Large Language Models](https://arxiv.org/abs/2309.15088)
 
+<!-- {% raw %} -->
 ```
 @ARTICLE{pradeep2023rankvicuna,
   title   = {{RankVicuna}: Zero-Shot Listwise Document Reranking with Open-Source Large Language Models},
   author  = {Ronak Pradeep and Sahel Sharifymoghaddam and Jimmy Lin},
   year    = {2023},
   journal = {arXiv:2309.15088}
 }
 ```
+<!-- {% endraw %} -->
+
 
 [[2312.02724] RankZephyr: Effective and Robust Zero-Shot Listwise Reranking is a Breeze!](https://arxiv.org/abs/2312.02724)
 
+<!-- {% raw %} -->
 ```
 @ARTICLE{pradeep2023rankzephyr,
   title   = {{RankZephyr}: Effective and Robust Zero-Shot Listwise Reranking is a Breeze!},
   author  = {Ronak Pradeep and Sahel Sharifymoghaddam and Jimmy Lin},
   year    = {2023},
   journal = {arXiv:2312.02724}
 }
 ```
+<!-- {% endraw %} -->
 
 ## 🙏 Acknowledgments
 
 This research is supported in part by the Natural Sciences and Engineering Research Council (NSERC) of Canada.
```

### Comparing `rank-llm-0.2.7/src/rank_llm.egg-info/SOURCES.txt` & `rank-llm-0.2.8/src/rank_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

