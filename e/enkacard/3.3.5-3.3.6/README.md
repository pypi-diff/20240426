# Comparing `tmp/enkacard-3.3.5.tar.gz` & `tmp/enkacard-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enkacard-3.3.5.tar", max compression
+gzip compressed data, was "enkacard-3.3.6.tar", max compression
```

## Comparing `enkacard-3.3.5.tar` & `enkacard-3.3.6.tar`

### file list

```diff
@@ -1,94 +1,38 @@
--rw-r--r--   0        0        0      313 2022-12-17 00:40:06.925303 enkacard-3.3.5/enkacard/enc_error.py
--rw-r--r--   0        0        0    10179 2024-04-18 22:10:58.709561 enkacard-3.3.5/enkacard/encbanner.py
--rw-r--r--   0        0        0     5145 2024-02-29 17:57:35.626280 enkacard-3.3.5/enkacard/enkatools.py
--rw-r--r--   0        0        0 11514084 2022-07-25 21:33:51.994087 enkacard-3.3.5/enkacard/src/assets/font/Genshin_Impact.ttf
--rw-r--r--   0        0        0    79268 2023-04-05 20:05:44.281954 enkacard-3.3.5/enkacard/src/assets/font/GSEnochian.ttf
--rw-r--r--   0        0        0     9259 2024-03-12 11:19:40.666625 enkacard-3.3.5/enkacard/src/generator/__pycache__/akasha_rank.cpython-311.pyc
--rw-r--r--   0        0        0     8281 2024-04-21 10:27:04.570454 enkacard-3.3.5/enkacard/src/generator/__pycache__/akasha_rank.cpython-312.pyc
--rw-r--r--   0        0        0    10680 2024-03-12 11:19:40.669627 enkacard-3.3.5/enkacard/src/generator/__pycache__/profile_teample_one.cpython-311.pyc
--rw-r--r--   0        0        0    11042 2024-04-21 10:27:04.572453 enkacard-3.3.5/enkacard/src/generator/__pycache__/profile_teample_one.cpython-312.pyc
--rw-r--r--   0        0        0     9363 2024-03-12 11:19:41.167913 enkacard-3.3.5/enkacard/src/generator/__pycache__/profile_teample_two.cpython-311.pyc
--rw-r--r--   0        0        0     9742 2024-04-21 10:32:16.720190 enkacard-3.3.5/enkacard/src/generator/__pycache__/profile_teample_two.cpython-312.pyc
--rw-r--r--   0        0        0    13080 2024-03-12 11:19:40.487430 enkacard-3.3.5/enkacard/src/generator/__pycache__/teample_one.cpython-311.pyc
--rw-r--r--   0        0        0    13342 2024-04-21 10:27:04.189857 enkacard-3.3.5/enkacard/src/generator/__pycache__/teample_one.cpython-312.pyc
--rw-r--r--   0        0        0    17916 2024-03-12 11:19:40.680148 enkacard-3.3.5/enkacard/src/generator/__pycache__/teample_two.cpython-311.pyc
--rw-r--r--   0        0        0    17976 2024-04-21 10:27:04.574456 enkacard-3.3.5/enkacard/src/generator/__pycache__/teample_two.cpython-312.pyc
--rw-r--r--   0        0        0     3819 2024-04-25 09:34:17.037508 enkacard-3.3.5/enkacard/src/generator/akasha_rank.py
--rw-r--r--   0        0        0    13628 2024-03-12 11:19:40.636054 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/artifact.cpython-311.pyc
--rw-r--r--   0        0        0    13604 2024-04-21 10:27:04.559942 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/artifact.cpython-312.pyc
--rw-r--r--   0        0        0     4882 2024-03-12 11:19:40.631536 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/background.cpython-311.pyc
--rw-r--r--   0        0        0     4942 2024-04-21 10:27:04.555438 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/background.cpython-312.pyc
--rw-r--r--   0        0        0     2798 2024-03-12 11:19:40.648579 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/constant.cpython-311.pyc
--rw-r--r--   0        0        0     2820 2024-04-21 10:27:04.562946 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/constant.cpython-312.pyc
--rw-r--r--   0        0        0     2356 2024-03-12 11:19:40.660102 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/prop.cpython-311.pyc
--rw-r--r--   0        0        0     2346 2024-04-21 10:27:04.567946 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/prop.cpython-312.pyc
--rw-r--r--   0        0        0     3475 2024-03-12 11:19:40.651579 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/skill.cpython-311.pyc
--rw-r--r--   0        0        0     3470 2024-04-21 10:27:04.563945 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/skill.cpython-312.pyc
--rw-r--r--   0        0        0    11270 2024-03-12 11:19:40.656100 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/stat.cpython-311.pyc
--rw-r--r--   0        0        0    10678 2024-04-21 10:27:04.566946 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/stat.cpython-312.pyc
--rw-r--r--   0        0        0     6516 2024-03-12 11:19:40.640055 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/weapon.cpython-311.pyc
--rw-r--r--   0        0        0     6799 2024-04-21 10:27:04.561946 enkacard-3.3.5/enkacard/src/generator/one/__pycache__/weapon.cpython-312.pyc
--rw-r--r--   0        0        0     6657 2023-12-10 18:28:18.819703 enkacard-3.3.5/enkacard/src/generator/one/artifact.py
--rw-r--r--   0        0        0     2363 2023-12-03 21:02:32.344488 enkacard-3.3.5/enkacard/src/generator/one/background.py
--rw-r--r--   0        0        0     1235 2023-12-10 20:39:47.204162 enkacard-3.3.5/enkacard/src/generator/one/constant.py
--rw-r--r--   0        0        0      869 2023-12-01 21:40:04.470207 enkacard-3.3.5/enkacard/src/generator/one/prop.py
--rw-r--r--   0        0        0     1378 2023-12-21 20:00:52.547008 enkacard-3.3.5/enkacard/src/generator/one/skill.py
--rw-r--r--   0        0        0     5749 2023-12-07 00:50:46.885608 enkacard-3.3.5/enkacard/src/generator/one/stat.py
--rw-r--r--   0        0        0     2989 2023-12-23 01:15:33.050226 enkacard-3.3.5/enkacard/src/generator/one/weapon.py
--rw-r--r--   0        0        0     6132 2024-01-06 15:22:38.238244 enkacard-3.3.5/enkacard/src/generator/profile_teample_one.py
--rw-r--r--   0        0        0     5229 2024-04-21 10:32:11.269924 enkacard-3.3.5/enkacard/src/generator/profile_teample_two.py
--rw-r--r--   0        0        0     6711 2023-12-21 20:25:56.721897 enkacard-3.3.5/enkacard/src/generator/teample_one.py
--rw-r--r--   0        0        0     9909 2024-01-06 15:59:41.426611 enkacard-3.3.5/enkacard/src/generator/teample_two.py
--rw-r--r--   0        0        0    12705 2024-03-12 11:19:41.160400 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/artifact.cpython-311.pyc
--rw-r--r--   0        0        0    12704 2024-04-21 10:27:04.967692 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/artifact.cpython-312.pyc
--rw-r--r--   0        0        0     5973 2024-03-12 11:19:41.156399 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/background.cpython-311.pyc
--rw-r--r--   0        0        0     6096 2024-04-21 10:27:04.963691 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/background.cpython-312.pyc
--rw-r--r--   0        0        0     3475 2024-03-12 11:19:41.165913 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/skill.cpython-311.pyc
--rw-r--r--   0        0        0     3470 2024-04-21 10:27:04.971200 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/skill.cpython-312.pyc
--rw-r--r--   0        0        0     7278 2024-03-12 11:19:41.163914 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/stat.cpython-311.pyc
--rw-r--r--   0        0        0     6910 2024-04-21 10:27:04.970200 enkacard-3.3.5/enkacard/src/generator/two/__pycache__/stat.cpython-312.pyc
--rw-r--r--   0        0        0     6377 2023-12-18 23:30:42.003393 enkacard-3.3.5/enkacard/src/generator/two/artifact.py
--rw-r--r--   0        0        0     3034 2023-12-17 22:37:02.037270 enkacard-3.3.5/enkacard/src/generator/two/background.py
--rw-r--r--   0        0        0     1368 2023-12-21 20:52:29.332377 enkacard-3.3.5/enkacard/src/generator/two/skill.py
--rw-r--r--   0        0        0     3346 2023-12-21 19:58:52.526652 enkacard-3.3.5/enkacard/src/generator/two/stat.py
--rw-r--r--   0        0        0     7501 2024-03-12 11:19:40.462381 enkacard-3.3.5/enkacard/src/modal/__pycache__/enkacardCread.cpython-311.pyc
--rw-r--r--   0        0        0     5542 2024-04-21 10:27:04.184354 enkacard-3.3.5/enkacard/src/modal/__pycache__/enkacardCread.cpython-312.pyc
--rw-r--r--   0        0        0     2072 2024-03-12 11:19:39.704683 enkacard-3.3.5/enkacard/src/modal/__pycache__/enkaToolsModel.cpython-311.pyc
--rw-r--r--   0        0        0     1604 2024-04-21 10:27:03.631178 enkacard-3.3.5/enkacard/src/modal/__pycache__/enkaToolsModel.cpython-312.pyc
--rw-r--r--   0        0        0     2553 2024-03-12 11:14:42.124404 enkacard-3.3.5/enkacard/src/modal/enkacardCread.py
--rw-r--r--   0        0        0      771 2023-12-17 22:08:52.342906 enkacard-3.3.5/enkacard/src/modal/enkaToolsModel.py
--rw-r--r--   0        0        0    59616 2023-12-25 12:23:22.739379 enkacard-3.3.5/enkacard/src/pickle_cashe/data_characters.pkz
--rw-r--r--   0        0        0        0 2023-12-25 12:23:29.173879 enkacard-3.3.5/enkacard/src/pickle_cashe/data_characters.pkz~
--rw-r--r--   0        0        0    10697 2024-03-12 11:19:40.352607 enkacard-3.3.5/enkacard/src/utils/__pycache__/affixes.cpython-311.pyc
--rw-r--r--   0        0        0     9733 2024-04-21 10:27:03.963075 enkacard-3.3.5/enkacard/src/utils/__pycache__/affixes.cpython-312.pyc
--rw-r--r--   0        0        0     7570 2024-03-12 11:19:40.683655 enkacard-3.3.5/enkacard/src/utils/__pycache__/diagram.cpython-311.pyc
--rw-r--r--   0        0        0     5714 2024-04-21 10:27:04.576454 enkacard-3.3.5/enkacard/src/utils/__pycache__/diagram.cpython-312.pyc
--rw-r--r--   0        0        0     9027 2024-03-12 11:19:40.448351 enkacard-3.3.5/enkacard/src/utils/__pycache__/git.cpython-311.pyc
--rw-r--r--   0        0        0     8437 2024-04-21 10:27:04.160338 enkacard-3.3.5/enkacard/src/utils/__pycache__/git.cpython-312.pyc
--rw-r--r--   0        0        0     6844 2024-03-12 11:19:40.348101 enkacard-3.3.5/enkacard/src/utils/__pycache__/options.cpython-311.pyc
--rw-r--r--   0        0        0     5947 2024-04-21 10:27:03.960076 enkacard-3.3.5/enkacard/src/utils/__pycache__/options.cpython-312.pyc
--rw-r--r--   0        0        0    11433 2024-03-12 11:19:40.451353 enkacard-3.3.5/enkacard/src/utils/__pycache__/pickle_cashe.cpython-311.pyc
--rw-r--r--   0        0        0     9513 2024-04-21 10:27:04.163336 enkacard-3.3.5/enkacard/src/utils/__pycache__/pickle_cashe.cpython-312.pyc
--rw-r--r--   0        0        0    33153 2024-03-12 11:19:40.497955 enkacard-3.3.5/enkacard/src/utils/__pycache__/pill.cpython-311.pyc
--rw-r--r--   0        0        0    29897 2024-04-21 10:27:04.197863 enkacard-3.3.5/enkacard/src/utils/__pycache__/pill.cpython-312.pyc
--rw-r--r--   0        0        0     1552 2024-03-12 11:19:40.457867 enkacard-3.3.5/enkacard/src/utils/__pycache__/translation.cpython-311.pyc
--rw-r--r--   0        0        0     1494 2024-04-21 10:27:04.183353 enkacard-3.3.5/enkacard/src/utils/__pycache__/translation.cpython-312.pyc
--rw-r--r--   0        0        0    18462 2023-11-30 22:40:24.144568 enkacard-3.3.5/enkacard/src/utils/affixes.py
--rw-r--r--   0        0        0     3501 2024-04-18 22:05:34.318028 enkacard-3.3.5/enkacard/src/utils/diagram.py
--rw-r--r--   0        0        0     1317 2024-03-12 11:19:40.127631 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     1281 2024-04-25 09:25:21.427292 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/config.cpython-312.pyc
--rw-r--r--   0        0        0    18978 2024-03-12 11:19:39.931560 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/enka_update.cpython-311.pyc
--rw-r--r--   0        0        0    15771 2024-04-25 09:29:12.217664 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/enka_update.cpython-312.pyc
--rw-r--r--   0        0        0     1044 2024-03-12 11:19:40.123621 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/pathfinding.cpython-311.pyc
--rw-r--r--   0        0        0     1006 2024-04-25 09:19:48.951886 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/__pycache__/pathfinding.cpython-312.pyc
--rw-r--r--   0        0        0     1510 2024-04-25 09:25:17.101442 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/config.py
--rw-r--r--   0        0        0    11477 2024-04-25 09:31:54.863565 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/enka_update.py
--rw-r--r--   0        0        0      537 2024-04-25 09:17:51.407630 enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/pathfinding.py
--rw-r--r--   0        0        0     5722 2023-12-25 11:21:01.889033 enkacard-3.3.5/enkacard/src/utils/git.py
--rw-r--r--   0        0        0     3977 2024-04-18 22:11:07.156131 enkacard-3.3.5/enkacard/src/utils/options.py
--rw-r--r--   0        0        0     6868 2023-12-13 21:43:08.363154 enkacard-3.3.5/enkacard/src/utils/pickle_cashe.py
--rw-r--r--   0        0        0    17229 2023-12-23 00:44:36.688489 enkacard-3.3.5/enkacard/src/utils/pill.py
--rw-r--r--   0        0        0     1852 2023-04-05 20:09:26.777243 enkacard-3.3.5/enkacard/src/utils/translation.py
--rw-r--r--   0        0        0      870 2024-04-25 10:05:30.157601 enkacard-3.3.5/pyproject.toml
--rw-r--r--   0        0        0     3699 2023-12-23 16:26:14.431089 enkacard-3.3.5/README.md
--rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 enkacard-3.3.5/PKG-INFO
+-rw-r--r--   0        0        0      313 2022-12-17 00:40:06.925303 enkacard-3.3.6/enkacard/enc_error.py
+-rw-r--r--   0        0        0    10179 2024-04-18 22:10:58.709561 enkacard-3.3.6/enkacard/encbanner.py
+-rw-r--r--   0        0        0     5145 2024-02-29 17:57:35.626280 enkacard-3.3.6/enkacard/enkatools.py
+-rw-r--r--   0        0        0 11514084 2022-07-25 21:33:51.994087 enkacard-3.3.6/enkacard/src/assets/font/Genshin_Impact.ttf
+-rw-r--r--   0        0        0    79268 2023-04-05 20:05:44.281954 enkacard-3.3.6/enkacard/src/assets/font/GSEnochian.ttf
+-rw-r--r--   0        0        0     3796 2024-04-25 11:36:07.075682 enkacard-3.3.6/enkacard/src/generator/akasha_rank.py
+-rw-r--r--   0        0        0     6657 2023-12-10 18:28:18.819703 enkacard-3.3.6/enkacard/src/generator/one/artifact.py
+-rw-r--r--   0        0        0     2363 2023-12-03 21:02:32.344488 enkacard-3.3.6/enkacard/src/generator/one/background.py
+-rw-r--r--   0        0        0     1235 2023-12-10 20:39:47.204162 enkacard-3.3.6/enkacard/src/generator/one/constant.py
+-rw-r--r--   0        0        0      869 2023-12-01 21:40:04.470207 enkacard-3.3.6/enkacard/src/generator/one/prop.py
+-rw-r--r--   0        0        0     1378 2023-12-21 20:00:52.547008 enkacard-3.3.6/enkacard/src/generator/one/skill.py
+-rw-r--r--   0        0        0     5749 2023-12-07 00:50:46.885608 enkacard-3.3.6/enkacard/src/generator/one/stat.py
+-rw-r--r--   0        0        0     2989 2023-12-23 01:15:33.050226 enkacard-3.3.6/enkacard/src/generator/one/weapon.py
+-rw-r--r--   0        0        0     6132 2024-01-06 15:22:38.238244 enkacard-3.3.6/enkacard/src/generator/profile_teample_one.py
+-rw-r--r--   0        0        0     5229 2024-04-21 10:32:11.269924 enkacard-3.3.6/enkacard/src/generator/profile_teample_two.py
+-rw-r--r--   0        0        0     6711 2023-12-21 20:25:56.721897 enkacard-3.3.6/enkacard/src/generator/teample_one.py
+-rw-r--r--   0        0        0     9568 2024-04-26 17:13:10.977992 enkacard-3.3.6/enkacard/src/generator/teample_two.py
+-rw-r--r--   0        0        0     6377 2023-12-18 23:30:42.003393 enkacard-3.3.6/enkacard/src/generator/two/artifact.py
+-rw-r--r--   0        0        0     3034 2023-12-17 22:37:02.037270 enkacard-3.3.6/enkacard/src/generator/two/background.py
+-rw-r--r--   0        0        0     1368 2023-12-21 20:52:29.332377 enkacard-3.3.6/enkacard/src/generator/two/skill.py
+-rw-r--r--   0        0        0     3346 2023-12-21 19:58:52.526652 enkacard-3.3.6/enkacard/src/generator/two/stat.py
+-rw-r--r--   0        0        0     2553 2024-03-12 11:14:42.124404 enkacard-3.3.6/enkacard/src/modal/enkacardCread.py
+-rw-r--r--   0        0        0      771 2023-12-17 22:08:52.342906 enkacard-3.3.6/enkacard/src/modal/enkaToolsModel.py
+-rw-r--r--   0        0        0    59616 2023-12-25 12:23:22.739379 enkacard-3.3.6/enkacard/src/pickle_cashe/data_characters.pkz
+-rw-r--r--   0        0        0        0 2023-12-25 12:23:29.173879 enkacard-3.3.6/enkacard/src/pickle_cashe/data_characters.pkz~
+-rw-r--r--   0        0        0    18462 2023-11-30 22:40:24.144568 enkacard-3.3.6/enkacard/src/utils/affixes.py
+-rw-r--r--   0        0        0     5338 2024-04-26 16:53:05.168162 enkacard-3.3.6/enkacard/src/utils/diagram.py
+-rw-r--r--   0        0        0     1510 2024-04-25 09:25:17.101442 enkacard-3.3.6/enkacard/src/utils/enkanetwork_update/config.py
+-rw-r--r--   0        0        0    11552 2024-04-26 18:31:42.197101 enkacard-3.3.6/enkacard/src/utils/enkanetwork_update/enka_update.py
+-rw-r--r--   0        0        0      549 2024-04-26 18:31:03.048071 enkacard-3.3.6/enkacard/src/utils/enkanetwork_update/pathfinding.py
+-rw-r--r--   0        0        0     5722 2023-12-25 11:21:01.889033 enkacard-3.3.6/enkacard/src/utils/git.py
+-rw-r--r--   0        0        0     7189 2024-04-26 17:12:31.292644 enkacard-3.3.6/enkacard/src/utils/options.py
+-rw-r--r--   0        0        0     6868 2023-12-13 21:43:08.363154 enkacard-3.3.6/enkacard/src/utils/pickle_cashe.py
+-rw-r--r--   0        0        0    17229 2023-12-23 00:44:36.688489 enkacard-3.3.6/enkacard/src/utils/pill.py
+-rw-r--r--   0        0        0     1852 2023-04-05 20:09:26.777243 enkacard-3.3.6/enkacard/src/utils/translation.py
+-rw-r--r--   0        0        0      870 2024-04-26 18:54:09.782680 enkacard-3.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3699 2023-12-23 16:26:14.431089 enkacard-3.3.6/README.md
+-rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 enkacard-3.3.6/PKG-INFO
```

### Comparing `enkacard-3.3.5/enkacard/encbanner.py` & `enkacard-3.3.6/enkacard/encbanner.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/enkatools.py` & `enkacard-3.3.6/enkacard/enkatools.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/assets/font/Genshin_Impact.ttf` & `enkacard-3.3.6/enkacard/src/assets/font/Genshin_Impact.ttf`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/assets/font/GSEnochian.ttf` & `enkacard-3.3.6/enkacard/src/assets/font/GSEnochian.ttf`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/akasha_rank.py` & `enkacard-3.3.6/enkacard/src/generator/akasha_rank.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     async def get_info_character(self, id):
         hash = await self.get_hash(id)
         url = f'https://akasha.cv/api/leaderboards/{self.uid}/{hash}?variant=profilePage'
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as response:
                 if response.status == 200:
                     data = await response.json()
