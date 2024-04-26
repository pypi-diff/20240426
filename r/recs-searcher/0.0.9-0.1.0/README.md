# Comparing `tmp/recs-searcher-0.0.9.tar.gz` & `tmp/recs-searcher-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recs-searcher-0.0.9.tar", last modified: Sun Apr 21 15:21:54 2024, max compression
+gzip compressed data, was "recs-searcher-0.1.0.tar", last modified: Fri Apr 26 12:06:52 2024, max compression
```

## Comparing `recs-searcher-0.0.9.tar` & `recs-searcher-0.1.0.tar`

### file list

```diff
@@ -1,57 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.797312 recs-searcher-0.0.9/
--rw-rw-rw-   0        0        0    11558 2023-12-10 08:31:53.000000 recs-searcher-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     2020 2024-04-21 15:21:54.785313 recs-searcher-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1208 2024-03-21 10:34:47.000000 recs-searcher-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.120318 recs-searcher-0.0.9/recs_searcher/
--rw-rw-rw-   0        0        0      188 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.155314 recs-searcher-0.0.9/recs_searcher/api/
--rw-rw-rw-   0        0        0       20 2024-02-20 13:20:56.000000 recs-searcher-0.0.9/recs_searcher/api/__init__.py
--rw-rw-rw-   0        0        0    15662 2024-04-14 15:18:10.000000 recs-searcher-0.0.9/recs_searcher/api/api.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.196313 recs-searcher-0.0.9/recs_searcher/augmentation/
--rw-rw-rw-   0        0        0       82 2024-03-21 12:35:06.000000 recs-searcher-0.0.9/recs_searcher/augmentation/__init__.py
--rw-rw-rw-   0        0        0      101 2024-03-21 12:30:21.000000 recs-searcher-0.0.9/recs_searcher/augmentation/_actions.py
--rw-rw-rw-   0        0        0     2951 2024-03-21 12:13:07.000000 recs-searcher-0.0.9/recs_searcher/augmentation/_base.py
--rw-rw-rw-   0        0        0     3283 2024-03-21 12:34:55.000000 recs-searcher-0.0.9/recs_searcher/augmentation/_char_aug.py
--rw-rw-rw-   0        0        0     2615 2024-03-21 12:34:58.000000 recs-searcher-0.0.9/recs_searcher/augmentation/_word_aug.py
--rw-rw-rw-   0        0        0    16750 2024-04-14 14:08:26.000000 recs-searcher-0.0.9/recs_searcher/base.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.246311 recs-searcher-0.0.9/recs_searcher/dataset/
--rw-rw-rw-   0        0        0       50 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/dataset/__init__.py
--rw-rw-rw-   0        0        0     1112 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/dataset/_base.py
--rw-rw-rw-   0        0        0     5723 2024-03-21 15:15:56.000000 recs-searcher-0.0.9/recs_searcher/dataset/_dataframes.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.577312 recs-searcher-0.0.9/recs_searcher/dataset/data/
--rw-rw-rw-   0        0        0        0 2023-09-29 14:44:09.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/__init__.py
--rw-rw-rw-   0        0        0 12021233 2023-09-29 14:39:29.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/address_krasnoyarsk.csv
--rw-rw-rw-   0        0        0    19744 2023-09-28 15:28:01.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/city_russia.csv
--rw-rw-rw-   0        0        0   214881 2023-09-28 15:25:56.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/company_russia.csv
--rw-rw-rw-   0        0        0    74441 2023-09-28 15:12:48.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/exoplanets.csv
--rw-rw-rw-   0        0        0    34438 2023-09-28 15:13:00.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/medical_supplies.csv
--rw-rw-rw-   0        0        0     4345 2023-09-28 15:13:03.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/mobile_phones.csv
--rw-rw-rw-   0        0        0  1050450 2024-03-21 15:14:59.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/russian_dictionary.csv
--rw-rw-rw-   0        0        0   309849 2023-10-01 17:08:19.000000 recs-searcher-0.0.9/recs_searcher/dataset/data/video_games.csv
-drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.598311 recs-searcher-0.0.9/recs_searcher/embeddings/
--rw-rw-rw-   0        0        0       22 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/embeddings/__init__.py
--rw-rw-rw-   0        0        0     7199 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/embeddings/_base.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.615312 recs-searcher-0.0.9/recs_searcher/explain/
--rw-rw-rw-   0        0        0       22 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/explain/__init__.py
--rw-rw-rw-   0        0        0     3278 2024-04-14 12:54:59.000000 recs-searcher-0.0.9/recs_searcher/explain/_base.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.651315 recs-searcher-0.0.9/recs_searcher/preprocessing/
--rw-rw-rw-   0        0        0       60 2023-12-22 09:05:10.000000 recs-searcher-0.0.9/recs_searcher/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     6186 2024-04-14 15:37:15.000000 recs-searcher-0.0.9/recs_searcher/preprocessing/_base_clear.py
--rw-rw-rw-   0        0        0     2154 2024-04-14 15:38:26.000000 recs-searcher-0.0.9/recs_searcher/preprocessing/_base_normalize.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.674311 recs-searcher-0.0.9/recs_searcher/similarity_search/
--rw-rw-rw-   0        0        0       48 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/similarity_search/__init__.py
--rw-rw-rw-   0        0        0     8170 2024-04-14 15:40:23.000000 recs-searcher-0.0.9/recs_searcher/similarity_search/_base.py
--rw-rw-rw-   0        0        0     2490 2024-04-14 15:45:59.000000 recs-searcher-0.0.9/recs_searcher/similarity_search/_validate.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.760313 recs-searcher-0.0.9/recs_searcher/utils/
--rw-rw-rw-   0        0        0       96 2024-03-13 07:55:35.000000 recs-searcher-0.0.9/recs_searcher/utils/__init__.py
--rw-rw-rw-   0        0        0     1637 2024-04-14 15:46:47.000000 recs-searcher-0.0.9/recs_searcher/utils/_concat_embeddings.py
--rw-rw-rw-   0        0        0      729 2024-04-14 15:48:15.000000 recs-searcher-0.0.9/recs_searcher/utils/_create_date_name.py
--rw-rw-rw-   0        0        0      712 2024-04-14 15:29:21.000000 recs-searcher-0.0.9/recs_searcher/utils/_distances.py
-drwxrwxrwx   0        0        0        0 2024-04-21 15:21:54.780315 recs-searcher-0.0.9/recs_searcher.egg-info/
--rw-rw-rw-   0        0        0     2020 2024-04-21 15:21:53.000000 recs-searcher-0.0.9/recs_searcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1571 2024-04-21 15:21:53.000000 recs-searcher-0.0.9/recs_searcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 15:21:53.000000 recs-searcher-0.0.9/recs_searcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2024-04-21 15:21:53.000000 recs-searcher-0.0.9/recs_searcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-21 15:21:53.000000 recs-searcher-0.0.9/recs_searcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-21 15:21:54.799312 recs-searcher-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1061 2024-04-21 15:21:17.000000 recs-searcher-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.506271 recs-searcher-0.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-12-10 08:31:53.000000 recs-searcher-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2043 2024-04-26 12:06:52.504274 recs-searcher-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1208 2024-03-21 10:34:47.000000 recs-searcher-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:50.200159 recs-searcher-0.1.0/recs_searcher/
+-rw-rw-rw-   0        0        0      188 2024-03-13 07:55:35.000000 recs-searcher-0.1.0/recs_searcher/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:50.239162 recs-searcher-0.1.0/recs_searcher/api/
+-rw-rw-rw-   0        0        0       20 2024-02-20 13:20:56.000000 recs-searcher-0.1.0/recs_searcher/api/__init__.py
+-rw-rw-rw-   0        0        0    17684 2024-04-25 14:15:29.000000 recs-searcher-0.1.0/recs_searcher/api/api.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:50.263159 recs-searcher-0.1.0/recs_searcher/augmentation/
+-rw-rw-rw-   0        0        0       82 2024-03-21 12:35:06.000000 recs-searcher-0.1.0/recs_searcher/augmentation/__init__.py
+-rw-rw-rw-   0        0        0      101 2024-03-21 12:30:21.000000 recs-searcher-0.1.0/recs_searcher/augmentation/_actions.py
+-rw-rw-rw-   0        0        0     2951 2024-03-21 12:13:07.000000 recs-searcher-0.1.0/recs_searcher/augmentation/_base.py
+-rw-rw-rw-   0        0        0     3283 2024-04-25 16:01:50.000000 recs-searcher-0.1.0/recs_searcher/augmentation/_char_aug.py
+-rw-rw-rw-   0        0        0     2615 2024-03-21 12:34:58.000000 recs-searcher-0.1.0/recs_searcher/augmentation/_word_aug.py
+-rw-rw-rw-   0        0        0    22723 2024-04-25 14:47:33.000000 recs-searcher-0.1.0/recs_searcher/base.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:50.272159 recs-searcher-0.1.0/recs_searcher/dataset/
+-rw-rw-rw-   0        0        0       50 2024-03-13 07:55:35.000000 recs-searcher-0.1.0/recs_searcher/dataset/__init__.py
+-rw-rw-rw-   0        0        0     1196 2024-04-24 16:50:37.000000 recs-searcher-0.1.0/recs_searcher/dataset/_base.py
+-rw-rw-rw-   0        0        0     5723 2024-04-25 15:57:26.000000 recs-searcher-0.1.0/recs_searcher/dataset/_dataframes.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.407219 recs-searcher-0.1.0/recs_searcher/dataset/data/
+-rw-rw-rw-   0        0        0        0 2023-09-29 14:44:09.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/__init__.py
+-rw-rw-rw-   0        0        0 12021233 2023-09-29 14:39:29.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/address_krasnoyarsk.csv
+-rw-rw-rw-   0        0        0    19744 2023-09-28 15:28:01.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/city_russia.csv
+-rw-rw-rw-   0        0        0   214881 2023-09-28 15:25:56.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/company_russia.csv
+-rw-rw-rw-   0        0        0    74441 2023-09-28 15:12:48.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/exoplanets.csv
+-rw-rw-rw-   0        0        0    34438 2023-09-28 15:13:00.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/medical_supplies.csv
+-rw-rw-rw-   0        0        0     4345 2023-09-28 15:13:03.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/mobile_phones.csv
+-rw-rw-rw-   0        0        0  1050450 2024-03-21 15:14:59.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/russian_dictionary.csv
+-rw-rw-rw-   0        0        0   309849 2023-10-01 17:08:19.000000 recs-searcher-0.1.0/recs_searcher/dataset/data/video_games.csv
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.426087 recs-searcher-0.1.0/recs_searcher/embeddings/
+-rw-rw-rw-   0        0        0       22 2024-03-13 07:55:35.000000 recs-searcher-0.1.0/recs_searcher/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     7199 2024-03-13 07:55:35.000000 recs-searcher-0.1.0/recs_searcher/embeddings/_base.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.431270 recs-searcher-0.1.0/recs_searcher/explain/
+-rw-rw-rw-   0        0        0       22 2024-03-13 07:55:35.000000 recs-searcher-0.1.0/recs_searcher/explain/__init__.py
+-rw-rw-rw-   0        0        0     3806 2024-04-25 10:27:27.000000 recs-searcher-0.1.0/recs_searcher/explain/_base.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.439274 recs-searcher-0.1.0/recs_searcher/preprocessing/
+-rw-rw-rw-   0        0        0       60 2023-12-22 09:05:10.000000 recs-searcher-0.1.0/recs_searcher/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     6186 2024-04-14 15:37:15.000000 recs-searcher-0.1.0/recs_searcher/preprocessing/_base_clear.py
+-rw-rw-rw-   0        0        0     2154 2024-04-14 15:38:26.000000 recs-searcher-0.1.0/recs_searcher/preprocessing/_base_normalize.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.449273 recs-searcher-0.1.0/recs_searcher/similarity_search/
+-rw-rw-rw-   0        0        0       48 2024-03-13 07:55:35.000000 recs-searcher-0.1.0/recs_searcher/similarity_search/__init__.py
+-rw-rw-rw-   0        0        0     8199 2024-04-25 13:43:04.000000 recs-searcher-0.1.0/recs_searcher/similarity_search/_base.py
+-rw-rw-rw-   0        0        0     2490 2024-04-14 15:45:59.000000 recs-searcher-0.1.0/recs_searcher/similarity_search/_validate.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.478268 recs-searcher-0.1.0/recs_searcher/utils/
+-rw-rw-rw-   0        0        0       96 2024-04-23 13:32:03.000000 recs-searcher-0.1.0/recs_searcher/utils/__init__.py
+-rw-rw-rw-   0        0        0     1637 2024-04-14 15:46:47.000000 recs-searcher-0.1.0/recs_searcher/utils/_concat_embeddings.py
+-rw-rw-rw-   0        0        0      729 2024-04-14 15:48:15.000000 recs-searcher-0.1.0/recs_searcher/utils/_create_date_name.py
+-rw-rw-rw-   0        0        0      712 2024-04-14 15:29:21.000000 recs-searcher-0.1.0/recs_searcher/utils/_distances.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.501270 recs-searcher-0.1.0/recs_searcher.egg-info/
+-rw-rw-rw-   0        0        0     2043 2024-04-26 12:06:44.000000 recs-searcher-0.1.0/recs_searcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1696 2024-04-26 12:06:45.000000 recs-searcher-0.1.0/recs_searcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 12:06:44.000000 recs-searcher-0.1.0/recs_searcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2024-04-26 12:06:44.000000 recs-searcher-0.1.0/recs_searcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-26 12:06:44.000000 recs-searcher-0.1.0/recs_searcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 12:06:52.510271 recs-searcher-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1076 2024-04-26 12:06:00.000000 recs-searcher-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:06:52.498270 recs-searcher-0.1.0/tests/
+-rw-rw-rw-   0        0        0      537 2024-04-25 16:04:59.000000 recs-searcher-0.1.0/tests/test_augmentation.py
+-rw-rw-rw-   0        0        0      265 2024-04-25 15:57:29.000000 recs-searcher-0.1.0/tests/test_dataset.py
+-rw-rw-rw-   0        0        0      973 2024-04-25 15:42:46.000000 recs-searcher-0.1.0/tests/test_embeddings.py
+-rw-rw-rw-   0        0        0     2770 2024-04-25 15:41:42.000000 recs-searcher-0.1.0/tests/test_pipeline.py
+-rw-rw-rw-   0        0        0      960 2024-04-25 15:54:07.000000 recs-searcher-0.1.0/tests/test_preprocessing.py
```

### Comparing `recs-searcher-0.0.9/LICENSE` & `recs-searcher-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/PKG-INFO` & `recs-searcher-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recs-searcher
-Version: 0.0.9
+Version: 0.1.0
 Summary: Search engine and registry error corrector
 Home-page: https://github.com/sheriff1max/recs-searcher
 Author: sheriff1max
 Author-email: kobelevmaxim48@gmail.com
 Project-URL: Bug tracker, https://github.com/sheriff1max/recs-searcher/issues
 Keywords: python searcher corrector faiss chroma-bd embeddings
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,15 @@
 Requires-Dist: sentence-transformers
 Requires-Dist: pymorphy3
 Requires-Dist: scikit-learn
 Requires-Dist: spacy
 Requires-Dist: thefuzz
 Requires-Dist: torch
 Requires-Dist: torchvision