-                    return data["data"].get("calculations",{})
+                    return data["data"]
                 else:
                     return {}
             
     async def get_rank_akasha(self):
         akaska_info = []
         if not self.uid in data_akasha:
             async with aiohttp.ClientSession() as session:
```

### Comparing `enkacard-3.3.5/enkacard/src/generator/one/artifact.py` & `enkacard-3.3.6/enkacard/src/generator/one/artifact.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/one/background.py` & `enkacard-3.3.6/enkacard/src/generator/one/background.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/one/constant.py` & `enkacard-3.3.6/enkacard/src/generator/one/constant.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/one/prop.py` & `enkacard-3.3.6/enkacard/src/generator/one/prop.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/one/skill.py` & `enkacard-3.3.6/enkacard/src/generator/one/skill.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/one/stat.py` & `enkacard-3.3.6/enkacard/src/generator/one/stat.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/one/weapon.py` & `enkacard-3.3.6/enkacard/src/generator/one/weapon.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/profile_teample_one.py` & `enkacard-3.3.6/enkacard/src/generator/profile_teample_one.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/profile_teample_two.py` & `enkacard-3.3.6/enkacard/src/generator/profile_teample_two.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/teample_one.py` & `enkacard-3.3.6/enkacard/src/generator/teample_one.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/teample_two.py` & `enkacard-3.3.6/enkacard/src/generator/teample_two.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import asyncio
 from PIL import ImageDraw,Image,ImageChops
+from enkanetwork.model.stats import CharacterStats
+
 from ..utils import pill, git,diagram,options
 from enkanetwork.enum import EquipmentsType
 from .two import background, artifact, stat, skill
 from .one import weapon,constant
 from .akasha_rank import AkashaCreat
-import random
 _of = git.ImageCache()
 
 
 
-
-
-
-
 class Creat:
     def __init__(self,characters,lang,img,hide,uid,name) -> None:
         self.character = characters
         self.lang = lang["lvl"]
         self.img = img
         self.hide = hide
         self.uid = uid
@@ -94,68 +91,52 @@
         d.text((int(324-x),51), friends, font= font_15, fill=(255,255,255,255))
        
     async def add_logo(self):
         logo = await _of.logo
         self.background.alpha_composite(logo, (1108,710))
     
     async def creat_diagram(self):
-        elementUp = True
-        akashaElement = False
-        data_user = []
-        
+        user_diagram = False
         dataAkasha = await AkashaCreat(uid = self.uid).get_info_character(self.character.id)
-        if dataAkasha == []:
-            dataAkasha = {}
-        if dataAkasha != {}:
-            dataAkasha  = dataAkasha[random.choice(list(dataAkasha.keys()))]['stats']
-        dataAkasha_new = []
-        
-        for key in self.character.stats:
-            if key[1].id in [40,41,42,43,44,45,46]:
-                if elementUp:
-                    key = max((x for x in self.character.stats if 40 <= x[1].id <= 46), key=lambda x: x[1].value)
-                    elementUp = False
-                    akashaElement = True
-                else:
-                    continue
-            if key[1].value != 0 and key[0] in options.IconAddTrue:
-                akasha_name = options.AkashaStats.get(key[0], None)
-                if not akasha_name is None or akashaElement:
-                    if akashaElement:
-                        for keys in dataAkasha:
-                            if "DMG" in keys and not "_CRITICAL" in keys:
-                                akasha_name = keys
-                                akashaElement = False
-                                    
-                    name = options.assets.get_hash_map(key[0])
-                    
-                    if "." in name:
-                        name = name.replace(".",".\n")
-                    else:
-                        name = name.replace(" ","\n")
-                    
-                    try:
-                        value = key[1].to_percentage()
-                        procent = True
-                    except:
-                        value = key[1].to_rounded()
-                        procent = False
-                        
-                    if dataAkasha != {}:
-                        if procent:
-                            dataAkasha_new.append({"name": name, "value": float('{:.2f}'.format(dataAkasha[akasha_name]))})
-                        else:
-                            dataAkasha_new.append({"name": name, "value": round(dataAkasha[akasha_name])})
+        if not dataAkasha["chartsData"] is None: 
+            chartsData = dataAkasha["chartsData"]["charts1pMetadata"][1]["avgStats"]
+        else:
+            user_diagram = True
+            chartsData = options._map_default
+        user_data = []
+        akasha_data = []
 