+Requires-Dist: pytest
 
 # recs-searcher (Registry error correction system - Searcher)
 
     pip install recs-searcher
 
 Система способна решить следующие задачи:
 1. Исправление реестровых ошибок пользовательского ввода при сравнении с базой данных;
```

### Comparing `recs-searcher-0.0.9/README.md` & `recs-searcher-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/api/api.py` & `recs-searcher-0.1.0/recs_searcher/api/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """ api.py
 Взаимодействие с системой."""
 
-from typing import List, Iterable, Dict, Type, Optional, Union, Tuple
+from typing import List, Iterable, Dict, Type, Optional, Union, Tuple, Literal
 
 from ..base import(
     BaseTransformation,
     BaseEmbedding,
     BaseSearch,
     BaseExplain,
 )
+from ..similarity_search import *
 from ..similarity_search import Validate
 
 import numpy as np
 import pandas as pd
 from pathlib import Path
 import pickle
 
@@ -71,16 +72,16 @@
         # Если True - обучаем модель для создания эмбеддингов.
         if isinstance(model, BaseEmbedding):
             self.__verbose('The training of the model has begun...', verbose)
             self._embedding_database = self.__fit_transform(self._model, self._clear_dataset)
 
         self.__type_explainer = explainer
 
-        # Класс поисковика для будущего дообучения.
-        self.__type_searcher = searcher
+        # Название поисковика.
+        self.__type_searcher = searcher.__name__  # TODO: костыль. Фиксит краш при сохранении ChromaDBSearcher
         self.__searcher_args = searcher_args
 
         self._searcher = self.__create_searcher(
             searcher=self.__type_searcher,
             model=self._model,
             embedding_database=self._embedding_database,
             original_array=self._original_dataset,
@@ -156,29 +157,29 @@
             Датасет в виде эмбеддингов.
         """
         embedding_database = model.fit_transform(dataset)
         return embedding_database
 
     def __create_searcher(
         self,
-        searcher: Type[BaseSearch],
+        searcher: str,
         model: Optional[BaseEmbedding],
         embedding_database: np.ndarray,
         original_array: Iterable[str],
         preprocessing: List[BaseTransformation],
         clear_array: Iterable[str],
         searcher_args: dict,
     ) -> BaseSearch:
         """
         Инициализация поискового алгоритма.
 
         Параметры
         ----------
-        searcher : Type[BaseSearch]
-            Тип поискового алгоритма.
+        searcher : str
+            Название поискового алгоритма.
         model : BaseEmbedding
             Модель для обучения.
         embedding_database : np.ndarray
             Датасет в виде эмбеддингов.
         original_array : Iterable[str]
             Исходный датасет.
         preprocessing : List[BaseTransformation]
@@ -189,14 +190,15 @@
             Словарь аргументов для поискового алгоритма.
 
         Returns
         -------
         searcher: BaseSearch
             Инициализированный объект поискового алгоритма.
         """
+        searcher = eval(searcher)
         if isinstance(model, BaseEmbedding):
             return searcher(
                 model=model,
                 embedding_database=embedding_database,
                 original_array=original_array,
                 preprocessing=preprocessing,
                 clear_array=clear_array,
@@ -211,15 +213,15 @@
 
     def get_model(self) -> Optional[BaseEmbedding]:
         return self._model
 
     def get_preprocessing(self) -> Optional[List[BaseTransformation]]:
         return self._preprocessing
 
-    def load(self, path_to_filename: str) -> object:
+    def load(self, path_to_filename: str) -> 'Pipeline':
         """
         Загрузка pipeline из файла.
 
         Параметры
         ----------
         path_to_filename : str
             Путь до файла.
@@ -252,14 +254,17 @@
         if not path_folder_save.exists():
             path_folder_save.mkdir()
 
         if '.pkl' not in filename:
             filename += '.pkl'
         path = path_folder_save / filename
 
+        # Удаляем объект поискового алгоритма для уменьшения объёма файла.
+        self._searcher = None
+
         with open(path, 'wb') as f:
             pickle.dump(self, f)
         return self
 
     def validate(
         self,
         augmentation_transforms: List[BaseTransformation],
@@ -315,50 +320,66 @@
         """
         return self._searcher.search(text, k, ascending=ascending)
 
     def explain(
         self,
         compared_text: str,
         original_text: str,
-        n_grams: Union[Tuple[int, int], int] = 1,
-        k: int = 10,
-        ascending: bool = True,
+        n_grams: Optional[Union[Tuple[int, int], int]] = 1,
+        analyzer: Optional[Literal['word', 'char']] = 'word',
+        sep: Optional[str] = ' ',
+        k: Optional[int] = 10,
+        ascending: Optional[bool] = True,
         **explainer_args
-    ) -> pd.DataFrame:
-        """Поиск наиболее схожих k-текстов из БД на text пользователя.
+    ) -> Tuple[pd.DataFrame, List[Tuple[int, int]]]:
+        """
+        Поиск наиболее схожих N-грамм из `compared_text` в `original_text`.
 
         Параметры
         ----------
-        text : str
-            Пользовательский текст, которому нужно найти наиболее
-            схожий текст из БД.
-        k : int
+        compared_text : str
+            Пользовательский текст, в котором нужно найти n-граммы,
+            похожие на original_text.
+        original_text : str
+            Текст, с которым сравнивается compared_text.
+        n_grams : Optional[Union[Tuple[int, int], int]]
+            Длины N-грамм, которые будут оцениваться.
+            Может приниматься либо одно число, либо список чисел.
+        analyzer: Optional[Literal['word', 'char']]
+            Считать схожесть текстов на основе N-грамм слов или символов.
+        sep: Optional[str]
+            Разделитель слов.
+        k : Optional[int]
             Кол-во выдаваемых результатов.
-        ascending : bool
+        ascending : Optional[bool]
             Флаг сортировки полученных результатов.
             False - убывающая, True - возрастающая сортировка.
 
         Returns
         -------
         df: pd.DataFrame
             Датафрейм с результатами.
             df.columns = ['text', 'similarity']
+        indeces_n_grams: List[Tuple[int, int]]
+            Список кортежей индексов старта и конца самых важных N-грамм из `df`.
         """
         if self.__type_explainer is None:
             raise ValueError(f'The `explainer` parameter was not declared during initialization.')
 
         explainer = self.__type_explainer(
             model=self.get_model(),
             preprocessing=self.get_preprocessing(),
             **explainer_args,
         )
         return explainer.explain(
             compared_text=compared_text,
             original_text=original_text,
             n_grams=n_grams,
+            analyzer=analyzer,
+            sep=sep,
             k=k,
             ascending=ascending,
         )
 
     def fine_tuning(self, dataset: Iterable[str]) -> object:
         """
         Дообучение пайплайна на новых данных.
@@ -383,44 +404,64 @@
             verbose=True,
             **self.__searcher_args,
         )
         return self
 
     def change_searcher(
         self,
-        searcher: Type[BaseSearch],
+        searcher: Optional[Type[BaseSearch]] = None,
         **searcher_args,
     ) -> None:
         """
-        Изменение поискового алгоритма.
+        Изменение или пересоздание поискового алгоритма.
 
         Параметры
         ----------
-        searcher : Type[BaseSearch]
+        searcher : Optional[Type[BaseSearch]]
             Тип поискового алгоритма.
-        searcher_args : dict
+        searcher_args : Optional[dict]
             Словарь аргументов для поискового алгоритма.
 
         Returns
         -------
         None
         """
-        self.__type_searcher = searcher
-        self.__searcher_args = searcher_args
+        if searcher:
+            self.__type_searcher = searcher.__name__
+        if searcher_args:
+            self.__searcher_args = searcher_args
 
         self._searcher = self.__create_searcher(
             searcher=self.__type_searcher,
             model=self._model,
             embedding_database=self._embedding_database,
             original_array=self._original_dataset,
             preprocessing=self._preprocessing,
             clear_array=self._clear_dataset,
-            searcher_args=searcher_args,
+            searcher_args=self.__searcher_args,
         )
 
+    def change_explainer(
+        self,
+        explainer: Type[BaseExplain],
+    ) -> None:
+        """
+        Изменение алгоритма для интерпретации результатов.
+
+        Параметры
+        ----------
+        explainer : Type[BaseExplain]
+            Тип алгоритма для интерпретации результатов.
+
+        Returns
+        -------
+        None
+        """
+        self.__type_explainer = explainer
+
 
 def load_pipeline(path_to_filename: str) -> Pipeline:
     """
     Загрузка pipeline из файла.
 
     Параметры
     ----------
@@ -434,8 +475,9 @@
     """
     if '.pkl' not in path_to_filename:
         path_to_filename += '.pkl'
 
     path_to_filename = Path(path_to_filename)
     with open(path_to_filename, 'rb') as f:
         pipeline = pickle.load(f)
+    pipeline.change_searcher()
     return pipeline
```

### Comparing `recs-searcher-0.0.9/recs_searcher/augmentation/_base.py` & `recs-searcher-0.1.0/recs_searcher/augmentation/_base.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/augmentation/_char_aug.py` & `recs-searcher-0.1.0/recs_searcher/augmentation/_char_aug.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/augmentation/_word_aug.py` & `recs-searcher-0.1.0/recs_searcher/augmentation/_word_aug.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/base.py` & `recs-searcher-0.1.0/recs_searcher/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Базовые классы модуля.
 """
 
 
 from abc import ABC, abstractmethod
 from pathlib import Path
 import pickle
-from typing import Iterable, List, Optional, Union, Tuple
+from typing import Iterable, List, Literal, Optional, Union, Tuple
 import random
 
 import pandas as pd
 import numpy as np
 
 import pathlib
 import platform
@@ -177,23 +177,30 @@
             self._clear_text = self._preprocessing_text(original_array, preprocessing)
 
     def _preprocessing_text(
         self,
         text: Union[Iterable[str], str],
         preprocessing: List[BaseTransformation],
     ) -> Union[List[str], str]:
-        """"""
-        if isinstance(text, str):
-            for transformator in preprocessing:
-                tmp_text = transformator.transform([text])[0]
-                if tmp_text:
-                    text = tmp_text
-        else:
-            for transformator in preprocessing:
-                text = transformator.transform(text)
+        """
+        Предобработка текста.
+
+        Параметры
+        ----------
+        text : Union[Iterable[str], str]
+            Необработанный текст.
+        preprocessing : List[BaseTransformation]
+            Список алгоритмов для предобработка текста.
+
+        Returns
+        -------
+        text: Union[List[str], str]
+            Обработанный текст.
+        """
+        text = _preprocessing_text(text, preprocessing)
         return text
 
     @abstractmethod
     def _search(
         self,
         clear_text: str,
         k: int,
@@ -345,116 +352,269 @@
         preprocessing: List[BaseTransformation] = [],
     ):
         self._model = model
         self._preprocessing = preprocessing
 
     def _preprocessing_text(
         self,
-        text: str,
+        text: Union[Iterable[str], str],
         preprocessing: List[BaseTransformation],
-    ) -> str:
+    ) -> Union[List[str], str]:
         """
         Предобработка текста.
 
         Параметры
         ----------
-        text : str
+        text : Union[Iterable[str], str]
             Необработанный текст.
         preprocessing : List[BaseTransformation]
             Список алгоритмов для предобработка текста.
 
         Returns
         -------
-        text: str
+        text: Union[List[str], str]
             Обработанный текст.
         """