-                    data_user.append({"name": name, "value": value})
-        
-        if dataAkasha == {}:
-            dataAkasha_new = [{'name': entry['name'], 'value': entry['value']} for entry in data_user]  
         
-        self.diagram = await diagram.create_normalized_radial_chart(data_user,dataAkasha_new,self.character.element.value)
+        for key in chartsData:
+            if user_diagram:
+                name = options.assets.get_hash_map(options._mapHash.get(key))
+                value = options.map_enka(key, self.character.stats)
+                if value.value == 0 and chartsData[key] == 0:
+                    continue
+                try:
+                    value = value.to_percentage()
+                except:
+                    value = value.to_rounded()
+                chartsData[key] = options.format_value(key, chartsData[key], options._mapProcent.get(key), 1)
+                user_data.append({"name": name.replace(".",".\n").replace(" ","\n"), "value": value})
+                akasha_data.append({"name": name.replace(".",".\n").replace(" ","\n"), "value": value})
+            else:
+                name = options.assets.get_hash_map(options._mapHash.get(key))
+                value = options.map_enka(key, self.character.stats)
+                if value.value == 0 and chartsData[key] == 0:
+                    continue
+                try:
+                    value = value.to_percentage()
+                except:
+                    value = value.to_rounded()
+                chartsData[key] = options.format_value(key, chartsData[key], options._mapProcent.get(key), 1)
+                user_data.append({"name": name.replace(".",".\n").replace(" ","\n"), "value": value})
+                akasha_data.append({"name": name.replace(".",".\n").replace(" ","\n"), "value": chartsData[key]})
+                
+        self.diagram = await diagram.RadialChart(user_data, akasha_data, self.character.element.value).create_normalized_radial_chart() #create_normalized_radial_chart(user_data,akasha_data,self.character.element.value)
 
     async def creat_stat(self):
         self.stat_background = Image.new("RGBA", (519, 601), (0,0,0,0))
         result = await stat.Stat(self.character.stats, self.character.element.value).start()
         if len(result) <= 1:
             x = 0 
         x = int(519 / (len(result) - 1))
```

### Comparing `enkacard-3.3.5/enkacard/src/generator/two/artifact.py` & `enkacard-3.3.6/enkacard/src/generator/two/artifact.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/two/background.py` & `enkacard-3.3.6/enkacard/src/generator/two/background.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/two/skill.py` & `enkacard-3.3.6/enkacard/src/generator/two/skill.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/generator/two/stat.py` & `enkacard-3.3.6/enkacard/src/generator/two/stat.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/modal/enkacardCread.py` & `enkacard-3.3.6/enkacard/src/modal/enkacardCread.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/modal/enkaToolsModel.py` & `enkacard-3.3.6/enkacard/src/modal/enkaToolsModel.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/pickle_cashe/data_characters.pkz` & `enkacard-3.3.6/enkacard/src/pickle_cashe/data_characters.pkz`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/utils/affixes.py` & `enkacard-3.3.6/enkacard/src/utils/affixes.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/utils/diagram.py` & `enkacard-3.3.6/enkacard/src/utils/diagram.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,93 +4,147 @@
 from . import pill
 import io
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import font_manager
 from pathlib import Path
 import warnings
+import random
 
 warnings.filterwarnings("ignore")
 
 assets = assets = Path(__file__).parent.parent / 'assets'
 
 font_path = str(assets / 'font' / 'Genshin_Impact.ttf')
 
 custom_font = font_manager.FontProperties(fname=font_path)
 plt.rcParams['font.family'] = custom_font.get_name()
 
-async def create_normalized_radial_chart(data, data_rect, rgb):
-    rgb = pill.element_color_text.get(rgb, (149,107,5,255))
-    params = [item['name'] for item in data]
-    values = [item['value'] for item in data]
+indices =  [2, 1, 0, 7, 6, 5, 4, 3, 9, 10, 11, 12]
 
-    max_values = {item['name']: item['value'] for item in data_rect}
+class RadialChart:
+    def __init__(self, data, data_rect, rgb):
+        self.data = data
+        self.data_rect = data_rect
+        self.rgb = rgb
 
-    max_data_rect_values = [item['value'] for item in data_rect]
+    @property
+    def data(self):
+        return self._data
 
-    num_vars = len(params)
-   
-    normalized_values = [values[i] / max_values[params[i]] if  max_values[params[i]] != 0 else 0 for i in range(num_vars)]
-    normalized_values += [normalized_values[0]]
+    @data.setter
+    def data(self, value):
+        self._data = self._reorder_data_by_indices(value)
 
+    @property
+    def data_rect(self):
+        return self._data_rect
 
-    angles = np.linspace(0, 2 * np.pi, num_vars, endpoint=False).tolist()
-    angles += angles[:1] 
+    @data_rect.setter
+    def data_rect(self, value):
+        self._data_rect = self._reorder_data_by_indices(value)
 
-    fig, ax = plt.subplots(subplot_kw=dict(polar=True))
-    
-    ax.grid(False)
+    @staticmethod
+    def _reorder_data_by_indices(lst):
+        normalized_indices = [i % len(lst) for i in indices if i < len(lst)]
+        return [lst[i] for i in normalized_indices]
 
-    normalized_values_rect = [max_data_rect_values[i] / max_values[params[i]] if max_values[params[i]] != 0 else 0 for i in range(num_vars)]
-    normalized_values_rect += [normalized_values_rect[0]]
-    
-    num_background_lines = 6
+    async def create_normalized_radial_chart(self):
 
-    max_data_rect_value = max(normalized_values_rect)
+        rgb = pill.element_color_text.get(self.rgb, (149, 107, 5, 255))
+        params = [item['name'] for item in self.data]
+        values = [item['value'] for item in self.data]
 
+        max_values = {item['name']: item['value'] for item in self.data_rect}
 
-    step = max_data_rect_value / num_background_lines
+        num_vars = len(params)
+        normalized_values = []
+        for i in range(num_vars):
+            if max_values[params[i]] != 0:
+                if max_values[params[i]] < values[i]:
+                    normalized_values.append(7)
+                else:
+                    normalized_values.append(values[i] / max_values[params[i]])
 
-    for i in range(1, num_background_lines + 2):
-        radii = [step * i] * len(angles)
-        radii.append(radii[0]) 
-        ax.plot(np.append(angles, angles[0]), radii, color='white', linestyle='-', linewidth=0.5, zorder=0, alpha=0.3)
-    
-    for i in range(1, len(data_rect)+1):
-        radii = [step * i for step in range(len(data_rect))]
-        ax.plot([angles[i], angles[i]], [0.16, 1.16], color='white', linestyle='-', linewidth=0.5, zorder=1, alpha=0.3)
+            else:
+                normalized_values.append(0)
 
-    valuess = [item['value'] for item in data_rect]
-    valuess += [valuess[0]]
-    ax.plot(angles, normalized_values_rect, linewidth=2, color='white', marker='o', linestyle='solid', zorder=0, alpha=0.5)
-    for i, (angle, value) in enumerate(zip(angles, normalized_values_rect)):
-        if valuess[i] % 1 == 0:
-            val = str(valuess[i])
+        normalized_values += [normalized_values[0]]
+
+        angles = np.linspace(0, 2 * np.pi, num_vars, endpoint=False).tolist()
+        angles += angles[:1]
+
+        fig, ax = plt.subplots(subplot_kw=dict(polar=True))
+
+        ax.grid(False)
+
+        normalized_values_rect = [6.0 if max_values[params[i]] != 0 else 0 for i in range(num_vars)]
+        normalized_values_rect += [normalized_values_rect[0]]
+
+        num_background_lines = 7
+
+        max_data_rect_value = max(normalized_values_rect)
+        min_data_rect_value = min(normalized_values_rect)
+
+        step = (max_data_rect_value - min_data_rect_value) / (num_background_lines - 1) if max_data_rect_value != min_data_rect_value else 1
+
+        radii_rect = [6] * len(normalized_values_rect)
+
+        radii_values = [self._get_value(item, max_values) for item in self.data]
+        radii_values.append(radii_values[0])
+
+        for i in range(1, num_background_lines + 1):
+            radii = [step * (i - 1) + 1] * len(angles)
+            radii.append(radii[0])
+            ax.plot(np.append(angles, angles[0]), radii, color='white', linestyle='-', linewidth=0.5, zorder=0,
+                    alpha=0.3)
+
+        for i in range(1, len(self.data_rect) + 1):
+            radii = [i + 0.16] * len(self.data_rect)
+            ax.plot([angles[i], angles[i]], [0.16, num_background_lines + 0.16], color='white', linestyle='-',
+                    linewidth=0.5, zorder=1, alpha=0.3)
+
+        valuess = [item['value'] for item in self.data_rect]
+        valuess += [valuess[0]]
+
+        ax.plot(angles, radii_rect, linewidth=2, color='white', marker='o', linestyle='solid', zorder=0, alpha=0.5)
+        for i, (angle, radius) in enumerate(zip(angles, radii_rect)):
+            if valuess[i] % 1 == 0:
+                val = str(valuess[i])
+            else:
+                val = '{:.1f}%'.format(valuess[i])
+
+            ax.annotate(val, (angle, radius), textcoords="offset points", xytext=(-10, -10), color="white",
+                        fontsize=9, ha='left', alpha=1)
+
+        ax.plot(angles, radii_values, linewidth=1, color=(rgb[0] / 255, rgb[1] / 255, rgb[2] / 255), marker='o',
+                zorder=1)
+        ax.fill(angles, radii_values, color=(rgb[0] / 255, rgb[1] / 255, rgb[2] / 255), alpha=0.3)
+
+        ax.xaxis.grid(linewidth=0)
+        ax.set_yticklabels([])
+        ax.set_xticks(np.linspace(0, 2 * np.pi, len(params), endpoint=False))
+        ax.set_xticklabels(params, color='white', fontproperties=custom_font, fontsize=10)
+
+        ax.spines['polar'].set_visible(False)
+
+        buffer = io.BytesIO()
+        plt.savefig(buffer, format='png', transparent=True)
+        buffer.seek(0)
+
+        img = Image.open(buffer)
+
+        plt.close(fig)
+
+        return img
+
+    @staticmethod
+    def _get_value(value_info, max_value_dict):
+        max_value = max_value_dict.get(value_info['name'], None)
+        if max_value is None:
+            return 1
+        if value_info['value'] > max_value:
+            normalized_value = 7 + (value_info['value'] - max_value) / (max_value * 0.3)
+            return min(7.5, normalized_value)
         else:
-            val = '{:.1f}%'.format(valuess[i])
-            
-        ax.annotate(val, (angle, value), textcoords="offset points", xytext=(-10, -10), color = "white", fontsize=7, ha='left', alpha = 1)
-
-    normalized_values_v = []
-    for key in normalized_values:
-        if key > 1.0:
-            key = 1.2
-        normalized_values_v.append(key)
-        
-    ax.plot(angles, normalized_values_v, linewidth=1, color = (rgb[0]/255,rgb[1]/255,rgb[2]/255), marker='o', zorder=1)
-    ax.fill(angles, normalized_values_v, color= (rgb[0]/255,rgb[1]/255,rgb[2]/255), alpha=0.3)
-
-    ax.xaxis.grid(linewidth=0) 
-    ax.set_yticklabels([])
-    ax.set_xticks(angles)
-    ax.set_xticklabels(params + params[:1], color='white', fontproperties=custom_font,fontsize=10)
-    ax.spines['polar'].set_visible(False)
-            
-    buffer = io.BytesIO()
-    plt.savefig(buffer, format='png', transparent=True)
-    buffer.seek(0)
-
-    img = Image.open(buffer)
-
-    plt.close(fig)
-    
-    return img
+            return int(1 + 5 * ((value_info['value'] / max_value) ** 2.5))
+
```