-        for transformator in preprocessing:
-            tmp_text = transformator.transform([text])[0]
-            if tmp_text:
-                text = tmp_text
+        text = _preprocessing_text(text, preprocessing)
         return text
 
+    def _split_by_words(
+        self,
+        clear_text: str,
+        n_grams: Optional[int] = 1,
+        sep: Optional[str] = ' ',
+    ) -> Tuple[List[str], List[Tuple[int, int]]]:
+        """
+        Получение N-грамм слов.
+
+        Параметры
+        ----------
+        clear_text : str
+            Предобработанный текст.
+        n_grams : Optional[int]
+            Длина N-грамм.
+        sep: Optional[str]
+            Разделитель слов.
+
+        Returns
+        -------
+        n_grams_list: List[str]
+            Список N-грамм слов.
+        indeces_n_grams_list: List[Tuple[int, int]]
+            Список кортежей индексов начала и конца N-граммы из `n_grams_list`.
+        """
+        tokens = clear_text.split(sep)
+
+        start_idx = 0
+        indeces_n_grams_list = []
+        n_grams_list = []
+        for i in range(len(tokens) - n_grams + 1):
+            n_tokens_list = tokens[i:i + n_grams]
+            n_gram = ' '.join(n_tokens_list)
+            n_grams_list.append(n_gram)
+
+            indeces = (start_idx, start_idx + len(n_gram))
+            indeces_n_grams_list.append(indeces)
+            start_idx += len(n_tokens_list[0]) + len(sep)
+        return n_grams_list, indeces_n_grams_list
+
+    def _split_by_chars(
+        self,
+        clear_text: str,
+        n_grams: Optional[int] = 1,
+        sep: Optional[str] = ' ',
+    ) -> Tuple[List[str], List[Tuple[int, int]]]:
+        """
+        Получение N-грамм символов.
+
+        Параметры
+        ----------
+        clear_text : str
+            Предобработанный текст.
+        n_grams : Optional[int]
+            Длина N-грамм.
+        sep: Optional[str]
+            Разделитель слов.
+
+        Returns
+        -------
+        n_grams_list: List[str]
+            Список N-грамм символов.
+        indeces_n_grams_list: List[Tuple[int, int]]
+            Список кортежей индексов начала и конца N-граммы из `n_grams_list`.
+        """
+        n_grams_words, _ = self._split_by_words(clear_text, n_grams=1, sep=sep)
+
+        start_idx = 0
+        indeces_n_grams_list = []
+        n_grams_list = []
+        for word in n_grams_words:
+            counter = 0
+            for i in range(len(word) - n_grams + 1):
+                n_gram = word[i:i + n_grams]
+                n_grams_list.append(n_gram)
+
+                indeces = (start_idx, start_idx + len(n_gram))
+                indeces_n_grams_list.append(indeces)
+                start_idx += 1
+                counter += 1
+            start_idx += len(sep) + (len(word) - counter)
+        return n_grams_list, indeces_n_grams_list
+
     @abstractmethod
     def _explain(
         self,
         clear_compared_text: str,
         clear_original_text: str,
         n_grams: int = 1,
-    ) -> Tuple[List[str], List[float]]:
+        analyzer: Literal['word', 'char'] = 'word',
+        sep: Optional[str] = ' ',
+    ) -> Tuple[List[str], List[float], List[Tuple[int, int]]]:
         """
         Поиск наиболее схожих N-грамм из clear_compared_text в clear_original_text.
 
         Параметры
         ----------
         clear_compared_text : str
             Пользовательский текст, в котором нужно найти n-граммы,
             похожие на clear_original_text.
         clear_original_text : str
             Текст, с которым сравнивается clear_compared_text.
         n_grams : int
             Длина N-грамм.
+        analyzer: Literal['word', 'char']
+            Считать схожесть текстов на основе N-грамм слов или символов.
+        sep: Optional[str]
+            Разделитель слов.
 
         Returns
         -------
-        list_text, list_similarity: Tuple[List[str]. List[float]]
-            Кортеж списков.
+        text_list: List[str]
+            Список N-грамм слов или символов.
+        similarity_list: List[float]
+            Список близости N-граммы к `clear_original_text`.
+        indeces_n_grams_list: List[Tuple[int, int]]
+            Список кортежей индексов старта и конца N-граммы из `text_list`.
         """
 
     def explain(
         self,
         compared_text: str,
         original_text: str,
-        n_grams: Union[Tuple[int, int], int] = 1,
-        k: int = 10,
-        ascending: bool = True,
-    ) -> pd.DataFrame:
+        n_grams: Optional[Union[Tuple[int, int], int]] = 1,
+        analyzer: Optional[Literal['word', 'char']] = 'word',
+        sep: Optional[str] = ' ',
+        k: Optional[int] = 10,
+        ascending: Optional[bool] = True,
+    ) -> Tuple[pd.DataFrame, List[Tuple[int, int]]]:
         """
-        Поиск наиболее схожих N-грамм из compared_text в original_text.
+        Поиск наиболее схожих N-грамм из `compared_text` в `original_text`.
 
         Параметры
         ----------
         compared_text : str
             Пользовательский текст, в котором нужно найти n-граммы,
             похожие на original_text.
         original_text : str
             Текст, с которым сравнивается compared_text.
-        n_grams : Union[Tuple[int, int], int]
+        n_grams : Optional[Union[Tuple[int, int], int]]
             Длины N-грамм, которые будут оцениваться.
             Может приниматься либо одно число, либо список чисел.
-        k : int
+        analyzer: Optional[Literal['word', 'char']]
+            Считать схожесть текстов на основе N-грамм слов или символов.
+        sep: Optional[str]
+            Разделитель слов.
+        k : Optional[int]
             Кол-во выдаваемых результатов.
-        ascending : bool
+        ascending : Optional[bool]
             Флаг сортировки полученных результатов.
             False - убывающая, True - возрастающая сортировка.
 
         Returns
         -------
         df: pd.DataFrame
             Датафрейм с результатами.
             df.columns = ['text', 'similarity']
+        indeces_n_grams: List[Tuple[int, int]]
+            Список кортежей индексов старта и конца самых важных N-грамм из `df`.
         """
-
         clear_compared_text = self._preprocessing_text(compared_text, self._preprocessing)
         clear_original_text = self._preprocessing_text(original_text, self._preprocessing)
 
         if isinstance(n_grams, int):
-            if n_grams == 0:
+            if n_grams <= 0:
                 raise ValueError('The `n_grams` parameter must be > 0')
-            
-            list_text, list_similarity = self._explain(clear_compared_text, clear_original_text, n_grams=n_grams)
+
+            text_list, similarity_list, indeces_n_grams_list = self._explain(
+                clear_compared_text,
+                clear_original_text,
+                n_grams=n_grams,
+                analyzer=analyzer,
+                sep=sep,
+            )
         else:
-            if n_grams[0] == 0:
+            if n_grams[0] <= 0:
                 raise ValueError('The min value `n_grams` parameter must be > 0')
-            
-            list_text = []
-            list_similarity = []
-            for i in range(n_grams[0], n_grams[1]+1):
-                tmp_list_text, tmp_list_similarity = self._explain(clear_compared_text, clear_original_text, n_grams=i)
-                list_text.extend(tmp_list_text)
-                list_similarity.extend(tmp_list_similarity)
 
-        df = pd.DataFrame({'text': list_text, 'similarity': list_similarity})
+            text_list = []
+            similarity_list = []
+            indeces_n_grams_list = []
+            for i in range(n_grams[0], n_grams[1]+1):
+                tmp_text_list, tmp_similarity_list, tmp_indeces_n_grams_list = self._explain(
+                    clear_compared_text,
+                    clear_original_text,
+                    n_grams=i,
+                    analyzer=analyzer,
+                    sep=sep,
+                )
+                text_list.extend(tmp_text_list)
+                similarity_list.extend(tmp_similarity_list)
+                indeces_n_grams_list.extend(tmp_indeces_n_grams_list)
+
+        df = pd.DataFrame({
+            'text': text_list,
+            'similarity': similarity_list,
+            'indeces_n_grams': indeces_n_grams_list,
+        })
         df = df.sort_values(by=['similarity'], ascending=ascending).reset_index(drop=True)
 
         k = min(k, df.shape[0])
         df = df.iloc[:k]