### Comparing `enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/config.py` & `enkacard-3.3.6/enkacard/src/utils/enkanetwork_update/config.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/enka_update.py` & `enkacard-3.3.6/enkacard/src/utils/enkanetwork_update/enka_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     "namecards": [],
     "skills": [],
     "weapons": [],
 }
 
 def save_json(NAME_JSON, data, path = "data"):
     global _PATH
-        
+    
     with open(f"{_PATH}/{path}/{NAME_JSON}", "w", encoding="utf-8") as file:
         json.dump(data, file, indent=4, ensure_ascii=False)
 
 async def fetch_data(url, key, lang = False):
     async with aiohttp.ClientSession() as session:
         async with session.get(url) as response:
             if response.status == 200:
@@ -288,14 +288,17 @@
 async def dowload(path = None):
     global _PATH
     
     if path is None:
         _PATH = await search()
     else:
         _PATH = path
+        
+    if "data" in _PATH:
+        _PATH = _PATH.replace("/data", "")
     
     print(f"Path to enkanetwork.py: {_PATH}")
     print("="*25)
     print(">> Start dowload data")
     variables = {key: globals()[key] for key in ENVKEY}
     task = []
     for key, value in variables.items():
```

### Comparing `enkacard-3.3.5/enkacard/src/utils/enkanetwork_update/pathfinding.py` & `enkacard-3.3.6/enkacard/src/utils/enkanetwork_update/pathfinding.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,9 @@
             break
 
     if enkanetwork_path:
         assets_path = os.path.join(enkanetwork_path, "assets")
 
         if not os.path.exists(assets_path):
             os.makedirs(assets_path)