-        return df
+
+        indeces_n_grams = df['indeces_n_grams'].values.tolist()
+        df.drop(['indeces_n_grams'], axis=1, inplace=True)
+        return df, indeces_n_grams
+
+
+"""
+Общие функции для Base-классов.
+"""
+
+
+def _preprocessing_text(
+    text: Union[Iterable[str], str],
+    preprocessing: List[BaseTransformation],
+) -> Union[List[str], str]:
+    """
+    Предобработка текста.
+
+    Параметры
+    ----------
+    text : Union[Iterable[str], str]
+        Необработанный текст.
+    preprocessing : List[BaseTransformation]
+        Список алгоритмов для предобработка текста.
+
+    Returns
+    -------
+    text: Union[List[str], str]
+        Обработанный текст.
+    """
+    if isinstance(text, str):
+        for transformator in preprocessing:
+            tmp_text = transformator.transform([text])[0]
+            if tmp_text:
+                text = tmp_text
+    else:
+        for transformator in preprocessing:
+            text = transformator.transform(text)
+    return text
```

### Comparing `recs-searcher-0.0.9/recs_searcher/dataset/_base.py` & `recs-searcher-0.1.0/recs_searcher/dataset/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from typing import Iterable, List, Optional
 from ..base import BaseTransformation
 from sentence_transformers import InputExample
 from torch.utils.data import Dataset
 
 
+# TODO: обновить для use-case поиска схожих текстов.
 class SentenceTransformerDataset(Dataset):
     """Обёртка дадасета для эмбеддингов из Sentence-Transformers."""
 
     def __init__(
         self,
         array: Iterable[str],
         augmentation_transform: Optional[List[BaseTransformation]] = None,
```

### Comparing `recs-searcher-0.0.9/recs_searcher/dataset/_dataframes.py` & `recs-searcher-0.1.0/recs_searcher/dataset/_dataframes.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
 def load_mobile_phones() -> pd.DataFrame:
     """Загрузка датасета с названиями смартфонов.
     Датасет содержит только уникальные значения.
 
 
     =================   ==============
-    Кол-во строк            224
+    Кол-во строк            223
     Кол-во столбцов         1
     =================   ==============
 
     Returns
     -------
     df: pd.DataFrame
         Считанные данные.
```

### Comparing `recs-searcher-0.0.9/recs_searcher/dataset/data/address_krasnoyarsk.csv` & `recs-searcher-0.1.0/recs_searcher/dataset/data/address_krasnoyarsk.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/dataset/data/city_russia.csv` & `recs-searcher-0.1.0/recs_searcher/dataset/data/city_russia.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/dataset/data/company_russia.csv` & `recs-searcher-0.1.0/recs_searcher/dataset/data/company_russia.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/dataset/data/exoplanets.csv` & `recs-searcher-0.1.0/recs_searcher/dataset/data/exoplanets.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/dataset/data/medical_supplies.csv` & `recs-searcher-0.1.0/recs_searcher/dataset/data/medical_supplies.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/dataset/data/mobile_phones.csv` & `recs-searcher-0.1.0/recs_searcher/dataset/data/mobile_phones.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/dataset/data/russian_dictionary.csv` & `recs-searcher-0.1.0/recs_searcher/dataset/data/russian_dictionary.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/dataset/data/video_games.csv` & `recs-searcher-0.1.0/recs_searcher/dataset/data/video_games.csv`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/embeddings/_base.py` & `recs-searcher-0.1.0/recs_searcher/embeddings/_base.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/preprocessing/_base_clear.py` & `recs-searcher-0.1.0/recs_searcher/preprocessing/_base_clear.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/preprocessing/_base_normalize.py` & `recs-searcher-0.1.0/recs_searcher/preprocessing/_base_normalize.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/similarity_search/_base.py` & `recs-searcher-0.1.0/recs_searcher/similarity_search/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Алгоритмы для получения результатов моделей.
 """
 
 from typing import Iterable, List, Literal, Optional, Tuple
 import numpy as np
+from tqdm import tqdm
 
 from ..utils import create_date_name
 from ..base import BaseSearch, BaseEmbeddingSearch, BaseEmbedding, BaseTransformation
 
 from thefuzz import process
 import faiss
 import chromadb
@@ -196,15 +197,15 @@
         name_database = create_date_name('database')
         chroma_database = chroma_client.create_collection(
             name=name_database,
             metadata={"hnsw:space": metric}
         )
 
         if original_array.shape[0] > self._MAX_BATCH_CHROMA_DB:
-            for i in range(0, original_array.shape[0] - self._MAX_BATCH_CHROMA_DB, self._MAX_BATCH_CHROMA_DB):
+            for i in tqdm(range(0, original_array.shape[0] - self._MAX_BATCH_CHROMA_DB, self._MAX_BATCH_CHROMA_DB)):
                 chroma_database.add(
                     embeddings=embedding_database[i:i+self._MAX_BATCH_CHROMA_DB].tolist(),
                     ids=original_array[i:i+self._MAX_BATCH_CHROMA_DB].tolist(),
                 )
         else:
             chroma_database.add(
                 embeddings=embedding_database.tolist(),
```

### Comparing `recs-searcher-0.0.9/recs_searcher/similarity_search/_validate.py` & `recs-searcher-0.1.0/recs_searcher/similarity_search/_validate.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/utils/_concat_embeddings.py` & `recs-searcher-0.1.0/recs_searcher/utils/_concat_embeddings.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/utils/_create_date_name.py` & `recs-searcher-0.1.0/recs_searcher/utils/_create_date_name.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher/utils/_distances.py` & `recs-searcher-0.1.0/recs_searcher/utils/_distances.py`

 * *Files identical despite different names*

### Comparing `recs-searcher-0.0.9/recs_searcher.egg-info/PKG-INFO` & `recs-searcher-0.1.0/recs_searcher.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recs-searcher
-Version: 0.0.9
+Version: 0.1.0
 Summary: Search engine and registry error corrector
 Home-page: https://github.com/sheriff1max/recs-searcher
 Author: sheriff1max
 Author-email: kobelevmaxim48@gmail.com
 Project-URL: Bug tracker, https://github.com/sheriff1max/recs-searcher/issues
 Keywords: python searcher corrector faiss chroma-bd embeddings
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,15 @@
 Requires-Dist: sentence-transformers
 Requires-Dist: pymorphy3
 Requires-Dist: scikit-learn
 Requires-Dist: spacy
 Requires-Dist: thefuzz
 Requires-Dist: torch
 Requires-Dist: torchvision
+Requires-Dist: pytest
 
 # recs-searcher (Registry error correction system - Searcher)
 
     pip install recs-searcher
 
 Система способна решить следующие задачи:
 1. Исправление реестровых ошибок пользовательского ввода при сравнении с базой данных;
```

### Comparing `recs-searcher-0.0.9/recs_searcher.egg-info/SOURCES.txt` & `recs-searcher-0.1.0/recs_searcher.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -37,8 +37,13 @@
 recs_searcher/preprocessing/_base_normalize.py
 recs_searcher/similarity_search/__init__.py
 recs_searcher/similarity_search/_base.py
 recs_searcher/similarity_search/_validate.py
 recs_searcher/utils/__init__.py
 recs_searcher/utils/_concat_embeddings.py
 recs_searcher/utils/_create_date_name.py
-recs_searcher/utils/_distances.py
+recs_searcher/utils/_distances.py
+tests/test_augmentation.py
+tests/test_dataset.py
+tests/test_embeddings.py
+tests/test_pipeline.py
+tests/test_preprocessing.py
```

### Comparing `recs-searcher-0.0.9/setup.py` & `recs-searcher-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
   with open('README.md', 'r', encoding='utf-8') as f:
     return f.read()
 
 setup(
   name='recs-searcher',
-  version='0.0.9',
+  version='0.1.0',
   author='sheriff1max',
   author_email='kobelevmaxim48@gmail.com',
   description='Search engine and registry error corrector',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/sheriff1max/recs-searcher',
   packages=find_packages(),
@@ -26,14 +26,15 @@
     'sentence-transformers',
     'pymorphy3',
     'scikit-learn',
     'spacy',
     'thefuzz',
     'torch',
     'torchvision',
+    'pytest',
   ],
   classifiers=[
     'Programming Language :: Python :: 3',
   ],
   keywords='python searcher corrector faiss chroma-bd embeddings',
   project_urls={
     'Bug tracker': 'https://github.com/sheriff1max/recs-searcher/issues'
```