-
+            
         return assets_path
```

### Comparing `enkacard-3.3.5/enkacard/src/utils/git.py` & `enkacard-3.3.6/enkacard/src/utils/git.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/utils/pickle_cashe.py` & `enkacard-3.3.6/enkacard/src/utils/pickle_cashe.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/utils/pill.py` & `enkacard-3.3.6/enkacard/src/utils/pill.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/enkacard/src/utils/translation.py` & `enkacard-3.3.6/enkacard/src/utils/translation.py`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/pyproject.toml` & `enkacard-3.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "enkacard"
-version = "3.3.5"
+version = "3.3.6"
 description = "An asynchronous module and API that allows you to connect to your bot the generation of Genshin character cards from the Enka.Network website."
 authors = ["None"]
 
 readme = 'README.md'  # Поддерживаются файлы в формате Markdown
 
 repository = "https://github.com/DEViantUA/EnkaCard"
 homepage = "https://github.com/DEViantUA/EnkaCard"
```

### Comparing `enkacard-3.3.5/README.md` & `enkacard-3.3.6/README.md`

 * *Files identical despite different names*

### Comparing `enkacard-3.3.5/PKG-INFO` & `enkacard-3.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enkacard
-Version: 3.3.5
+Version: 3.3.6
 Summary: An asynchronous module and API that allows you to connect to your bot the generation of Genshin character cards from the Enka.Network website.
 Home-page: https://github.com/DEViantUA/EnkaCard
 Author: None
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

