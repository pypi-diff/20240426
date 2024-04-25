# Comparing `tmp/lute3-3.3.1.tar.gz` & `tmp/lute3-3.3.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lute3-3.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lute3-3.3.2b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lute3-3.3.1.tar` & `lute3-3.3.2b1.tar`

### file list

```diff
@@ -1,544 +1,637 @@
--rw-r--r--   0        0        0      170 2023-11-09 08:26:12.050479 lute3-3.3.1/.dockerignore
--rw-r--r--   0        0        0     1280 2024-03-08 03:05:01.842902 lute3-3.3.1/.github/ISSUE_TEMPLATE/add_language.md
--rw-r--r--   0        0        0      590 2024-03-08 03:05:01.843291 lute3-3.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      649 2024-03-08 03:05:01.843443 lute3-3.3.1/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      578 2024-03-08 03:05:01.843637 lute3-3.3.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     7227 2024-03-25 09:32:17.209529 lute3-3.3.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2626 2024-02-07 07:50:18.742841 lute3-3.3.1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     2172 2024-03-08 03:05:01.844585 lute3-3.3.1/.gitignore
--rw-r--r--   0        0        0      395 2024-01-13 04:05:05.193611 lute3-3.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    24735 2023-11-20 01:37:46.796733 lute3-3.3.1/.pylintrc
--rw-r--r--   0        0        0     1076 2024-01-13 04:05:05.194389 lute3-3.3.1/.pytest.ini
--rw-r--r--   0        0        0     1068 2023-11-09 05:33:09.100157 lute3-3.3.1/LICENSE.txt
--rw-r--r--   0        0        0     1677 2024-03-08 03:05:01.844814 lute3-3.3.1/README.md
--rw-r--r--   0        0        0     1036 2024-03-08 03:05:01.845187 lute3-3.3.1/README_PyPi.md
--rw-r--r--   0        0        0     1578 2024-03-08 03:05:01.845433 lute3-3.3.1/devstart.py
--rw-r--r--   0        0        0      965 2023-11-10 18:48:16.706091 lute3-3.3.1/docker/Dockerfile
--rw-r--r--   0        0        0      496 2024-01-13 04:05:05.195405 lute3-3.3.1/docker/README.md
--rwxr-xr-x   0        0        0     1545 2024-01-13 04:05:05.195617 lute3-3.3.1/docker/build_all.sh
--rwxr-xr-x   0        0        0       89 2024-01-13 04:05:05.195716 lute3-3.3.1/docker/build_test.sh
--rw-r--r--   0        0        0     1076 2023-11-09 08:26:12.052441 lute3-3.3.1/docker/check_mounts_and_start.sh
--rw-r--r--   0        0        0      309 2023-11-09 08:26:12.052717 lute3-3.3.1/docker/docker-compose.yml.example
--rw-r--r--   0        0        0     3285 2023-11-10 21:04:52.845194 lute3-3.3.1/docker/docker_hub_overview.md
--rwxr-xr-x   0        0        0     1127 2024-01-13 04:05:05.195822 lute3-3.3.1/docker/try_build_multi.sh
--rw-r--r--   0        0        0    13116 2024-03-25 17:55:55.463221 lute3-3.3.1/docs/CHANGELOG.md
--rw-r--r--   0        0        0       71 2024-01-13 04:05:05.196786 lute3-3.3.1/docs/README.md
--rw-r--r--   0        0        0     1068 2023-11-09 05:33:09.101369 lute3-3.3.1/lute/LICENSE.txt
--rw-r--r--   0        0        0      380 2024-03-25 17:56:07.702354 lute3-3.3.1/lute/__init__.py
--rw-r--r--   0        0        0    11145 2024-03-15 03:25:40.864716 lute3-3.3.1/lute/app_factory.py
--rw-r--r--   0        0        0        0 2023-10-30 00:38:51.292984 lute3-3.3.1/lute/backup/__init__.py
--rw-r--r--   0        0        0     2300 2024-03-15 03:25:40.865078 lute3-3.3.1/lute/backup/routes.py
--rw-r--r--   0        0        0     5303 2024-03-15 03:25:40.865445 lute3-3.3.1/lute/backup/service.py
--rw-r--r--   0        0        0        0 2023-10-24 05:43:55.066190 lute3-3.3.1/lute/bing/__init__.py
--rw-r--r--   0        0        0     3736 2024-03-13 16:30:50.197607 lute3-3.3.1/lute/bing/routes.py
--rw-r--r--   0        0        0        0 2023-10-16 06:20:14.169949 lute3-3.3.1/lute/book/__init__.py
--rw-r--r--   0        0        0     2541 2024-03-15 03:25:40.865805 lute3-3.3.1/lute/book/datatables.py
--rw-r--r--   0        0        0     5118 2024-03-25 09:32:17.256759 lute3-3.3.1/lute/book/forms.py
--rw-r--r--   0        0        0     3229 2024-02-07 07:50:18.747552 lute3-3.3.1/lute/book/model.py
--rw-r--r--   0        0        0     5021 2024-03-25 09:32:17.257357 lute3-3.3.1/lute/book/routes.py
--rw-r--r--   0        0        0     6395 2024-03-25 09:32:17.258143 lute3-3.3.1/lute/book/service.py
--rw-r--r--   0        0        0     3598 2024-02-07 07:50:18.749346 lute3-3.3.1/lute/book/stats.py
--rw-r--r--   0        0        0      475 2024-01-13 04:05:05.200591 lute3-3.3.1/lute/cli/README.md
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.200653 lute3-3.3.1/lute/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-01-13 04:05:05.200788 lute3-3.3.1/lute/cli/commands.py
--rw-r--r--   0        0        0     6313 2024-02-07 07:50:18.749980 lute3-3.3.1/lute/cli/language_term_export.py
--rw-r--r--   0        0        0        0 2023-11-04 21:50:44.080272 lute3-3.3.1/lute/config/__init__.py
--rw-r--r--   0        0        0     2951 2024-03-08 03:05:01.852258 lute3-3.3.1/lute/config/app_config.py
--rw-r--r--   0        0        0      265 2024-01-13 04:05:05.201516 lute3-3.3.1/lute/config/config.yml.docker
--rw-r--r--   0        0        0      667 2024-01-13 04:05:05.201703 lute3-3.3.1/lute/config/config.yml.example
--rw-r--r--   0        0        0      280 2024-01-13 04:05:05.201898 lute3-3.3.1/lute/config/config.yml.prod
--rw-r--r--   0        0        0      108 2023-10-20 18:48:10.167405 lute3-3.3.1/lute/db/__init__.py
--rw-r--r--   0        0        0     1021 2024-02-07 07:50:18.750797 lute3-3.3.1/lute/db/data_cleanup.py
--rw-r--r--   0        0        0     5149 2024-02-19 02:42:49.327314 lute3-3.3.1/lute/db/demo.py
--rw-r--r--   0        0        0      218 2023-11-04 21:50:44.081606 lute3-3.3.1/lute/db/demo/README.md
--rw-r--r--   0        0        0      329 2024-02-19 02:42:49.327569 lute3-3.3.1/lute/db/demo/languages/_language.yaml.example
--rw-r--r--   0        0        0      555 2024-03-13 16:31:06.434103 lute3-3.3.1/lute/db/demo/languages/arabic.yaml
--rw-r--r--   0        0        0      416 2024-03-13 16:31:06.435007 lute3-3.3.1/lute/db/demo/languages/classical_chinese.yaml
--rw-r--r--   0        0        0      377 2024-03-13 16:30:50.199703 lute3-3.3.1/lute/db/demo/languages/czech.yaml
--rw-r--r--   0        0        0      468 2024-03-08 03:05:01.854310 lute3-3.3.1/lute/db/demo/languages/english.yaml
--rw-r--r--   0        0        0      370 2024-02-19 02:42:49.328806 lute3-3.3.1/lute/db/demo/languages/french.yaml
--rw-r--r--   0        0        0      522 2024-03-25 09:32:17.258859 lute3-3.3.1/lute/db/demo/languages/german.yaml
--rw-r--r--   0        0        0      635 2024-02-19 02:42:49.345862 lute3-3.3.1/lute/db/demo/languages/greek.yaml
--rw-r--r--   0        0        0      566 2024-03-17 12:47:12.943581 lute3-3.3.1/lute/db/demo/languages/hindi.yaml
--rw-r--r--   0        0        0      539 2024-02-19 02:42:49.353007 lute3-3.3.1/lute/db/demo/languages/japanese.yaml
--rw-r--r--   0        0        0      470 2024-02-19 02:42:49.353261 lute3-3.3.1/lute/db/demo/languages/russian.yaml
--rw-r--r--   0        0        0      477 2024-02-19 02:42:49.353524 lute3-3.3.1/lute/db/demo/languages/sanskrit.yaml
--rw-r--r--   0        0        0      526 2024-02-19 02:42:49.353778 lute3-3.3.1/lute/db/demo/languages/spanish.yaml
--rw-r--r--   0        0        0      497 2024-03-13 16:30:50.200498 lute3-3.3.1/lute/db/demo/languages/turkish.yaml
--rw-r--r--   0        0        0       41 2024-01-13 04:05:05.205521 lute3-3.3.1/lute/db/demo/stories/_language.txt.example
--rw-r--r--   0        0        0     1147 2023-11-04 21:50:44.084462 lute3-3.3.1/lute/db/demo/stories/ar_demo.txt
--rw-r--r--   0        0        0     1412 2023-11-04 21:50:44.084742 lute3-3.3.1/lute/db/demo/stories/cc_demo.txt
--rw-r--r--   0        0        0      518 2024-01-13 04:05:05.205664 lute3-3.3.1/lute/db/demo/stories/czech.txt
--rw-r--r--   0        0        0     1058 2024-02-07 07:50:18.752049 lute3-3.3.1/lute/db/demo/stories/de_Stadtmusikanten.txt
--rw-r--r--   0        0        0      534 2023-11-04 21:50:44.085346 lute3-3.3.1/lute/db/demo/stories/es_aladino.txt
--rw-r--r--   0        0        0      469 2023-11-04 21:50:44.085648 lute3-3.3.1/lute/db/demo/stories/fr_goldilocks.txt
--rw-r--r--   0        0        0     1649 2023-11-04 21:50:44.085961 lute3-3.3.1/lute/db/demo/stories/gr_demo.txt
--rw-r--r--   0        0        0      587 2024-01-13 04:05:05.206792 lute3-3.3.1/lute/db/demo/stories/hi_wikipedia.txt
--rw-r--r--   0        0        0      428 2023-11-04 21:50:44.086295 lute3-3.3.1/lute/db/demo/stories/jp_kitakaze_to_taiyou.txt
--rw-r--r--   0        0        0      546 2024-01-13 04:05:05.206925 lute3-3.3.1/lute/db/demo/stories/ru_medved.txt
--rw-r--r--   0        0        0     1027 2024-02-07 07:50:18.752322 lute3-3.3.1/lute/db/demo/stories/sanskrit.txt
--rw-r--r--   0        0        0      941 2023-11-04 21:50:44.086743 lute3-3.3.1/lute/db/demo/stories/tr_demo.txt
--rw-r--r--   0        0        0     7053 2024-02-19 02:42:49.354480 lute3-3.3.1/lute/db/demo/stories/tutorial.txt
--rw-r--r--   0        0        0     3555 2024-02-19 02:42:49.354846 lute3-3.3.1/lute/db/demo/stories/tutorial_follow_up.txt
--rw-r--r--   0        0        0      615 2023-11-09 09:07:06.767671 lute3-3.3.1/lute/db/management.py
--rw-r--r--   0        0        0     1620 2023-10-26 01:04:31.825247 lute3-3.3.1/lute/db/schema/README.md
--rw-r--r--   0        0        0    42691 2024-03-25 09:32:17.260034 lute3-3.3.1/lute/db/schema/baseline.sql
--rw-r--r--   0        0        0     8817 2024-03-08 03:05:01.856057 lute3-3.3.1/lute/db/schema/empty.sql
--rw-r--r--   0        0        0      246 2023-10-20 18:48:10.168442 lute3-3.3.1/lute/db/schema/migrations/20230409_224327_load_statuses.sql
--rw-r--r--   0        0        0      178 2023-10-20 18:48:10.168634 lute3-3.3.1/lute/db/schema/migrations/20230414_225828_add_texttokens_TokTextLC.sql
--rw-r--r--   0        0        0      245 2023-10-20 18:48:10.168826 lute3-3.3.1/lute/db/schema/migrations/20230428_224656_create_wordflashmessages_table.sql
--rw-r--r--   0        0        0     2067 2023-10-20 18:48:10.169209 lute3-3.3.1/lute/db/schema/migrations/20230518_190000_remove_old_words_fields.sql
--rw-r--r--   0        0        0      680 2023-10-20 18:48:10.169512 lute3-3.3.1/lute/db/schema/migrations/20230519_194627_add_TxDateRead.sql
--rw-r--r--   0        0        0       96 2023-10-20 18:48:10.169708 lute3-3.3.1/lute/db/schema/migrations/20230621_010000_drop_texttags_table.sql
--rw-r--r--   0        0        0     1143 2023-10-20 18:48:10.169918 lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_01_booktags.sql
--rw-r--r--   0        0        0     1141 2023-10-20 18:48:10.170132 lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_02_wordtags.sql
--rw-r--r--   0        0        0     1226 2023-10-20 18:48:10.170317 lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_03_sentences.sql
--rw-r--r--   0        0        0     1214 2023-10-20 18:48:10.170503 lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_04_texttokens.sql
--rw-r--r--   0        0        0     1559 2023-10-20 18:48:10.170690 lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_05_texts.sql
--rw-r--r--   0        0        0     1147 2023-10-20 18:48:10.170868 lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_06_bookstats.sql
--rw-r--r--   0        0        0     1038 2023-10-20 18:48:10.171044 lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_07_termimages.sql
--rw-r--r--   0        0        0     1044 2023-10-20 18:48:10.171217 lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_08_wordflashmessages.sql
--rw-r--r--   0        0        0     1213 2023-10-20 18:48:10.171396 lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_09_wordparents.sql
--rw-r--r--   0        0        0     2022 2023-10-20 18:48:10.171568 lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_10_words.sql
--rw-r--r--   0        0        0     1227 2023-10-20 18:48:10.171723 lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_11_books.sql
--rw-r--r--   0        0        0       56 2023-10-20 18:48:10.171870 lute3-3.3.1/lute/db/schema/migrations/20230623_234104_drop_TxTitle.sql
--rw-r--r--   0        0        0       38 2023-10-20 18:48:10.172012 lute3-3.3.1/lute/db/schema/migrations/20230624_182104_drop_index_TxBkIDTxOrder.sql
--rw-r--r--   0        0        0      908 2023-10-20 18:48:10.172172 lute3-3.3.1/lute/db/schema/migrations/20230818_201200_add_BkWordCount.sql
--rw-r--r--   0        0        0       87 2023-10-20 18:48:10.172337 lute3-3.3.1/lute/db/schema/migrations/20230819_044107_drop_texttokens.sql
--rw-r--r--   0        0        0      168 2023-10-20 18:48:10.172618 lute3-3.3.1/lute/db/schema/migrations/20230819_050036_vacuum.sql
--rw-r--r--   0        0        0      736 2023-10-20 18:48:10.172795 lute3-3.3.1/lute/db/schema/migrations/20230827_052154_allow_multiple_word_parents.sql
--rw-r--r--   0        0        0     1031 2023-10-20 18:48:10.173096 lute3-3.3.1/lute/db/schema/migrations/20231018_211236_remove_excess_texts_fields.sql
--rw-r--r--   0        0        0      930 2023-11-03 01:33:16.686624 lute3-3.3.1/lute/db/schema/migrations/20231101_203811_modify_settings_schema.sql
--rw-r--r--   0        0        0      114 2024-01-13 04:05:05.209858 lute3-3.3.1/lute/db/schema/migrations/20231130_141236_add_TxWordCount.sql
--rw-r--r--   0        0        0      194 2024-01-13 04:05:05.210324 lute3-3.3.1/lute/db/schema/migrations/20231210_103924_add_book_audio_fields.sql
--rw-r--r--   0        0        0       65 2024-02-07 07:50:18.754352 lute3-3.3.1/lute/db/schema/migrations/20240101_122610_add_bookstats_status_distribution.sql
--rw-r--r--   0        0        0       70 2024-02-07 07:50:18.754640 lute3-3.3.1/lute/db/schema/migrations/20240113_215142_add_term_follow_parent_bool.sql
--rw-r--r--   0        0        0      194 2024-02-07 07:50:18.754951 lute3-3.3.1/lute/db/schema/migrations/20240118_154258_change_status_abbrev.sql
--rw-r--r--   0        0        0     1487 2024-02-07 07:50:18.755302 lute3-3.3.1/lute/db/schema/migrations/20240125_drop_BkWordCount.sql
--rw-r--r--   0        0        0     1188 2024-02-07 07:50:18.755674 lute3-3.3.1/lute/db/schema/migrations/20240125_drop_bookstats_wordcount.sql
--rw-r--r--   0        0        0     1877 2024-02-19 02:42:49.355669 lute3-3.3.1/lute/db/schema/migrations/20240207_01_create_languagedicts.sql
--rw-r--r--   0        0        0     1570 2024-02-19 02:42:49.355795 lute3-3.3.1/lute/db/schema/migrations/20240207_02_drop_old_language_fields.sql
--rw-r--r--   0        0        0      224 2023-10-20 18:48:10.173345 lute3-3.3.1/lute/db/schema/migrations/README.md
--rw-r--r--   0        0        0      222 2023-11-03 01:33:16.686865 lute3-3.3.1/lute/db/schema/migrations_repeatable/README.md
--rw-r--r--   0        0        0      992 2024-02-07 07:50:18.756034 lute3-3.3.1/lute/db/schema/migrations_repeatable/trig_wordparents.sql
--rw-r--r--   0        0        0     1751 2024-03-25 09:32:17.264354 lute3-3.3.1/lute/db/schema/migrations_repeatable/trig_words.sql
--rw-r--r--   0        0        0       36 2023-11-03 01:33:16.687020 lute3-3.3.1/lute/db/schema/migrations_repeatable/vacuum.sql
--rw-r--r--   0        0        0        0 2023-10-20 18:48:10.173889 lute3-3.3.1/lute/db/setup/__init__.py
--rw-r--r--   0        0        0     5201 2023-11-11 22:05:26.094785 lute3-3.3.1/lute/db/setup/main.py
--rw-r--r--   0        0        0     3726 2023-11-08 00:06:31.606907 lute3-3.3.1/lute/db/setup/migrator.py
--rw-r--r--   0        0        0        0 2023-11-01 07:45:01.506123 lute3-3.3.1/lute/dev_api/__init__.py
--rw-r--r--   0        0        0     5096 2024-02-19 02:42:49.356009 lute3-3.3.1/lute/dev_api/routes.py
--rw-r--r--   0        0        0        0 2023-10-16 06:20:14.170764 lute3-3.3.1/lute/language/__init__.py
--rw-r--r--   0        0        0     3088 2024-02-19 02:42:49.356211 lute3-3.3.1/lute/language/forms.py
--rw-r--r--   0        0        0     5565 2024-03-13 16:30:50.202194 lute3-3.3.1/lute/language/routes.py
--rw-r--r--   0        0        0     3267 2024-01-13 04:05:05.211861 lute3-3.3.1/lute/main.py
--rw-r--r--   0        0        0        0 2023-10-04 05:48:35.020519 lute3-3.3.1/lute/models/__init__.py
--rw-r--r--   0        0        0    11122 2024-03-15 03:25:40.869518 lute3-3.3.1/lute/models/book.py
--rw-r--r--   0        0        0     6055 2024-03-08 03:05:01.857922 lute3-3.3.1/lute/models/language.py
--rw-r--r--   0        0        0     8672 2024-03-13 16:31:06.436856 lute3-3.3.1/lute/models/setting.py
--rw-r--r--   0        0        0    11738 2024-03-25 09:32:17.265003 lute3-3.3.1/lute/models/term.py
--rw-r--r--   0        0        0        0 2023-10-07 05:09:39.898452 lute3-3.3.1/lute/parse/__init__.py
--rw-r--r--   0        0        0     3918 2024-03-08 03:05:01.859321 lute3-3.3.1/lute/parse/base.py
--rw-r--r--   0        0        0     1646 2023-11-08 00:06:31.610408 lute3-3.3.1/lute/parse/character_parser.py
--rw-r--r--   0        0        0     4735 2024-03-08 03:05:01.859524 lute3-3.3.1/lute/parse/mecab_parser.py
--rw-r--r--   0        0        0     1680 2024-03-08 03:05:01.859845 lute3-3.3.1/lute/parse/registry.py
--rw-r--r--   0        0        0     4182 2024-03-17 12:47:12.946271 lute3-3.3.1/lute/parse/space_delimited_parser.py
--rw-r--r--   0        0        0        0 2023-10-16 06:20:14.172648 lute3-3.3.1/lute/read/__init__.py
--rw-r--r--   0        0        0      211 2023-11-08 00:06:31.611930 lute3-3.3.1/lute/read/forms.py
--rw-r--r--   0        0        0        0 2023-10-18 06:43:42.367570 lute3-3.3.1/lute/read/render/__init__.py
--rw-r--r--   0        0        0    17547 2024-03-25 09:32:17.265933 lute3-3.3.1/lute/read/render/renderable_calculator.py
--rw-r--r--   0        0        0     5653 2024-03-25 17:52:05.380914 lute3-3.3.1/lute/read/render/service.py
--rw-r--r--   0        0        0     7010 2024-03-25 09:32:17.266834 lute3-3.3.1/lute/read/routes.py
--rw-r--r--   0        0        0     5429 2024-03-25 17:48:03.854029 lute3-3.3.1/lute/read/service.py
--rw-r--r--   0        0        0        0 2023-11-03 06:31:15.939906 lute3-3.3.1/lute/settings/__init__.py
--rw-r--r--   0        0        0     5264 2024-03-13 16:31:06.437777 lute3-3.3.1/lute/settings/routes.py
--rw-r--r--   0        0        0     1738 2023-10-04 05:48:35.022956 lute3-3.3.1/lute/static/css/images/animated-overlay.gif
--rw-r--r--   0        0        0     2434 2023-10-04 05:48:35.023257 lute3-3.3.1/lute/static/css/images/jplayer-black-and-yellow.png
--rw-r--r--   0        0        0    14525 2023-10-04 05:48:35.023672 lute3-3.3.1/lute/static/css/images/jplayer.blue.monday.jpg
--rw-r--r--   0        0        0   304064 2023-10-04 05:48:35.024510 lute3-3.3.1/lute/static/css/images/pbar-ani.gif
--rw-r--r--   0        0        0      212 2023-10-04 05:48:35.024852 lute3-3.3.1/lute/static/css/images/ui-bg_flat_0_555555_40x100.png
--rw-r--r--   0        0        0      180 2023-10-04 05:48:35.025123 lute3-3.3.1/lute/static/css/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-r--r--   0        0        0      220 2023-10-04 05:48:35.025729 lute3-3.3.1/lute/static/css/images/ui-bg_flat_75_222222_40x100.png
--rw-r--r--   0        0        0      220 2023-10-04 05:48:35.026029 lute3-3.3.1/lute/static/css/images/ui-bg_flat_75_444444_40x100.png
--rw-r--r--   0        0        0      178 2023-10-04 05:48:35.026359 lute3-3.3.1/lute/static/css/images/ui-bg_flat_75_ffffff_40x100.png
--rw-r--r--   0        0        0      120 2023-10-04 05:48:35.026642 lute3-3.3.1/lute/static/css/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0        0        0      105 2023-10-04 05:48:35.026929 lute3-3.3.1/lute/static/css/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0        0        0      111 2023-10-04 05:48:35.027288 lute3-3.3.1/lute/static/css/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0        0        0      110 2023-10-04 05:48:35.027566 lute3-3.3.1/lute/static/css/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0        0        0      119 2023-10-04 05:48:35.027847 lute3-3.3.1/lute/static/css/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0        0        0      277 2023-10-04 05:48:35.028257 lute3-3.3.1/lute/static/css/images/ui-bg_highlight-soft_75_222222_1x100.png
--rw-r--r--   0        0        0      101 2023-10-04 05:48:35.028513 lute3-3.3.1/lute/static/css/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0        0        0      251 2023-10-04 05:48:35.028793 lute3-3.3.1/lute/static/css/images/ui-bg_inset-hard_55_333333_1x100.png
--rw-r--r--   0        0        0      251 2023-10-04 05:48:35.029316 lute3-3.3.1/lute/static/css/images/ui-bg_inset-hard_95_444444_1x100.png
--rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.029681 lute3-3.3.1/lute/static/css/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.030066 lute3-3.3.1/lute/static/css/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0        0        0     6992 2023-10-04 05:48:35.030537 lute3-3.3.1/lute/static/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.030833 lute3-3.3.1/lute/static/css/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     6988 2023-10-04 05:48:35.031207 lute3-3.3.1/lute/static/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     4549 2023-10-04 05:48:35.031493 lute3-3.3.1/lute/static/css/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     6999 2023-10-04 05:48:35.031792 lute3-3.3.1/lute/static/css/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.032071 lute3-3.3.1/lute/static/css/images/ui-icons_888888_256x240.png
--rw-r--r--   0        0        0     6991 2023-10-04 05:48:35.032366 lute3-3.3.1/lute/static/css/images/ui-icons_BBBBBB_256x240.png
--rw-r--r--   0        0        0     4549 2023-10-04 05:48:35.032703 lute3-3.3.1/lute/static/css/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.033223 lute3-3.3.1/lute/static/css/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0     6299 2023-10-04 05:48:35.033571 lute3-3.3.1/lute/static/css/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0     7193 2024-02-07 07:50:18.761528 lute3-3.3.1/lute/static/css/player-styles.css
--rw-r--r--   0        0        0    40805 2024-03-25 09:32:17.268825 lute3-3.3.1/lute/static/css/styles.css
--rw-r--r--   0        0        0    15406 2023-10-04 05:48:35.035622 lute3-3.3.1/lute/static/favicon.ico
--rw-r--r--   0        0        0    15406 2023-10-04 05:48:35.036140 lute3-3.3.1/lute/static/favicon_dev.ico
--rw-r--r--   0        0        0      485 2023-10-04 05:48:35.036488 lute3-3.3.1/lute/static/icn/arrow-000-medium.png
--rw-r--r--   0        0        0      479 2023-10-04 05:48:35.036809 lute3-3.3.1/lute/static/icn/arrow-180-medium.png
--rw-r--r--   0        0        0      811 2023-10-04 05:48:35.037131 lute3-3.3.1/lute/static/icn/arrow-circle-135.png
--rw-r--r--   0        0        0      790 2023-10-04 05:48:35.037385 lute3-3.3.1/lute/static/icn/arrow-circle-225-left.png
--rw-r--r--   0        0        0      786 2023-10-04 05:48:35.037680 lute3-3.3.1/lute/static/icn/arrow-circle-315.png
--rw-r--r--   0        0        0      485 2023-10-04 05:48:35.037925 lute3-3.3.1/lute/static/icn/arrow-norepeat.png
--rw-r--r--   0        0        0      587 2023-10-04 05:48:35.038190 lute3-3.3.1/lute/static/icn/arrow-repeat.png
--rw-r--r--   0        0        0      601 2023-10-04 05:48:35.038457 lute3-3.3.1/lute/static/icn/arrow-stop.png
--rw-r--r--   0        0        0      622 2023-10-04 05:48:35.038703 lute3-3.3.1/lute/static/icn/book--pencil.png
--rw-r--r--   0        0        0      650 2023-10-04 05:48:35.038940 lute3-3.3.1/lute/static/icn/book-open-bookmark.png
--rw-r--r--   0        0        0      613 2023-10-04 05:48:35.039204 lute3-3.3.1/lute/static/icn/book-open-text.png
--rw-r--r--   0        0        0      600 2024-02-19 02:42:49.358289 lute3-3.3.1/lute/static/icn/book-open-text.svg
--rw-r--r--   0        0        0      552 2024-01-13 04:05:05.217231 lute3-3.3.1/lute/static/icn/bookmark-off.svg
--rw-r--r--   0        0        0      414 2024-01-13 04:05:05.217572 lute3-3.3.1/lute/static/icn/bookmark-on.svg
--rw-r--r--   0        0        0      784 2023-10-04 05:48:35.039508 lute3-3.3.1/lute/static/icn/broom.png
--rw-r--r--   0        0        0      398 2023-10-04 05:48:35.039745 lute3-3.3.1/lute/static/icn/calculator.png
--rw-r--r--   0        0        0      405 2023-10-04 05:48:35.040009 lute3-3.3.1/lute/static/icn/card--minus.png
--rw-r--r--   0        0        0      556 2023-10-04 05:48:35.040231 lute3-3.3.1/lute/static/icn/card--pencil.png
--rw-r--r--   0        0        0      504 2023-10-04 05:48:35.040493 lute3-3.3.1/lute/static/icn/card--plus.png
--rw-r--r--   0        0        0      473 2023-10-04 05:48:35.040762 lute3-3.3.1/lute/static/icn/cards-stack.png
--rw-r--r--   0        0        0      434 2024-01-13 04:05:05.218143 lute3-3.3.1/lute/static/icn/caret-left.svg
--rw-r--r--   0        0        0      427 2024-01-13 04:05:05.218284 lute3-3.3.1/lute/static/icn/caret-right.svg
--rw-r--r--   0        0        0      369 2023-10-04 05:48:35.041070 lute3-3.3.1/lute/static/icn/chain.png
--rw-r--r--   0        0        0      624 2023-10-04 05:48:35.041330 lute3-3.3.1/lute/static/icn/clock.png
--rw-r--r--   0        0        0      952 2024-02-07 07:50:18.763469 lute3-3.3.1/lute/static/icn/close-white.svg
--rw-r--r--   0        0        0     1438 2024-01-13 04:05:05.219492 lute3-3.3.1/lute/static/icn/close.svg
--rw-r--r--   0        0        0      404 2023-10-04 05:48:35.041576 lute3-3.3.1/lute/static/icn/control-180.png
--rw-r--r--   0        0        0      511 2023-10-04 05:48:35.041944 lute3-3.3.1/lute/static/icn/control-stop-180.png
--rw-r--r--   0        0        0      523 2023-10-04 05:48:35.042219 lute3-3.3.1/lute/static/icn/control-stop.png
--rw-r--r--   0        0        0      405 2023-10-04 05:48:35.042485 lute3-3.3.1/lute/static/icn/control.png
--rw-r--r--   0        0        0      920 2023-10-04 05:48:35.042813 lute3-3.3.1/lute/static/icn/cross-big.png
--rw-r--r--   0        0        0      555 2023-10-04 05:48:35.043135 lute3-3.3.1/lute/static/icn/cross-button.png
--rw-r--r--   0        0        0      544 2023-10-04 05:48:35.043410 lute3-3.3.1/lute/static/icn/cross.png
--rw-r--r--   0        0        0      658 2023-10-04 05:48:35.043716 lute3-3.3.1/lute/static/icn/document--pencil.png
--rw-r--r--   0        0        0     1761 2024-02-07 07:50:18.763842 lute3-3.3.1/lute/static/icn/drag-handle.svg
--rw-r--r--   0        0        0      674 2023-10-04 05:48:35.043952 lute3-3.3.1/lute/static/icn/drawer--minus.png
--rw-r--r--   0        0        0      717 2023-10-04 05:48:35.044272 lute3-3.3.1/lute/static/icn/drawer--plus.png
--rwxr-xr-x   0        0        0       55 2023-10-04 05:48:35.044638 lute3-3.3.1/lute/static/icn/empty.gif
--rw-r--r--   0        0        0      680 2023-10-04 05:48:35.044851 lute3-3.3.1/lute/static/icn/eraser.png
--rw-r--r--   0        0        0      539 2023-10-04 05:48:35.045049 lute3-3.3.1/lute/static/icn/exclamation-button.png
--rw-r--r--   0        0        0      658 2023-10-04 05:48:35.045241 lute3-3.3.1/lute/static/icn/exclamation-red.png
--rw-r--r--   0        0        0      685 2023-10-04 05:48:35.045451 lute3-3.3.1/lute/static/icn/external.png
--rw-r--r--   0        0        0      536 2023-10-04 05:48:35.045663 lute3-3.3.1/lute/static/icn/eye.png
--rw-r--r--   0        0        0      792 2023-10-04 05:48:35.045884 lute3-3.3.1/lute/static/icn/feed--pencil.png
--rw-r--r--   0        0        0      737 2023-10-04 05:48:35.046102 lute3-3.3.1/lute/static/icn/feed--plus.png
--rw-r--r--   0        0        0      566 2024-01-13 04:05:05.221040 lute3-3.3.1/lute/static/icn/ff.svg
--rw-r--r--   0        0        0     1297 2024-01-13 04:05:05.221203 lute3-3.3.1/lute/static/icn/font-decrease.svg
--rw-r--r--   0        0        0     1378 2024-01-13 04:05:05.221326 lute3-3.3.1/lute/static/icn/font-increase.svg
--rw-r--r--   0        0        0      630 2023-10-04 05:48:35.046306 lute3-3.3.1/lute/static/icn/funnel--minus.png
--rw-r--r--   0        0        0      543 2023-10-04 05:48:35.046715 lute3-3.3.1/lute/static/icn/funnel.png
--rw-r--r--   0        0        0      617 2024-02-19 02:42:49.358629 lute3-3.3.1/lute/static/icn/images.svg
--rw-r--r--   0        0        0      692 2023-10-04 05:48:35.047033 lute3-3.3.1/lute/static/icn/inbox-download.png
--rw-r--r--   0        0        0      674 2023-10-04 05:48:35.047235 lute3-3.3.1/lute/static/icn/inbox-upload.png
--rw-r--r--   0        0        0     1553 2023-10-04 05:48:35.047472 lute3-3.3.1/lute/static/icn/indicator.gif
--rw-r--r--   0        0        0     1039 2023-10-04 05:48:35.047683 lute3-3.3.1/lute/static/icn/light-bulb-A.png
--rw-r--r--   0        0        0     1037 2023-10-04 05:48:35.047913 lute3-3.3.1/lute/static/icn/light-bulb-T.png
--rw-r--r--   0        0        0     1010 2023-10-04 05:48:35.048117 lute3-3.3.1/lute/static/icn/light-bulb-off-A.png
--rw-r--r--   0        0        0     1001 2023-10-04 05:48:35.048320 lute3-3.3.1/lute/static/icn/light-bulb-off-T.png
--rw-r--r--   0        0        0      943 2023-10-04 05:48:35.048686 lute3-3.3.1/lute/static/icn/light-bulb-off.png
--rw-r--r--   0        0        0      947 2023-10-04 05:48:35.048956 lute3-3.3.1/lute/static/icn/light-bulb.png
--rw-r--r--   0        0        0      631 2023-10-04 05:48:35.049160 lute3-3.3.1/lute/static/icn/lightning.png
--rw-r--r--   0        0        0     1687 2024-01-13 04:05:05.222154 lute3-3.3.1/lute/static/icn/line-spacing-decrease.svg
--rw-r--r--   0        0        0     2575 2024-01-13 04:05:05.222293 lute3-3.3.1/lute/static/icn/line-spacing-increase.svg
--rw-r--r--   0        0        0      277 2024-02-19 02:42:49.358831 lute3-3.3.1/lute/static/icn/list.svg
--rw-r--r--   0        0        0      451 2023-10-04 05:48:35.049360 lute3-3.3.1/lute/static/icn/minus-button.png
--rw-r--r--   0        0        0      259 2023-10-04 05:48:35.049740 lute3-3.3.1/lute/static/icn/minus.png
--rw-r--r--   0        0        0      489 2023-10-04 05:48:35.049931 lute3-3.3.1/lute/static/icn/navigation-000-button-light.png
--rw-r--r--   0        0        0      614 2023-10-04 05:48:35.050311 lute3-3.3.1/lute/static/icn/navigation-000-button.png
--rw-r--r--   0        0        0      486 2023-10-04 05:48:35.050548 lute3-3.3.1/lute/static/icn/navigation-180-button-light.png
--rw-r--r--   0        0        0      620 2023-10-04 05:48:35.050750 lute3-3.3.1/lute/static/icn/navigation-180-button.png
--rw-r--r--   0        0        0      607 2023-10-04 05:48:35.050975 lute3-3.3.1/lute/static/icn/new_line.png
--rw-r--r--   0        0        0      458 2024-01-13 04:05:05.222661 lute3-3.3.1/lute/static/icn/next.svg
--rw-r--r--   0        0        0      633 2023-10-04 05:48:35.051264 lute3-3.3.1/lute/static/icn/notebook--minus.png
--rw-r--r--   0        0        0      723 2023-10-04 05:48:35.051477 lute3-3.3.1/lute/static/icn/notebook--pencil.png
--rw-r--r--   0        0        0      664 2023-10-04 05:48:35.051850 lute3-3.3.1/lute/static/icn/notebook--plus.png
--rw-r--r--   0        0        0      541 2023-10-04 05:48:35.052045 lute3-3.3.1/lute/static/icn/notebook.png
--rw-r--r--   0        0        0      790 2024-01-13 04:05:05.223020 lute3-3.3.1/lute/static/icn/open.svg
--rw-r--r--   0        0        0      428 2024-01-13 04:05:05.223265 lute3-3.3.1/lute/static/icn/pause.svg
--rw-r--r--   0        0        0      475 2023-10-04 05:48:35.052249 lute3-3.3.1/lute/static/icn/pencil.png
--rw-r--r--   0        0        0     1154 2023-10-04 05:48:35.052521 lute3-3.3.1/lute/static/icn/photo-album.png
--rw-r--r--   0        0        0      591 2024-01-13 04:05:05.223508 lute3-3.3.1/lute/static/icn/pin.svg
--rw-r--r--   0        0        0      142 2023-10-04 05:48:35.052720 lute3-3.3.1/lute/static/icn/placeholder.png
--rw-r--r--   0        0        0      461 2024-01-13 04:05:05.223871 lute3-3.3.1/lute/static/icn/play.svg
--rw-r--r--   0        0        0      583 2023-10-04 05:48:35.052918 lute3-3.3.1/lute/static/icn/plus-button.png
--rw-r--r--   0        0        0      521 2023-10-04 05:48:35.053238 lute3-3.3.1/lute/static/icn/plus.png
--rw-r--r--   0        0        0      445 2024-01-13 04:05:05.224128 lute3-3.3.1/lute/static/icn/prev.svg
--rw-r--r--   0        0        0      722 2023-10-04 05:48:35.053446 lute3-3.3.1/lute/static/icn/printer.png
--rw-r--r--   0        0        0      722 2023-10-04 05:48:35.053709 lute3-3.3.1/lute/static/icn/question-balloon.png
--rw-r--r--   0        0        0      924 2023-10-04 05:48:35.053893 lute3-3.3.1/lute/static/icn/question-frame.png
--rw-r--r--   0        0        0     1921 2024-02-07 07:50:18.764174 lute3-3.3.1/lute/static/icn/reload.png
--rw-r--r--   0        0        0      558 2024-01-13 04:05:05.224511 lute3-3.3.1/lute/static/icn/rewind.svg
--rw-r--r--   0        0        0      837 2023-10-04 05:48:35.054103 lute3-3.3.1/lute/static/icn/script-import.png
--rw-r--r--   0        0        0     1041 2024-03-13 16:31:06.440554 lute3-3.3.1/lute/static/icn/settings-gear-icon.svg
--rw-r--r--   0        0        0      526 2024-01-13 04:05:05.224876 lute3-3.3.1/lute/static/icn/skip-back.svg
--rw-r--r--   0        0        0      755 2023-10-04 05:48:35.054284 lute3-3.3.1/lute/static/icn/smiley-sad.png
--rw-r--r--   0        0        0      811 2023-10-04 05:48:35.054463 lute3-3.3.1/lute/static/icn/smiley.png
--rw-r--r--   0        0        0      452 2023-10-04 05:48:35.054648 lute3-3.3.1/lute/static/icn/speaker-volume-none.png
--rw-r--r--   0        0        0      543 2023-10-04 05:48:35.054955 lute3-3.3.1/lute/static/icn/speaker-volume.png
--rw-r--r--   0        0        0      504 2024-01-13 04:05:05.225270 lute3-3.3.1/lute/static/icn/speed.svg
--rw-r--r--   0        0        0      757 2023-10-04 05:48:35.055365 lute3-3.3.1/lute/static/icn/star.png
--rw-r--r--   0        0        0      432 2023-10-04 05:48:35.055719 lute3-3.3.1/lute/static/icn/status-away.png
--rw-r--r--   0        0        0      407 2023-10-04 05:48:35.056570 lute3-3.3.1/lute/static/icn/status-busy.png
--rw-r--r--   0        0        0      401 2023-10-04 05:48:35.056940 lute3-3.3.1/lute/static/icn/status.png
--rw-r--r--   0        0        0      466 2023-10-04 05:48:35.057163 lute3-3.3.1/lute/static/icn/sticky-note--minus.png
--rw-r--r--   0        0        0      638 2023-10-04 05:48:35.057670 lute3-3.3.1/lute/static/icn/sticky-note--pencil.png
--rw-r--r--   0        0        0      571 2023-10-04 05:48:35.057865 lute3-3.3.1/lute/static/icn/sticky-note--plus.png
--rw-r--r--   0        0        0      520 2023-10-04 05:48:35.058304 lute3-3.3.1/lute/static/icn/sticky-note-text.png
--rw-r--r--   0        0        0      425 2023-10-04 05:48:35.058599 lute3-3.3.1/lute/static/icn/sticky-note.png
--rw-r--r--   0        0        0      533 2023-10-04 05:48:35.058808 lute3-3.3.1/lute/static/icn/sticky-notes-stack.png
--rw-r--r--   0        0        0      618 2023-10-04 05:48:35.059020 lute3-3.3.1/lute/static/icn/sticky-notes-text.png
--rw-r--r--   0        0        0      546 2023-10-04 05:48:35.059221 lute3-3.3.1/lute/static/icn/sticky-notes.png
--rw-r--r--   0        0        0     2805 2023-10-04 05:48:35.059585 lute3-3.3.1/lute/static/icn/test_correct.png
--rw-r--r--   0        0        0     2805 2023-10-04 05:48:35.059871 lute3-3.3.1/lute/static/icn/test_notyet.png
--rw-r--r--   0        0        0     2805 2023-10-04 05:48:35.060061 lute3-3.3.1/lute/static/icn/test_wrong.png
--rw-r--r--   0        0        0      803 2024-01-13 04:05:05.225875 lute3-3.3.1/lute/static/icn/text-column-one.svg
--rw-r--r--   0        0        0     1613 2024-01-13 04:05:05.226200 lute3-3.3.1/lute/static/icn/text-column-two.svg
--rw-r--r--   0        0        0      732 2023-10-04 05:48:35.060251 lute3-3.3.1/lute/static/icn/thumb-up.png
--rw-r--r--   0        0        0      751 2023-10-04 05:48:35.060509 lute3-3.3.1/lute/static/icn/thumb.png
--rwxr-xr-x   0        0        0      620 2023-10-04 05:48:35.060685 lute3-3.3.1/lute/static/icn/tick-button-small.png
--rw-r--r--   0        0        0      568 2023-10-04 05:48:35.060894 lute3-3.3.1/lute/static/icn/tick-button.png
--rw-r--r--   0        0        0      582 2023-10-04 05:48:35.061228 lute3-3.3.1/lute/static/icn/tick.png
--rw-r--r--   0        0        0      521 2024-01-13 04:05:05.226487 lute3-3.3.1/lute/static/icn/volume.svg
--rw-r--r--   0        0        0     3208 2023-10-04 05:48:35.061448 lute3-3.3.1/lute/static/icn/waiting.gif
--rw-r--r--   0        0        0      847 2023-10-04 05:48:35.061633 lute3-3.3.1/lute/static/icn/waiting2.gif
--rw-r--r--   0        0        0     5450 2023-10-04 05:48:35.061895 lute3-3.3.1/lute/static/icn/wizard.png
--rw-r--r--   0        0        0      916 2023-10-04 05:48:35.062193 lute3-3.3.1/lute/static/icn/wrench-screwdriver.png
--rw-r--r--   0        0        0    19567 2023-10-04 05:48:35.062586 lute3-3.3.1/lute/static/img/apple-touch-icon-114x114.png
--rw-r--r--   0        0        0     5618 2023-10-04 05:48:35.062872 lute3-3.3.1/lute/static/img/apple-touch-icon-57x57.png
--rw-r--r--   0        0        0     8461 2023-10-04 05:48:35.063084 lute3-3.3.1/lute/static/img/apple-touch-icon-72x72.png
--rw-r--r--   0        0        0    34198 2023-10-04 05:48:35.063762 lute3-3.3.1/lute/static/img/apple-touch-startup.png
--rw-r--r--   0        0        0    49403 2024-01-13 04:05:05.227551 lute3-3.3.1/lute/static/img/lute.png
--rw-r--r--   0        0        0     1405 2023-10-04 05:48:35.065233 lute3-3.3.1/lute/static/img/public_domain.png
--rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.065440 lute3-3.3.1/lute/static/img/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     3767 2023-10-04 05:48:35.065634 lute3-3.3.1/lute/static/img/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     3767 2023-10-04 05:48:35.065982 lute3-3.3.1/lute/static/img/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.066190 lute3-3.3.1/lute/static/img/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.066397 lute3-3.3.1/lute/static/img/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.069007 lute3-3.3.1/lute/static/img/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    11246 2024-03-13 16:31:06.443010 lute3-3.3.1/lute/static/js/dict-tabs.js
--rw-r--r--   0        0        0    21093 2024-03-25 09:32:17.270330 lute3-3.3.1/lute/static/js/lute.js
--rw-r--r--   0        0        0    12329 2024-03-13 16:31:06.444763 lute3-3.3.1/lute/static/js/player.js
--rw-r--r--   0        0        0     7406 2024-03-13 16:30:50.206756 lute3-3.3.1/lute/static/js/resize.js
--rw-r--r--   0        0        0     4346 2024-02-07 07:50:18.767242 lute3-3.3.1/lute/static/js/text-options.js
--rw-r--r--   0        0        0   202357 2024-03-15 03:25:40.872972 lute3-3.3.1/lute/static/vendor/chartjs/chart.umd.js
--rw-r--r--   0        0        0    50650 2024-03-15 03:25:40.873223 lute3-3.3.1/lute/static/vendor/chartjs/chartjs-adapter-date-fns.js
--rw-r--r--   0        0        0      624 2024-03-15 03:25:40.873755 lute3-3.3.1/lute/static/vendor/datatables/README.md
--rw-r--r--   0        0        0     4145 2024-03-15 03:25:40.873884 lute3-3.3.1/lute/static/vendor/datatables/datatables.button.download.js
--rw-r--r--   0        0        0    41393 2024-03-15 03:25:40.874305 lute3-3.3.1/lute/static/vendor/datatables/datatables.min.css
--rw-r--r--   0        0        0   164670 2024-03-15 03:25:40.875473 lute3-3.3.1/lute/static/vendor/datatables/datatables.min.js
--rw-r--r--   0        0        0     5253 2024-03-15 03:25:40.876688 lute3-3.3.1/lute/static/vendor/jquery/jplayer.css
--rw-r--r--   0        0        0    34497 2024-03-15 03:25:40.876886 lute3-3.3.1/lute/static/vendor/jquery/jquery-ui.css
--rw-r--r--   0        0        0   240422 2024-03-15 03:25:40.879055 lute3-3.3.1/lute/static/vendor/jquery/jquery-ui.min.js
--rw-r--r--   0        0        0     1753 2024-03-15 03:25:40.879212 lute3-3.3.1/lute/static/vendor/jquery/jquery.hoverIntent.js
--rw-r--r--   0        0        0     8067 2024-03-15 03:25:40.879335 lute3-3.3.1/lute/static/vendor/jquery/jquery.jeditable.mini.js
--rw-r--r--   0        0        0    69303 2024-03-15 03:25:40.879593 lute3-3.3.1/lute/static/vendor/jquery/jquery.jplayer.js
--rw-r--r--   0        0        0    60951 2024-03-15 03:25:40.880095 lute3-3.3.1/lute/static/vendor/jquery/jquery.jplayer.min.js
--rw-r--r--   0        0        0    13714 2024-03-15 03:25:40.880340 lute3-3.3.1/lute/static/vendor/jquery/jquery.jplayer.swf
--rw-r--r--   0        0        0    97163 2024-03-15 03:25:40.880764 lute3-3.3.1/lute/static/vendor/jquery/jquery.js
--rwxr-xr-x   0        0        0     2442 2024-03-15 03:25:40.880893 lute3-3.3.1/lute/static/vendor/jquery/jquery.scrollTo.min.js
--rw-r--r--   0        0        0    80119 2024-03-15 03:25:40.881202 lute3-3.3.1/lute/static/vendor/jquery/jquery.xpath.min.js
--rw-r--r--   0        0        0    11207 2024-03-15 03:25:40.881421 lute3-3.3.1/lute/static/vendor/tagify/tagify.css
--rw-r--r--   0        0        0    60507 2024-03-15 03:25:40.881716 lute3-3.3.1/lute/static/vendor/tagify/tagify.min.js
--rw-r--r--   0        0        0    23275 2024-03-15 03:25:40.881883 lute3-3.3.1/lute/static/vendor/tagify/tagify.polyfills.min.js
--rw-r--r--   0        0        0     1723 2024-03-15 03:25:40.882103 lute3-3.3.1/lute/static/vendor/tagify/tagify_overrides.css
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.232444 lute3-3.3.1/lute/stats/__init__.py
--rw-r--r--   0        0        0      482 2024-01-13 04:05:05.232852 lute3-3.3.1/lute/stats/routes.py
--rw-r--r--   0        0        0     2702 2024-02-07 07:50:18.767674 lute3-3.3.1/lute/stats/service.py
--rw-r--r--   0        0        0     1134 2024-03-15 03:25:40.883026 lute3-3.3.1/lute/templates/backup/backup.html
--rw-r--r--   0        0        0      872 2024-02-19 02:42:49.360741 lute3-3.3.1/lute/templates/backup/index.html
--rw-r--r--   0        0        0     6842 2024-03-15 03:25:40.896772 lute3-3.3.1/lute/templates/base.html
--rw-r--r--   0        0        0     3080 2024-03-25 09:32:17.271785 lute3-3.3.1/lute/templates/book/create_new.html
--rw-r--r--   0        0        0     2503 2024-03-13 16:31:06.446279 lute3-3.3.1/lute/templates/book/edit.html
--rw-r--r--   0        0        0      627 2024-03-25 09:32:17.272608 lute3-3.3.1/lute/templates/book/import_webpage.html
--rw-r--r--   0        0        0      204 2023-11-09 21:55:59.870577 lute3-3.3.1/lute/templates/book/index.html
--rw-r--r--   0        0        0    10771 2024-03-25 09:32:17.273450 lute3-3.3.1/lute/templates/book/tablelisting.html
--rw-r--r--   0        0        0      651 2024-01-13 04:05:05.236118 lute3-3.3.1/lute/templates/errors/404_error.html
--rw-r--r--   0        0        0     1185 2024-01-13 04:05:05.236533 lute3-3.3.1/lute/templates/errors/500_error.html
--rw-r--r--   0        0        0     2278 2024-03-03 03:12:19.455018 lute3-3.3.1/lute/templates/hotkeys.html
--rw-r--r--   0        0        0     5206 2024-03-15 03:25:40.899605 lute3-3.3.1/lute/templates/imagesearch/index.html
--rw-r--r--   0        0        0     1191 2024-03-13 16:31:06.448178 lute3-3.3.1/lute/templates/index.html
--rw-r--r--   0        0        0     7009 2024-02-19 02:42:49.361906 lute3-3.3.1/lute/templates/language/_form.html
--rw-r--r--   0        0        0      131 2023-11-01 07:45:01.587557 lute3-3.3.1/lute/templates/language/edit.html
--rw-r--r--   0        0        0     1312 2024-03-13 16:29:08.915083 lute3-3.3.1/lute/templates/language/index.html
--rw-r--r--   0        0        0      533 2024-02-07 07:50:18.771534 lute3-3.3.1/lute/templates/language/new.html
--rw-r--r--   0        0        0     2232 2024-02-07 07:50:18.771905 lute3-3.3.1/lute/templates/read/audio_player.html
--rw-r--r--   0        0        0      551 2024-03-15 03:25:40.900713 lute3-3.3.1/lute/templates/read/flashcopied.html
--rw-r--r--   0        0        0     1885 2024-03-25 08:52:45.544428 lute3-3.3.1/lute/templates/read/frameform.html
--rw-r--r--   0        0        0    17957 2024-03-15 03:25:40.902256 lute3-3.3.1/lute/templates/read/index.html
--rw-r--r--   0        0        0      605 2024-02-07 07:50:18.773525 lute3-3.3.1/lute/templates/read/page_content.html
--rw-r--r--   0        0        0      755 2024-02-19 02:42:49.362657 lute3-3.3.1/lute/templates/read/page_edit_form.html
--rw-r--r--   0        0        0     3341 2024-03-15 03:25:40.902930 lute3-3.3.1/lute/templates/read/reading_menu.html
--rw-r--r--   0        0        0     1742 2024-03-15 03:25:40.903466 lute3-3.3.1/lute/templates/read/termpopup.html
--rw-r--r--   0        0        0      499 2024-03-08 03:05:01.875375 lute3-3.3.1/lute/templates/read/textitem.html
--rw-r--r--   0        0        0      643 2024-03-15 03:25:40.903763 lute3-3.3.1/lute/templates/read/updated.html
--rw-r--r--   0        0        0     4862 2024-03-15 03:25:40.904111 lute3-3.3.1/lute/templates/settings/form.html
--rw-r--r--   0        0        0     3807 2024-03-15 03:25:40.904464 lute3-3.3.1/lute/templates/stats/index.html
--rw-r--r--   0        0        0    12698 2024-03-25 09:32:17.274542 lute3-3.3.1/lute/templates/term/_form.html
--rw-r--r--   0        0        0     2215 2024-03-13 16:31:06.452196 lute3-3.3.1/lute/templates/term/formframes.html
--rw-r--r--   0        0        0    16103 2024-03-15 03:25:40.905424 lute3-3.3.1/lute/templates/term/index.html
--rw-r--r--   0        0        0     1579 2024-02-19 02:42:49.365133 lute3-3.3.1/lute/templates/term/sentences.html
--rw-r--r--   0        0        0      502 2024-03-15 03:25:40.905825 lute3-3.3.1/lute/templates/term_parent_map/index.html
--rw-r--r--   0        0        0     1093 2024-03-25 09:32:17.275220 lute3-3.3.1/lute/templates/termimport/index.html
--rw-r--r--   0        0        0      755 2024-03-25 09:32:17.275871 lute3-3.3.1/lute/templates/termtag/_form.html
--rw-r--r--   0        0        0      119 2023-10-30 05:47:07.311779 lute3-3.3.1/lute/templates/termtag/edit.html
--rw-r--r--   0        0        0     2653 2023-11-09 21:55:59.873127 lute3-3.3.1/lute/templates/termtag/index.html
--rw-r--r--   0        0        0      170 2023-10-30 05:47:07.312798 lute3-3.3.1/lute/templates/termtag/new.html
--rw-r--r--   0        0        0      654 2024-03-08 03:05:01.878803 lute3-3.3.1/lute/templates/version.html
--rw-r--r--   0        0        0        0 2023-10-21 00:58:40.674085 lute3-3.3.1/lute/term/__init__.py
--rw-r--r--   0        0        0     3353 2024-03-25 09:32:17.277337 lute3-3.3.1/lute/term/datatables.py
--rw-r--r--   0        0        0     4130 2024-03-25 09:32:17.278674 lute3-3.3.1/lute/term/forms.py
--rw-r--r--   0        0        0    16216 2024-03-25 09:32:17.279461 lute3-3.3.1/lute/term/model.py
--rw-r--r--   0        0        0     9968 2024-03-25 09:32:17.280135 lute3-3.3.1/lute/term/routes.py
--rw-r--r--   0        0        0        0 2023-10-28 20:14:27.720594 lute3-3.3.1/lute/term_parent_map/__init__.py
--rw-r--r--   0        0        0     1459 2024-03-15 03:25:40.907485 lute3-3.3.1/lute/term_parent_map/routes.py
--rw-r--r--   0        0        0      866 2024-03-15 03:25:40.907878 lute3-3.3.1/lute/term_parent_map/service.py
--rw-r--r--   0        0        0        0 2023-10-27 22:52:35.310439 lute3-3.3.1/lute/termimport/__init__.py
--rw-r--r--   0        0        0     1793 2024-03-25 09:32:17.280829 lute3-3.3.1/lute/termimport/routes.py
--rw-r--r--   0        0        0     8599 2024-03-25 09:32:17.282132 lute3-3.3.1/lute/termimport/service.py
--rw-r--r--   0        0        0        0 2023-10-30 05:47:07.312889 lute3-3.3.1/lute/termtag/__init__.py
--rw-r--r--   0        0        0      652 2023-11-08 00:06:31.617316 lute3-3.3.1/lute/termtag/datatables.py
--rw-r--r--   0        0        0      309 2023-11-08 00:06:31.617623 lute3-3.3.1/lute/termtag/forms.py
--rw-r--r--   0        0        0     1857 2023-11-08 00:06:31.617959 lute3-3.3.1/lute/termtag/routes.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.250549 lute3-3.3.1/lute/themes/__init__.py
--rw-r--r--   0        0        0     1021 2024-03-08 03:05:01.881349 lute3-3.3.1/lute/themes/css/Apple_Books.css
--rw-r--r--   0        0        0     2603 2024-03-15 03:25:40.908418 lute3-3.3.1/lute/themes/css/Dark_slate.css
--rw-r--r--   0        0        0      949 2024-03-13 16:30:50.208931 lute3-3.3.1/lute/themes/css/LWT.css
--rw-r--r--   0        0        0     1096 2024-03-13 16:30:50.209490 lute3-3.3.1/lute/themes/css/LingQ.css
--rw-r--r--   0        0        0     2835 2024-03-15 03:25:40.909175 lute3-3.3.1/lute/themes/css/Night.css
--rw-r--r--   0        0        0      174 2024-01-13 04:05:05.252115 lute3-3.3.1/lute/themes/css/README.md
--rw-r--r--   0        0        0     1153 2024-03-08 03:05:01.882428 lute3-3.3.1/lute/themes/routes.py
--rw-r--r--   0        0        0     1882 2024-03-13 16:30:50.210261 lute3-3.3.1/lute/themes/service.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.253134 lute3-3.3.1/lute/useraudio/__init__.py
--rw-r--r--   0        0        0      545 2024-01-13 04:05:05.253460 lute3-3.3.1/lute/useraudio/routes.py
--rw-r--r--   0        0        0        0 2023-10-24 05:43:55.069141 lute3-3.3.1/lute/userimage/__init__.py
--rw-r--r--   0        0        0      656 2023-11-08 00:06:31.618260 lute3-3.3.1/lute/userimage/routes.py
--rw-r--r--   0        0        0        0 2023-10-09 03:35:20.090603 lute3-3.3.1/lute/utils/__init__.py
--rw-r--r--   0        0        0     7072 2024-03-13 16:31:06.454810 lute3-3.3.1/lute/utils/data_tables.py
--rw-r--r--   0        0        0     2043 2024-02-07 07:50:18.794729 lute3-3.3.1/lute/utils/debug_helpers.py
--rw-r--r--   0        0        0     1326 2024-03-13 16:30:50.210892 lute3-3.3.1/lute/utils/formutils.py
--rw-r--r--   0        0        0     1226 2024-03-15 04:43:49.944669 lute3-3.3.1/pyproject.toml
--rw-r--r--   0        0        0     1510 2024-03-15 04:43:49.945269 lute3-3.3.1/requirements.txt
--rw-r--r--   0        0        0    10239 2024-02-07 07:50:18.798118 lute3-3.3.1/tasks.py
--rw-r--r--   0        0        0      160 2023-10-22 05:50:12.570821 lute3-3.3.1/tests/__init__.py
--rw-r--r--   0        0        0      442 2023-10-31 05:25:17.232229 lute3-3.3.1/tests/acceptance/README.md
--rw-r--r--   0        0        0      132 2023-11-01 07:45:01.591037 lute3-3.3.1/tests/acceptance/__init__.py
--rw-r--r--   0        0        0     6294 2024-03-25 17:52:05.381459 lute3-3.3.1/tests/acceptance/book.feature
--rw-r--r--   0        0        0    13761 2024-03-25 17:52:05.381988 lute3-3.3.1/tests/acceptance/conftest.py
--rw-r--r--   0        0        0      102 2024-03-15 03:25:40.911823 lute3-3.3.1/tests/acceptance/disabled_test_sync_status.py
--rw-r--r--   0        0        0        3 2023-10-31 05:25:17.232861 lute3-3.3.1/tests/acceptance/failure_screenshots/.gitignore
--rw-r--r--   0        0        0       78 2023-10-31 05:25:17.233099 lute3-3.3.1/tests/acceptance/failure_screenshots/README.md
--rw-r--r--   0        0        0    13194 2024-03-15 03:25:40.912431 lute3-3.3.1/tests/acceptance/lute_test_client.py
--rw-r--r--   0        0        0    10086 2024-03-15 03:25:40.912826 lute3-3.3.1/tests/acceptance/reading.feature
--rw-r--r--   0        0        0     1282 2024-02-07 07:50:18.801083 lute3-3.3.1/tests/acceptance/sample_files/Hola.epub
--rw-r--r--   0        0        0     1433 2024-02-07 07:50:18.801387 lute3-3.3.1/tests/acceptance/sample_files/Hola.pdf
--rw-r--r--   0        0        0       48 2024-03-15 03:25:40.913611 lute3-3.3.1/tests/acceptance/sample_files/Hola.srt
--rw-r--r--   0        0        0       56 2024-03-15 03:25:40.913905 lute3-3.3.1/tests/acceptance/sample_files/Hola.vtt
--rw-r--r--   0        0        0       16 2024-01-13 04:05:05.265704 lute3-3.3.1/tests/acceptance/sample_files/hola.txt
--rw-r--r--   0        0        0       16 2024-02-07 07:50:18.801723 lute3-3.3.1/tests/acceptance/sample_files/invalid.epub
--rw-r--r--   0        0        0       16 2024-02-07 07:50:18.801856 lute3-3.3.1/tests/acceptance/sample_files/invalid.pdf
--rw-r--r--   0        0        0       16 2024-03-15 03:25:40.914165 lute3-3.3.1/tests/acceptance/sample_files/invalid.srt
--rw-r--r--   0        0        0       16 2024-03-15 03:25:40.914274 lute3-3.3.1/tests/acceptance/sample_files/invalid.vtt
--rw-r--r--   0        0        0     1417 2024-03-25 09:32:17.283465 lute3-3.3.1/tests/acceptance/sample_files/invalid_empty.epub
--rw-r--r--   0        0        0       74 2024-02-07 07:50:18.802571 lute3-3.3.1/tests/acceptance/sample_files/non_utf_8.txt
--rw-r--r--   0        0        0     2256 2024-03-25 09:32:17.283950 lute3-3.3.1/tests/acceptance/smoke.feature
--rw-r--r--   0        0        0      630 2024-03-08 03:05:01.891609 lute3-3.3.1/tests/acceptance/start_acceptance_app.py
--rw-r--r--   0        0        0     2082 2024-03-25 09:32:17.284644 lute3-3.3.1/tests/acceptance/sync_status.feature
--rw-r--r--   0        0        0     2153 2024-03-15 03:25:40.915397 lute3-3.3.1/tests/acceptance/term.feature
--rw-r--r--   0        0        0       92 2023-11-08 00:06:31.621311 lute3-3.3.1/tests/acceptance/test_book.py
--rw-r--r--   0        0        0       98 2023-11-08 00:06:31.621627 lute3-3.3.1/tests/acceptance/test_reading.py
--rw-r--r--   0        0        0       83 2024-03-25 09:32:17.285207 lute3-3.3.1/tests/acceptance/test_smoke.py
--rw-r--r--   0        0        0       92 2023-11-08 00:06:31.622287 lute3-3.3.1/tests/acceptance/test_term.py
--rw-r--r--   0        0        0      109 2023-11-08 00:06:31.622737 lute3-3.3.1/tests/acceptance/test_unsupported_parser.py
--rw-r--r--   0        0        0     1304 2024-03-25 09:32:17.285870 lute3-3.3.1/tests/acceptance/unsupported_parser.feature
--rw-r--r--   0        0        0     4299 2024-03-17 12:47:12.955608 lute3-3.3.1/tests/conftest.py
--rw-r--r--   0        0        0     1771 2023-11-08 00:06:31.623664 lute3-3.3.1/tests/dbasserts.py
--rw-r--r--   0        0        0      676 2023-10-22 17:27:11.801049 lute3-3.3.1/tests/features/README.md
--rw-r--r--   0        0        0    15205 2024-03-08 03:05:01.894503 lute3-3.3.1/tests/features/rendering.feature
--rw-r--r--   0        0        0    14799 2024-03-25 09:32:17.286789 lute3-3.3.1/tests/features/term_import.feature
--rw-r--r--   0        0        0     2907 2024-03-25 09:32:17.287963 lute3-3.3.1/tests/features/term_import_status_0.feature
--rw-r--r--   0        0        0     3696 2024-03-23 10:37:45.604972 lute3-3.3.1/tests/features/test_rendering.py
--rw-r--r--   0        0        0     3760 2024-03-25 09:32:17.288599 lute3-3.3.1/tests/features/test_term_import.py
--rw-r--r--   0        0        0        0 2023-09-20 06:21:29.988625 lute3-3.3.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     1206 2024-01-13 04:05:05.275517 lute3-3.3.1/tests/integration/test_main.py
--rw-r--r--   0        0        0       97 2023-10-20 06:39:27.112890 lute3-3.3.1/tests/orm/README.md
--rw-r--r--   0        0        0        0 2023-10-20 06:39:27.113017 lute3-3.3.1/tests/orm/__init__.py
--rw-r--r--   0        0        0     2808 2024-02-07 07:50:18.812178 lute3-3.3.1/tests/orm/test_Book.py
--rw-r--r--   0        0        0     3659 2024-02-19 02:42:49.366795 lute3-3.3.1/tests/orm/test_Language.py
--rw-r--r--   0        0        0     9757 2024-03-25 09:32:17.289215 lute3-3.3.1/tests/orm/test_Term.py
--rw-r--r--   0        0        0      871 2023-11-08 00:06:31.626423 lute3-3.3.1/tests/orm/test_Text.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.275609 lute3-3.3.1/tests/playwright/__init__.py
--rw-r--r--   0        0        0     8254 2024-03-25 09:32:17.289837 lute3-3.3.1/tests/playwright/playwright.py
--rw-r--r--   0        0        0        0 2023-09-10 06:10:01.992940 lute3-3.3.1/tests/unit/__init__.py
--rw-r--r--   0        0        0        0 2023-10-30 00:38:51.297976 lute3-3.3.1/tests/unit/backup/__init__.py
--rw-r--r--   0        0        0     9602 2024-02-19 02:42:49.368373 lute3-3.3.1/tests/unit/backup/test_backup.py
--rw-r--r--   0        0        0        0 2023-10-20 18:52:22.684248 lute3-3.3.1/tests/unit/book/__init__.py
--rw-r--r--   0        0        0     3273 2024-02-07 07:50:18.814795 lute3-3.3.1/tests/unit/book/test_Repository.py
--rw-r--r--   0        0        0     2241 2024-03-13 16:30:50.212038 lute3-3.3.1/tests/unit/book/test_datatables.py
--rw-r--r--   0        0        0     4124 2024-02-07 07:50:18.815696 lute3-3.3.1/tests/unit/book/test_stats.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.277883 lute3-3.3.1/tests/unit/cli/__init__.py
--rw-r--r--   0        0        0      521 2024-01-13 04:05:05.278085 lute3-3.3.1/tests/unit/cli/test_language_term_export.py
--rw-r--r--   0        0        0        0 2023-11-04 21:50:44.092388 lute3-3.3.1/tests/unit/config/__init__.py
--rw-r--r--   0        0        0     3035 2024-01-13 04:05:05.278929 lute3-3.3.1/tests/unit/config/test_app_config.py
--rw-r--r--   0        0        0        0 2023-10-26 01:04:31.832624 lute3-3.3.1/tests/unit/db/__init__.py
--rw-r--r--   0        0        0        0 2023-10-20 18:48:10.174878 lute3-3.3.1/tests/unit/db/setup/__init__.py
--rw-r--r--   0        0        0       28 2023-10-20 18:48:10.175186 lute3-3.3.1/tests/unit/db/setup/schema/README.md
--rw-r--r--   0        0        0      134 2023-10-20 18:48:10.175437 lute3-3.3.1/tests/unit/db/setup/schema/baseline/schema.sql
--rw-r--r--   0        0        0       24 2023-10-20 18:48:10.175796 lute3-3.3.1/tests/unit/db/setup/schema/migrations/123_create_B.sql
--rw-r--r--   0        0        0       68 2023-10-20 18:48:10.176170 lute3-3.3.1/tests/unit/db/setup/schema/repeatable/view_A.sql
--rw-r--r--   0        0        0     1241 2023-11-08 00:06:31.628181 lute3-3.3.1/tests/unit/db/setup/test_BackupManager.py
--rw-r--r--   0        0        0     8127 2023-11-08 00:06:31.628506 lute3-3.3.1/tests/unit/db/setup/test_Setup.py
--rw-r--r--   0        0        0     3681 2023-11-08 00:06:31.628800 lute3-3.3.1/tests/unit/db/setup/test_SqliteMigrator.py
--rw-r--r--   0        0        0     4349 2024-02-19 02:42:49.368584 lute3-3.3.1/tests/unit/db/test_demo.py
--rw-r--r--   0        0        0     1534 2023-11-11 22:05:26.100552 lute3-3.3.1/tests/unit/db/test_management.py
--rw-r--r--   0        0        0        0 2023-10-04 05:48:35.085848 lute3-3.3.1/tests/unit/models/__init__.py
--rw-r--r--   0        0        0     1820 2024-03-13 16:30:50.212544 lute3-3.3.1/tests/unit/models/test_Book.py
--rw-r--r--   0        0        0     3102 2024-03-15 03:25:40.916767 lute3-3.3.1/tests/unit/models/test_Book_add_remove_pages.py
--rw-r--r--   0        0        0     1962 2024-02-19 02:42:49.368775 lute3-3.3.1/tests/unit/models/test_Language.py
--rw-r--r--   0        0        0     6167 2024-02-19 02:42:49.368998 lute3-3.3.1/tests/unit/models/test_Setting.py
--rw-r--r--   0        0        0     8034 2024-03-25 09:32:17.290517 lute3-3.3.1/tests/unit/models/test_Term.py
--rw-r--r--   0        0        0     1398 2023-11-08 00:06:31.630600 lute3-3.3.1/tests/unit/models/test_TermTag.py
--rw-r--r--   0        0        0      970 2024-02-07 07:50:18.820113 lute3-3.3.1/tests/unit/models/test_Text.py
--rw-r--r--   0        0        0        0 2023-10-07 05:09:39.900041 lute3-3.3.1/tests/unit/parse/__init__.py
--rw-r--r--   0        0        0     1806 2023-11-08 00:06:31.631135 lute3-3.3.1/tests/unit/parse/test_ClassicalChineseParser.py
--rw-r--r--   0        0        0     2655 2024-03-08 03:05:01.896542 lute3-3.3.1/tests/unit/parse/test_JapaneseParser.py
--rw-r--r--   0        0        0     1452 2023-11-08 00:06:31.631582 lute3-3.3.1/tests/unit/parse/test_SentenceGroupIterator.py
--rw-r--r--   0        0        0     5103 2024-03-18 03:32:09.327775 lute3-3.3.1/tests/unit/parse/test_SpaceDelimitedParser.py
--rw-r--r--   0        0        0      437 2023-11-08 00:06:31.632019 lute3-3.3.1/tests/unit/parse/test_TurkishParser.py
--rw-r--r--   0        0        0     1343 2024-01-13 04:05:05.283548 lute3-3.3.1/tests/unit/parse/test_registry.py
--rw-r--r--   0        0        0        0 2023-10-18 06:43:42.369680 lute3-3.3.1/tests/unit/read/__init__.py
--rw-r--r--   0        0        0        0 2023-10-18 06:43:42.370116 lute3-3.3.1/tests/unit/read/render/__init__.py
--rw-r--r--   0        0        0     3678 2023-11-08 00:06:31.632488 lute3-3.3.1/tests/unit/read/render/test_RenderableCalculator.py
--rw-r--r--   0        0        0     1965 2023-11-08 00:06:31.632694 lute3-3.3.1/tests/unit/read/render/test_TokenLocator.py
--rw-r--r--   0        0        0     5991 2024-03-25 09:32:17.291177 lute3-3.3.1/tests/unit/read/test_service.py
--rw-r--r--   0        0        0     3872 2024-03-25 09:32:17.292242 lute3-3.3.1/tests/unit/read/test_service_popup_data.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.283732 lute3-3.3.1/tests/unit/stats/__init__.py
--rw-r--r--   0        0        0     2467 2024-02-07 07:50:18.821867 lute3-3.3.1/tests/unit/stats/test_service.py
--rw-r--r--   0        0        0        0 2023-10-21 00:58:40.675868 lute3-3.3.1/tests/unit/term/__init__.py
--rw-r--r--   0        0        0    23300 2024-03-25 09:32:17.293137 lute3-3.3.1/tests/unit/term/test_Repository.py
--rw-r--r--   0        0        0     2082 2024-02-07 07:50:18.824210 lute3-3.3.1/tests/unit/term/test_TermForm.py
--rw-r--r--   0        0        0     6766 2024-02-07 07:50:18.824963 lute3-3.3.1/tests/unit/term/test_Term_status_follow.py
--rw-r--r--   0        0        0     1629 2024-01-13 04:05:05.285150 lute3-3.3.1/tests/unit/term/test_datatables.py
--rw-r--r--   0        0        0        0 2023-10-30 23:02:04.731925 lute3-3.3.1/tests/unit/term_parent_map/__init__.py
--rw-r--r--   0        0        0     1255 2024-03-15 03:25:40.918632 lute3-3.3.1/tests/unit/term_parent_map/test_service.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.285261 lute3-3.3.1/tests/unit/termtag/__init__.py
--rw-r--r--   0        0        0      679 2023-11-08 00:06:31.633834 lute3-3.3.1/tests/unit/termtag/test_datatables.py
--rw-r--r--   0        0        0        0 2024-01-13 04:05:05.285353 lute3-3.3.1/tests/unit/themes/__init__.py
--rw-r--r--   0        0        0     1550 2024-03-08 03:05:01.897112 lute3-3.3.1/tests/unit/themes/test_service.py
--rw-r--r--   0        0        0        0 2023-10-09 03:35:20.091806 lute3-3.3.1/tests/unit/utils/__init__.py
--rw-r--r--   0        0        0     5151 2024-01-18 07:46:16.382578 lute3-3.3.1/tests/unit/utils/test_DataTablesSqliteQuery.py
--rw-r--r--   0        0        0      786 2024-03-13 16:30:50.213297 lute3-3.3.1/tests/unit/utils/test_formutils.py
--rw-r--r--   0        0        0     1629 2024-02-07 07:50:18.825866 lute3-3.3.1/tests/utils.py
--rwxr-xr-x   0        0        0     1575 2024-02-19 02:42:49.369401 lute3-3.3.1/utils/dump_changelog.sh
--rwxr-xr-x   0        0        0      565 2024-03-15 03:25:40.919140 lute3-3.3.1/utils/findstring.sh
--rw-r--r--   0        0        0     4820 2023-11-22 00:36:49.803896 lute3-3.3.1/utils/todos.py
--rw-r--r--   0        0        0      698 2023-11-09 08:26:12.057924 lute3-3.3.1/utils/verify.py
--rw-r--r--   0        0        0     2219 1970-01-01 00:00:00.000000 lute3-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0      170 2023-11-09 08:26:12.050479 lute3-3.3.2b1/.dockerignore
+-rw-r--r--   0        0        0     1280 2024-03-08 03:05:01.842902 lute3-3.3.2b1/.github/ISSUE_TEMPLATE/add_language.md
+-rw-r--r--   0        0        0      590 2024-03-08 03:05:01.843291 lute3-3.3.2b1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      649 2024-03-30 00:54:09.932549 lute3-3.3.2b1/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      578 2024-03-08 03:05:01.843637 lute3-3.3.2b1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     7213 2024-04-21 08:30:46.468084 lute3-3.3.2b1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2663 2024-04-11 08:18:12.378459 lute3-3.3.2b1/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     2172 2024-04-05 03:40:57.739326 lute3-3.3.2b1/.gitignore
+-rw-r--r--   0        0        0      119 2024-04-11 08:18:12.378773 lute3-3.3.2b1/.gitmodules
+-rw-r--r--   0        0        0      395 2024-01-13 04:05:05.193611 lute3-3.3.2b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    24735 2023-11-20 01:37:46.796733 lute3-3.3.2b1/.pylintrc
+-rw-r--r--   0        0        0     1076 2024-01-13 04:05:05.194389 lute3-3.3.2b1/.pytest.ini
+-rw-r--r--   0        0        0     1068 2023-11-09 05:33:09.100157 lute3-3.3.2b1/LICENSE.txt
+-rw-r--r--   0        0        0     1641 2024-03-30 00:51:18.285586 lute3-3.3.2b1/README.md
+-rw-r--r--   0        0        0     1145 2024-04-01 09:04:21.548972 lute3-3.3.2b1/README_PyPi.md
+-rw-r--r--   0        0        0     1578 2024-03-08 03:05:01.845433 lute3-3.3.2b1/devstart.py
+-rw-r--r--   0        0        0      965 2023-11-10 18:48:16.706091 lute3-3.3.2b1/docker/Dockerfile
+-rw-r--r--   0        0        0      496 2024-01-13 04:05:05.195405 lute3-3.3.2b1/docker/README.md
+-rwxr-xr-x   0        0        0     1545 2024-01-13 04:05:05.195617 lute3-3.3.2b1/docker/build_all.sh
+-rwxr-xr-x   0        0        0       89 2024-01-13 04:05:05.195716 lute3-3.3.2b1/docker/build_test.sh
+-rw-r--r--   0        0        0     1076 2023-11-09 08:26:12.052441 lute3-3.3.2b1/docker/check_mounts_and_start.sh
+-rw-r--r--   0        0        0      309 2023-11-09 08:26:12.052717 lute3-3.3.2b1/docker/docker-compose.yml.example
+-rw-r--r--   0        0        0     3249 2024-04-01 09:22:59.620728 lute3-3.3.2b1/docker/docker_hub_overview.md
+-rwxr-xr-x   0        0        0     1127 2024-01-13 04:05:05.195822 lute3-3.3.2b1/docker/try_build_multi.sh
+-rw-r--r--   0        0        0    13116 2024-03-25 17:57:11.309042 lute3-3.3.2b1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       71 2024-01-13 04:05:05.196786 lute3-3.3.2b1/docs/README.md
+-rw-r--r--   0        0        0     1068 2023-11-09 05:33:09.101369 lute3-3.3.2b1/lute/LICENSE.txt
+-rw-r--r--   0        0        0      382 2024-04-25 23:45:40.269705 lute3-3.3.2b1/lute/__init__.py
+-rw-r--r--   0        0        0    11145 2024-03-15 03:25:40.864716 lute3-3.3.2b1/lute/app_factory.py
+-rw-r--r--   0        0        0        0 2023-10-30 00:38:51.292984 lute3-3.3.2b1/lute/backup/__init__.py
+-rw-r--r--   0        0        0     2300 2024-03-15 03:25:40.865078 lute3-3.3.2b1/lute/backup/routes.py
+-rw-r--r--   0        0        0     5303 2024-03-15 03:25:40.865445 lute3-3.3.2b1/lute/backup/service.py
+-rw-r--r--   0        0        0        0 2023-10-24 05:43:55.066190 lute3-3.3.2b1/lute/bing/__init__.py
+-rw-r--r--   0        0        0     3736 2024-03-13 16:30:50.197607 lute3-3.3.2b1/lute/bing/routes.py
+-rw-r--r--   0        0        0        0 2023-10-16 06:20:14.169949 lute3-3.3.2b1/lute/book/__init__.py
+-rw-r--r--   0        0        0     2541 2024-03-15 03:25:40.865805 lute3-3.3.2b1/lute/book/datatables.py
+-rw-r--r--   0        0        0     5118 2024-03-25 09:32:17.256759 lute3-3.3.2b1/lute/book/forms.py
+-rw-r--r--   0        0        0     3633 2024-04-21 08:30:46.468432 lute3-3.3.2b1/lute/book/model.py
+-rw-r--r--   0        0        0     5021 2024-03-25 09:32:17.257357 lute3-3.3.2b1/lute/book/routes.py
+-rw-r--r--   0        0        0     6395 2024-03-25 09:32:17.258143 lute3-3.3.2b1/lute/book/service.py
+-rw-r--r--   0        0        0     3598 2024-02-07 07:50:18.749346 lute3-3.3.2b1/lute/book/stats.py
+-rw-r--r--   0        0        0      475 2024-01-13 04:05:05.200591 lute3-3.3.2b1/lute/cli/README.md
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.200653 lute3-3.3.2b1/lute/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-01-13 04:05:05.200788 lute3-3.3.2b1/lute/cli/commands.py
+-rw-r--r--   0        0        0     6313 2024-02-07 07:50:18.749980 lute3-3.3.2b1/lute/cli/language_term_export.py
+-rw-r--r--   0        0        0        0 2023-11-04 21:50:44.080272 lute3-3.3.2b1/lute/config/__init__.py
+-rw-r--r--   0        0        0     2951 2024-03-08 03:05:01.852258 lute3-3.3.2b1/lute/config/app_config.py
+-rw-r--r--   0        0        0      265 2024-01-13 04:05:05.201516 lute3-3.3.2b1/lute/config/config.yml.docker
+-rw-r--r--   0        0        0      667 2024-01-13 04:05:05.201703 lute3-3.3.2b1/lute/config/config.yml.example
+-rw-r--r--   0        0        0      280 2024-01-13 04:05:05.201898 lute3-3.3.2b1/lute/config/config.yml.prod
+-rw-r--r--   0        0        0      108 2023-10-20 18:48:10.167405 lute3-3.3.2b1/lute/db/__init__.py
+-rw-r--r--   0        0        0     1021 2024-02-07 07:50:18.750797 lute3-3.3.2b1/lute/db/data_cleanup.py
+-rw-r--r--   0        0        0     3032 2024-04-21 08:30:46.468710 lute3-3.3.2b1/lute/db/demo.py
+-rw-r--r--   0        0        0      525 2024-04-11 08:21:17.603012 lute3-3.3.2b1/lute/db/language_defs/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1799 2024-04-20 09:34:27.212777 lute3-3.3.2b1/lute/db/language_defs/README.md
+-rw-r--r--   0        0        0      379 2024-04-11 08:21:17.603341 lute3-3.3.2b1/lute/db/language_defs/_templates/definition.yaml.example
+-rw-r--r--   0        0        0       35 2024-04-11 08:21:17.603445 lute3-3.3.2b1/lute/db/language_defs/_templates/story.txt.example
+-rw-r--r--   0        0        0      820 2024-04-20 05:57:30.283599 lute3-3.3.2b1/lute/db/language_defs/afrikaans/definition.yaml
+-rw-r--r--   0        0        0      582 2024-04-20 05:37:09.814096 lute3-3.3.2b1/lute/db/language_defs/afrikaans/die_diere_grawe_n_put.txt
+-rw-r--r--   0        0        0      816 2024-04-18 11:04:50.550746 lute3-3.3.2b1/lute/db/language_defs/albanian/definition.yaml
+-rw-r--r--   0        0        0      791 2024-04-18 11:04:50.551098 lute3-3.3.2b1/lute/db/language_defs/albanian/shqiponja_dhe_mbreti.txt
+-rw-r--r--   0        0        0      943 2024-04-21 06:50:19.757643 lute3-3.3.2b1/lute/db/language_defs/amharic/definition.yaml
+-rw-r--r--   0        0        0      898 2024-04-21 06:50:19.758439 lute3-3.3.2b1/lute/db/language_defs/amharic/story_1.txt
+-rw-r--r--   0        0        0     1147 2024-04-11 08:21:17.603662 lute3-3.3.2b1/lute/db/language_defs/arabic/ar_demo.txt
+-rw-r--r--   0        0        0      555 2024-04-11 08:21:17.603806 lute3-3.3.2b1/lute/db/language_defs/arabic/definition.yaml
+-rw-r--r--   0        0        0     1453 2024-04-21 06:43:41.206331 lute3-3.3.2b1/lute/db/language_defs/armenian/definition.yaml
+-rw-r--r--   0        0        0     3063 2024-04-21 06:43:41.216493 lute3-3.3.2b1/lute/db/language_defs/armenian/story_1.txt
+-rw-r--r--   0        0        0     1473 2024-04-21 06:43:41.141949 lute3-3.3.2b1/lute/db/language_defs/azerbaijani/definition.yaml
+-rw-r--r--   0        0        0     2742 2024-04-21 06:43:41.149861 lute3-3.3.2b1/lute/db/language_defs/azerbaijani/story_1.txt
+-rw-r--r--   0        0        0      885 2024-04-21 06:50:19.755501 lute3-3.3.2b1/lute/db/language_defs/basque/definition.yaml
+-rw-r--r--   0        0        0      663 2024-04-21 06:50:19.756168 lute3-3.3.2b1/lute/db/language_defs/basque/story_1.txt
+-rw-r--r--   0        0        0     1024 2024-04-21 06:43:41.218579 lute3-3.3.2b1/lute/db/language_defs/belarusian/definition.yaml
+-rw-r--r--   0        0        0     2573 2024-04-21 06:43:41.227439 lute3-3.3.2b1/lute/db/language_defs/belarusian/story_1.txt
+-rw-r--r--   0        0        0     2176 2024-04-18 11:04:50.551602 lute3-3.3.2b1/lute/db/language_defs/bengali/aharshi_the_bengal_tiger.txt
+-rw-r--r--   0        0        0      988 2024-04-18 11:04:50.551950 lute3-3.3.2b1/lute/db/language_defs/bengali/definition.yaml
+-rw-r--r--   0        0        0     1220 2024-04-21 06:43:41.195177 lute3-3.3.2b1/lute/db/language_defs/breton/definition.yaml
+-rw-r--r--   0        0        0     1991 2024-04-21 06:43:41.202857 lute3-3.3.2b1/lute/db/language_defs/breton/story_1.txt
+-rw-r--r--   0        0        0     1499 2024-04-18 11:04:50.552403 lute3-3.3.2b1/lute/db/language_defs/bulgarian/definition.yaml
+-rw-r--r--   0        0        0      731 2024-04-18 11:04:50.552717 lute3-3.3.2b1/lute/db/language_defs/bulgarian/yesterday_film_description.txt
+-rw-r--r--   0        0        0     1991 2024-04-18 11:04:50.553230 lute3-3.3.2b1/lute/db/language_defs/catalan/definition.yaml
+-rw-r--r--   0        0        0      718 2024-04-18 11:04:50.553549 lute3-3.3.2b1/lute/db/language_defs/catalan/merlí_series_description.txt
+-rw-r--r--   0        0        0     1412 2024-04-11 08:21:17.604020 lute3-3.3.2b1/lute/db/language_defs/classical_chinese/cc_demo.txt
+-rw-r--r--   0        0        0      416 2024-04-11 08:21:17.604146 lute3-3.3.2b1/lute/db/language_defs/classical_chinese/definition.yaml
+-rw-r--r--   0        0        0      948 2024-04-24 06:10:24.478842 lute3-3.3.2b1/lute/db/language_defs/croatian/definition.yaml
+-rw-r--r--   0        0        0      530 2024-04-24 06:10:24.481122 lute3-3.3.2b1/lute/db/language_defs/croatian/story_1.txt
+-rw-r--r--   0        0        0      518 2024-04-11 08:21:17.604342 lute3-3.3.2b1/lute/db/language_defs/czech/czech.txt
+-rw-r--r--   0        0        0      377 2024-04-11 08:21:17.604467 lute3-3.3.2b1/lute/db/language_defs/czech/definition.yaml
+-rw-r--r--   0        0        0     1093 2024-04-18 11:04:50.554156 lute3-3.3.2b1/lute/db/language_defs/danish/definition.yaml
+-rw-r--r--   0        0        0      670 2024-04-18 11:04:50.554527 lute3-3.3.2b1/lute/db/language_defs/danish/prinsessen_pa_arten.txt
+-rw-r--r--   0        0        0      474 2024-04-20 05:58:35.660612 lute3-3.3.2b1/lute/db/language_defs/dutch/de_doortocht.txt
+-rw-r--r--   0        0        0     1127 2024-04-20 05:57:30.289710 lute3-3.3.2b1/lute/db/language_defs/dutch/definition.yaml
+-rw-r--r--   0        0        0      468 2024-04-11 13:38:31.614736 lute3-3.3.2b1/lute/db/language_defs/english/definition.yaml
+-rw-r--r--   0        0        0     7159 2024-04-21 10:32:38.532708 lute3-3.3.2b1/lute/db/language_defs/english/tutorial.txt
+-rw-r--r--   0        0        0     3534 2024-04-11 08:21:17.604946 lute3-3.3.2b1/lute/db/language_defs/english/tutorial_follow_up.txt
+-rw-r--r--   0        0        0      858 2024-04-21 06:50:19.753232 lute3-3.3.2b1/lute/db/language_defs/esperanto/definition.yaml
+-rw-r--r--   0        0        0      535 2024-04-21 06:50:19.753991 lute3-3.3.2b1/lute/db/language_defs/esperanto/story_1.txt
+-rw-r--r--   0        0        0     2043 2024-04-21 06:43:41.175532 lute3-3.3.2b1/lute/db/language_defs/estonian/definition.yaml
+-rw-r--r--   0        0        0      746 2024-04-21 06:43:41.183334 lute3-3.3.2b1/lute/db/language_defs/estonian/story_1.txt
+-rw-r--r--   0        0        0     1000 2024-04-21 01:33:29.601303 lute3-3.3.2b1/lute/db/language_defs/farsi/definition.yaml
+-rw-r--r--   0        0        0      951 2024-04-21 01:33:43.684967 lute3-3.3.2b1/lute/db/language_defs/farsi/story_1.txt
+-rw-r--r--   0        0        0     2450 2024-04-21 06:43:41.163772 lute3-3.3.2b1/lute/db/language_defs/finnish/definition.yaml
+-rw-r--r--   0        0        0      537 2024-04-21 06:43:41.172220 lute3-3.3.2b1/lute/db/language_defs/finnish/story_1.txt
+-rw-r--r--   0        0        0      370 2024-04-11 08:21:17.605117 lute3-3.3.2b1/lute/db/language_defs/french/definition.yaml
+-rw-r--r--   0        0        0      469 2024-04-11 08:21:17.605223 lute3-3.3.2b1/lute/db/language_defs/french/fr_goldilocks.txt
+-rw-r--r--   0        0        0     1672 2024-04-21 06:43:41.230538 lute3-3.3.2b1/lute/db/language_defs/galician/definition.yaml
+-rw-r--r--   0        0        0      544 2024-04-21 06:43:41.238873 lute3-3.3.2b1/lute/db/language_defs/galician/story_1.txt
+-rw-r--r--   0        0        0     1306 2024-04-21 06:43:41.185436 lute3-3.3.2b1/lute/db/language_defs/georgian/definition.yaml
+-rw-r--r--   0        0        0      953 2024-04-21 06:43:41.193023 lute3-3.3.2b1/lute/db/language_defs/georgian/story_1.txt
+-rw-r--r--   0        0        0     1058 2024-04-11 08:21:17.605401 lute3-3.3.2b1/lute/db/language_defs/german/de_Stadtmusikanten.txt
+-rw-r--r--   0        0        0      522 2024-04-11 08:21:17.605497 lute3-3.3.2b1/lute/db/language_defs/german/definition.yaml
+-rw-r--r--   0        0        0      858 2024-04-21 06:50:19.765471 lute3-3.3.2b1/lute/db/language_defs/gothic/definition.yaml
+-rw-r--r--   0        0        0     1317 2024-04-21 06:50:19.766099 lute3-3.3.2b1/lute/db/language_defs/gothic/story_1.txt
+-rw-r--r--   0        0        0      635 2024-04-11 08:21:17.605663 lute3-3.3.2b1/lute/db/language_defs/greek/definition.yaml
+-rw-r--r--   0        0        0     1649 2024-04-11 08:21:17.605770 lute3-3.3.2b1/lute/db/language_defs/greek/gr_demo.txt
+-rw-r--r--   0        0        0     2165 2024-04-21 06:43:41.259836 lute3-3.3.2b1/lute/db/language_defs/hebrew/definition.yaml
+-rw-r--r--   0        0        0      945 2024-04-21 06:43:41.268997 lute3-3.3.2b1/lute/db/language_defs/hebrew/story_1.txt
+-rw-r--r--   0        0        0      566 2024-04-11 08:21:17.605935 lute3-3.3.2b1/lute/db/language_defs/hindi/definition.yaml
+-rw-r--r--   0        0        0      587 2024-04-11 08:21:17.606066 lute3-3.3.2b1/lute/db/language_defs/hindi/hi_wikipedia.txt
+-rw-r--r--   0        0        0     2484 2024-04-18 11:04:50.554908 lute3-3.3.2b1/lute/db/language_defs/hungarian/definition.yaml
+-rw-r--r--   0        0        0      308 2024-04-18 11:04:50.555170 lute3-3.3.2b1/lute/db/language_defs/hungarian/satantango_film_description.txt
+-rw-r--r--   0        0        0     1505 2024-04-21 06:43:41.152286 lute3-3.3.2b1/lute/db/language_defs/icelandic/definition.yaml
+-rw-r--r--   0        0        0     1262 2024-04-21 06:43:41.159994 lute3-3.3.2b1/lute/db/language_defs/icelandic/story_1.txt
+-rw-r--r--   0        0        0      868 2024-04-20 05:57:30.287406 lute3-3.3.2b1/lute/db/language_defs/indonesian/definition.yaml
+-rw-r--r--   0        0        0      643 2024-04-20 05:58:35.661145 lute3-3.3.2b1/lute/db/language_defs/indonesian/kura-kura_yang_sombong.txt
+-rw-r--r--   0        0        0     3101 2024-04-18 11:04:50.555587 lute3-3.3.2b1/lute/db/language_defs/italian/definition.yaml
+-rw-r--r--   0        0        0      905 2024-04-18 11:04:50.555843 lute3-3.3.2b1/lute/db/language_defs/italian/le_avventure_di_pinocchio.txt
+-rw-r--r--   0        0        0      539 2024-04-11 08:21:17.606295 lute3-3.3.2b1/lute/db/language_defs/japanese/definition.yaml
+-rw-r--r--   0        0        0      428 2024-04-11 08:21:17.606410 lute3-3.3.2b1/lute/db/language_defs/japanese/jp_kitakaze_to_taiyou.txt
+-rw-r--r--   0        0        0     2188 2024-04-24 06:13:00.188660 lute3-3.3.2b1/lute/db/language_defs/latin/definition.yaml
+-rw-r--r--   0        0        0      497 2024-04-24 06:13:00.194030 lute3-3.3.2b1/lute/db/language_defs/latin/story_1.txt
+-rw-r--r--   0        0        0     1796 2024-04-24 06:13:00.196974 lute3-3.3.2b1/lute/db/language_defs/latvian/definition.yaml
+-rw-r--r--   0        0        0      562 2024-04-24 06:13:00.202327 lute3-3.3.2b1/lute/db/language_defs/latvian/story_1.txt
+-rw-r--r--   0        0        0     1850 2024-04-24 06:13:00.205297 lute3-3.3.2b1/lute/db/language_defs/lithuanian/definition.yaml
+-rw-r--r--   0        0        0     1104 2024-04-24 06:13:00.210453 lute3-3.3.2b1/lute/db/language_defs/lithuanian/story_1.txt
+-rw-r--r--   0        0        0      800 2024-04-20 05:57:30.293738 lute3-3.3.2b1/lute/db/language_defs/norwegian/definition.yaml
+-rw-r--r--   0        0        0      955 2024-04-20 05:58:35.661516 lute3-3.3.2b1/lute/db/language_defs/norwegian/vildanden.txt
+-rw-r--r--   0        0        0     1141 2024-04-18 11:04:50.556275 lute3-3.3.2b1/lute/db/language_defs/polish/adam_i_smoczy_skarb.txt
+-rw-r--r--   0        0        0     2903 2024-04-18 11:04:50.556560 lute3-3.3.2b1/lute/db/language_defs/polish/definition.yaml
+-rw-r--r--   0        0        0     1047 2024-04-18 11:04:50.557000 lute3-3.3.2b1/lute/db/language_defs/portuguese/a_maldicao.txt
+-rw-r--r--   0        0        0     3471 2024-04-18 11:04:50.557288 lute3-3.3.2b1/lute/db/language_defs/portuguese/definition.yaml
+-rw-r--r--   0        0        0     1143 2024-04-21 06:50:19.763422 lute3-3.3.2b1/lute/db/language_defs/punjabi/definition.yaml
+-rw-r--r--   0        0        0     1390 2024-04-21 06:50:19.764091 lute3-3.3.2b1/lute/db/language_defs/punjabi/story_1.txt
+-rw-r--r--   0        0        0       14 2024-04-11 08:21:17.606516 lute3-3.3.2b1/lute/db/language_defs/requirements.txt
+-rw-r--r--   0        0        0     2898 2024-04-21 06:43:41.129590 lute3-3.3.2b1/lute/db/language_defs/romanian/definition.yaml
+-rw-r--r--   0        0        0      472 2024-04-21 06:43:41.139463 lute3-3.3.2b1/lute/db/language_defs/romanian/story_1.txt
+-rw-r--r--   0        0        0      470 2024-04-11 08:21:17.606692 lute3-3.3.2b1/lute/db/language_defs/russian/definition.yaml
+-rw-r--r--   0        0        0      546 2024-04-11 08:21:17.606839 lute3-3.3.2b1/lute/db/language_defs/russian/ru_medved.txt
+-rw-r--r--   0        0        0      477 2024-04-11 08:21:17.607040 lute3-3.3.2b1/lute/db/language_defs/sanskrit/definition.yaml
+-rw-r--r--   0        0        0     1027 2024-04-11 08:21:17.607150 lute3-3.3.2b1/lute/db/language_defs/sanskrit/sanskrit.txt
+-rw-r--r--   0        0        0     1028 2024-04-24 06:10:24.482926 lute3-3.3.2b1/lute/db/language_defs/serbian/definition.yaml
+-rw-r--r--   0        0        0      740 2024-04-24 06:10:24.483663 lute3-3.3.2b1/lute/db/language_defs/serbian/story_1.txt
+-rw-r--r--   0        0        0     2055 2024-04-24 06:13:00.213596 lute3-3.3.2b1/lute/db/language_defs/slovak/definition.yaml
+-rw-r--r--   0        0        0      729 2024-04-24 06:13:00.219313 lute3-3.3.2b1/lute/db/language_defs/slovak/story_1.txt
+-rw-r--r--   0        0        0     1644 2024-04-24 06:13:00.221962 lute3-3.3.2b1/lute/db/language_defs/slovene/definition.yaml
+-rw-r--r--   0        0        0      464 2024-04-24 06:13:00.227091 lute3-3.3.2b1/lute/db/language_defs/slovene/story_1.txt
+-rw-r--r--   0        0        0      526 2024-04-11 08:21:17.607350 lute3-3.3.2b1/lute/db/language_defs/spanish/definition.yaml
+-rw-r--r--   0        0        0      534 2024-04-11 08:21:17.607465 lute3-3.3.2b1/lute/db/language_defs/spanish/es_aladino.txt
+-rw-r--r--   0        0        0     1302 2024-04-24 06:13:00.229331 lute3-3.3.2b1/lute/db/language_defs/swahili/definition.yaml
+-rw-r--r--   0        0        0      755 2024-04-24 06:13:00.234330 lute3-3.3.2b1/lute/db/language_defs/swahili/story_1.txt
+-rw-r--r--   0        0        0     2821 2024-04-24 06:13:00.238299 lute3-3.3.2b1/lute/db/language_defs/swedish/definition.yaml
+-rw-r--r--   0        0        0      566 2024-04-24 06:13:00.243830 lute3-3.3.2b1/lute/db/language_defs/swedish/story_1.txt
+-rw-r--r--   0        0        0     1858 2024-04-21 06:50:19.748999 lute3-3.3.2b1/lute/db/language_defs/tibetan/definition.yaml
+-rw-r--r--   0        0        0     1464 2024-04-21 06:50:19.751706 lute3-3.3.2b1/lute/db/language_defs/tibetan/story_1.txt
+-rw-r--r--   0        0        0      497 2024-04-11 08:21:17.607666 lute3-3.3.2b1/lute/db/language_defs/turkish/definition.yaml
+-rw-r--r--   0        0        0      941 2024-04-11 08:21:17.607779 lute3-3.3.2b1/lute/db/language_defs/turkish/tr_demo.txt
+-rw-r--r--   0        0        0     2211 2024-04-24 06:13:00.177691 lute3-3.3.2b1/lute/db/language_defs/ukrainian/definition.yaml
+-rw-r--r--   0        0        0     1034 2024-04-24 06:13:00.185004 lute3-3.3.2b1/lute/db/language_defs/ukrainian/story_1.txt
+-rw-r--r--   0        0        0     1773 2024-04-11 08:21:17.607893 lute3-3.3.2b1/lute/db/language_defs/verify_files.py
+-rw-r--r--   0        0        0      798 2024-04-20 05:57:30.291713 lute3-3.3.2b1/lute/db/language_defs/vietnamese/definition.yaml
+-rw-r--r--   0        0        0      658 2024-04-20 05:37:09.817363 lute3-3.3.2b1/lute/db/language_defs/vietnamese/lan_bien.txt
+-rw-r--r--   0        0        0      615 2023-11-09 09:07:06.767671 lute3-3.3.2b1/lute/db/management.py
+-rw-r--r--   0        0        0     1620 2023-10-26 01:04:31.825247 lute3-3.3.2b1/lute/db/schema/README.md
+-rw-r--r--   0        0        0    42817 2024-04-25 23:14:02.658081 lute3-3.3.2b1/lute/db/schema/baseline.sql
+-rw-r--r--   0        0        0     8817 2024-03-08 03:05:01.856057 lute3-3.3.2b1/lute/db/schema/empty.sql
+-rw-r--r--   0        0        0      246 2023-10-20 18:48:10.168442 lute3-3.3.2b1/lute/db/schema/migrations/20230409_224327_load_statuses.sql
+-rw-r--r--   0        0        0      178 2023-10-20 18:48:10.168634 lute3-3.3.2b1/lute/db/schema/migrations/20230414_225828_add_texttokens_TokTextLC.sql
+-rw-r--r--   0        0        0      245 2023-10-20 18:48:10.168826 lute3-3.3.2b1/lute/db/schema/migrations/20230428_224656_create_wordflashmessages_table.sql
+-rw-r--r--   0        0        0     2067 2023-10-20 18:48:10.169209 lute3-3.3.2b1/lute/db/schema/migrations/20230518_190000_remove_old_words_fields.sql
+-rw-r--r--   0        0        0      680 2023-10-20 18:48:10.169512 lute3-3.3.2b1/lute/db/schema/migrations/20230519_194627_add_TxDateRead.sql
+-rw-r--r--   0        0        0       96 2023-10-20 18:48:10.169708 lute3-3.3.2b1/lute/db/schema/migrations/20230621_010000_drop_texttags_table.sql
+-rw-r--r--   0        0        0     1143 2023-10-20 18:48:10.169918 lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_01_booktags.sql
+-rw-r--r--   0        0        0     1141 2023-10-20 18:48:10.170132 lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_02_wordtags.sql
+-rw-r--r--   0        0        0     1226 2023-10-20 18:48:10.170317 lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_03_sentences.sql
+-rw-r--r--   0        0        0     1214 2023-10-20 18:48:10.170503 lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_04_texttokens.sql
+-rw-r--r--   0        0        0     1559 2023-10-20 18:48:10.170690 lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_05_texts.sql
+-rw-r--r--   0        0        0     1147 2023-10-20 18:48:10.170868 lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_06_bookstats.sql
+-rw-r--r--   0        0        0     1038 2023-10-20 18:48:10.171044 lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_07_termimages.sql
+-rw-r--r--   0        0        0     1044 2023-10-20 18:48:10.171217 lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_08_wordflashmessages.sql
+-rw-r--r--   0        0        0     1213 2023-10-20 18:48:10.171396 lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_09_wordparents.sql
+-rw-r--r--   0        0        0     2022 2023-10-20 18:48:10.171568 lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_10_words.sql
+-rw-r--r--   0        0        0     1227 2023-10-20 18:48:10.171723 lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_11_books.sql
+-rw-r--r--   0        0        0       56 2023-10-20 18:48:10.171870 lute3-3.3.2b1/lute/db/schema/migrations/20230623_234104_drop_TxTitle.sql
+-rw-r--r--   0        0        0       38 2023-10-20 18:48:10.172012 lute3-3.3.2b1/lute/db/schema/migrations/20230624_182104_drop_index_TxBkIDTxOrder.sql
+-rw-r--r--   0        0        0      908 2023-10-20 18:48:10.172172 lute3-3.3.2b1/lute/db/schema/migrations/20230818_201200_add_BkWordCount.sql
+-rw-r--r--   0        0        0       87 2023-10-20 18:48:10.172337 lute3-3.3.2b1/lute/db/schema/migrations/20230819_044107_drop_texttokens.sql
+-rw-r--r--   0        0        0      168 2023-10-20 18:48:10.172618 lute3-3.3.2b1/lute/db/schema/migrations/20230819_050036_vacuum.sql
+-rw-r--r--   0        0        0      736 2023-10-20 18:48:10.172795 lute3-3.3.2b1/lute/db/schema/migrations/20230827_052154_allow_multiple_word_parents.sql
+-rw-r--r--   0        0        0     1031 2023-10-20 18:48:10.173096 lute3-3.3.2b1/lute/db/schema/migrations/20231018_211236_remove_excess_texts_fields.sql
+-rw-r--r--   0        0        0      930 2023-11-03 01:33:16.686624 lute3-3.3.2b1/lute/db/schema/migrations/20231101_203811_modify_settings_schema.sql
+-rw-r--r--   0        0        0      114 2024-01-13 04:05:05.209858 lute3-3.3.2b1/lute/db/schema/migrations/20231130_141236_add_TxWordCount.sql
+-rw-r--r--   0        0        0      194 2024-01-13 04:05:05.210324 lute3-3.3.2b1/lute/db/schema/migrations/20231210_103924_add_book_audio_fields.sql
+-rw-r--r--   0        0        0       65 2024-02-07 07:50:18.754352 lute3-3.3.2b1/lute/db/schema/migrations/20240101_122610_add_bookstats_status_distribution.sql
+-rw-r--r--   0        0        0       70 2024-02-07 07:50:18.754640 lute3-3.3.2b1/lute/db/schema/migrations/20240113_215142_add_term_follow_parent_bool.sql
+-rw-r--r--   0        0        0      194 2024-02-07 07:50:18.754951 lute3-3.3.2b1/lute/db/schema/migrations/20240118_154258_change_status_abbrev.sql
+-rw-r--r--   0        0        0     1487 2024-02-07 07:50:18.755302 lute3-3.3.2b1/lute/db/schema/migrations/20240125_drop_BkWordCount.sql
+-rw-r--r--   0        0        0     1188 2024-02-07 07:50:18.755674 lute3-3.3.2b1/lute/db/schema/migrations/20240125_drop_bookstats_wordcount.sql
+-rw-r--r--   0        0        0     1877 2024-02-19 02:42:49.355669 lute3-3.3.2b1/lute/db/schema/migrations/20240207_01_create_languagedicts.sql
+-rw-r--r--   0        0        0     1570 2024-02-19 02:42:49.355795 lute3-3.3.2b1/lute/db/schema/migrations/20240207_02_drop_old_language_fields.sql
+-rw-r--r--   0        0        0      224 2023-10-20 18:48:10.173345 lute3-3.3.2b1/lute/db/schema/migrations/README.md
+-rw-r--r--   0        0        0      222 2023-11-03 01:33:16.686865 lute3-3.3.2b1/lute/db/schema/migrations_repeatable/README.md
+-rw-r--r--   0        0        0      992 2024-02-07 07:50:18.756034 lute3-3.3.2b1/lute/db/schema/migrations_repeatable/trig_wordparents.sql
+-rw-r--r--   0        0        0     1751 2024-03-25 09:32:17.264354 lute3-3.3.2b1/lute/db/schema/migrations_repeatable/trig_words.sql
+-rw-r--r--   0        0        0       36 2023-11-03 01:33:16.687020 lute3-3.3.2b1/lute/db/schema/migrations_repeatable/vacuum.sql
+-rw-r--r--   0        0        0        0 2023-10-20 18:48:10.173889 lute3-3.3.2b1/lute/db/setup/__init__.py
+-rw-r--r--   0        0        0     5201 2023-11-11 22:05:26.094785 lute3-3.3.2b1/lute/db/setup/main.py
+-rw-r--r--   0        0        0     3726 2023-11-08 00:06:31.606907 lute3-3.3.2b1/lute/db/setup/migrator.py
+-rw-r--r--   0        0        0        0 2023-11-01 07:45:01.506123 lute3-3.3.2b1/lute/dev_api/__init__.py
+-rw-r--r--   0        0        0     5096 2024-02-19 02:42:49.356009 lute3-3.3.2b1/lute/dev_api/routes.py
+-rw-r--r--   0        0        0        0 2023-10-16 06:20:14.170764 lute3-3.3.2b1/lute/language/__init__.py
+-rw-r--r--   0        0        0     3088 2024-02-19 02:42:49.356211 lute3-3.3.2b1/lute/language/forms.py
+-rw-r--r--   0        0        0     6393 2024-04-21 08:30:46.469042 lute3-3.3.2b1/lute/language/routes.py
+-rw-r--r--   0        0        0     2260 2024-04-21 08:30:46.469211 lute3-3.3.2b1/lute/language/service.py
+-rw-r--r--   0        0        0     3329 2024-04-11 08:34:46.297126 lute3-3.3.2b1/lute/main.py
+-rw-r--r--   0        0        0        0 2023-10-04 05:48:35.020519 lute3-3.3.2b1/lute/models/__init__.py
+-rw-r--r--   0        0        0    11122 2024-03-15 03:25:40.869518 lute3-3.3.2b1/lute/models/book.py
+-rw-r--r--   0        0        0     8776 2024-04-18 00:26:46.670181 lute3-3.3.2b1/lute/models/language.py
+-rw-r--r--   0        0        0     8672 2024-03-13 16:31:06.436856 lute3-3.3.2b1/lute/models/setting.py
+-rw-r--r--   0        0        0    11351 2024-04-21 08:40:18.045190 lute3-3.3.2b1/lute/models/term.py
+-rw-r--r--   0        0        0        0 2023-10-07 05:09:39.898452 lute3-3.3.2b1/lute/parse/__init__.py
+-rw-r--r--   0        0        0     3918 2024-03-08 03:05:01.859321 lute3-3.3.2b1/lute/parse/base.py
+-rw-r--r--   0        0        0     1646 2023-11-08 00:06:31.610408 lute3-3.3.2b1/lute/parse/character_parser.py
+-rw-r--r--   0        0        0     4735 2024-03-08 03:05:01.859524 lute3-3.3.2b1/lute/parse/mecab_parser.py
+-rw-r--r--   0        0        0     1680 2024-03-08 03:05:01.859845 lute3-3.3.2b1/lute/parse/registry.py
+-rw-r--r--   0        0        0     4182 2024-03-17 12:47:12.946271 lute3-3.3.2b1/lute/parse/space_delimited_parser.py
+-rw-r--r--   0        0        0        0 2023-10-16 06:20:14.172648 lute3-3.3.2b1/lute/read/__init__.py
+-rw-r--r--   0        0        0      211 2023-11-08 00:06:31.611930 lute3-3.3.2b1/lute/read/forms.py
+-rw-r--r--   0        0        0        0 2023-10-18 06:43:42.367570 lute3-3.3.2b1/lute/read/render/__init__.py
+-rw-r--r--   0        0        0    17547 2024-03-25 09:32:17.265933 lute3-3.3.2b1/lute/read/render/renderable_calculator.py
+-rw-r--r--   0        0        0     5653 2024-03-25 17:57:11.309963 lute3-3.3.2b1/lute/read/render/service.py
+-rw-r--r--   0        0        0     7010 2024-03-25 09:32:17.266834 lute3-3.3.2b1/lute/read/routes.py
+-rw-r--r--   0        0        0     5429 2024-03-25 17:48:03.854029 lute3-3.3.2b1/lute/read/service.py
+-rw-r--r--   0        0        0        0 2023-11-03 06:31:15.939906 lute3-3.3.2b1/lute/settings/__init__.py
+-rw-r--r--   0        0        0     5264 2024-03-13 16:31:06.437777 lute3-3.3.2b1/lute/settings/routes.py
+-rw-r--r--   0        0        0     1738 2023-10-04 05:48:35.022956 lute3-3.3.2b1/lute/static/css/images/animated-overlay.gif
+-rw-r--r--   0        0        0     2434 2023-10-04 05:48:35.023257 lute3-3.3.2b1/lute/static/css/images/jplayer-black-and-yellow.png
+-rw-r--r--   0        0        0    14525 2023-10-04 05:48:35.023672 lute3-3.3.2b1/lute/static/css/images/jplayer.blue.monday.jpg
+-rw-r--r--   0        0        0   304064 2023-10-04 05:48:35.024510 lute3-3.3.2b1/lute/static/css/images/pbar-ani.gif
+-rw-r--r--   0        0        0      212 2023-10-04 05:48:35.024852 lute3-3.3.2b1/lute/static/css/images/ui-bg_flat_0_555555_40x100.png
+-rw-r--r--   0        0        0      180 2023-10-04 05:48:35.025123 lute3-3.3.2b1/lute/static/css/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-r--r--   0        0        0      220 2023-10-04 05:48:35.025729 lute3-3.3.2b1/lute/static/css/images/ui-bg_flat_75_222222_40x100.png
+-rw-r--r--   0        0        0      220 2023-10-04 05:48:35.026029 lute3-3.3.2b1/lute/static/css/images/ui-bg_flat_75_444444_40x100.png
+-rw-r--r--   0        0        0      178 2023-10-04 05:48:35.026359 lute3-3.3.2b1/lute/static/css/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-r--r--   0        0        0      120 2023-10-04 05:48:35.026642 lute3-3.3.2b1/lute/static/css/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0        0        0      105 2023-10-04 05:48:35.026929 lute3-3.3.2b1/lute/static/css/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0        0        0      111 2023-10-04 05:48:35.027288 lute3-3.3.2b1/lute/static/css/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0        0        0      110 2023-10-04 05:48:35.027566 lute3-3.3.2b1/lute/static/css/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0        0        0      119 2023-10-04 05:48:35.027847 lute3-3.3.2b1/lute/static/css/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0        0        0      277 2023-10-04 05:48:35.028257 lute3-3.3.2b1/lute/static/css/images/ui-bg_highlight-soft_75_222222_1x100.png
+-rw-r--r--   0        0        0      101 2023-10-04 05:48:35.028513 lute3-3.3.2b1/lute/static/css/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0        0        0      251 2023-10-04 05:48:35.028793 lute3-3.3.2b1/lute/static/css/images/ui-bg_inset-hard_55_333333_1x100.png
+-rw-r--r--   0        0        0      251 2023-10-04 05:48:35.029316 lute3-3.3.2b1/lute/static/css/images/ui-bg_inset-hard_95_444444_1x100.png
+-rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.029681 lute3-3.3.2b1/lute/static/css/images/ui-icons_222222_256x240.png
+-rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.030066 lute3-3.3.2b1/lute/static/css/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0        0        0     6992 2023-10-04 05:48:35.030537 lute3-3.3.2b1/lute/static/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.030833 lute3-3.3.2b1/lute/static/css/images/ui-icons_454545_256x240.png
+-rw-r--r--   0        0        0     6988 2023-10-04 05:48:35.031207 lute3-3.3.2b1/lute/static/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     4549 2023-10-04 05:48:35.031493 lute3-3.3.2b1/lute/static/css/images/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     6999 2023-10-04 05:48:35.031792 lute3-3.3.2b1/lute/static/css/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.032071 lute3-3.3.2b1/lute/static/css/images/ui-icons_888888_256x240.png
+-rw-r--r--   0        0        0     6991 2023-10-04 05:48:35.032366 lute3-3.3.2b1/lute/static/css/images/ui-icons_BBBBBB_256x240.png
+-rw-r--r--   0        0        0     4549 2023-10-04 05:48:35.032703 lute3-3.3.2b1/lute/static/css/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     4369 2023-10-04 05:48:35.033223 lute3-3.3.2b1/lute/static/css/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0        0        0     6299 2023-10-04 05:48:35.033571 lute3-3.3.2b1/lute/static/css/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0     8434 2024-04-03 08:59:19.275790 lute3-3.3.2b1/lute/static/css/player-styles.css
+-rw-r--r--   0        0        0    40805 2024-03-25 09:32:17.268825 lute3-3.3.2b1/lute/static/css/styles.css
+-rw-r--r--   0        0        0    15406 2023-10-04 05:48:35.035622 lute3-3.3.2b1/lute/static/favicon.ico
+-rw-r--r--   0        0        0    15406 2023-10-04 05:48:35.036140 lute3-3.3.2b1/lute/static/favicon_dev.ico
+-rw-r--r--   0        0        0      485 2023-10-04 05:48:35.036488 lute3-3.3.2b1/lute/static/icn/arrow-000-medium.png
+-rw-r--r--   0        0        0      479 2023-10-04 05:48:35.036809 lute3-3.3.2b1/lute/static/icn/arrow-180-medium.png
+-rw-r--r--   0        0        0      811 2023-10-04 05:48:35.037131 lute3-3.3.2b1/lute/static/icn/arrow-circle-135.png
+-rw-r--r--   0        0        0      790 2023-10-04 05:48:35.037385 lute3-3.3.2b1/lute/static/icn/arrow-circle-225-left.png
+-rw-r--r--   0        0        0      786 2023-10-04 05:48:35.037680 lute3-3.3.2b1/lute/static/icn/arrow-circle-315.png
+-rw-r--r--   0        0        0      485 2023-10-04 05:48:35.037925 lute3-3.3.2b1/lute/static/icn/arrow-norepeat.png
+-rw-r--r--   0        0        0      587 2023-10-04 05:48:35.038190 lute3-3.3.2b1/lute/static/icn/arrow-repeat.png
+-rw-r--r--   0        0        0      601 2023-10-04 05:48:35.038457 lute3-3.3.2b1/lute/static/icn/arrow-stop.png
+-rw-r--r--   0        0        0      622 2023-10-04 05:48:35.038703 lute3-3.3.2b1/lute/static/icn/book--pencil.png
+-rw-r--r--   0        0        0      650 2023-10-04 05:48:35.038940 lute3-3.3.2b1/lute/static/icn/book-open-bookmark.png
+-rw-r--r--   0        0        0      613 2023-10-04 05:48:35.039204 lute3-3.3.2b1/lute/static/icn/book-open-text.png
+-rw-r--r--   0        0        0      600 2024-02-19 02:42:49.358289 lute3-3.3.2b1/lute/static/icn/book-open-text.svg
+-rw-r--r--   0        0        0      552 2024-01-13 04:05:05.217231 lute3-3.3.2b1/lute/static/icn/bookmark-off.svg
+-rw-r--r--   0        0        0      414 2024-01-13 04:05:05.217572 lute3-3.3.2b1/lute/static/icn/bookmark-on.svg
+-rw-r--r--   0        0        0      784 2023-10-04 05:48:35.039508 lute3-3.3.2b1/lute/static/icn/broom.png
+-rw-r--r--   0        0        0      398 2023-10-04 05:48:35.039745 lute3-3.3.2b1/lute/static/icn/calculator.png
+-rw-r--r--   0        0        0      405 2023-10-04 05:48:35.040009 lute3-3.3.2b1/lute/static/icn/card--minus.png
+-rw-r--r--   0        0        0      556 2023-10-04 05:48:35.040231 lute3-3.3.2b1/lute/static/icn/card--pencil.png
+-rw-r--r--   0        0        0      504 2023-10-04 05:48:35.040493 lute3-3.3.2b1/lute/static/icn/card--plus.png
+-rw-r--r--   0        0        0      473 2023-10-04 05:48:35.040762 lute3-3.3.2b1/lute/static/icn/cards-stack.png
+-rw-r--r--   0        0        0      434 2024-01-13 04:05:05.218143 lute3-3.3.2b1/lute/static/icn/caret-left.svg
+-rw-r--r--   0        0        0      427 2024-01-13 04:05:05.218284 lute3-3.3.2b1/lute/static/icn/caret-right.svg
+-rw-r--r--   0        0        0      369 2023-10-04 05:48:35.041070 lute3-3.3.2b1/lute/static/icn/chain.png
+-rw-r--r--   0        0        0      624 2023-10-04 05:48:35.041330 lute3-3.3.2b1/lute/static/icn/clock.png
+-rw-r--r--   0        0        0      952 2024-02-07 07:50:18.763469 lute3-3.3.2b1/lute/static/icn/close-white.svg
+-rw-r--r--   0        0        0     1438 2024-01-13 04:05:05.219492 lute3-3.3.2b1/lute/static/icn/close.svg
+-rw-r--r--   0        0        0      404 2023-10-04 05:48:35.041576 lute3-3.3.2b1/lute/static/icn/control-180.png
+-rw-r--r--   0        0        0      511 2023-10-04 05:48:35.041944 lute3-3.3.2b1/lute/static/icn/control-stop-180.png
+-rw-r--r--   0        0        0      523 2023-10-04 05:48:35.042219 lute3-3.3.2b1/lute/static/icn/control-stop.png
+-rw-r--r--   0        0        0      405 2023-10-04 05:48:35.042485 lute3-3.3.2b1/lute/static/icn/control.png
+-rw-r--r--   0        0        0      920 2023-10-04 05:48:35.042813 lute3-3.3.2b1/lute/static/icn/cross-big.png
+-rw-r--r--   0        0        0      555 2023-10-04 05:48:35.043135 lute3-3.3.2b1/lute/static/icn/cross-button.png
+-rw-r--r--   0        0        0      544 2023-10-04 05:48:35.043410 lute3-3.3.2b1/lute/static/icn/cross.png
+-rw-r--r--   0        0        0      658 2023-10-04 05:48:35.043716 lute3-3.3.2b1/lute/static/icn/document--pencil.png
+-rw-r--r--   0        0        0     1761 2024-02-07 07:50:18.763842 lute3-3.3.2b1/lute/static/icn/drag-handle.svg
+-rw-r--r--   0        0        0      674 2023-10-04 05:48:35.043952 lute3-3.3.2b1/lute/static/icn/drawer--minus.png
+-rw-r--r--   0        0        0      717 2023-10-04 05:48:35.044272 lute3-3.3.2b1/lute/static/icn/drawer--plus.png
+-rwxr-xr-x   0        0        0       55 2023-10-04 05:48:35.044638 lute3-3.3.2b1/lute/static/icn/empty.gif
+-rw-r--r--   0        0        0      680 2023-10-04 05:48:35.044851 lute3-3.3.2b1/lute/static/icn/eraser.png
+-rw-r--r--   0        0        0      539 2023-10-04 05:48:35.045049 lute3-3.3.2b1/lute/static/icn/exclamation-button.png
+-rw-r--r--   0        0        0      658 2023-10-04 05:48:35.045241 lute3-3.3.2b1/lute/static/icn/exclamation-red.png
+-rw-r--r--   0        0        0      685 2023-10-04 05:48:35.045451 lute3-3.3.2b1/lute/static/icn/external.png
+-rw-r--r--   0        0        0      536 2023-10-04 05:48:35.045663 lute3-3.3.2b1/lute/static/icn/eye.png
+-rw-r--r--   0        0        0      792 2023-10-04 05:48:35.045884 lute3-3.3.2b1/lute/static/icn/feed--pencil.png
+-rw-r--r--   0        0        0      737 2023-10-04 05:48:35.046102 lute3-3.3.2b1/lute/static/icn/feed--plus.png
+-rw-r--r--   0        0        0      566 2024-01-13 04:05:05.221040 lute3-3.3.2b1/lute/static/icn/ff.svg
+-rw-r--r--   0        0        0     1297 2024-01-13 04:05:05.221203 lute3-3.3.2b1/lute/static/icn/font-decrease.svg
+-rw-r--r--   0        0        0     1378 2024-01-13 04:05:05.221326 lute3-3.3.2b1/lute/static/icn/font-increase.svg
+-rw-r--r--   0        0        0      630 2023-10-04 05:48:35.046306 lute3-3.3.2b1/lute/static/icn/funnel--minus.png
+-rw-r--r--   0        0        0      543 2023-10-04 05:48:35.046715 lute3-3.3.2b1/lute/static/icn/funnel.png
+-rw-r--r--   0        0        0      617 2024-02-19 02:42:49.358629 lute3-3.3.2b1/lute/static/icn/images.svg
+-rw-r--r--   0        0        0      692 2023-10-04 05:48:35.047033 lute3-3.3.2b1/lute/static/icn/inbox-download.png
+-rw-r--r--   0        0        0      674 2023-10-04 05:48:35.047235 lute3-3.3.2b1/lute/static/icn/inbox-upload.png
+-rw-r--r--   0        0        0     1553 2023-10-04 05:48:35.047472 lute3-3.3.2b1/lute/static/icn/indicator.gif
+-rw-r--r--   0        0        0     1039 2023-10-04 05:48:35.047683 lute3-3.3.2b1/lute/static/icn/light-bulb-A.png
+-rw-r--r--   0        0        0     1037 2023-10-04 05:48:35.047913 lute3-3.3.2b1/lute/static/icn/light-bulb-T.png
+-rw-r--r--   0        0        0     1010 2023-10-04 05:48:35.048117 lute3-3.3.2b1/lute/static/icn/light-bulb-off-A.png
+-rw-r--r--   0        0        0     1001 2023-10-04 05:48:35.048320 lute3-3.3.2b1/lute/static/icn/light-bulb-off-T.png
+-rw-r--r--   0        0        0      943 2023-10-04 05:48:35.048686 lute3-3.3.2b1/lute/static/icn/light-bulb-off.png
+-rw-r--r--   0        0        0      947 2023-10-04 05:48:35.048956 lute3-3.3.2b1/lute/static/icn/light-bulb.png
+-rw-r--r--   0        0        0      631 2023-10-04 05:48:35.049160 lute3-3.3.2b1/lute/static/icn/lightning.png
+-rw-r--r--   0        0        0     1687 2024-01-13 04:05:05.222154 lute3-3.3.2b1/lute/static/icn/line-spacing-decrease.svg
+-rw-r--r--   0        0        0     2575 2024-01-13 04:05:05.222293 lute3-3.3.2b1/lute/static/icn/line-spacing-increase.svg
+-rw-r--r--   0        0        0      277 2024-02-19 02:42:49.358831 lute3-3.3.2b1/lute/static/icn/list.svg
+-rw-r--r--   0        0        0      451 2023-10-04 05:48:35.049360 lute3-3.3.2b1/lute/static/icn/minus-button.png
+-rw-r--r--   0        0        0      259 2023-10-04 05:48:35.049740 lute3-3.3.2b1/lute/static/icn/minus.png
+-rw-r--r--   0        0        0      489 2023-10-04 05:48:35.049931 lute3-3.3.2b1/lute/static/icn/navigation-000-button-light.png
+-rw-r--r--   0        0        0      614 2023-10-04 05:48:35.050311 lute3-3.3.2b1/lute/static/icn/navigation-000-button.png
+-rw-r--r--   0        0        0      486 2023-10-04 05:48:35.050548 lute3-3.3.2b1/lute/static/icn/navigation-180-button-light.png
+-rw-r--r--   0        0        0      620 2023-10-04 05:48:35.050750 lute3-3.3.2b1/lute/static/icn/navigation-180-button.png
+-rw-r--r--   0        0        0      607 2023-10-04 05:48:35.050975 lute3-3.3.2b1/lute/static/icn/new_line.png
+-rw-r--r--   0        0        0      458 2024-01-13 04:05:05.222661 lute3-3.3.2b1/lute/static/icn/next.svg
+-rw-r--r--   0        0        0      633 2023-10-04 05:48:35.051264 lute3-3.3.2b1/lute/static/icn/notebook--minus.png
+-rw-r--r--   0        0        0      723 2023-10-04 05:48:35.051477 lute3-3.3.2b1/lute/static/icn/notebook--pencil.png
+-rw-r--r--   0        0        0      664 2023-10-04 05:48:35.051850 lute3-3.3.2b1/lute/static/icn/notebook--plus.png
+-rw-r--r--   0        0        0      541 2023-10-04 05:48:35.052045 lute3-3.3.2b1/lute/static/icn/notebook.png
+-rw-r--r--   0        0        0      790 2024-01-13 04:05:05.223020 lute3-3.3.2b1/lute/static/icn/open.svg
+-rw-r--r--   0        0        0      428 2024-01-13 04:05:05.223265 lute3-3.3.2b1/lute/static/icn/pause.svg
+-rw-r--r--   0        0        0      475 2023-10-04 05:48:35.052249 lute3-3.3.2b1/lute/static/icn/pencil.png
+-rw-r--r--   0        0        0     1154 2023-10-04 05:48:35.052521 lute3-3.3.2b1/lute/static/icn/photo-album.png
+-rw-r--r--   0        0        0      591 2024-01-13 04:05:05.223508 lute3-3.3.2b1/lute/static/icn/pin.svg
+-rw-r--r--   0        0        0      142 2023-10-04 05:48:35.052720 lute3-3.3.2b1/lute/static/icn/placeholder.png
+-rw-r--r--   0        0        0      461 2024-01-13 04:05:05.223871 lute3-3.3.2b1/lute/static/icn/play.svg
+-rw-r--r--   0        0        0      583 2023-10-04 05:48:35.052918 lute3-3.3.2b1/lute/static/icn/plus-button.png
+-rw-r--r--   0        0        0      521 2023-10-04 05:48:35.053238 lute3-3.3.2b1/lute/static/icn/plus.png
+-rw-r--r--   0        0        0      445 2024-01-13 04:05:05.224128 lute3-3.3.2b1/lute/static/icn/prev.svg
+-rw-r--r--   0        0        0      722 2023-10-04 05:48:35.053446 lute3-3.3.2b1/lute/static/icn/printer.png
+-rw-r--r--   0        0        0      722 2023-10-04 05:48:35.053709 lute3-3.3.2b1/lute/static/icn/question-balloon.png
+-rw-r--r--   0        0        0      924 2023-10-04 05:48:35.053893 lute3-3.3.2b1/lute/static/icn/question-frame.png
+-rw-r--r--   0        0        0     1921 2024-02-07 07:50:18.764174 lute3-3.3.2b1/lute/static/icn/reload.png
+-rw-r--r--   0        0        0      558 2024-01-13 04:05:05.224511 lute3-3.3.2b1/lute/static/icn/rewind.svg
+-rw-r--r--   0        0        0      837 2023-10-04 05:48:35.054103 lute3-3.3.2b1/lute/static/icn/script-import.png
+-rw-r--r--   0        0        0     1041 2024-03-13 16:31:06.440554 lute3-3.3.2b1/lute/static/icn/settings-gear-icon.svg
+-rw-r--r--   0        0        0      526 2024-01-13 04:05:05.224876 lute3-3.3.2b1/lute/static/icn/skip-back.svg
+-rw-r--r--   0        0        0      755 2023-10-04 05:48:35.054284 lute3-3.3.2b1/lute/static/icn/smiley-sad.png
+-rw-r--r--   0        0        0      811 2023-10-04 05:48:35.054463 lute3-3.3.2b1/lute/static/icn/smiley.png
+-rw-r--r--   0        0        0      452 2023-10-04 05:48:35.054648 lute3-3.3.2b1/lute/static/icn/speaker-volume-none.png
+-rw-r--r--   0        0        0      543 2023-10-04 05:48:35.054955 lute3-3.3.2b1/lute/static/icn/speaker-volume.png
+-rw-r--r--   0        0        0      757 2023-10-04 05:48:35.055365 lute3-3.3.2b1/lute/static/icn/star.png
+-rw-r--r--   0        0        0      432 2023-10-04 05:48:35.055719 lute3-3.3.2b1/lute/static/icn/status-away.png
+-rw-r--r--   0        0        0      407 2023-10-04 05:48:35.056570 lute3-3.3.2b1/lute/static/icn/status-busy.png
+-rw-r--r--   0        0        0      401 2023-10-04 05:48:35.056940 lute3-3.3.2b1/lute/static/icn/status.png
+-rw-r--r--   0        0        0      466 2023-10-04 05:48:35.057163 lute3-3.3.2b1/lute/static/icn/sticky-note--minus.png
+-rw-r--r--   0        0        0      638 2023-10-04 05:48:35.057670 lute3-3.3.2b1/lute/static/icn/sticky-note--pencil.png
+-rw-r--r--   0        0        0      571 2023-10-04 05:48:35.057865 lute3-3.3.2b1/lute/static/icn/sticky-note--plus.png
+-rw-r--r--   0        0        0      520 2023-10-04 05:48:35.058304 lute3-3.3.2b1/lute/static/icn/sticky-note-text.png
+-rw-r--r--   0        0        0      425 2023-10-04 05:48:35.058599 lute3-3.3.2b1/lute/static/icn/sticky-note.png
+-rw-r--r--   0        0        0      533 2023-10-04 05:48:35.058808 lute3-3.3.2b1/lute/static/icn/sticky-notes-stack.png
+-rw-r--r--   0        0        0      618 2023-10-04 05:48:35.059020 lute3-3.3.2b1/lute/static/icn/sticky-notes-text.png
+-rw-r--r--   0        0        0      546 2023-10-04 05:48:35.059221 lute3-3.3.2b1/lute/static/icn/sticky-notes.png
+-rw-r--r--   0        0        0     2805 2023-10-04 05:48:35.059585 lute3-3.3.2b1/lute/static/icn/test_correct.png
+-rw-r--r--   0        0        0     2805 2023-10-04 05:48:35.059871 lute3-3.3.2b1/lute/static/icn/test_notyet.png
+-rw-r--r--   0        0        0     2805 2023-10-04 05:48:35.060061 lute3-3.3.2b1/lute/static/icn/test_wrong.png
+-rw-r--r--   0        0        0      803 2024-01-13 04:05:05.225875 lute3-3.3.2b1/lute/static/icn/text-column-one.svg
+-rw-r--r--   0        0        0     1613 2024-01-13 04:05:05.226200 lute3-3.3.2b1/lute/static/icn/text-column-two.svg
+-rw-r--r--   0        0        0      732 2023-10-04 05:48:35.060251 lute3-3.3.2b1/lute/static/icn/thumb-up.png
+-rw-r--r--   0        0        0      751 2023-10-04 05:48:35.060509 lute3-3.3.2b1/lute/static/icn/thumb.png
+-rwxr-xr-x   0        0        0      620 2023-10-04 05:48:35.060685 lute3-3.3.2b1/lute/static/icn/tick-button-small.png
+-rw-r--r--   0        0        0      568 2023-10-04 05:48:35.060894 lute3-3.3.2b1/lute/static/icn/tick-button.png
+-rw-r--r--   0        0        0      582 2023-10-04 05:48:35.061228 lute3-3.3.2b1/lute/static/icn/tick.png
+-rw-r--r--   0        0        0      521 2024-01-13 04:05:05.226487 lute3-3.3.2b1/lute/static/icn/volume.svg
+-rw-r--r--   0        0        0     3208 2023-10-04 05:48:35.061448 lute3-3.3.2b1/lute/static/icn/waiting.gif
+-rw-r--r--   0        0        0      847 2023-10-04 05:48:35.061633 lute3-3.3.2b1/lute/static/icn/waiting2.gif
+-rw-r--r--   0        0        0     5450 2023-10-04 05:48:35.061895 lute3-3.3.2b1/lute/static/icn/wizard.png
+-rw-r--r--   0        0        0      916 2023-10-04 05:48:35.062193 lute3-3.3.2b1/lute/static/icn/wrench-screwdriver.png
+-rw-r--r--   0        0        0    19567 2023-10-04 05:48:35.062586 lute3-3.3.2b1/lute/static/img/apple-touch-icon-114x114.png
+-rw-r--r--   0        0        0     5618 2023-10-04 05:48:35.062872 lute3-3.3.2b1/lute/static/img/apple-touch-icon-57x57.png
+-rw-r--r--   0        0        0     8461 2023-10-04 05:48:35.063084 lute3-3.3.2b1/lute/static/img/apple-touch-icon-72x72.png
+-rw-r--r--   0        0        0    34198 2023-10-04 05:48:35.063762 lute3-3.3.2b1/lute/static/img/apple-touch-startup.png
+-rw-r--r--   0        0        0    49403 2024-01-13 04:05:05.227551 lute3-3.3.2b1/lute/static/img/lute.png
+-rw-r--r--   0        0        0     1405 2023-10-04 05:48:35.065233 lute3-3.3.2b1/lute/static/img/public_domain.png
+-rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.065440 lute3-3.3.2b1/lute/static/img/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     3767 2023-10-04 05:48:35.065634 lute3-3.3.2b1/lute/static/img/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     3767 2023-10-04 05:48:35.065982 lute3-3.3.2b1/lute/static/img/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.066190 lute3-3.3.2b1/lute/static/img/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.066397 lute3-3.3.2b1/lute/static/img/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     3764 2023-10-04 05:48:35.069007 lute3-3.3.2b1/lute/static/img/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    11246 2024-03-13 16:31:06.443010 lute3-3.3.2b1/lute/static/js/dict-tabs.js
+-rw-r--r--   0        0        0    21071 2024-04-25 20:26:14.880502 lute3-3.3.2b1/lute/static/js/lute.js
+-rw-r--r--   0        0        0    12092 2024-04-03 08:59:19.276203 lute3-3.3.2b1/lute/static/js/player.js
+-rw-r--r--   0        0        0     7406 2024-03-13 16:30:50.206756 lute3-3.3.2b1/lute/static/js/resize.js
+-rw-r--r--   0        0        0     4346 2024-02-07 07:50:18.767242 lute3-3.3.2b1/lute/static/js/text-options.js
+-rw-r--r--   0        0        0   202357 2024-03-15 03:25:40.872972 lute3-3.3.2b1/lute/static/vendor/chartjs/chart.umd.js
+-rw-r--r--   0        0        0    50650 2024-03-15 03:25:40.873223 lute3-3.3.2b1/lute/static/vendor/chartjs/chartjs-adapter-date-fns.js
+-rw-r--r--   0        0        0      624 2024-03-15 03:25:40.873755 lute3-3.3.2b1/lute/static/vendor/datatables/README.md
+-rw-r--r--   0        0        0     4145 2024-03-15 03:25:40.873884 lute3-3.3.2b1/lute/static/vendor/datatables/datatables.button.download.js
+-rw-r--r--   0        0        0    41393 2024-03-15 03:25:40.874305 lute3-3.3.2b1/lute/static/vendor/datatables/datatables.min.css
+-rw-r--r--   0        0        0   164670 2024-03-15 03:25:40.875473 lute3-3.3.2b1/lute/static/vendor/datatables/datatables.min.js
+-rw-r--r--   0        0        0     5253 2024-03-15 03:25:40.876688 lute3-3.3.2b1/lute/static/vendor/jquery/jplayer.css
+-rw-r--r--   0        0        0    34497 2024-03-15 03:25:40.876886 lute3-3.3.2b1/lute/static/vendor/jquery/jquery-ui.css
+-rw-r--r--   0        0        0   240422 2024-03-15 03:25:40.879055 lute3-3.3.2b1/lute/static/vendor/jquery/jquery-ui.min.js
+-rw-r--r--   0        0        0     1753 2024-03-15 03:25:40.879212 lute3-3.3.2b1/lute/static/vendor/jquery/jquery.hoverIntent.js
+-rw-r--r--   0        0        0     8067 2024-03-15 03:25:40.879335 lute3-3.3.2b1/lute/static/vendor/jquery/jquery.jeditable.mini.js
+-rw-r--r--   0        0        0    69303 2024-03-15 03:25:40.879593 lute3-3.3.2b1/lute/static/vendor/jquery/jquery.jplayer.js
+-rw-r--r--   0        0        0    60951 2024-03-15 03:25:40.880095 lute3-3.3.2b1/lute/static/vendor/jquery/jquery.jplayer.min.js
+-rw-r--r--   0        0        0    13714 2024-03-15 03:25:40.880340 lute3-3.3.2b1/lute/static/vendor/jquery/jquery.jplayer.swf
+-rw-r--r--   0        0        0    97163 2024-03-15 03:25:40.880764 lute3-3.3.2b1/lute/static/vendor/jquery/jquery.js
+-rwxr-xr-x   0        0        0     2442 2024-03-15 03:25:40.880893 lute3-3.3.2b1/lute/static/vendor/jquery/jquery.scrollTo.min.js
+-rw-r--r--   0        0        0    80119 2024-03-15 03:25:40.881202 lute3-3.3.2b1/lute/static/vendor/jquery/jquery.xpath.min.js
+-rw-r--r--   0        0        0    11207 2024-03-15 03:25:40.881421 lute3-3.3.2b1/lute/static/vendor/tagify/tagify.css
+-rw-r--r--   0        0        0    60507 2024-03-15 03:25:40.881716 lute3-3.3.2b1/lute/static/vendor/tagify/tagify.min.js
+-rw-r--r--   0        0        0    23275 2024-03-15 03:25:40.881883 lute3-3.3.2b1/lute/static/vendor/tagify/tagify.polyfills.min.js
+-rw-r--r--   0        0        0     1723 2024-03-15 03:25:40.882103 lute3-3.3.2b1/lute/static/vendor/tagify/tagify_overrides.css
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.232444 lute3-3.3.2b1/lute/stats/__init__.py
+-rw-r--r--   0        0        0      482 2024-01-13 04:05:05.232852 lute3-3.3.2b1/lute/stats/routes.py
+-rw-r--r--   0        0        0     2702 2024-02-07 07:50:18.767674 lute3-3.3.2b1/lute/stats/service.py
+-rw-r--r--   0        0        0     1134 2024-03-15 03:25:40.883026 lute3-3.3.2b1/lute/templates/backup/backup.html
+-rw-r--r--   0        0        0      872 2024-02-19 02:42:49.360741 lute3-3.3.2b1/lute/templates/backup/index.html
+-rw-r--r--   0        0        0     6842 2024-03-30 00:53:12.174491 lute3-3.3.2b1/lute/templates/base.html
+-rw-r--r--   0        0        0     3080 2024-03-25 09:32:17.271785 lute3-3.3.2b1/lute/templates/book/create_new.html
+-rw-r--r--   0        0        0     2503 2024-03-13 16:31:06.446279 lute3-3.3.2b1/lute/templates/book/edit.html
+-rw-r--r--   0        0        0      627 2024-03-25 09:32:17.272608 lute3-3.3.2b1/lute/templates/book/import_webpage.html
+-rw-r--r--   0        0        0      204 2023-11-09 21:55:59.870577 lute3-3.3.2b1/lute/templates/book/index.html
+-rw-r--r--   0        0        0    10771 2024-04-01 08:37:12.255992 lute3-3.3.2b1/lute/templates/book/tablelisting.html
+-rw-r--r--   0        0        0      651 2024-01-13 04:05:05.236118 lute3-3.3.2b1/lute/templates/errors/404_error.html
+-rw-r--r--   0        0        0     1185 2024-01-13 04:05:05.236533 lute3-3.3.2b1/lute/templates/errors/500_error.html
+-rw-r--r--   0        0        0     2278 2024-03-03 03:12:19.455018 lute3-3.3.2b1/lute/templates/hotkeys.html
+-rw-r--r--   0        0        0     5206 2024-03-15 03:25:40.899605 lute3-3.3.2b1/lute/templates/imagesearch/index.html
+-rw-r--r--   0        0        0     1278 2024-04-21 08:30:46.469505 lute3-3.3.2b1/lute/templates/index.html
+-rw-r--r--   0        0        0     7009 2024-02-19 02:42:49.361906 lute3-3.3.2b1/lute/templates/language/_form.html
+-rw-r--r--   0        0        0      131 2023-11-01 07:45:01.587557 lute3-3.3.2b1/lute/templates/language/edit.html
+-rw-r--r--   0        0        0     1427 2024-04-21 08:30:46.469784 lute3-3.3.2b1/lute/templates/language/index.html
+-rw-r--r--   0        0        0     1024 2024-04-21 08:30:46.469937 lute3-3.3.2b1/lute/templates/language/list_predefined.html
+-rw-r--r--   0        0        0      533 2024-02-07 07:50:18.771534 lute3-3.3.2b1/lute/templates/language/new.html
+-rw-r--r--   0        0        0     2522 2024-04-03 08:59:19.276550 lute3-3.3.2b1/lute/templates/read/audio_player.html
+-rw-r--r--   0        0        0      551 2024-03-15 03:25:40.900713 lute3-3.3.2b1/lute/templates/read/flashcopied.html
+-rw-r--r--   0        0        0     1885 2024-03-25 08:52:45.544428 lute3-3.3.2b1/lute/templates/read/frameform.html
+-rw-r--r--   0        0        0    17957 2024-03-15 03:25:40.902256 lute3-3.3.2b1/lute/templates/read/index.html
+-rw-r--r--   0        0        0      605 2024-02-07 07:50:18.773525 lute3-3.3.2b1/lute/templates/read/page_content.html
+-rw-r--r--   0        0        0      755 2024-02-19 02:42:49.362657 lute3-3.3.2b1/lute/templates/read/page_edit_form.html
+-rw-r--r--   0        0        0     3341 2024-03-15 03:25:40.902930 lute3-3.3.2b1/lute/templates/read/reading_menu.html
+-rw-r--r--   0        0        0     1742 2024-03-15 03:25:40.903466 lute3-3.3.2b1/lute/templates/read/termpopup.html
+-rw-r--r--   0        0        0      499 2024-03-08 03:05:01.875375 lute3-3.3.2b1/lute/templates/read/textitem.html
+-rw-r--r--   0        0        0      643 2024-03-15 03:25:40.903763 lute3-3.3.2b1/lute/templates/read/updated.html
+-rw-r--r--   0        0        0     4862 2024-03-30 00:52:04.168998 lute3-3.3.2b1/lute/templates/settings/form.html
+-rw-r--r--   0        0        0     3807 2024-03-15 03:25:40.904464 lute3-3.3.2b1/lute/templates/stats/index.html
+-rw-r--r--   0        0        0    12956 2024-04-23 01:46:59.725369 lute3-3.3.2b1/lute/templates/term/_form.html
+-rw-r--r--   0        0        0     2215 2024-03-13 16:31:06.452196 lute3-3.3.2b1/lute/templates/term/formframes.html
+-rw-r--r--   0        0        0    16104 2024-03-30 00:44:45.757999 lute3-3.3.2b1/lute/templates/term/index.html
+-rw-r--r--   0        0        0     1579 2024-03-30 00:53:36.233514 lute3-3.3.2b1/lute/templates/term/sentences.html
+-rw-r--r--   0        0        0      502 2024-03-15 03:25:40.905825 lute3-3.3.2b1/lute/templates/term_parent_map/index.html
+-rw-r--r--   0        0        0     1093 2024-03-30 00:52:55.723618 lute3-3.3.2b1/lute/templates/termimport/index.html
+-rw-r--r--   0        0        0      755 2024-03-25 09:32:17.275871 lute3-3.3.2b1/lute/templates/termtag/_form.html
+-rw-r--r--   0        0        0      119 2023-10-30 05:47:07.311779 lute3-3.3.2b1/lute/templates/termtag/edit.html
+-rw-r--r--   0        0        0     2654 2024-03-30 00:44:45.758396 lute3-3.3.2b1/lute/templates/termtag/index.html
+-rw-r--r--   0        0        0      170 2023-10-30 05:47:07.312798 lute3-3.3.2b1/lute/templates/termtag/new.html
+-rw-r--r--   0        0        0      654 2024-03-08 03:05:01.878803 lute3-3.3.2b1/lute/templates/version.html
+-rw-r--r--   0        0        0        0 2023-10-21 00:58:40.674085 lute3-3.3.2b1/lute/term/__init__.py
+-rw-r--r--   0        0        0     3353 2024-03-25 09:32:17.277337 lute3-3.3.2b1/lute/term/datatables.py
+-rw-r--r--   0        0        0     4130 2024-03-25 09:32:17.278674 lute3-3.3.2b1/lute/term/forms.py
+-rw-r--r--   0        0        0    16216 2024-03-25 09:32:17.279461 lute3-3.3.2b1/lute/term/model.py
+-rw-r--r--   0        0        0     9475 2024-04-21 08:40:18.045588 lute3-3.3.2b1/lute/term/routes.py
+-rw-r--r--   0        0        0        0 2023-10-28 20:14:27.720594 lute3-3.3.2b1/lute/term_parent_map/__init__.py
+-rw-r--r--   0        0        0     1459 2024-03-15 03:25:40.907485 lute3-3.3.2b1/lute/term_parent_map/routes.py
+-rw-r--r--   0        0        0      866 2024-03-15 03:25:40.907878 lute3-3.3.2b1/lute/term_parent_map/service.py
+-rw-r--r--   0        0        0        0 2023-10-27 22:52:35.310439 lute3-3.3.2b1/lute/termimport/__init__.py
+-rw-r--r--   0        0        0     1793 2024-03-25 09:32:17.280829 lute3-3.3.2b1/lute/termimport/routes.py
+-rw-r--r--   0        0        0     8888 2024-04-03 15:41:04.623267 lute3-3.3.2b1/lute/termimport/service.py
+-rw-r--r--   0        0        0        0 2023-10-30 05:47:07.312889 lute3-3.3.2b1/lute/termtag/__init__.py
+-rw-r--r--   0        0        0      652 2023-11-08 00:06:31.617316 lute3-3.3.2b1/lute/termtag/datatables.py
+-rw-r--r--   0        0        0      309 2023-11-08 00:06:31.617623 lute3-3.3.2b1/lute/termtag/forms.py
+-rw-r--r--   0        0        0     1857 2023-11-08 00:06:31.617959 lute3-3.3.2b1/lute/termtag/routes.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.250549 lute3-3.3.2b1/lute/themes/__init__.py
+-rw-r--r--   0        0        0     1021 2024-03-08 03:05:01.881349 lute3-3.3.2b1/lute/themes/css/Apple_Books.css
+-rw-r--r--   0        0        0     2603 2024-03-15 03:25:40.908418 lute3-3.3.2b1/lute/themes/css/Dark_slate.css
+-rw-r--r--   0        0        0      949 2024-03-13 16:30:50.208931 lute3-3.3.2b1/lute/themes/css/LWT.css
+-rw-r--r--   0        0        0     1096 2024-03-13 16:30:50.209490 lute3-3.3.2b1/lute/themes/css/LingQ.css
+-rw-r--r--   0        0        0     2835 2024-03-15 03:25:40.909175 lute3-3.3.2b1/lute/themes/css/Night.css
+-rw-r--r--   0        0        0      174 2024-01-13 04:05:05.252115 lute3-3.3.2b1/lute/themes/css/README.md
+-rw-r--r--   0        0        0     1153 2024-03-08 03:05:01.882428 lute3-3.3.2b1/lute/themes/routes.py
+-rw-r--r--   0        0        0     1882 2024-03-13 16:30:50.210261 lute3-3.3.2b1/lute/themes/service.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.253134 lute3-3.3.2b1/lute/useraudio/__init__.py
+-rw-r--r--   0        0        0      545 2024-01-13 04:05:05.253460 lute3-3.3.2b1/lute/useraudio/routes.py
+-rw-r--r--   0        0        0        0 2023-10-24 05:43:55.069141 lute3-3.3.2b1/lute/userimage/__init__.py
+-rw-r--r--   0        0        0      656 2023-11-08 00:06:31.618260 lute3-3.3.2b1/lute/userimage/routes.py
+-rw-r--r--   0        0        0        0 2023-10-09 03:35:20.090603 lute3-3.3.2b1/lute/utils/__init__.py
+-rw-r--r--   0        0        0     7072 2024-03-13 16:31:06.454810 lute3-3.3.2b1/lute/utils/data_tables.py
+-rw-r--r--   0        0        0     2043 2024-02-07 07:50:18.794729 lute3-3.3.2b1/lute/utils/debug_helpers.py
+-rw-r--r--   0        0        0     1326 2024-03-13 16:30:50.210892 lute3-3.3.2b1/lute/utils/formutils.py
+-rw-r--r--   0        0        0     1226 2024-04-05 03:40:57.741720 lute3-3.3.2b1/pyproject.toml
+-rw-r--r--   0        0        0     1510 2024-03-30 02:16:42.569672 lute3-3.3.2b1/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-21 08:30:46.470025 lute3-3.3.2b1/scripts/__init__.py
+-rw-r--r--   0        0        0     2564 2024-04-21 08:30:46.470241 lute3-3.3.2b1/scripts/dump_lang_data.py
+-rw-r--r--   0        0        0    10316 2024-04-21 08:30:46.470529 lute3-3.3.2b1/tasks.py
+-rw-r--r--   0        0        0      160 2023-10-22 05:50:12.570821 lute3-3.3.2b1/tests/__init__.py
+-rw-r--r--   0        0        0      442 2023-10-31 05:25:17.232229 lute3-3.3.2b1/tests/acceptance/README.md
+-rw-r--r--   0        0        0      132 2023-11-01 07:45:01.591037 lute3-3.3.2b1/tests/acceptance/__init__.py
+-rw-r--r--   0        0        0     6294 2024-03-25 17:57:11.310500 lute3-3.3.2b1/tests/acceptance/book.feature
+-rw-r--r--   0        0        0    13784 2024-04-03 08:58:27.787631 lute3-3.3.2b1/tests/acceptance/conftest.py
+-rw-r--r--   0        0        0      102 2024-03-15 03:25:40.911823 lute3-3.3.2b1/tests/acceptance/disabled_test_sync_status.py
+-rw-r--r--   0        0        0        3 2023-10-31 05:25:17.232861 lute3-3.3.2b1/tests/acceptance/failure_screenshots/.gitignore
+-rw-r--r--   0        0        0       78 2023-10-31 05:25:17.233099 lute3-3.3.2b1/tests/acceptance/failure_screenshots/README.md
+-rw-r--r--   0        0        0    13194 2024-03-15 03:25:40.912431 lute3-3.3.2b1/tests/acceptance/lute_test_client.py
+-rw-r--r--   0        0        0    10086 2024-03-15 03:25:40.912826 lute3-3.3.2b1/tests/acceptance/reading.feature
+-rw-r--r--   0        0        0     1282 2024-02-07 07:50:18.801083 lute3-3.3.2b1/tests/acceptance/sample_files/Hola.epub
+-rw-r--r--   0        0        0     1433 2024-02-07 07:50:18.801387 lute3-3.3.2b1/tests/acceptance/sample_files/Hola.pdf
+-rw-r--r--   0        0        0       48 2024-03-15 03:25:40.913611 lute3-3.3.2b1/tests/acceptance/sample_files/Hola.srt
+-rw-r--r--   0        0        0       56 2024-03-15 03:25:40.913905 lute3-3.3.2b1/tests/acceptance/sample_files/Hola.vtt
+-rw-r--r--   0        0        0       16 2024-01-13 04:05:05.265704 lute3-3.3.2b1/tests/acceptance/sample_files/hola.txt
+-rw-r--r--   0        0        0       16 2024-02-07 07:50:18.801723 lute3-3.3.2b1/tests/acceptance/sample_files/invalid.epub
+-rw-r--r--   0        0        0       16 2024-02-07 07:50:18.801856 lute3-3.3.2b1/tests/acceptance/sample_files/invalid.pdf
+-rw-r--r--   0        0        0       16 2024-03-15 03:25:40.914165 lute3-3.3.2b1/tests/acceptance/sample_files/invalid.srt
+-rw-r--r--   0        0        0       16 2024-03-15 03:25:40.914274 lute3-3.3.2b1/tests/acceptance/sample_files/invalid.vtt
+-rw-r--r--   0        0        0     1417 2024-03-25 09:32:17.283465 lute3-3.3.2b1/tests/acceptance/sample_files/invalid_empty.epub
+-rw-r--r--   0        0        0       74 2024-02-07 07:50:18.802571 lute3-3.3.2b1/tests/acceptance/sample_files/non_utf_8.txt
+-rw-r--r--   0        0        0     2256 2024-03-25 09:32:17.283950 lute3-3.3.2b1/tests/acceptance/smoke.feature
+-rw-r--r--   0        0        0      630 2024-03-08 03:05:01.891609 lute3-3.3.2b1/tests/acceptance/start_acceptance_app.py
+-rw-r--r--   0        0        0     2082 2024-03-25 09:32:17.284644 lute3-3.3.2b1/tests/acceptance/sync_status.feature
+-rw-r--r--   0        0        0     2153 2024-03-15 03:25:40.915397 lute3-3.3.2b1/tests/acceptance/term.feature
+-rw-r--r--   0        0        0       92 2023-11-08 00:06:31.621311 lute3-3.3.2b1/tests/acceptance/test_book.py
+-rw-r--r--   0        0        0       98 2023-11-08 00:06:31.621627 lute3-3.3.2b1/tests/acceptance/test_reading.py
+-rw-r--r--   0        0        0       83 2024-03-25 09:32:17.285207 lute3-3.3.2b1/tests/acceptance/test_smoke.py
+-rw-r--r--   0        0        0       92 2023-11-08 00:06:31.622287 lute3-3.3.2b1/tests/acceptance/test_term.py
+-rw-r--r--   0        0        0      109 2023-11-08 00:06:31.622737 lute3-3.3.2b1/tests/acceptance/test_unsupported_parser.py
+-rw-r--r--   0        0        0     1304 2024-03-25 09:32:17.285870 lute3-3.3.2b1/tests/acceptance/unsupported_parser.feature
+-rw-r--r--   0        0        0     3708 2024-04-21 08:30:46.470801 lute3-3.3.2b1/tests/conftest.py
+-rw-r--r--   0        0        0     1771 2023-11-08 00:06:31.623664 lute3-3.3.2b1/tests/dbasserts.py
+-rw-r--r--   0        0        0      676 2023-10-22 17:27:11.801049 lute3-3.3.2b1/tests/features/README.md
+-rw-r--r--   0        0        0    15205 2024-03-08 03:05:01.894503 lute3-3.3.2b1/tests/features/rendering.feature
+-rw-r--r--   0        0        0    17666 2024-04-03 15:41:04.623769 lute3-3.3.2b1/tests/features/term_import.feature
+-rw-r--r--   0        0        0     2907 2024-03-25 09:32:17.287963 lute3-3.3.2b1/tests/features/term_import_status_0.feature
+-rw-r--r--   0        0        0     3696 2024-03-23 10:37:45.604972 lute3-3.3.2b1/tests/features/test_rendering.py
+-rw-r--r--   0        0        0     3760 2024-03-25 09:32:17.288599 lute3-3.3.2b1/tests/features/test_term_import.py
+-rw-r--r--   0        0        0        0 2023-09-20 06:21:29.988625 lute3-3.3.2b1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1206 2024-01-13 04:05:05.275517 lute3-3.3.2b1/tests/integration/test_main.py
+-rw-r--r--   0        0        0       97 2023-10-20 06:39:27.112890 lute3-3.3.2b1/tests/orm/README.md
+-rw-r--r--   0        0        0        0 2023-10-20 06:39:27.113017 lute3-3.3.2b1/tests/orm/__init__.py
+-rw-r--r--   0        0        0     2808 2024-02-07 07:50:18.812178 lute3-3.3.2b1/tests/orm/test_Book.py
+-rw-r--r--   0        0        0     3659 2024-02-19 02:42:49.366795 lute3-3.3.2b1/tests/orm/test_Language.py
+-rw-r--r--   0        0        0     8881 2024-04-21 08:40:18.046050 lute3-3.3.2b1/tests/orm/test_Term.py
+-rw-r--r--   0        0        0      871 2023-11-08 00:06:31.626423 lute3-3.3.2b1/tests/orm/test_Text.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.275609 lute3-3.3.2b1/tests/playwright/__init__.py
+-rw-r--r--   0        0        0     8255 2024-04-21 08:30:46.471119 lute3-3.3.2b1/tests/playwright/playwright.py
+-rw-r--r--   0        0        0        0 2023-09-10 06:10:01.992940 lute3-3.3.2b1/tests/unit/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-30 00:38:51.297976 lute3-3.3.2b1/tests/unit/backup/__init__.py
+-rw-r--r--   0        0        0     9602 2024-02-19 02:42:49.368373 lute3-3.3.2b1/tests/unit/backup/test_backup.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:52:22.684248 lute3-3.3.2b1/tests/unit/book/__init__.py
+-rw-r--r--   0        0        0     3884 2024-04-21 08:30:46.471402 lute3-3.3.2b1/tests/unit/book/test_Repository.py
+-rw-r--r--   0        0        0     2241 2024-03-13 16:30:50.212038 lute3-3.3.2b1/tests/unit/book/test_datatables.py
+-rw-r--r--   0        0        0     4124 2024-02-07 07:50:18.815696 lute3-3.3.2b1/tests/unit/book/test_stats.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.277883 lute3-3.3.2b1/tests/unit/cli/__init__.py
+-rw-r--r--   0        0        0      521 2024-01-13 04:05:05.278085 lute3-3.3.2b1/tests/unit/cli/test_language_term_export.py
+-rw-r--r--   0        0        0        0 2023-11-04 21:50:44.092388 lute3-3.3.2b1/tests/unit/config/__init__.py
+-rw-r--r--   0        0        0     3035 2024-01-13 04:05:05.278929 lute3-3.3.2b1/tests/unit/config/test_app_config.py
+-rw-r--r--   0        0        0        0 2023-10-26 01:04:31.832624 lute3-3.3.2b1/tests/unit/db/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-20 18:48:10.174878 lute3-3.3.2b1/tests/unit/db/setup/__init__.py
+-rw-r--r--   0        0        0       28 2023-10-20 18:48:10.175186 lute3-3.3.2b1/tests/unit/db/setup/schema/README.md
+-rw-r--r--   0        0        0      134 2023-10-20 18:48:10.175437 lute3-3.3.2b1/tests/unit/db/setup/schema/baseline/schema.sql
+-rw-r--r--   0        0        0       24 2023-10-20 18:48:10.175796 lute3-3.3.2b1/tests/unit/db/setup/schema/migrations/123_create_B.sql
+-rw-r--r--   0        0        0       68 2023-10-20 18:48:10.176170 lute3-3.3.2b1/tests/unit/db/setup/schema/repeatable/view_A.sql
+-rw-r--r--   0        0        0     1241 2023-11-08 00:06:31.628181 lute3-3.3.2b1/tests/unit/db/setup/test_BackupManager.py
+-rw-r--r--   0        0        0     8127 2023-11-08 00:06:31.628506 lute3-3.3.2b1/tests/unit/db/setup/test_Setup.py
+-rw-r--r--   0        0        0     3681 2023-11-08 00:06:31.628800 lute3-3.3.2b1/tests/unit/db/setup/test_SqliteMigrator.py
+-rw-r--r--   0        0        0     3071 2024-04-21 08:30:46.471661 lute3-3.3.2b1/tests/unit/db/test_demo.py
+-rw-r--r--   0        0        0     1534 2023-11-11 22:05:26.100552 lute3-3.3.2b1/tests/unit/db/test_management.py
+-rw-r--r--   0        0        0        0 2024-04-21 08:30:46.471743 lute3-3.3.2b1/tests/unit/language/__init__.py
+-rw-r--r--   0        0        0     2376 2024-04-21 08:30:46.471939 lute3-3.3.2b1/tests/unit/language/test_service.py
+-rw-r--r--   0        0        0        0 2023-10-04 05:48:35.085848 lute3-3.3.2b1/tests/unit/models/__init__.py
+-rw-r--r--   0        0        0     1820 2024-03-13 16:30:50.212544 lute3-3.3.2b1/tests/unit/models/test_Book.py
+-rw-r--r--   0        0        0     3102 2024-03-15 03:25:40.916767 lute3-3.3.2b1/tests/unit/models/test_Book_add_remove_pages.py
+-rw-r--r--   0        0        0     2420 2024-04-18 00:26:46.675610 lute3-3.3.2b1/tests/unit/models/test_Language.py
+-rw-r--r--   0        0        0     6167 2024-02-19 02:42:49.368998 lute3-3.3.2b1/tests/unit/models/test_Setting.py
+-rw-r--r--   0        0        0     8034 2024-03-25 09:32:17.290517 lute3-3.3.2b1/tests/unit/models/test_Term.py
+-rw-r--r--   0        0        0     1398 2023-11-08 00:06:31.630600 lute3-3.3.2b1/tests/unit/models/test_TermTag.py
+-rw-r--r--   0        0        0      970 2024-02-07 07:50:18.820113 lute3-3.3.2b1/tests/unit/models/test_Text.py
+-rw-r--r--   0        0        0        0 2023-10-07 05:09:39.900041 lute3-3.3.2b1/tests/unit/parse/__init__.py
+-rw-r--r--   0        0        0     1806 2023-11-08 00:06:31.631135 lute3-3.3.2b1/tests/unit/parse/test_ClassicalChineseParser.py
+-rw-r--r--   0        0        0     2655 2024-03-08 03:05:01.896542 lute3-3.3.2b1/tests/unit/parse/test_JapaneseParser.py
+-rw-r--r--   0        0        0     1452 2023-11-08 00:06:31.631582 lute3-3.3.2b1/tests/unit/parse/test_SentenceGroupIterator.py
+-rw-r--r--   0        0        0     5103 2024-03-18 03:32:09.327775 lute3-3.3.2b1/tests/unit/parse/test_SpaceDelimitedParser.py
+-rw-r--r--   0        0        0      437 2023-11-08 00:06:31.632019 lute3-3.3.2b1/tests/unit/parse/test_TurkishParser.py
+-rw-r--r--   0        0        0     1343 2024-01-13 04:05:05.283548 lute3-3.3.2b1/tests/unit/parse/test_registry.py
+-rw-r--r--   0        0        0        0 2023-10-18 06:43:42.369680 lute3-3.3.2b1/tests/unit/read/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-18 06:43:42.370116 lute3-3.3.2b1/tests/unit/read/render/__init__.py
+-rw-r--r--   0        0        0     3678 2023-11-08 00:06:31.632488 lute3-3.3.2b1/tests/unit/read/render/test_RenderableCalculator.py
+-rw-r--r--   0        0        0     1965 2023-11-08 00:06:31.632694 lute3-3.3.2b1/tests/unit/read/render/test_TokenLocator.py
+-rw-r--r--   0        0        0     5991 2024-03-25 09:32:17.291177 lute3-3.3.2b1/tests/unit/read/test_service.py
+-rw-r--r--   0        0        0     3872 2024-03-25 09:32:17.292242 lute3-3.3.2b1/tests/unit/read/test_service_popup_data.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.283732 lute3-3.3.2b1/tests/unit/stats/__init__.py
+-rw-r--r--   0        0        0     2467 2024-02-07 07:50:18.821867 lute3-3.3.2b1/tests/unit/stats/test_service.py
+-rw-r--r--   0        0        0        0 2023-10-21 00:58:40.675868 lute3-3.3.2b1/tests/unit/term/__init__.py
+-rw-r--r--   0        0        0    23300 2024-03-25 09:32:17.293137 lute3-3.3.2b1/tests/unit/term/test_Repository.py
+-rw-r--r--   0        0        0     2082 2024-02-07 07:50:18.824210 lute3-3.3.2b1/tests/unit/term/test_TermForm.py
+-rw-r--r--   0        0        0     6766 2024-02-07 07:50:18.824963 lute3-3.3.2b1/tests/unit/term/test_Term_status_follow.py
+-rw-r--r--   0        0        0     1629 2024-01-13 04:05:05.285150 lute3-3.3.2b1/tests/unit/term/test_datatables.py
+-rw-r--r--   0        0        0        0 2023-10-30 23:02:04.731925 lute3-3.3.2b1/tests/unit/term_parent_map/__init__.py
+-rw-r--r--   0        0        0     1255 2024-03-15 03:25:40.918632 lute3-3.3.2b1/tests/unit/term_parent_map/test_service.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.285261 lute3-3.3.2b1/tests/unit/termtag/__init__.py
+-rw-r--r--   0        0        0      679 2023-11-08 00:06:31.633834 lute3-3.3.2b1/tests/unit/termtag/test_datatables.py
+-rw-r--r--   0        0        0        0 2024-01-13 04:05:05.285353 lute3-3.3.2b1/tests/unit/themes/__init__.py
+-rw-r--r--   0        0        0     1550 2024-03-08 03:05:01.897112 lute3-3.3.2b1/tests/unit/themes/test_service.py
+-rw-r--r--   0        0        0        0 2023-10-09 03:35:20.091806 lute3-3.3.2b1/tests/unit/utils/__init__.py
+-rw-r--r--   0        0        0     5151 2024-01-18 07:46:16.382578 lute3-3.3.2b1/tests/unit/utils/test_DataTablesSqliteQuery.py
+-rw-r--r--   0        0        0      786 2024-03-13 16:30:50.213297 lute3-3.3.2b1/tests/unit/utils/test_formutils.py
+-rw-r--r--   0        0        0     1629 2024-02-07 07:50:18.825866 lute3-3.3.2b1/tests/utils.py
+-rwxr-xr-x   0        0        0     1575 2024-02-19 02:42:49.369401 lute3-3.3.2b1/utils/dump_changelog.sh
+-rwxr-xr-x   0        0        0      565 2024-03-15 03:25:40.919140 lute3-3.3.2b1/utils/findstring.sh
+-rw-r--r--   0        0        0     4820 2023-11-22 00:36:49.803896 lute3-3.3.2b1/utils/todos.py
+-rw-r--r--   0        0        0      698 2023-11-09 08:26:12.057924 lute3-3.3.2b1/utils/verify.py
+-rw-r--r--   0        0        0     2330 1970-01-01 00:00:00.000000 lute3-3.3.2b1/PKG-INFO
```

### Comparing `lute3-3.3.1/.github/ISSUE_TEMPLATE/add_language.md` & `lute3-3.3.2b1/.github/ISSUE_TEMPLATE/add_language.md`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `lute3-3.3.2b1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/.github/ISSUE_TEMPLATE/documentation.md` & `lute3-3.3.2b1/.github/ISSUE_TEMPLATE/documentation.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 labels: ''
 assignees: ''
 
 ---
 
 **Description**
 
-Brief description of documentation edit/creation requirement for https://jzohrab.github.io/lute-manual/.
+Brief description of documentation edit/creation requirement for https://luteorg.github.io/lute-manual/.
 
 **For broken/incorrect documentation:**
 
-* specify page in https://jzohrab.github.io/lute-manual/, section, and link
+* specify page in https://luteorg.github.io/lute-manual/, section, and link
 * Take a first shot at correcting the issue.  I'll edit it for tone/consistency.
 
 **For new documentation:**
 
 * Include details about what you think is needed, e.g. your system setup etc.
 * Take a first shot at correcting the issue.  I'll edit it for tone/consistency.
 * Specify where you think it should go
```

### Comparing `lute3-3.3.1/.github/ISSUE_TEMPLATE/feature_request.md` & `lute3-3.3.2b1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/.github/workflows/ci.yml` & `lute3-3.3.2b1/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 name: ci
 
 on:
   push:
     # A branch github-ci-updates can be created and used for ci
     # experiments and tweaks.
-    branches: [ "develop", "master", "github-ci-updates", "windows" ]
+    branches: [ "develop", "master", "github-ci", "windows" ]
   pull_request:
     branches: [ "develop", "master" ]
 
 permissions:
   contents: read
 
 jobs:
@@ -32,15 +32,17 @@
         # so it can be exported before running tests.
         # Without the export, natto-py fails on github.
         # echo FIND THE LIB:
         # which mecab
         # actual=`readlink -f /usr/bin/mecab`
         # ldd $actual
 
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
+      with:
+        submodules: true
 
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python_version }}
         cache: 'pip' # caching pip dependencies
 
     - run: pip install -r requirements.txt
@@ -52,27 +54,25 @@
         echo "DATAPATH: ${{ github.workspace }}/data" >> ${{ github.workspace }}/lute/config/config.yml
         echo "DBNAME: test_lute.db" >> ${{ github.workspace }}/lute/config/config.yml
         ls ${{ github.workspace }}
         cat ${{ github.workspace }}/lute/config/config.yml
 
     - name: Test
       run: |
-        # Have to explicitly set MECAB_PATH for natto-py.
         set -e
+        # Have to explicitly set MECAB_PATH for natto-py.
         export MECAB_PATH=/lib/x86_64-linux-gnu/libmecab.so.2
         pytest
 
-    # Note that these seem to *pass* even if an acceptance
-    # test fails in GitHub actions ... which is annoying,
-    # because everything passes/fails correctly locally.
     - name: Acceptance testing
       run: |
         set -e
+        # Have to explicitly set MECAB_PATH for natto-py.
         export MECAB_PATH=/lib/x86_64-linux-gnu/libmecab.so.2
-        inv accept --headless -s
+        inv accept --show --verbose
 
     # Playwright tests were hanging far too often on github ci,
     # but not consistently.  No idea what was going wrong.
     # TODO github ci: fix playwright hanging.
     - name: Playwright install
       run: playwright install
 
@@ -89,15 +89,15 @@
     # Run one particular sanity check.
     #
     # Note this isn't _completely_ valid because the test loads
     # only supported language stories, whereas a prod release
     # comes with _all_ stories pre-loaded and the invalid ones
     # are deleted ...
     - name: Smoke test no mecab
-      run: inv accept --headless -s -k disabled_data_is_hidden
+      run: inv accept -s -k disabled_data_is_hidden
 
     - name: Check flit package
       run: |
         mkdir ${{ github.workspace }}/../lute_flit
         cd ${{ github.workspace }}/../lute_flit
         flit -f ${{ github.workspace }}/pyproject.toml install
 
@@ -119,15 +119,18 @@
 
     strategy:
       matrix:
         python_version: [ '3.11' ]
 
     steps:
 
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
+      with:
+        submodules: true
+
 
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python_version }}
         cache: 'pip' # caching pip dependencies
 
     - run: pip install -r requirements.txt
@@ -143,15 +146,18 @@
   # Test build docker container and try running.
   # Slightly wasteful re-setup of node.
   docker-build:
     runs-on: ubuntu-latest
     timeout-minutes: 30
     needs: base-ci
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
+      with:
+        submodules: true
+
     - uses: actions/setup-python@v4
       with:
         python-version: 3.11
         cache: 'pip' # caching pip dependencies
     - run: pip install -r requirements.txt
     - name: Test docker build
       run: |
@@ -173,15 +179,18 @@
 
     strategy:
       matrix:
         python_version: [ '3.8', '3.9', '3.10', '3.11' ]
 
     steps:
 
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
+      with:
+        submodules: true
+
 
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python_version }}
         cache: 'pip' # caching pip dependencies
 
     - name: Setup config
@@ -205,19 +214,19 @@
     #   run: playwright install
     # - name: Playwright smoke test
     #   run: inv playwright || exit /b
 
     # Run specific sanity check.
     # Old tests no longer run -- datatables may have timing issues on Windows tests,
     # tests were far too flaky.
-    # inv accept --headless -s -k test_unsupported_language_not_shown || exit /b
-    # inv accept --headless -s -k import_a_valid_term_file || exit /b
+    # inv accept -s -k test_unsupported_language_not_shown || exit /b
+    # inv accept -s -k import_a_valid_term_file || exit /b
     - name: Smoke tests
       run: |
-        inv accept --headless -s -k test_updating_term_status_updates_the_reading_frame || exit /b
+        inv accept -s -k test_updating_term_status_updates_the_reading_frame || exit /b
 
     - name: Remove config to force using prod config
       run: del ${{ github.workspace }}\lute\config\config.yml
       shell: cmd
 
     - name: Install prod-like flit package
       run: |
```

### Comparing `lute3-3.3.1/.github/workflows/coverage.yml` & `lute3-3.3.2b1/.github/workflows/coverage.yml`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,17 @@
         # so it can be exported before running tests.
         # Without the export, natto-py fails on github.
         # echo FIND THE LIB:
         # which mecab
         # actual=`readlink -f /usr/bin/mecab`
         # ldd $actual
 
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
+      with:
+        submodules: true
 
     - uses: actions/setup-python@v4
       with:
         python-version: '3.8'
         cache: 'pip' # caching pip dependencies
 
     - run: pip install -r requirements.txt
```

### Comparing `lute3-3.3.1/.gitignore` & `lute3-3.3.2b1/.gitignore`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/.pylintrc` & `lute3-3.3.2b1/.pylintrc`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/.pytest.ini` & `lute3-3.3.2b1/.pytest.ini`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/LICENSE.txt` & `lute3-3.3.2b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/README.md` & `lute3-3.3.2b1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 [![coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/jzohrab/a15001ec2ff889f7be0b553df9881566/raw/covbadge.json)](https://github.com/jzohrab/lute_v3/actions/workflows/ci.yml?query=branch%3Amaster)
 [![Discord Server](https://badgen.net/badge/icon/discord?icon=discord&label)](https://discord.gg/CzFUQP5m8u)
 
 
 This repo contains the source code for Lute (Learning Using Texts) v3, a Python/Flask tool for learning foreign languages through reading.
 
-To learn more about Lute v3, or to install it for your own use and study, please see the [Lute v3 manual](https://jzohrab.github.io/lute-manual/).
+To learn more about Lute v3, or to install it for your own use and study, please see the [Lute v3 manual](https://luteorg.github.io/lute-manual/).
 
-![Lute v3 demo](https://github.com/jzohrab/lute-manual/assets/1637133/7e7f5f66-20bb-4e94-a11c-7b7ffc43255a)
+![Lute v3 demo](https://luteorg.github.io/lute-manual/assets/intro.gif)
 
 # Getting Started
 
 ## Users
 
-See the [Lute v3 manual](https://jzohrab.github.io/lute-manual/).  Hop onto the [Discord](https://discord.gg/CzFUQP5m8u) too.
+See the [Lute v3 manual](https://luteorg.github.io/lute-manual/).  Hop onto the [Discord](https://discord.gg/CzFUQP5m8u) too.
 
 ## Developing
 
 For more information on building and developing, please see [Development](../../wiki/Development).
 
 ## Contributing
```

### Comparing `lute3-3.3.1/README_PyPi.md` & `lute3-3.3.2b1/README_PyPi.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # `lute3`
 
 Learning Using Texts v3.
 
-Lute is for learning foreign languages through reading.  `lute3` is a rewrite of the original Lute PHP application in Python and Flask.
-
+Lute is for learning foreign languages through reading.  `lute3` is a rewrite of the original Lute PHP application in Python and Flask.  See the [Lute manual](https://luteorg.github.io/lute-manual/) for more detail, and notes about installation.
 
 
 ## Requirements
 
 Python 3.8+ (tested with python 3.8 through 3.11)
 
 Japanese learners will also need to install MeCab.
```

### Comparing `lute3-3.3.1/devstart.py` & `lute3-3.3.2b1/devstart.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/docker/Dockerfile` & `lute3-3.3.2b1/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/docker/build_all.sh` & `lute3-3.3.2b1/docker/build_all.sh`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/docker/check_mounts_and_start.sh` & `lute3-3.3.2b1/docker/check_mounts_and_start.sh`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/docker/docker_hub_overview.md` & `lute3-3.3.2b1/docker/docker_hub_overview.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!-- Description to be copy-pasted into the "Repository overview" in hub.docker.com -->
 
 # What is Lute v3?
 
 LUTE (Learning Using Texts) is an application for learning foreign languages through reading.
 
-<img src="https://github.com/jzohrab/lute-manual/assets/1637133/7e7f5f66-20bb-4e94-a11c-7b7ffc43255a" width="700">
+<img src="https://luteorg.github.io/lute-manual/assets/intro.gif" width="700">
 
-For more information, see the [Lute manual](https://jzohrab.github.io/lute-manual/).
+For more information, see the [Lute manual](https://luteorg.github.io/lute-manual/).
 
 # How to use this image
 
 ```
 docker run -p 5000:5000 -v <MY_DATA_PATH>:/lute_data -v <MY_BACKUP_PATH>:/lute_backup jzohrab/lute3:latest
 ```
 
@@ -99,18 +99,18 @@
 `lute3` has two variants:
 
 * `lute3:<version>` (or `lute3:latest`): Lute v3 and all requirements, plus [MeCab](https://en.wikipedia.org/wiki/MeCab) and a MeCab dictionary for Japanese. ~830 MB.
 * `lute3:<version>-lean` (or `lute3:latest-lean`): The same as the above, but without MeCab (Japanese parsing and the Japanese demo are disabled). ~300 MB
 
 # Source code and building your own images
 
-Lute v3 is on [GitHub](https://github.com/jzohrab/lute-v3/).
+Lute v3 is on [GitHub](https://github.com/luteorg/lute-v3/).
 
 The Dockerfile used to build the images, and docs, are in `/docker` in that repo.
 
 # Help
 
-If you encounter any issues or have questions, please check the [GitHub Issues](https://github.com/jzohrab/lute-v3/issues) or join the [Discord](https://discord.gg/CzFUQP5m8u).
+If you encounter any issues or have questions, please check the [GitHub Issues](https://github.com/luteorg/lute-v3/issues) or join the [Discord](https://discord.gg/CzFUQP5m8u).
 
 # License
 
-Lute v3 and its Docker image are under the [MIT license](https://github.com/jzohrab/lute-v3/blob/master/LICENSE.txt).
+Lute v3 and its Docker image are under the [MIT license](https://github.com/luteorg/lute-v3/blob/master/LICENSE.txt).
```

### Comparing `lute3-3.3.1/docker/try_build_multi.sh` & `lute3-3.3.2b1/docker/try_build_multi.sh`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/docs/CHANGELOG.md` & `lute3-3.3.2b1/docs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/LICENSE.txt` & `lute3-3.3.2b1/lute/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/app_factory.py` & `lute3-3.3.2b1/lute/app_factory.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/backup/routes.py` & `lute3-3.3.2b1/lute/backup/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/backup/service.py` & `lute3-3.3.2b1/lute/backup/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/bing/routes.py` & `lute3-3.3.2b1/lute/bing/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/book/datatables.py` & `lute3-3.3.2b1/lute/book/datatables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/book/forms.py` & `lute3-3.3.2b1/lute/book/forms.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/book/routes.py` & `lute3-3.3.2b1/lute/book/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/book/service.py` & `lute3-3.3.2b1/lute/book/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/book/stats.py` & `lute3-3.3.2b1/lute/book/stats.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/cli/commands.py` & `lute3-3.3.2b1/lute/cli/commands.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/cli/language_term_export.py` & `lute3-3.3.2b1/lute/cli/language_term_export.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/config/app_config.py` & `lute3-3.3.2b1/lute/config/app_config.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/config/config.yml.example` & `lute3-3.3.2b1/lute/config/config.yml.example`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/data_cleanup.py` & `lute3-3.3.2b1/lute/db/data_cleanup.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/languages/arabic.yaml` & `lute3-3.3.2b1/lute/db/language_defs/arabic/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/languages/german.yaml` & `lute3-3.3.2b1/lute/db/language_defs/german/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/languages/greek.yaml` & `lute3-3.3.2b1/lute/db/language_defs/greek/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/languages/hindi.yaml` & `lute3-3.3.2b1/lute/db/language_defs/hindi/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/languages/japanese.yaml` & `lute3-3.3.2b1/lute/db/language_defs/japanese/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/languages/spanish.yaml` & `lute3-3.3.2b1/lute/db/language_defs/spanish/definition.yaml`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/stories/ar_demo.txt` & `lute3-3.3.2b1/lute/db/language_defs/arabic/ar_demo.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/stories/cc_demo.txt` & `lute3-3.3.2b1/lute/db/language_defs/classical_chinese/cc_demo.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/stories/czech.txt` & `lute3-3.3.2b1/lute/db/language_defs/czech/czech.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/stories/de_Stadtmusikanten.txt` & `lute3-3.3.2b1/lute/db/language_defs/german/de_Stadtmusikanten.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/stories/es_aladino.txt` & `lute3-3.3.2b1/lute/db/language_defs/spanish/es_aladino.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/stories/gr_demo.txt` & `lute3-3.3.2b1/lute/db/language_defs/greek/gr_demo.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/stories/hi_wikipedia.txt` & `lute3-3.3.2b1/lute/db/language_defs/hindi/hi_wikipedia.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/stories/ru_medved.txt` & `lute3-3.3.2b1/lute/db/language_defs/russian/ru_medved.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/stories/sanskrit.txt` & `lute3-3.3.2b1/lute/db/language_defs/sanskrit/sanskrit.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/stories/tr_demo.txt` & `lute3-3.3.2b1/lute/db/language_defs/turkish/tr_demo.txt`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/demo/stories/tutorial.txt` & `lute3-3.3.2b1/lute/db/language_defs/english/tutorial.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # title: Tutorial
-# language: English
-#
+
 Welcome to Lute!  This short guide should get you going.
 
 Navigation
 This tutorial has multiple pages.  At the top of the page is a slider to navigate forwards and backwards, or you can click the arrows at either end of the slider.
 
 1. The Basics
 All of these words are blue because they are "unknown" - according to Lute, this is the first time you're seeing these words.
 You can click on a word, and create a definition.  For example, click on this word: elephant.
 When the form pops up in the right-hand frame, a dictionary is loaded below.  Copy-paste something from the dictionary into the translation, or make up your own, mark the status, add some tags if you want (eg, type "noun" in the tags field), and click save.  From now on, every English text that you read that contains the word "elephant" will show the status.  If you hover over any "elephant", you'll see some information.
 
 1.1 Multiple dictionaries.
 Languages can have multiple dictionaries, configured in the "Languages" link on the homepage.  Each dictionary is shown as a small tab.  For this demo, English has been configured with two dictionaries.  The second dictionary will open a popup window.  If you have many dictionaries, the extra ones will be shown in a small list box next to the tabs.
 
 1.2 Images
-Lute can do a simple image search for terms.  Next to the Sentences tab is a small image button.  If you click on it, you'll see some happy elephants (if you clicked on elephant!).  If you click on one of the images shown in the list, that image is saved in your data/userimages folder.  When you hover over the word in the reading pane, that picture is included in the word hover.  Try adding an image for your elephant by clicking on the term, clicking the eye icon, and clicking a picture you like.  Then hover over your elephant.
+Lute can do a simple image search for terms.  Next to the Sentences tab is a small image button.  If you click on it, you'll see some happy elephants (if you clicked on elephant!).  If you click on one of the images shown in the list, that image is saved in your data/userimages folder.  When you hover over the word in the reading pane, that picture is included in the word hover.  Try adding an image for your elephant by clicking on the term, clicking the image icon, and clicking a picture you like.  Then hover over your elephant.
 Note: sometimes these images make _no sense_ -- it's using Bing image search, and it does the best it can with the limited context it has.
 To delete an image added to your term, click on it.  Its border will change to red.  Hit Delete or Backspace to delete it, and then save the term (you must save!).
 
 2. Multi-word Terms
 You can create multi-word terms by clicking and dragging across multiple words, then release the mouse.  Try creating a term for the phrase "the cat's pyjamas", and add a translation and set the status.
 (A brief side note: Lute keeps track of where you are in any text.  If you click the Home link above to leave this tutorial, and later click the Tutorial link from the Text listing, Lute will open the last page you were at.)
 
@@ -30,15 +29,15 @@
 
 4. Mark the remainder as "Well Known"
 When you're done creating Terms on a page, you will likely still have a bunch of blue words, or "unknowns", left over, even though you really know these words.  You can set all of these to "Well Known" and move to the next page in one shot with the green checkmark at the bottom of the page.  Try that now to see what happens, and then come back to this page using the arrows in the header to finish reading this page.
 The ">" link moves to the next page as well, without setting the unknown terms to "Well Known."  This can be useful if you're reading quickly, without stopping to define every last term in detail.
 Note: both of these links also mark the page as "Read", which Lute uses when it searches for references to terms you create.  There's more on this in the tutorial follow-up, which you should read after this tutorial.
 
 5. Keyboard shortcuts
-The small blue question mark in the header shows some keyboard shortcuts.
+The "hamburger menu" next to the Lute logo at the top right of the reading screen opens up a small menu of items, including a link to some keyboard shortcuts.  This section introduces a few of them.
 
 5.1 Updating Status
 If you've worked through the tutorial, you'll have noted that words are underlined in blue when you move the mouse over them.  You can quickly change the status of the current word by hitting 1, 2, 3, 4, 5, w (for Well-Known), or i (for Ignore).  Try hovering over the following words and hit the status buttons: apple, banana, cranberry, donut.
 If you click on a word, it's underlined in red, and the Term edit form is shown.  Before you switch over to the Term editing form, you can still update its status using the hotkeys above, or by using the up and down arrows.  You can jump over to the edit form by hitting Tab, and then start editing.
 When a word has been clicked, it's "active", so it keeps the focus.  Hovering the mouse over other words won't underline them in blue anymore, and hitting status update hotkeys (1 - 5, w, i) will only update the active word.  To "un-click" a word underlined in red, click it again, or hit Escape or Return.  Then you'll be back in "Hover mode".  In "Hover mode", the hotkeys 1-5, w, and i still update the status, but the arrow keys just scroll the window.  Try clicking and un-clicking or Escaping any word in this paragraph to get a feel for it.
 Note that for the keyboard shortcuts to work, the reading pane (where the text is) must have the "focus".  Click anywhere on the reading pane to re-establish focus.
```

### Comparing `lute3-3.3.1/lute/db/demo/stories/tutorial_follow_up.txt` & `lute3-3.3.2b1/lute/db/language_defs/english/tutorial_follow_up.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # title: Tutorial follow-up
-# language: English
-#
+
 Hopefully you've gone through the Tutorial, and created some Terms.
 From the Tutorial, you've already told Lute that you know most of the words on this page.  You can hover over words to see information about them, such as your information you might have added about dogs.
 There are still a few blue words, which according to Lute are still "unknown" to you.  You can process them like you did on the last text.
 (fyi - If a text has a spelling mikstaske, you can edit it by clicking the "hamburger menu" -- three lines -- in the top left corner of this screen, and click "Edit page".  If you'd like, correct the mistake now, and resave this text.)
 Now we'll do a brief spin through a few other things Lute does.  You can read about them and other features in the manual too.
 
 1. The Menus
```

### Comparing `lute3-3.3.1/lute/db/management.py` & `lute3-3.3.2b1/lute/db/management.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/README.md` & `lute3-3.3.2b1/lute/db/schema/README.md`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/baseline.sql` & `lute3-3.3.2b1/lute/db/schema/baseline.sql`

 * *Files 1% similar despite different names*

```diff
@@ -131,36 +131,36 @@
 	"TxBkID" INTEGER NOT NULL  ,
 	"TxOrder" INTEGER NOT NULL  ,
         "TxText" TEXT NOT NULL  ,
 	TxReadDate datetime null, TxWordCount INTEGER null,
 	PRIMARY KEY ("TxID"),
 	FOREIGN KEY("TxBkID") REFERENCES "books" ("BkID") ON UPDATE NO ACTION ON DELETE CASCADE
 );
-INSERT INTO texts VALUES(1,1,1,'V jedné rozpadlé chaloupce žil tatínek, maminka a jejich chlapec Tonda. Byli velmi chudí, do střechy jim teklo a často neměli ani na jídlo. Tonda, aby rodičům pomohl, pracoval jako pasáček ovcí. Ale i tak neměl ani na pořádné oblečení, chodil v roztrhaných kalhotách, do kabátku mu táhlo a jeho čepice vypadala stejně otrhaně jako zbytek oděvu. I přesto si každé ráno cestou na pastvu vesele pohvizdoval.',NULL,67);
-INSERT INTO texts VALUES(2,2,1,replace('काशीनगरे एकः पण्डितः अस्ति । पण्डितसमीपम् एकः शिष्यः आगच्छति । शिष्यः वदति - "आचार्य!\nविद्याभ्यासार्थम् आगतः ।" पण्डितः शिष्यबुद्धिपरीक्षार्थं पृच्छति - "वत्स, देवः कुत्र अस्ति?" शिष्यः वदति -\n''गुरो! देवः कुत्र नास्ति? कृपया भवान् एव समाधानं वदतु ।" सन्तुष्टः गुरुः वदति - "दैवः सर्वत्र अस्ति । देवः\nसर्वव्यापी । त्वं बुद्धिमान ।अतः विद्याभ्यासार्थम् अत्रैव वस।"','\n',char(10)),NULL,45);
-INSERT INTO texts VALUES(3,3,1,'北冥有魚，其名為鯤。鯤之大，不知其幾千里也。化而為鳥，其名為鵬。鵬之背，不知其幾千里也；怒而飛，其翼若垂天之雲。是鳥也，海運則將徙於南冥。南冥者，天池也。齊諧者，志怪者也。諧之言曰：「鵬之徙於南冥也，水擊三千里，摶扶搖而上者九萬里，去以六月息者也。」野馬也，塵埃也，生物之以息相吹也。天之蒼蒼，其正色邪？其遠而無所至極邪？其視下也亦若是，則已矣。且夫水之積也不厚，則負大舟也無力。覆杯水於坳堂之上，則芥為之舟，置杯焉則膠，水淺而舟大也。風之積也不厚，則其負大翼也無力。故九萬里則風斯在下矣，而後乃今培風；背負青天而莫之夭閼者，而後乃今將圖南。',NULL,228);
-INSERT INTO texts VALUES(4,3,2,'蜩與學鳩笑之曰：「我決起而飛，槍1榆、枋，時則不至而控於地而已矣，奚以之九萬里而南為？」適莽蒼者三湌而反，腹猶果然；適百里者宿舂糧；適千里者三月聚糧。之二蟲又何知！小知不及大知，小年不及大年。奚以知其然也？朝菌不知晦朔，蟪蛄不知春秋，此小年也。楚之南有冥靈者，以五百歲為春，五百歲為秋；上古有大椿者，以八千歲為春，八千歲為秋。而彭祖乃今以久特聞，眾人匹之，不亦悲乎！',NULL,154);
-INSERT INTO texts VALUES(5,4,1,replace('Érase una vez un muchacho llamado Aladino que vivía en el lejano Oriente con su madre, en una casa sencilla y humilde. Tenían lo justo para vivir, así que cada día, Aladino recorría el centro de la ciudad en busca de algún alimento que llevarse a la boca.\n\nEn una ocasión paseaba entre los puestos de fruta del mercado, cuando se cruzó con un hombre muy extraño con pinta de extranjero. Aladino se quedó sorprendido al escuchar que le llamaba por su nombre.','\n',char(10)),NULL,83);
-INSERT INTO texts VALUES(6,5,1,'Встреча с медведем может быть очень опасна. Русские люди любят ходить в лес и собирать грибы и ягоды. Они делают это с осторожностью, так как медведи тоже очень любят ягоды и могут напасть на человека. Медведь ест все: ягоды, рыбу, мясо и даже насекомых. Особенно он любит мед.',NULL,48);
-INSERT INTO texts VALUES(7,6,1,replace('Welcome to Lute! This short guide should get you going.\n\nNavigation\nThis tutorial has multiple pages. At the top of the page is a slider to navigate forwards and backwards, or you can click the arrows at either end of the slider.\n\n1. The Basics\nAll of these words are blue because they are "unknown" - according to Lute, this is the first time you''re seeing these words.\nYou can click on a word, and create a definition. For example, click on this word: elephant.\nWhen the form pops up in the right-hand frame, a dictionary is loaded below. Copy-paste something from the dictionary into the translation, or make up your own, mark the status, add some tags if you want (eg, type "noun" in the tags field), and click save. From now on, every English text that you read that contains the word "elephant" will show the status. If you hover over any "elephant", you''ll see some information.\n\n1.1 Multiple dictionaries.\nLanguages can have multiple dictionaries, configured in the "Languages" link on the homepage. Each dictionary is shown as a small tab. For this demo, English has been configured with two dictionaries. The second dictionary will open a popup window. If you have many dictionaries, the extra ones will be shown in a small list box next to the tabs.\n\n1.2 Images\nLute can do a simple image search for terms. Next to the Sentences tab is a small image button.','\n',char(10)),NULL,242);
-INSERT INTO texts VALUES(8,6,2,replace('If you click on it, you''ll see some happy elephants (if you clicked on elephant!). If you click on one of the images shown in the list, that image is saved in your data/userimages folder. When you hover over the word in the reading pane, that picture is included in the word hover. Try adding an image for your elephant by clicking on the term, clicking the eye icon, and clicking a picture you like. Then hover over your elephant.\nNote: sometimes these images make _no sense_ -- it''s using Bing image search, and it does the best it can with the limited context it has.\nTo delete an image added to your term, click on it. Its border will change to red. Hit Delete or Backspace to delete it, and then save the term (you must save!).\n\n2. Multi-word Terms\nYou can create multi-word terms by clicking and dragging across multiple words, then release the mouse. Try creating a term for the phrase "the cat''s pyjamas", and add a translation and set the status.\n(A brief side note: Lute keeps track of where you are in any text. If you click the Home link above to leave this tutorial, and later click the Tutorial link from the Text listing, Lute will open the last page you were at.)\n\n3. Parent Terms\nSometimes it helps to associate terms with a "parent".','\n',char(10)),NULL,234);
-INSERT INTO texts VALUES(9,6,3,replace('For example, the verb "to have" is conjugated in various forms as "I have a cold", "he has a dog", "they had dinner". First create a Term for "have". Then create a Term for "has", and in the Parent field start typing "have". Lute will show the existing Term "have" in the drop down, and if you select it, "has" will be associated with that on save, and when you hover over "has" you''ll see the parent''s information as well.\nIf you enter a non-existent Parent word, Lute will create a placeholder Term for that Parent, copying some content from your term. For example, try creating a Term for the word "dogs", associating it with the non-existent Term "dog". When you save "dogs", both will be updated.\nTerms can have multiple parents, too. Hit the Enter (or Return) key after each parent. For example, if you wanted to associate the Term "puppies" with both "puppy" and "dog", click on "puppies", and in the Parents text box type "puppy", hit Enter, type "dog", and hit Enter. Sometimes this is necessary: for example, in Spanish, "se sienta" can either be a conjugation of "sentirse" (to feel) or "sentarse" (to sit), depending on the context.\n\n4. Mark the remainder as "Well Known"\nWhen you''re done creating Terms on a page, you will likely still have a bunch of blue words, or "unknowns", left over, even though you really know these words.','\n',char(10)),NULL,242);
-INSERT INTO texts VALUES(10,6,4,replace('You can set all of these to "Well Known" and move to the next page in one shot with the green checkmark at the bottom of the page. Try that now to see what happens, and then come back to this page using the arrows in the header to finish reading this page.\nThe ">" link moves to the next page as well, without setting the unknown terms to "Well Known." This can be useful if you''re reading quickly, without stopping to define every last term in detail.\nNote: both of these links also mark the page as "Read", which Lute uses when it searches for references to terms you create. There''s more on this in the tutorial follow-up, which you should read after this tutorial.\n\n5. Keyboard shortcuts\nThe small blue question mark in the header shows some keyboard shortcuts.\n\n5.1 Updating Status\nIf you''ve worked through the tutorial, you''ll have noted that words are underlined in blue when you move the mouse over them. You can quickly change the status of the current word by hitting 1, 2, 3, 4, 5, w (for Well-Known), or i (for Ignore). Try hovering over the following words and hit the status buttons: apple, banana, cranberry, donut.\nIf you click on a word, it''s underlined in red, and the Term edit form is shown. Before you switch over to the Term editing form, you can still update its status using the hotkeys above, or by using the up and down arrows.','\n',char(10)),NULL,248);
-INSERT INTO texts VALUES(11,6,5,replace('You can jump over to the edit form by hitting Tab, and then start editing.\nWhen a word has been clicked, it''s "active", so it keeps the focus. Hovering the mouse over other words won''t underline them in blue anymore, and hitting status update hotkeys (1 - 5, w, i) will only update the active word. To "un-click" a word underlined in red, click it again, or hit Escape or Return. Then you''ll be back in "Hover mode". In "Hover mode", the hotkeys 1-5, w, and i still update the status, but the arrow keys just scroll the window. Try clicking and un-clicking or Escaping any word in this paragraph to get a feel for it.\nNote that for the keyboard shortcuts to work, the reading pane (where the text is) must have the "focus". Click anywhere on the reading pane to re-establish focus.\n\n5.1 Bulk updates\nIf you hold down Shift and click a bunch of words, you can bulk update their statuses. This works for the up and down arrow keys as well.\n\n5.2 Arrow keys\nThe Right and Left arrow keys click the next and previous words. Hit Escape or Return to get back to "hover mode".\n\n5.3 Copying text\nWhen a word is hovered over or clicked, hit "c" to copy that word''s sentence to your clipboard. Hit "C" to copy the word''s full paragraph (multiple sentences).','\n',char(10)),NULL,232);
-INSERT INTO texts VALUES(12,6,6,replace('You can also copy arbitrary sections of text by holding down the Shift key while highlighting the text with your mouse.\n\n6. Next steps\nAll done this text!\nLute keeps track of all of this in your database, so any time you create or import a new Book, all the info you''ve created is carried forward.\nThere''s a tutorial follow-up: go to the Home screen, and click the "Tutorial follow-up" in the table.','\n',char(10)),NULL,76);
-INSERT INTO texts VALUES(13,7,1,replace('Hopefully you''ve gone through the Tutorial, and created some Terms.\nFrom the Tutorial, you''ve already told Lute that you know most of the words on this page. You can hover over words to see information about them, such as your information you might have added about dogs.\nThere are still a few blue words, which according to Lute are still "unknown" to you. You can process them like you did on the last text.\n(fyi - If a text has a spelling mikstaske, you can edit it by clicking the "hamburger menu" -- three lines -- in the top left corner of this screen, and click "Edit page". If you''d like, correct the mistake now, and resave this text.)\nNow we''ll do a brief spin through a few other things Lute does. You can read about them and other features in the manual too.\n\n1. The Menus\nIn case you missed it, on the Home screen there are some menu bar items on the top right. Go back there and hover over them to see what you can do. This is all demo data, so you can do what you want. (But don''t delete the tutorials until you''ve gone through them.)\n\n2. Term Sentences\nIn the "Term" edit form, you can click on the "Sentences" tab to see where that term or its relations have been used. Click on "elephant", and then click the Sentences tab to see where that term has been used.','\n',char(10)),NULL,245);
-INSERT INTO texts VALUES(14,7,2,replace('You''re only shown sentences on pages that have been marked "Read", using the controls in the footer of the reading screen, i.e. the green checkmark or the ">". This ensures that you only see references that you have already seen before, so you don''t get overwhelmed with new vocabulary, and avoids spoilers of the material you''re reading.\n\n3. Archiving, Unarchiving, and Deleting Books\nWhen you''re done reading a book, you can Archive or Delete it.\nArchiving just removes the book from your book listing on the home screen, and you can unarchive at any time. The sentences for archived books are still available for searching with the Term "Sentences" link.\nOn the last page of every book, Lute shows a link for you to archive the book. You can also archive it from the Home screen by clicking on the "Archive" action (the image with the little down arrow) in the right-most column. To unarchive the text, go to Home, Book Archive, and click the "Unarchive" action (the little up arrow).\nDeleting a book completely removes it and its sentences.\nNeither archiving nor deleting touch any Terms you''ve created.\n\n4. Audio\nYou can add an audio file (mp3, wav, or ogg) to your books, so you can read along to an audio track. See the Lute manual for more notes on usage and tips.\n\n5. Themes and toggling highlighting\nLute has a few themes to make reading more pleasant.','\n',char(10)),NULL,242);
-INSERT INTO texts VALUES(15,7,3,replace('From the "hamburger menu" on the reading screen you can switch to the next theme, or hit the hotkey (m). You can also toggle highlights, because sometimes they get distracting.\n\n===\n\nThose are the the core feature of Lute! There are some sample stories for other languages. Try those out or create your own.\nWhen you''re done with the demo, go back to the Home screen and click the link to clear out the database. Lute will delete all of the demo data, and you can get started. You''ll be prompted to create your first language, and then you can create your first book. Lute will then ask you to specify your backup preferences, and with that all done, you''ll be off and running.\nThere is a Lute Discord and manual as well -- see the "About" menu bar.\nI hope that you find Lute a fun tool to use for learning languages. Cheers and best wishes!','\n',char(10)),NULL,158);
+INSERT INTO texts VALUES(1,1,1,replace('مرحبا، كيف حالك ؟\nمرحبا, أنا بخير\nهل انت جديدٌ هنا؟ لم أراك من قبل\nانا طالب جديد.لقد وصلت البارحة\nانا محمد, تشرفت بلقائك\n\nشجرة الحياة\n\nتحكي هذه القصة عن ولد صغير يُدعى «يوسف»، يعيش مع أمه الأرملة الفقيرة، يساعدها ويحنو عليها ويحبها حبًا جمًا. وفي يوم من الأيام يصيب المرض أم يوسف ويشتد عليها، ولا يعرف يوسف ماذا يفعل لإنقاذها، فلا يجد أمامه سوى اللجوء إلى الجِنِّيَّة «وِداد» التي تدله على شجرة فيها الشفاء لأمه، هذه الشجرة تقع في أعلى الجبل المقابل لمنزلهم، وعلى يوسف أن يتسلق هذا الجبل ويواجه المخاطر من أجل أن يأتي لأمه بالدواء الموجود في أوراق هذه الشجرة، فهل سينجح يوسف في ذلك؟ وماذا ينتظره من مخاطر وأهوال؟','\n',char(10)),NULL,115);
+INSERT INTO texts VALUES(2,2,1,'北冥有魚，其名為鯤。鯤之大，不知其幾千里也。化而為鳥，其名為鵬。鵬之背，不知其幾千里也；怒而飛，其翼若垂天之雲。是鳥也，海運則將徙於南冥。南冥者，天池也。齊諧者，志怪者也。諧之言曰：「鵬之徙於南冥也，水擊三千里，摶扶搖而上者九萬里，去以六月息者也。」野馬也，塵埃也，生物之以息相吹也。天之蒼蒼，其正色邪？其遠而無所至極邪？其視下也亦若是，則已矣。且夫水之積也不厚，則負大舟也無力。覆杯水於坳堂之上，則芥為之舟，置杯焉則膠，水淺而舟大也。風之積也不厚，則其負大翼也無力。故九萬里則風斯在下矣，而後乃今培風；背負青天而莫之夭閼者，而後乃今將圖南。',NULL,228);
+INSERT INTO texts VALUES(3,2,2,'蜩與學鳩笑之曰：「我決起而飛，槍1榆、枋，時則不至而控於地而已矣，奚以之九萬里而南為？」適莽蒼者三湌而反，腹猶果然；適百里者宿舂糧；適千里者三月聚糧。之二蟲又何知！小知不及大知，小年不及大年。奚以知其然也？朝菌不知晦朔，蟪蛄不知春秋，此小年也。楚之南有冥靈者，以五百歲為春，五百歲為秋；上古有大椿者，以八千歲為春，八千歲為秋。而彭祖乃今以久特聞，眾人匹之，不亦悲乎！',NULL,154);
+INSERT INTO texts VALUES(4,3,1,'V jedné rozpadlé chaloupce žil tatínek, maminka a jejich chlapec Tonda. Byli velmi chudí, do střechy jim teklo a často neměli ani na jídlo. Tonda, aby rodičům pomohl, pracoval jako pasáček ovcí. Ale i tak neměl ani na pořádné oblečení, chodil v roztrhaných kalhotách, do kabátku mu táhlo a jeho čepice vypadala stejně otrhaně jako zbytek oděvu. I přesto si každé ráno cestou na pastvu vesele pohvizdoval.',NULL,67);
+INSERT INTO texts VALUES(5,4,1,replace('Welcome to Lute! This short guide should get you going.\n\nNavigation\nThis tutorial has multiple pages. At the top of the page is a slider to navigate forwards and backwards, or you can click the arrows at either end of the slider.\n\n1. The Basics\nAll of these words are blue because they are "unknown" - according to Lute, this is the first time you''re seeing these words.\nYou can click on a word, and create a definition. For example, click on this word: elephant.\nWhen the form pops up in the right-hand frame, a dictionary is loaded below. Copy-paste something from the dictionary into the translation, or make up your own, mark the status, add some tags if you want (eg, type "noun" in the tags field), and click save. From now on, every English text that you read that contains the word "elephant" will show the status. If you hover over any "elephant", you''ll see some information.\n\n1.1 Multiple dictionaries.\nLanguages can have multiple dictionaries, configured in the "Languages" link on the homepage. Each dictionary is shown as a small tab. For this demo, English has been configured with two dictionaries. The second dictionary will open a popup window. If you have many dictionaries, the extra ones will be shown in a small list box next to the tabs.\n\n1.2 Images\nLute can do a simple image search for terms. Next to the Sentences tab is a small image button.','\n',char(10)),NULL,242);
+INSERT INTO texts VALUES(6,4,2,replace('If you click on it, you''ll see some happy elephants (if you clicked on elephant!). If you click on one of the images shown in the list, that image is saved in your data/userimages folder. When you hover over the word in the reading pane, that picture is included in the word hover. Try adding an image for your elephant by clicking on the term, clicking the image icon, and clicking a picture you like. Then hover over your elephant.\nNote: sometimes these images make _no sense_ -- it''s using Bing image search, and it does the best it can with the limited context it has.\nTo delete an image added to your term, click on it. Its border will change to red. Hit Delete or Backspace to delete it, and then save the term (you must save!).\n\n2. Multi-word Terms\nYou can create multi-word terms by clicking and dragging across multiple words, then release the mouse. Try creating a term for the phrase "the cat''s pyjamas", and add a translation and set the status.\n(A brief side note: Lute keeps track of where you are in any text. If you click the Home link above to leave this tutorial, and later click the Tutorial link from the Text listing, Lute will open the last page you were at.)\n\n3. Parent Terms\nSometimes it helps to associate terms with a "parent".','\n',char(10)),NULL,234);
+INSERT INTO texts VALUES(7,4,3,replace('For example, the verb "to have" is conjugated in various forms as "I have a cold", "he has a dog", "they had dinner". First create a Term for "have". Then create a Term for "has", and in the Parent field start typing "have". Lute will show the existing Term "have" in the drop down, and if you select it, "has" will be associated with that on save, and when you hover over "has" you''ll see the parent''s information as well.\nIf you enter a non-existent Parent word, Lute will create a placeholder Term for that Parent, copying some content from your term. For example, try creating a Term for the word "dogs", associating it with the non-existent Term "dog". When you save "dogs", both will be updated.\nTerms can have multiple parents, too. Hit the Enter (or Return) key after each parent. For example, if you wanted to associate the Term "puppies" with both "puppy" and "dog", click on "puppies", and in the Parents text box type "puppy", hit Enter, type "dog", and hit Enter. Sometimes this is necessary: for example, in Spanish, "se sienta" can either be a conjugation of "sentirse" (to feel) or "sentarse" (to sit), depending on the context.\n\n4. Mark the remainder as "Well Known"\nWhen you''re done creating Terms on a page, you will likely still have a bunch of blue words, or "unknowns", left over, even though you really know these words.','\n',char(10)),NULL,242);
+INSERT INTO texts VALUES(8,4,4,replace('You can set all of these to "Well Known" and move to the next page in one shot with the green checkmark at the bottom of the page. Try that now to see what happens, and then come back to this page using the arrows in the header to finish reading this page.\nThe ">" link moves to the next page as well, without setting the unknown terms to "Well Known." This can be useful if you''re reading quickly, without stopping to define every last term in detail.\nNote: both of these links also mark the page as "Read", which Lute uses when it searches for references to terms you create. There''s more on this in the tutorial follow-up, which you should read after this tutorial.\n\n5. Keyboard shortcuts\nThe "hamburger menu" next to the Lute logo at the top right of the reading screen opens up a small menu of items, including a link to some keyboard shortcuts. This section introduces a few of them.\n\n5.1 Updating Status\nIf you''ve worked through the tutorial, you''ll have noted that words are underlined in blue when you move the mouse over them. You can quickly change the status of the current word by hitting 1, 2, 3, 4, 5, w (for Well-Known), or i (for Ignore). Try hovering over the following words and hit the status buttons: apple, banana, cranberry, donut.\nIf you click on a word, it''s underlined in red, and the Term edit form is shown.','\n',char(10)),NULL,246);
+INSERT INTO texts VALUES(9,4,5,replace('Before you switch over to the Term editing form, you can still update its status using the hotkeys above, or by using the up and down arrows. You can jump over to the edit form by hitting Tab, and then start editing.\nWhen a word has been clicked, it''s "active", so it keeps the focus. Hovering the mouse over other words won''t underline them in blue anymore, and hitting status update hotkeys (1 - 5, w, i) will only update the active word. To "un-click" a word underlined in red, click it again, or hit Escape or Return. Then you''ll be back in "Hover mode". In "Hover mode", the hotkeys 1-5, w, and i still update the status, but the arrow keys just scroll the window. Try clicking and un-clicking or Escaping any word in this paragraph to get a feel for it.\nNote that for the keyboard shortcuts to work, the reading pane (where the text is) must have the "focus". Click anywhere on the reading pane to re-establish focus.\n\n5.1 Bulk updates\nIf you hold down Shift and click a bunch of words, you can bulk update their statuses. This works for the up and down arrow keys as well.\n\n5.2 Arrow keys\nThe Right and Left arrow keys click the next and previous words. Hit Escape or Return to get back to "hover mode".\n\n5.3 Copying text\nWhen a word is hovered over or clicked, hit "c" to copy that word''s sentence to your clipboard.','\n',char(10)),NULL,248);
+INSERT INTO texts VALUES(10,4,6,replace('Hit "C" to copy the word''s full paragraph (multiple sentences). You can also copy arbitrary sections of text by holding down the Shift key while highlighting the text with your mouse.\n\n6. Next steps\nAll done this text!\nLute keeps track of all of this in your database, so any time you create or import a new Book, all the info you''ve created is carried forward.\nThere''s a tutorial follow-up: go to the Home screen, and click the "Tutorial follow-up" in the table.','\n',char(10)),NULL,87);
+INSERT INTO texts VALUES(11,5,1,replace('Hopefully you''ve gone through the Tutorial, and created some Terms.\nFrom the Tutorial, you''ve already told Lute that you know most of the words on this page. You can hover over words to see information about them, such as your information you might have added about dogs.\nThere are still a few blue words, which according to Lute are still "unknown" to you. You can process them like you did on the last text.\n(fyi - If a text has a spelling mikstaske, you can edit it by clicking the "hamburger menu" -- three lines -- in the top left corner of this screen, and click "Edit page". If you''d like, correct the mistake now, and resave this text.)\nNow we''ll do a brief spin through a few other things Lute does. You can read about them and other features in the manual too.\n\n1. The Menus\nIn case you missed it, on the Home screen there are some menu bar items on the top right. Go back there and hover over them to see what you can do. This is all demo data, so you can do what you want. (But don''t delete the tutorials until you''ve gone through them.)\n\n2. Term Sentences\nIn the "Term" edit form, you can click on the "Sentences" tab to see where that term or its relations have been used. Click on "elephant", and then click the Sentences tab to see where that term has been used.','\n',char(10)),NULL,245);
+INSERT INTO texts VALUES(12,5,2,replace('You''re only shown sentences on pages that have been marked "Read", using the controls in the footer of the reading screen, i.e. the green checkmark or the ">". This ensures that you only see references that you have already seen before, so you don''t get overwhelmed with new vocabulary, and avoids spoilers of the material you''re reading.\n\n3. Archiving, Unarchiving, and Deleting Books\nWhen you''re done reading a book, you can Archive or Delete it.\nArchiving just removes the book from your book listing on the home screen, and you can unarchive at any time. The sentences for archived books are still available for searching with the Term "Sentences" link.\nOn the last page of every book, Lute shows a link for you to archive the book. You can also archive it from the Home screen by clicking on the "Archive" action (the image with the little down arrow) in the right-most column. To unarchive the text, go to Home, Book Archive, and click the "Unarchive" action (the little up arrow).\nDeleting a book completely removes it and its sentences.\nNeither archiving nor deleting touch any Terms you''ve created.\n\n4. Audio\nYou can add an audio file (mp3, wav, or ogg) to your books, so you can read along to an audio track. See the Lute manual for more notes on usage and tips.\n\n5. Themes and toggling highlighting\nLute has a few themes to make reading more pleasant.','\n',char(10)),NULL,242);
+INSERT INTO texts VALUES(13,5,3,replace('From the "hamburger menu" on the reading screen you can switch to the next theme, or hit the hotkey (m). You can also toggle highlights, because sometimes they get distracting.\n\n===\n\nThose are the the core feature of Lute! There are some sample stories for other languages. Try those out or create your own.\nWhen you''re done with the demo, go back to the Home screen and click the link to clear out the database. Lute will delete all of the demo data, and you can get started. You''ll be prompted to create your first language, and then you can create your first book. Lute will then ask you to specify your backup preferences, and with that all done, you''ll be off and running.\nThere is a Lute Discord and manual as well -- see the "About" menu bar.\nI hope that you find Lute a fun tool to use for learning languages. Cheers and best wishes!','\n',char(10)),NULL,158);
+INSERT INTO texts VALUES(14,6,1,replace('Il était une fois trois ours: un papa ours, une maman ours et un bébé ours. Ils habitaient tous ensemble dans une maison jaune au milieu d''une grande forêt.\n\nUn jour, Maman Ours prépara une grande marmite de porridge délicieux et fumant pour le petit déjeuner. Il était trop chaud pour pouvoir être mangé, alors les ours décidèrent d''aller se promener en attendant que le porridge refroidisse.','\n',char(10)),NULL,69);
+INSERT INTO texts VALUES(15,7,1,replace('Es hatte ein Mann einen Esel, der schon lange Jahre die Säcke unverdrossen zur Mühle getragen hatte, dessen Kräfte aber nun zu Ende gingen, sodass er zur Arbeit immer untauglicher wurde. Da dachte der Herr daran, ihn aus dem Futter zu schaffen, aber der Esel merkte, dass kein guter Wind wehte, lief fort und machte sich auf den Weg nach Bremen; dort, meinte er, könnte er ja Stadtmusikant werden.\n\nAls er ein Weilchen fortgegangen war, fand er einen Jagdhund auf dem Weg liegen, der japste wie einer, der sich müde gelaufen hat. "Nun, was japst du so, Packan?" fragte der Esel. "Ach," sagte der Hund, "weil ich alt bin und jeden Tag schwächer werde, auch auf der Jagd nicht mehr fort kann, hat mich mein Herr wollen totschlagen, da hab ich Reißaus genommen; aber womit soll ich nun mein Brot verdienen?" - "Weißt du was?" sprach der Esel, "ich gehe nach Bremen und werde dort Stadtmusikant, geh mit und lass dich auch bei der Musik annehmen. Ich spiele die Laute, und du schlägst die Pauken.','\n',char(10)),NULL,174);
 INSERT INTO texts VALUES(16,8,1,replace('Πέτρος: Γεια σου, Νίκη. Ο Πέτρος είμαι.\nΝίκη: Α, γεια σου Πέτρο. Τι κάνεις;\nΠέτρος: Μια χαρά. Σε παίρνω για να πάμε καμιά βόλτα αργότερα. Τι λες;\nΝίκη: Α, ωραία. Κι εγώ θέλω να βγω λίγο. Συνέχεια διαβάζω για τις εξετάσεις… κουράστηκα πια. Πού λες να πάμε;\nΠέτρος: Στη γνωστή καφετέρια στην πλατεία. Θα είναι και άλλα παιδιά από την τάξη μας εκεί.\nΝίκη: Ναι; Ποιοι θα είναι;\nΠέτρος: Ο Γιάννης, ο Αντρέας και η Ελπίδα.\nΝίκη: Ωραία. Θα πάτε και πουθενά αλλού μετά;\nΠέτρος: Ναι, λέμε να πάμε στον κινηματογράφο που είναι κοντά στην καφετέρια. Παίζει μια κωμωδία.\nΝίκη: Α, δεν μπορώ να καθίσω έξω μέχρι τόσο αργά. Πρέπει να γυρίσω σπίτι για να διαβάσω.\nΠέτρος: Έλα τώρα. Διαβάζεις αύριο…\nΝίκη: Όχι, όχι, αδύνατον. Είμαι πολύ πίσω στο διάβασμά μου.\nΠέτρος: Καλά, έλα μόνο στην καφετέρια τότε. Θα περάσω να σε πάρω γύρω στις έξι να πάμε μαζί. Εντάξει;\nΝίκη: Εντάξει. Γεια.\nΠέτρο: Τα λέμε. Γεια.','\n',char(10)),NULL,157);
-INSERT INTO texts VALUES(17,9,1,replace('مرحبا، كيف حالك ؟\nمرحبا, أنا بخير\nهل انت جديدٌ هنا؟ لم أراك من قبل\nانا طالب جديد.لقد وصلت البارحة\nانا محمد, تشرفت بلقائك\n\nشجرة الحياة\n\nتحكي هذه القصة عن ولد صغير يُدعى «يوسف»، يعيش مع أمه الأرملة الفقيرة، يساعدها ويحنو عليها ويحبها حبًا جمًا. وفي يوم من الأيام يصيب المرض أم يوسف ويشتد عليها، ولا يعرف يوسف ماذا يفعل لإنقاذها، فلا يجد أمامه سوى اللجوء إلى الجِنِّيَّة «وِداد» التي تدله على شجرة فيها الشفاء لأمه، هذه الشجرة تقع في أعلى الجبل المقابل لمنزلهم، وعلى يوسف أن يتسلق هذا الجبل ويواجه المخاطر من أجل أن يأتي لأمه بالدواء الموجود في أوراق هذه الشجرة، فهل سينجح يوسف في ذلك؟ وماذا ينتظره من مخاطر وأهوال؟','\n',char(10)),NULL,115);
-INSERT INTO texts VALUES(18,10,1,replace('Büyük ağaç eskiden aşılanmış ve her yıl güzel, iri, pembe şeftaliler verirmiş, insanın eline sığmazmış bu şeftaliler. Öyle güzelmişler ki insan yemeye kıyamazmış onları. Bahçıvan, bu büyük ağacı yabancı bir uzmanın kendi ülkesinden getirdiği bir tohumla aşıladığını söylermiş. Belli ki böyle masraf edilen bir ağaçta yetişen şeftaliler oldukça değerliymiş.\n\nİki ağacın da gövdelerine nazar değmesin diye birer nazarlık asılıymış.\n\nAğaçlardan küçük olanında her yıl bin tane çiçek açarmış ama bir tek şeftali bile yetişmezmiş üzerinde. Ya çiçekleri dökülürmüş, ya da ham şeftaliler kuruyup dallardan düşermiş. Bahçıvan küçük ağaç için elinden geleni yapmış ama değişen bir şey olmamış. Yıllar geçtikçe dalları ve yaprakları çoğalmış ama bir tek şeftali bile görünmemiş üzerinde.','\n',char(10)),NULL,110);
-INSERT INTO texts VALUES(19,11,1,replace('Es hatte ein Mann einen Esel, der schon lange Jahre die Säcke unverdrossen zur Mühle getragen hatte, dessen Kräfte aber nun zu Ende gingen, sodass er zur Arbeit immer untauglicher wurde. Da dachte der Herr daran, ihn aus dem Futter zu schaffen, aber der Esel merkte, dass kein guter Wind wehte, lief fort und machte sich auf den Weg nach Bremen; dort, meinte er, könnte er ja Stadtmusikant werden.\n\nAls er ein Weilchen fortgegangen war, fand er einen Jagdhund auf dem Weg liegen, der japste wie einer, der sich müde gelaufen hat. "Nun, was japst du so, Packan?" fragte der Esel. "Ach," sagte der Hund, "weil ich alt bin und jeden Tag schwächer werde, auch auf der Jagd nicht mehr fort kann, hat mich mein Herr wollen totschlagen, da hab ich Reißaus genommen; aber womit soll ich nun mein Brot verdienen?" - "Weißt du was?" sprach der Esel, "ich gehe nach Bremen und werde dort Stadtmusikant, geh mit und lass dich auch bei der Musik annehmen. Ich spiele die Laute, und du schlägst die Pauken.','\n',char(10)),NULL,174);
-INSERT INTO texts VALUES(20,12,1,replace('Il était une fois trois ours: un papa ours, une maman ours et un bébé ours. Ils habitaient tous ensemble dans une maison jaune au milieu d''une grande forêt.\n\nUn jour, Maman Ours prépara une grande marmite de porridge délicieux et fumant pour le petit déjeuner. Il était trop chaud pour pouvoir être mangé, alors les ours décidèrent d''aller se promener en attendant que le porridge refroidisse.','\n',char(10)),NULL,69);
-INSERT INTO texts VALUES(21,13,1,replace('北風と太陽\n\n「おれの方が強い。」「いいや、ぼくの方が強い。」\n北風と太陽の声が聞こえます。二人はどちらの力が強いかでケンカをしているようです。\n「太陽が毎日元気だから、暑くてみんな困っているよ。おれが涼しい風を吹くと、みんな嬉しそうだ。」','\n',char(10)),NULL,64);
-INSERT INTO texts VALUES(22,14,1,'अनुच्छेद १(एक): सभी मनुष्य जन्म से स्वतन्त्र तथा मर्यादा और अधिकारों में समान होते हैं। वे तर्क और विवेक से सम्पन्न हैं तथा उन्हें भ्रातृत्व की भावना से परस्पर के प्रति कार्य करना चाहिए।',NULL,35);
+INSERT INTO texts VALUES(17,9,1,'अनुच्छेद १(एक): सभी मनुष्य जन्म से स्वतन्त्र तथा मर्यादा और अधिकारों में समान होते हैं। वे तर्क और विवेक से सम्पन्न हैं तथा उन्हें भ्रातृत्व की भावना से परस्पर के प्रति कार्य करना चाहिए।',NULL,35);
+INSERT INTO texts VALUES(18,10,1,replace('北風と太陽\n\n「おれの方が強い。」「いいや、ぼくの方が強い。」\n北風と太陽の声が聞こえます。二人はどちらの力が強いかでケンカをしているようです。\n「太陽が毎日元気だから、暑くてみんな困っているよ。おれが涼しい風を吹くと、みんな嬉しそうだ。」','\n',char(10)),NULL,64);
+INSERT INTO texts VALUES(19,11,1,'Встреча с медведем может быть очень опасна. Русские люди любят ходить в лес и собирать грибы и ягоды. Они делают это с осторожностью, так как медведи тоже очень любят ягоды и могут напасть на человека. Медведь ест все: ягоды, рыбу, мясо и даже насекомых. Особенно он любит мед.',NULL,48);
+INSERT INTO texts VALUES(20,12,1,replace('काशीनगरे एकः पण्डितः अस्ति । पण्डितसमीपम् एकः शिष्यः आगच्छति । शिष्यः वदति - "आचार्य!\nविद्याभ्यासार्थम् आगतः ।" पण्डितः शिष्यबुद्धिपरीक्षार्थं पृच्छति - "वत्स, देवः कुत्र अस्ति?" शिष्यः वदति -\n''गुरो! देवः कुत्र नास्ति? कृपया भवान् एव समाधानं वदतु ।" सन्तुष्टः गुरुः वदति - "दैवः सर्वत्र अस्ति । देवः\nसर्वव्यापी । त्वं बुद्धिमान ।अतः विद्याभ्यासार्थम् अत्रैव वस।"','\n',char(10)),NULL,45);
+INSERT INTO texts VALUES(21,13,1,replace('Érase una vez un muchacho llamado Aladino que vivía en el lejano Oriente con su madre, en una casa sencilla y humilde. Tenían lo justo para vivir, así que cada día, Aladino recorría el centro de la ciudad en busca de algún alimento que llevarse a la boca.\n\nEn una ocasión paseaba entre los puestos de fruta del mercado, cuando se cruzó con un hombre muy extraño con pinta de extranjero. Aladino se quedó sorprendido al escuchar que le llamaba por su nombre.','\n',char(10)),NULL,83);
+INSERT INTO texts VALUES(22,14,1,replace('Büyük ağaç eskiden aşılanmış ve her yıl güzel, iri, pembe şeftaliler verirmiş, insanın eline sığmazmış bu şeftaliler. Öyle güzelmişler ki insan yemeye kıyamazmış onları. Bahçıvan, bu büyük ağacı yabancı bir uzmanın kendi ülkesinden getirdiği bir tohumla aşıladığını söylermiş. Belli ki böyle masraf edilen bir ağaçta yetişen şeftaliler oldukça değerliymiş.\n\nİki ağacın da gövdelerine nazar değmesin diye birer nazarlık asılıymış.\n\nAğaçlardan küçük olanında her yıl bin tane çiçek açarmış ama bir tek şeftali bile yetişmezmiş üzerinde. Ya çiçekleri dökülürmüş, ya da ham şeftaliler kuruyup dallardan düşermiş. Bahçıvan küçük ağaç için elinden geleni yapmış ama değişen bir şey olmamış. Yıllar geçtikçe dalları ve yaprakları çoğalmış ama bir tek şeftali bile görünmemiş üzerinde.','\n',char(10)),NULL,110);
 CREATE TABLE IF NOT EXISTS "settings" (
 	"StKey" VARCHAR(40) NOT NULL,
         "StKeyType" TEXT NOT NULL,
 	"StValue" TEXT NULL,
 	PRIMARY KEY ("StKey")
 );
 INSERT INTO settings VALUES('IsDemoData','system','1');
@@ -173,51 +173,51 @@
 	"BkCurrentTxID" INTEGER NOT NULL DEFAULT '0',
         BkAudioFilename TEXT NULL,
         BkAudioCurrentPos REAL NULL,
         BkAudioBookmarks TEXT NULL,
 	PRIMARY KEY ("BkID"),
 	FOREIGN KEY("BkLgID") REFERENCES "languages" ("LgID") ON UPDATE NO ACTION ON DELETE CASCADE
 );
-INSERT INTO books VALUES(1,3,'Hrad Cimburk – Jak vzal vítr pasáčkovi čepici',NULL,0,0,NULL,NULL,NULL);
-INSERT INTO books VALUES(2,11,'बुद्धिमान् शिष्यः',NULL,0,0,NULL,NULL,NULL);
-INSERT INTO books VALUES(3,2,'逍遙遊',NULL,0,0,NULL,NULL,NULL);
-INSERT INTO books VALUES(4,12,'Aladino y la lámpara maravillosa',NULL,0,0,NULL,NULL,NULL);
-INSERT INTO books VALUES(5,10,'медведь',NULL,0,0,NULL,NULL,NULL);
-INSERT INTO books VALUES(6,4,'Tutorial',NULL,0,0,NULL,NULL,NULL);
-INSERT INTO books VALUES(7,4,'Tutorial follow-up',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(1,1,'Examples',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(2,2,'逍遙遊',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(3,3,'Hrad Cimburk – Jak vzal vítr pasáčkovi čepici',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(4,4,'Tutorial',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(5,4,'Tutorial follow-up',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(6,5,'Boucles d’or et les trois ours',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(7,6,'Die Bremer Stadtmusikanten',NULL,0,0,NULL,NULL,NULL);
 INSERT INTO books VALUES(8,7,'Γεια σου, Νίκη. Ο Πέτρος είμαι.',NULL,0,0,NULL,NULL,NULL);
-INSERT INTO books VALUES(9,1,'Examples',NULL,0,0,NULL,NULL,NULL);
-INSERT INTO books VALUES(10,13,'Büyük ağaç',NULL,0,0,NULL,NULL,NULL);
-INSERT INTO books VALUES(11,6,'Die Bremer Stadtmusikanten',NULL,0,0,NULL,NULL,NULL);
-INSERT INTO books VALUES(12,5,'Boucles d’or et les trois ours',NULL,0,0,NULL,NULL,NULL);
-INSERT INTO books VALUES(13,9,'北風と太陽 - きたかぜたいよう',NULL,0,0,NULL,NULL,NULL);
-INSERT INTO books VALUES(14,8,'Universal Declaration of Human Rights',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(9,8,'Universal Declaration of Human Rights',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(10,9,'北風と太陽 - きたかぜたいよう',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(11,10,'медведь',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(12,11,'बुद्धिमान् शिष्यः',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(13,12,'Aladino y la lámpara maravillosa',NULL,0,0,NULL,NULL,NULL);
+INSERT INTO books VALUES(14,13,'Büyük ağaç',NULL,0,0,NULL,NULL,NULL);
 CREATE TABLE IF NOT EXISTS "bookstats" (
 	"BkID" INTEGER NOT NULL  ,
 	"distinctterms" INTEGER NULL  ,
 	"distinctunknowns" INTEGER NULL  ,
 	"unknownpercent" INTEGER NULL  ,
         status_distribution VARCHAR(100) NULL,
 	PRIMARY KEY ("BkID"),
 	FOREIGN KEY("BkID") REFERENCES "books" ("BkID") ON UPDATE NO ACTION ON DELETE CASCADE
 );
-INSERT INTO bookstats VALUES(1,57,57,100,'{"0": 57, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
-INSERT INTO bookstats VALUES(2,33,33,100,'{"0": 33, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
-INSERT INTO bookstats VALUES(3,170,170,100,'{"0": 170, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
-INSERT INTO bookstats VALUES(4,63,63,100,'{"0": 63, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
-INSERT INTO bookstats VALUES(5,40,40,100,'{"0": 40, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
-INSERT INTO bookstats VALUES(6,355,355,100,'{"0": 355, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
-INSERT INTO bookstats VALUES(7,247,247,100,'{"0": 247, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(1,100,100,100,'{"0": 100, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(2,170,170,100,'{"0": 170, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(3,57,57,100,'{"0": 57, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(4,361,361,100,'{"0": 361, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(5,247,247,100,'{"0": 247, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(6,49,49,100,'{"0": 49, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(7,120,120,100,'{"0": 120, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
 INSERT INTO bookstats VALUES(8,99,99,100,'{"0": 99, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
-INSERT INTO bookstats VALUES(9,100,100,100,'{"0": 100, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
-INSERT INTO bookstats VALUES(10,85,85,100,'{"0": 85, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
-INSERT INTO bookstats VALUES(11,120,120,100,'{"0": 120, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
-INSERT INTO bookstats VALUES(12,49,49,100,'{"0": 49, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
-INSERT INTO bookstats VALUES(13,41,41,100,'{"0": 41, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
-INSERT INTO bookstats VALUES(14,30,30,100,'{"0": 30, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(9,30,30,100,'{"0": 30, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(10,41,41,100,'{"0": 41, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(11,40,40,100,'{"0": 40, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(12,33,33,100,'{"0": 33, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(13,63,63,100,'{"0": 63, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
+INSERT INTO bookstats VALUES(14,85,85,100,'{"0": 85, "1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "98": 0, "99": 0}');
 CREATE TABLE languagedicts (
   "LdID" INTEGER NOT NULL,
   "LdLgID" INTEGER NOT NULL,
   "LdUseFor" VARCHAR(20) NOT NULL,
   "LdType" VARCHAR(20) NOT NULL,
   "LdDictURI" VARCHAR(200) NOT NULL,
   "LdIsActive" TINYINT NOT NULL DEFAULT 1,
```

### Comparing `lute3-3.3.1/lute/db/schema/empty.sql` & `lute3-3.3.2b1/lute/db/schema/empty.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230518_190000_remove_old_words_fields.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230518_190000_remove_old_words_fields.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230519_194627_add_TxDateRead.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230519_194627_add_TxDateRead.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_01_booktags.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_01_booktags.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_02_wordtags.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_02_wordtags.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_03_sentences.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_03_sentences.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_04_texttokens.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_04_texttokens.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_05_texts.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_05_texts.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_06_bookstats.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_06_bookstats.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_07_termimages.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_07_termimages.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_08_wordflashmessages.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_08_wordflashmessages.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_09_wordparents.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_09_wordparents.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_10_words.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_10_words.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230621_224416_fk_11_books.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230621_224416_fk_11_books.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230818_201200_add_BkWordCount.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230818_201200_add_BkWordCount.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20230827_052154_allow_multiple_word_parents.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20230827_052154_allow_multiple_word_parents.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20231018_211236_remove_excess_texts_fields.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20231018_211236_remove_excess_texts_fields.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20231101_203811_modify_settings_schema.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20231101_203811_modify_settings_schema.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20240125_drop_BkWordCount.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20240125_drop_BkWordCount.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20240125_drop_bookstats_wordcount.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20240125_drop_bookstats_wordcount.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20240207_01_create_languagedicts.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20240207_01_create_languagedicts.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations/20240207_02_drop_old_language_fields.sql` & `lute3-3.3.2b1/lute/db/schema/migrations/20240207_02_drop_old_language_fields.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations_repeatable/trig_wordparents.sql` & `lute3-3.3.2b1/lute/db/schema/migrations_repeatable/trig_wordparents.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/schema/migrations_repeatable/trig_words.sql` & `lute3-3.3.2b1/lute/db/schema/migrations_repeatable/trig_words.sql`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/setup/main.py` & `lute3-3.3.2b1/lute/db/setup/main.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/db/setup/migrator.py` & `lute3-3.3.2b1/lute/db/setup/migrator.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/dev_api/routes.py` & `lute3-3.3.2b1/lute/dev_api/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/language/forms.py` & `lute3-3.3.2b1/lute/language/forms.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/language/routes.py` & `lute3-3.3.2b1/lute/language/routes.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from sqlalchemy import func
 from sqlalchemy.exc import IntegrityError
 from flask import Blueprint, current_app, render_template, redirect, url_for, flash
 from lute.models.language import Language
 from lute.models.setting import UserSetting
 from lute.models.book import Book
 from lute.models.term import Term
+import lute.language.service
 from lute.language.forms import LanguageForm
 from lute.db import db
-from lute.db.demo import predefined_languages
 from lute.parse.registry import supported_parsers
 
 bp = Blueprint("language", __name__, url_prefix="/language")
 
 
 @bp.route("/index")
 def index():
@@ -126,15 +126,15 @@
 
 @bp.route("/new", defaults={"langname": None}, methods=["GET", "POST"])
 @bp.route("/new/<string:langname>", methods=["GET", "POST"])
 def new(langname):
     """
     Create a new language.
     """
-    predefined = predefined_languages()
+    predefined = lute.language.service.predefined_languages()
     language = Language()
     if langname is not None:
         candidates = [lang for lang in predefined if lang.name == langname]
         if len(candidates) == 1:
             language = candidates[0]
 
     form = LanguageForm(obj=language)
@@ -166,7 +166,27 @@
     Delete a language.
     """
     language = db.session.get(Language, langid)
     if not language:
         flash(f"Language {langid} not found")
     Language.delete(language)
     return redirect(url_for("language.index"))
+
+
+@bp.route("/list_predefined", methods=["GET"])
+def list_predefined():
+    "Show predefined languages that are not already in the db."
+    predefined = lute.language.service.predefined_languages()
+    existing_langs = db.session.query(Language).all()
+    existing_names = [l.name for l in existing_langs]
+    new_langs = [p for p in predefined if p.name not in existing_names]
+    return render_template("language/list_predefined.html", predefined=new_langs)
+
+
+@bp.route("/load_predefined/<langname>", methods=["GET"])
+def load_predefined(langname):
+    "Load a predefined language and its stories."
+    lang_id = lute.language.service.load_language_def(langname)
+    UserSetting.set_value("current_language_id", lang_id)
+    db.session.commit()
+    flash(f"Loaded {langname} and sample book(s)")
+    return redirect("/")
```

### Comparing `lute3-3.3.1/lute/main.py` & `lute3-3.3.2b1/lute/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,8 +112,9 @@
         _start(parser.parse_args())
     except Exception as e:  # pylint: disable=broad-exception-caught
         print("\n")
         print("-" * 50)
         print("Error during startup:")
         print(e)
         print("Please try again, or report an issue on GitHub.")
+        print("Additionally, help is available with --help.")
         print("-" * 50)
```

### Comparing `lute3-3.3.1/lute/models/book.py` & `lute3-3.3.2b1/lute/models/book.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/models/language.py` & `lute3-3.3.2b1/lute/models/language.py`

 * *Files 25% similar despite different names*

```diff
@@ -175,7 +175,86 @@
     def find_by_name(name):
         "Get by name."
         return (
             db.session.query(Language)
             .filter(func.lower(Language.name) == func.lower(name))
             .first()
         )
+
+    def to_dict(self):
+        "Return dictionary of data, for serialization."
+        ret = {}
+        ret["name"] = self.name
+        ret["dictionaries"] = []
+        for d in self.dictionaries:
+            dd = {}
+            dd["for"] = d.usefor
+            dd["type"] = d.dicttype.replace("html", "")
+            dd["url"] = d.dicturi
+            dd["active"] = d.is_active
+            ret["dictionaries"].append(dd)
+        ret["show_romanization"] = self.show_romanization
+        ret["right_to_left"] = self.right_to_left
+        ret["parser_type"] = self.parser_type
+        ret["character_substitutions"] = self.character_substitutions
+        ret["split_sentences"] = self.regexp_split_sentences
+        ret["split_sentence_exceptions"] = self.exceptions_split_sentences
+        ret["word_chars"] = self.word_characters
+        return ret
+
+    @staticmethod
+    def from_dict(d):
+        "Create new Language from dictionary d."
+
+        lang = Language()
+
+        def load(key, method):
+            if key in d:
+                val = d[key]
+                # Handle boolean values
+                if isinstance(val, str):
+                    temp = val.lower()
+                    if temp == "true":
+                        val = True
+                    elif temp == "false":
+                        val = False
+                setattr(lang, method, val)
+
+        # Define mappings for fields
+        mappings = {
+            "name": "name",
+            "show_romanization": "show_romanization",
+            "right_to_left": "right_to_left",
+            "parser_type": "parser_type",
+            "character_substitutions": "character_substitutions",
+            "split_sentences": "regexp_split_sentences",
+            "split_sentence_exceptions": "exceptions_split_sentences",
+            "word_chars": "word_characters",
+        }
+
+        for key in d.keys():
+            funcname = mappings.get(key, "")
+            if funcname:
+                load(key, funcname)
+
+        ld_sort = 1
+        for ld_data in d["dictionaries"]:
+            dtype = ld_data["type"]
+            if dtype == "embedded":
+                dtype = "embeddedhtml"
+            elif dtype == "popup":
+                dtype = "popuphtml"
+            else:
+                raise ValueError(f"Invalid dictionary type {dtype}")
+
+            ld = LanguageDictionary()
+            # ld.language = lang -- if you do this, the dict is added twice.
+            ld.usefor = ld_data["for"]
+            ld.dicttype = dtype
+            ld.dicturi = ld_data["url"]
+            ld.is_active = ld_data.get("active", True)
+
+            ld.sort_order = ld_sort
+            ld_sort += 1
+            lang.dictionaries.append(ld)
+
+        return lang
```

### Comparing `lute3-3.3.1/lute/models/setting.py` & `lute3-3.3.2b1/lute/models/setting.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/models/term.py` & `lute3-3.3.2b1/lute/models/term.py`

 * *Files 5% similar despite different names*

```diff
@@ -358,27 +358,14 @@
             and_(Term.language_id == langid, Term.text_lc == text_lc)
         )
         terms = query.all()
         if not terms:
             return None
         return terms[0]
 
-    @staticmethod
-    def delete_all_status_0_terms():
-        """
-        Data clean up, in case alpha release of
-        https://github.com/jzohrab/lute-v3/issues/99
-        doesn't go well.
-        """
-        terms = db.session.query(Term).filter(Term.status == 0).all()
-        for t in terms:
-            db.session.delete(t)
-        db.session.commit()
-        return len(terms)
-
 
 class Status:
     """
     Term statuses.
     """
 
     UNKNOWN = 0
```

### Comparing `lute3-3.3.1/lute/parse/base.py` & `lute3-3.3.2b1/lute/parse/base.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/parse/character_parser.py` & `lute3-3.3.2b1/lute/parse/character_parser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/parse/mecab_parser.py` & `lute3-3.3.2b1/lute/parse/mecab_parser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/parse/registry.py` & `lute3-3.3.2b1/lute/parse/registry.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/parse/space_delimited_parser.py` & `lute3-3.3.2b1/lute/parse/space_delimited_parser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/read/render/renderable_calculator.py` & `lute3-3.3.2b1/lute/read/render/renderable_calculator.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/read/render/service.py` & `lute3-3.3.2b1/lute/read/render/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/read/routes.py` & `lute3-3.3.2b1/lute/read/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/read/service.py` & `lute3-3.3.2b1/lute/read/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/settings/routes.py` & `lute3-3.3.2b1/lute/settings/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/animated-overlay.gif` & `lute3-3.3.2b1/lute/static/css/images/animated-overlay.gif`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/jplayer-black-and-yellow.png` & `lute3-3.3.2b1/lute/static/css/images/jplayer-black-and-yellow.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/jplayer.blue.monday.jpg` & `lute3-3.3.2b1/lute/static/css/images/jplayer.blue.monday.jpg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/pbar-ani.gif` & `lute3-3.3.2b1/lute/static/css/images/pbar-ani.gif`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/ui-icons_222222_256x240.png` & `lute3-3.3.2b1/lute/static/css/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/ui-icons_2e83ff_256x240.png` & `lute3-3.3.2b1/lute/static/css/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/ui-icons_444444_256x240.png` & `lute3-3.3.2b1/lute/static/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/ui-icons_454545_256x240.png` & `lute3-3.3.2b1/lute/static/css/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/ui-icons_555555_256x240.png` & `lute3-3.3.2b1/lute/static/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/ui-icons_777620_256x240.png` & `lute3-3.3.2b1/lute/static/css/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/ui-icons_777777_256x240.png` & `lute3-3.3.2b1/lute/static/css/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/ui-icons_888888_256x240.png` & `lute3-3.3.2b1/lute/static/css/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/ui-icons_BBBBBB_256x240.png` & `lute3-3.3.2b1/lute/static/css/images/ui-icons_BBBBBB_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/ui-icons_cc0000_256x240.png` & `lute3-3.3.2b1/lute/static/css/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/ui-icons_cd0a0a_256x240.png` & `lute3-3.3.2b1/lute/static/css/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/images/ui-icons_ffffff_256x240.png` & `lute3-3.3.2b1/lute/static/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/css/player-styles.css` & `lute3-3.3.2b1/lute/static/css/player-styles.css`

 * *Files 13% similar despite different names*

```diff
@@ -6,26 +6,32 @@
   border: 2px solid #d7e6f4;
   border-radius: 5px;
   padding: 0.9rem;
   background-color: var(--audio-color-3);
   width: 80%;
   margin: 0 auto;
   margin-bottom: 1.6rem;
-  min-width: 520px;
+  min-width: fit-content;
   box-sizing: border-box;
   z-index: 999;
 
   --audio-color-1: #6da9e9;
   --audio-color-2: #ff5252;
   --audio-color-3: aliceblue;
   --audio-color-4: #79b7e7;
   --audio-color-5: #d6edff;
+  --button-size-smaller: 22px;
   --button-size-small: 28px;
   --button-size-big: 64px;
 
+  /* use variables to fix marker placement in the bookmark container*/
+  --padding-top-val: 0.2rem;
+  --padding-sides-val: 0.5rem;
+  --timeline-height: 0.7rem;
+
   position: relative;
 }
 
 .audio-player-top-container {
   display: grid;
   grid-template-columns: min-content 2.2fr min-content;
   align-items: center;
@@ -39,19 +45,14 @@
   position: relative;
 
   background-color: var(--audio-color-3);
   padding: var(--padding-top-val) var(--padding-sides-val);
   border-radius: 5px;
   box-sizing: border-box;
   margin-bottom: 6px;
-
-  /* use variables to fix marker placement in the bookmark container*/
-  --padding-top-val: 0.2rem;
-  --padding-sides-val: 0.5rem;
-  --timeline-height: 0.7rem;
 }
 
 .audio-player-central-container {
   background-color: var(--audio-color-5);
   border-radius: 5px;
   padding: 0.5rem;
 }
@@ -76,39 +77,38 @@
   cursor: pointer;
   user-select: none;
   --webkit-user-select: none;
 }
 
 #play-btn {
   background-image: url("/static/icn/play.svg");
-  height: 64px;
-  width: 64px;
+  height: var(--button-size-big);
+  width: var(--button-size-big);
   display: block;
 
   transition: all 50ms;
 }
 
-#playback-rate-btn {
-  background-image: url("/static/icn/speed.svg");
-  height: var(--button-size-small);
-  width: var(--button-size-small);
-  display: block;
-  position: relative;
-  font-family: inherit;
+#playback-rate-container {
+  display: flex;
+  gap: 0.3rem;
+  align-items: center;
 }
 
-#playback-rate-btn span {
-  position: absolute;
-  bottom: 0;
-
-  left: 50%;
-  transform: translate(-50%, 0);
-  font-family: inherit;
+.rate-btn {
+  width: var(--button-size-smaller);
+  height: var(--button-size-smaller);
+  display: block;
+  background-color: #79b7e7;
   color: #fff;
-  font-size: .6rem;
+}
+
+#playback-rate-indicator {
+  font-size: 0.9rem;
+  cursor: pointer;
 }
 
 #skip-back-btn {
   background-image: url("/static/icn/skip-back.svg");
   height: var(--button-size-small);
   width: var(--button-size-small);
 }
@@ -232,14 +232,15 @@
   display: flex;
   justify-content: center;
   align-items: center;
   gap: 0.3rem;
 }
 
 #rewind-option {
+  background-color: #d6edff;
   border: none;
   border-radius: 5px;
   /* width: 90%; */
   height: 1.6rem;
   padding-left: 0.8rem;
   font-family: inherit;
 }
@@ -346,7 +347,84 @@
   transform: scale(1.04);
   filter: brightness(110%);
 }
 
 .audio-button:active {
   filter: brightness(70%);
 }
+
+@media screen and (max-width: 480px) {
+  #read_pane_container {
+    --player-height: 90px;
+  }
+
+  .audio-player-container {
+    min-width: unset;
+    padding: 0.4rem;
+    --button-size-big: 36px;
+    --button-size-small: 22px;
+    --padding-top-val: 0px;
+    --padding-sides-val: 0px;
+  }
+  
+  .duration-container {
+    font-size: 0.8rem;
+  }
+
+  .audio-player-timeline-container {
+    background-color: var(--audio-color-5);
+  }
+
+  .audio-player-central-container {
+    padding: 0.3rem;
+  }
+
+  .audio-player-top-container {
+    gap: 0.2rem;
+  }
+
+  .audio-player-controls-container {
+    gap: 0.7rem;
+  }
+
+  .rewind-container {
+    background-color: unset;
+    padding: 0;
+    gap: 0.4rem;
+  }
+
+  .rewind-btn-container {
+    gap: 0.5rem;
+  }
+
+  #playback-rate-indicator {
+    font-size: 0.8rem;
+  }
+
+  .bookmark-buttons-container {
+    background-color: unset;
+    padding: 0;
+    column-gap: 0;
+    row-gap: 0.6rem;
+  }
+  
+  #bkm-save-btn {
+    grid-column: 1 / 3;
+    justify-self: center;
+  }
+
+  #rewind-option {
+    background-color: aliceblue;
+    padding-left: 0.2rem;
+    min-width: 2.3rem;
+    font-size: 0.6rem;
+  }
+
+  .volume {
+    display: none;
+    width: 90%;
+  }
+
+  #pin {
+    display: none;
+  }
+}
```

### Comparing `lute3-3.3.1/lute/static/css/styles.css` & `lute3-3.3.2b1/lute/static/css/styles.css`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/favicon.ico` & `lute3-3.3.2b1/lute/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/favicon_dev.ico` & `lute3-3.3.2b1/lute/static/favicon_dev.ico`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/arrow-circle-135.png` & `lute3-3.3.2b1/lute/static/icn/arrow-circle-135.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/arrow-circle-225-left.png` & `lute3-3.3.2b1/lute/static/icn/arrow-circle-225-left.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/arrow-circle-315.png` & `lute3-3.3.2b1/lute/static/icn/arrow-circle-315.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/arrow-repeat.png` & `lute3-3.3.2b1/lute/static/icn/arrow-repeat.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/arrow-stop.png` & `lute3-3.3.2b1/lute/static/icn/arrow-stop.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/book--pencil.png` & `lute3-3.3.2b1/lute/static/icn/book--pencil.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/book-open-bookmark.png` & `lute3-3.3.2b1/lute/static/icn/book-open-bookmark.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/book-open-text.png` & `lute3-3.3.2b1/lute/static/icn/book-open-text.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/book-open-text.svg` & `lute3-3.3.2b1/lute/static/icn/book-open-text.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/bookmark-off.svg` & `lute3-3.3.2b1/lute/static/icn/bookmark-off.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/broom.png` & `lute3-3.3.2b1/lute/static/icn/broom.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/card--pencil.png` & `lute3-3.3.2b1/lute/static/icn/card--pencil.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/clock.png` & `lute3-3.3.2b1/lute/static/icn/clock.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/close-white.svg` & `lute3-3.3.2b1/lute/static/icn/close-white.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/close.svg` & `lute3-3.3.2b1/lute/static/icn/close.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/control-stop.png` & `lute3-3.3.2b1/lute/static/icn/control-stop.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/cross-big.png` & `lute3-3.3.2b1/lute/static/icn/cross-big.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/cross-button.png` & `lute3-3.3.2b1/lute/static/icn/cross-button.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/cross.png` & `lute3-3.3.2b1/lute/static/icn/cross.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/document--pencil.png` & `lute3-3.3.2b1/lute/static/icn/document--pencil.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/drag-handle.svg` & `lute3-3.3.2b1/lute/static/icn/drag-handle.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/drawer--minus.png` & `lute3-3.3.2b1/lute/static/icn/drawer--minus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/drawer--plus.png` & `lute3-3.3.2b1/lute/static/icn/drawer--plus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/eraser.png` & `lute3-3.3.2b1/lute/static/icn/eraser.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/exclamation-button.png` & `lute3-3.3.2b1/lute/static/icn/exclamation-button.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/exclamation-red.png` & `lute3-3.3.2b1/lute/static/icn/exclamation-red.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/external.png` & `lute3-3.3.2b1/lute/static/icn/external.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/eye.png` & `lute3-3.3.2b1/lute/static/icn/eye.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/feed--pencil.png` & `lute3-3.3.2b1/lute/static/icn/feed--pencil.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/feed--plus.png` & `lute3-3.3.2b1/lute/static/icn/feed--plus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/ff.svg` & `lute3-3.3.2b1/lute/static/icn/ff.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/font-decrease.svg` & `lute3-3.3.2b1/lute/static/icn/font-decrease.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/font-increase.svg` & `lute3-3.3.2b1/lute/static/icn/font-increase.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/funnel--minus.png` & `lute3-3.3.2b1/lute/static/icn/funnel--minus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/funnel.png` & `lute3-3.3.2b1/lute/static/icn/funnel.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/images.svg` & `lute3-3.3.2b1/lute/static/icn/images.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/inbox-download.png` & `lute3-3.3.2b1/lute/static/icn/inbox-download.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/inbox-upload.png` & `lute3-3.3.2b1/lute/static/icn/inbox-upload.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/indicator.gif` & `lute3-3.3.2b1/lute/static/icn/indicator.gif`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/light-bulb-A.png` & `lute3-3.3.2b1/lute/static/icn/light-bulb-A.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/light-bulb-T.png` & `lute3-3.3.2b1/lute/static/icn/light-bulb-T.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/light-bulb-off-A.png` & `lute3-3.3.2b1/lute/static/icn/light-bulb-off-A.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/light-bulb-off-T.png` & `lute3-3.3.2b1/lute/static/icn/light-bulb-off-T.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/light-bulb-off.png` & `lute3-3.3.2b1/lute/static/icn/light-bulb-off.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/light-bulb.png` & `lute3-3.3.2b1/lute/static/icn/light-bulb.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/lightning.png` & `lute3-3.3.2b1/lute/static/icn/lightning.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/line-spacing-decrease.svg` & `lute3-3.3.2b1/lute/static/icn/line-spacing-decrease.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/line-spacing-increase.svg` & `lute3-3.3.2b1/lute/static/icn/line-spacing-increase.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/navigation-000-button.png` & `lute3-3.3.2b1/lute/static/icn/navigation-000-button.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/navigation-180-button.png` & `lute3-3.3.2b1/lute/static/icn/navigation-180-button.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/new_line.png` & `lute3-3.3.2b1/lute/static/icn/new_line.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/notebook--minus.png` & `lute3-3.3.2b1/lute/static/icn/notebook--minus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/notebook--pencil.png` & `lute3-3.3.2b1/lute/static/icn/notebook--pencil.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/notebook--plus.png` & `lute3-3.3.2b1/lute/static/icn/notebook--plus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/notebook.png` & `lute3-3.3.2b1/lute/static/icn/notebook.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/open.svg` & `lute3-3.3.2b1/lute/static/icn/open.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/photo-album.png` & `lute3-3.3.2b1/lute/static/icn/photo-album.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/pin.svg` & `lute3-3.3.2b1/lute/static/icn/pin.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/plus-button.png` & `lute3-3.3.2b1/lute/static/icn/plus-button.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/plus.png` & `lute3-3.3.2b1/lute/static/icn/plus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/printer.png` & `lute3-3.3.2b1/lute/static/icn/printer.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/question-balloon.png` & `lute3-3.3.2b1/lute/static/icn/question-balloon.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/question-frame.png` & `lute3-3.3.2b1/lute/static/icn/question-frame.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/reload.png` & `lute3-3.3.2b1/lute/static/icn/reload.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/rewind.svg` & `lute3-3.3.2b1/lute/static/icn/rewind.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/script-import.png` & `lute3-3.3.2b1/lute/static/icn/script-import.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/settings-gear-icon.svg` & `lute3-3.3.2b1/lute/static/icn/settings-gear-icon.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/skip-back.svg` & `lute3-3.3.2b1/lute/static/icn/skip-back.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/smiley-sad.png` & `lute3-3.3.2b1/lute/static/icn/smiley-sad.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/smiley.png` & `lute3-3.3.2b1/lute/static/icn/smiley.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/speaker-volume.png` & `lute3-3.3.2b1/lute/static/icn/speaker-volume.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/star.png` & `lute3-3.3.2b1/lute/static/icn/star.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/sticky-note--pencil.png` & `lute3-3.3.2b1/lute/static/icn/sticky-note--pencil.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/sticky-note--plus.png` & `lute3-3.3.2b1/lute/static/icn/sticky-note--plus.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/sticky-note-text.png` & `lute3-3.3.2b1/lute/static/icn/sticky-note-text.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/sticky-notes-stack.png` & `lute3-3.3.2b1/lute/static/icn/sticky-notes-stack.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/sticky-notes-text.png` & `lute3-3.3.2b1/lute/static/icn/sticky-notes-text.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/sticky-notes.png` & `lute3-3.3.2b1/lute/static/icn/sticky-notes.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/test_correct.png` & `lute3-3.3.2b1/lute/static/icn/test_correct.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/test_notyet.png` & `lute3-3.3.2b1/lute/static/icn/test_notyet.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/test_wrong.png` & `lute3-3.3.2b1/lute/static/icn/test_wrong.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/text-column-one.svg` & `lute3-3.3.2b1/lute/static/icn/text-column-one.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/text-column-two.svg` & `lute3-3.3.2b1/lute/static/icn/text-column-two.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/thumb-up.png` & `lute3-3.3.2b1/lute/static/icn/thumb-up.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/thumb.png` & `lute3-3.3.2b1/lute/static/icn/thumb.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/tick-button-small.png` & `lute3-3.3.2b1/lute/static/icn/tick-button-small.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/tick-button.png` & `lute3-3.3.2b1/lute/static/icn/tick-button.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/tick.png` & `lute3-3.3.2b1/lute/static/icn/tick.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/volume.svg` & `lute3-3.3.2b1/lute/static/icn/volume.svg`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/waiting.gif` & `lute3-3.3.2b1/lute/static/icn/waiting.gif`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/waiting2.gif` & `lute3-3.3.2b1/lute/static/icn/waiting2.gif`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/wizard.png` & `lute3-3.3.2b1/lute/static/icn/wizard.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/icn/wrench-screwdriver.png` & `lute3-3.3.2b1/lute/static/icn/wrench-screwdriver.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/img/apple-touch-icon-114x114.png` & `lute3-3.3.2b1/lute/static/img/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/img/apple-touch-icon-57x57.png` & `lute3-3.3.2b1/lute/static/img/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/img/apple-touch-icon-72x72.png` & `lute3-3.3.2b1/lute/static/img/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/img/apple-touch-startup.png` & `lute3-3.3.2b1/lute/static/img/apple-touch-startup.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/img/lute.png` & `lute3-3.3.2b1/lute/static/img/lute.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/img/public_domain.png` & `lute3-3.3.2b1/lute/static/img/public_domain.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/img/ui-icons_444444_256x240.png` & `lute3-3.3.2b1/lute/static/img/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/img/ui-icons_555555_256x240.png` & `lute3-3.3.2b1/lute/static/img/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/img/ui-icons_777620_256x240.png` & `lute3-3.3.2b1/lute/static/img/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/img/ui-icons_777777_256x240.png` & `lute3-3.3.2b1/lute/static/img/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/img/ui-icons_cc0000_256x240.png` & `lute3-3.3.2b1/lute/static/img/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/img/ui-icons_ffffff_256x240.png` & `lute3-3.3.2b1/lute/static/img/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/js/dict-tabs.js` & `lute3-3.3.2b1/lute/static/js/dict-tabs.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/js/lute.js` & `lute3-3.3.2b1/lute/static/js/lute.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -374,17 +374,15 @@
     target.addClass('kwordmarked');
     save_curr_data_order(target);
     apply_status_class(target);
     $(window).scrollTo(target, {
         axis: 'y',
         offset: -150
     });
-    show_term_edit_form(target, {
-        autofocus: false
-    });
+    show_term_edit_form(target);
 }
 
 
 /** SENTENCE TRANSLATIONS *************************/
 
 // LUTE_SENTENCE_LOOKUP_URIS is rendered in templates/read/index.html.
 // Hitting "t" repeatedly cycles through the uris.  Moving to a new
```

### Comparing `lute3-3.3.1/lute/static/js/player.js` & `lute3-3.3.2b1/lute/static/js/player.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -4,26 +4,26 @@
 const timeline = document.querySelector(".timeline");
 const volumeLine = document.querySelector(".volume");
 const playBtn = document.querySelector("#play-btn");
 const durationElement = document.querySelector(".duration-container .duration");
 const currentTimeElement = document.querySelector(
     ".duration-container .current-time"
 );
+const playbackRateIncButton = document.getElementById("playback-rate-increase");
+const playbackRateDecButton = document.getElementById("playback-rate-decrease");
+const playbackRateIndicator = document.getElementById("playback-rate-indicator");
 const rewindButton = document.querySelector("#rewind-btn");
 const ffButton = document.querySelector("#ff-btn");
-const skipbackButton = document.querySelector("#skip-back-btn");
-const playbackRateButton = document.querySelector("#playback-rate-btn");
-const playbackRateIndicator = document.querySelector("#playback-rate-btn span");
 const rewindAmountOption = document.querySelector("#rewind-option");
+const skipbackButton = document.querySelector("#skip-back-btn");
 
 const pinButton = document.querySelector("#pin");
 
 const playerContainer = document.querySelector(".audio-player-container");
 const bookmarkContainer = document.querySelector(".bookmark-markers-container");
-// const timelineContainer = document.querySelector("#timeline-container");
 const bookmarkSaveDeleteBtn = document.querySelector("#bkm-save-btn");
 const bookmarkPrevBtn = document.querySelector("#bkm-prev-btn");
 const bookmarkNextBtn = document.querySelector("#bkm-next-btn");
 
 var bookmarksArray = [];
 let lastPlayTime = null;
 let playerSticky = localStorage.getItem("player-sticky") ?? 0;
@@ -177,44 +177,36 @@
 });
 
 skipbackButton.addEventListener("click", function() {
     player.currentTime = 0;
 });
 
 /* ****************************
- * Playback rate.
+ Playback rate.
  */
-
-playbackRateButton.addEventListener("mouseover", function() {
-    const scrollLeft = document.documentElement.scrollLeft;
-    const scrollTop = document.documentElement.scrollTop;
-    window.onscroll = function() {
-        window.scrollTo(scrollLeft, scrollTop);
-    };
+playbackRateIncButton.addEventListener("click", () => {
+    setPlaybackRateDelta(0.1);
 });
-
-playbackRateButton.addEventListener("mouseleave", function() {
-    window.onscroll = function() {};
+playbackRateDecButton.addEventListener("click", () => {
+    setPlaybackRateDelta(-0.1);
 });
 
-playbackRateButton.addEventListener("wheel", function(e) {
+playbackRateIndicator.addEventListener("click", resetPlaybackRate);
+
+function setPlaybackRateDelta(delta) {
     let r = player.playbackRate;
-    if (e.deltaY < 0)
-        r += 0.1;
-    else
-        r -= 0.1;
-    if (r < 0.1)
-        r = 0.1;
+    r += delta;
     if (r > 10)
         r = 10;
+    if (r < 0.1)
+        r = 0.1;
+
     player.playbackRate = r;
     playbackRateIndicator.textContent = player.playbackRate.toFixed(1);
-});
-
-playbackRateButton.addEventListener("click", resetPlaybackRate);
+}
 
 function resetPlaybackRate() {
     player.playbackRate = 1.0;
     playbackRateIndicator.textContent = "1.0";
 }
 
 /* ****************************
```

### Comparing `lute3-3.3.1/lute/static/js/resize.js` & `lute3-3.3.2b1/lute/static/js/resize.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/js/text-options.js` & `lute3-3.3.2b1/lute/static/js/text-options.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/chartjs/chart.umd.js` & `lute3-3.3.2b1/lute/static/vendor/chartjs/chart.umd.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/chartjs/chartjs-adapter-date-fns.js` & `lute3-3.3.2b1/lute/static/vendor/chartjs/chartjs-adapter-date-fns.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/datatables/README.md` & `lute3-3.3.2b1/lute/static/vendor/datatables/README.md`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/datatables/datatables.button.download.js` & `lute3-3.3.2b1/lute/static/vendor/datatables/datatables.button.download.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/datatables/datatables.min.css` & `lute3-3.3.2b1/lute/static/vendor/datatables/datatables.min.css`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/datatables/datatables.min.js` & `lute3-3.3.2b1/lute/static/vendor/datatables/datatables.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/jquery/jplayer.css` & `lute3-3.3.2b1/lute/static/vendor/jquery/jplayer.css`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/jquery/jquery-ui.css` & `lute3-3.3.2b1/lute/static/vendor/jquery/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/jquery/jquery-ui.min.js` & `lute3-3.3.2b1/lute/static/vendor/jquery/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/jquery/jquery.hoverIntent.js` & `lute3-3.3.2b1/lute/static/vendor/jquery/jquery.hoverIntent.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/jquery/jquery.jeditable.mini.js` & `lute3-3.3.2b1/lute/static/vendor/jquery/jquery.jeditable.mini.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/jquery/jquery.jplayer.js` & `lute3-3.3.2b1/lute/static/vendor/jquery/jquery.jplayer.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/jquery/jquery.jplayer.min.js` & `lute3-3.3.2b1/lute/static/vendor/jquery/jquery.jplayer.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/jquery/jquery.jplayer.swf` & `lute3-3.3.2b1/lute/static/vendor/jquery/jquery.jplayer.swf`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/jquery/jquery.js` & `lute3-3.3.2b1/lute/static/vendor/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/jquery/jquery.scrollTo.min.js` & `lute3-3.3.2b1/lute/static/vendor/jquery/jquery.scrollTo.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/jquery/jquery.xpath.min.js` & `lute3-3.3.2b1/lute/static/vendor/jquery/jquery.xpath.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/tagify/tagify.css` & `lute3-3.3.2b1/lute/static/vendor/tagify/tagify.css`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/tagify/tagify.min.js` & `lute3-3.3.2b1/lute/static/vendor/tagify/tagify.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/tagify/tagify.polyfills.min.js` & `lute3-3.3.2b1/lute/static/vendor/tagify/tagify.polyfills.min.js`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/static/vendor/tagify/tagify_overrides.css` & `lute3-3.3.2b1/lute/static/vendor/tagify/tagify_overrides.css`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/stats/service.py` & `lute3-3.3.2b1/lute/stats/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/backup/backup.html` & `lute3-3.3.2b1/lute/templates/backup/backup.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/backup/index.html` & `lute3-3.3.2b1/lute/templates/backup/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/base.html` & `lute3-3.3.2b1/lute/templates/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
       </div>
       {% endif %}
       <div class="menu-item">
         <span id="menu_about">About</span>
         <ul class="sub-menu last-sub-menu">
           <li><a href="/version">Version and software info</a></li>
           <li><a href="/stats/">Statistics</a></li>
-          <li><a href="https://jzohrab.github.io/lute-manual/" target="_blank">Docs</a></li>
+          <li><a href="https://luteorg.github.io/lute-manual/" target="_blank">Docs</a></li>
           <li><a href="https://discord.gg/CzFUQP5m8u" target="_blank">Discord</a></li>
         </ul>
       </div>
     </div>
   </div>
   {% endif %}
```

### Comparing `lute3-3.3.1/lute/templates/book/create_new.html` & `lute3-3.3.2b1/lute/templates/book/create_new.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/book/edit.html` & `lute3-3.3.2b1/lute/templates/book/edit.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/book/import_webpage.html` & `lute3-3.3.2b1/lute/templates/book/import_webpage.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/book/tablelisting.html` & `lute3-3.3.2b1/lute/templates/book/tablelisting.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/errors/404_error.html` & `lute3-3.3.2b1/lute/templates/errors/404_error.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/errors/500_error.html` & `lute3-3.3.2b1/lute/templates/errors/500_error.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/hotkeys.html` & `lute3-3.3.2b1/lute/templates/hotkeys.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/imagesearch/index.html` & `lute3-3.3.2b1/lute/templates/imagesearch/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/index.html` & `lute3-3.3.2b1/lute/templates/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -26,14 +26,14 @@
 {% if is_production_data and backup_show_warning %}
 <div class="flash-notice">
   <p>Warning: {{ backup_warning_msg }} <a href="/backup/backup">Create a backup.</a></p>
 </div>
 {% endif %}
 
 {% if not have_languages %}
-  <p>To get started using Lute, first <a href="/language/new">create your language.</a>
+  <p>To get started using Lute, first <a href="/language/list_predefined">load a predefined language and sample text</a>, or <a href="/language/new">create your language.</a>
 </p>
 {% else %}
   {% include "book/tablelisting.html" %}
 {% endif %}
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -5,9 +5,10 @@
 short texts for you to try out.
 When you're done trying out the demo, _c_l_i_c_k_ _h_e_r_e to clear out the database.
 Note: this removes everything in the db.
 Or instead, _d_i_s_m_i_s_s this message.
 {% endif %} {% if is_production_data and backup_show_warning %}
 Warning: {{ backup_warning_msg }} _C_r_e_a_t_e_ _a_ _b_a_c_k_u_p_.
 {% endif %} {% if not have_languages %}
-To get started using Lute, first _c_r_e_a_t_e_ _y_o_u_r_ _l_a_n_g_u_a_g_e_.
+To get started using Lute, first _l_o_a_d_ _a_ _p_r_e_d_e_f_i_n_e_d_ _l_a_n_g_u_a_g_e_ _a_n_d_ _s_a_m_p_l_e_ _t_e_x_t, or
+_c_r_e_a_t_e_ _y_o_u_r_ _l_a_n_g_u_a_g_e_.
 {% else %} {% include "book/tablelisting.html" %} {% endif %} {% endblock %}
```

### Comparing `lute3-3.3.1/lute/templates/language/_form.html` & `lute3-3.3.2b1/lute/templates/language/_form.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/language/index.html` & `lute3-3.3.2b1/lute/templates/language/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -34,23 +34,24 @@
   </tbody>
 </table>
 </div>
 
 {% endif %}
 
 <br />
-<a href="{{ url_for('language.new') }}">Create new</a>
+<p><a href="{{ url_for('language.list_predefined') }}">Load predefined language and sample stories</a></p>
+<p><a href="{{ url_for('language.new') }}">Create new</a></p>
 
 <script>
   var language_listing_table;
 
   let setup_lang_datatable = function() {
     lang_listing_table = $('#languagetable').DataTable({
       responsive: true,
-      select: true,
+      select: false,
       lengthMenu: [ 10, 25, 50 ],
       pageLength: 25,
       paging: true,
       info: true,
       searching: true,
       processing: true,
       stateSave: true,
```

### Comparing `lute3-3.3.1/lute/templates/language/new.html` & `lute3-3.3.2b1/lute/templates/language/new.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/read/audio_player.html` & `lute3-3.3.2b1/lute/templates/read/audio_player.html`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,19 @@
             <option value="3">3 sec</option>
             <option value="5" selected>5 sec</option>
             <option value="10">10 sec</option>
             <option value="30">30 sec</option>
             <option value="60">60 sec</option>
           </select>
         </div>
-        <button id="playback-rate-btn" class="audio-button"><span>1.0</span></button>
+        <div id="playback-rate-container" title="Playback rate controls. Click on the indicator to reset">
+          <button id="playback-rate-decrease" class="audio-button rate-btn"><span>-</span></button>
+          <div id="playback-rate-indicator">1.0</div>
+          <button id="playback-rate-increase" class="audio-button rate-btn"><span>+</span></button>
+        </div>
       </div>
     </div>
     <div class="audio-player-right-container">
       <input type="range" class="volume" max="100" value="100"/>
       <div class="bookmark-buttons-container">
         <button id="bkm-save-btn" class="audio-button"></button>
         <div class="bookmark-jump-container">
```

### Comparing `lute3-3.3.1/lute/templates/read/flashcopied.html` & `lute3-3.3.2b1/lute/templates/read/flashcopied.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/read/frameform.html` & `lute3-3.3.2b1/lute/templates/read/frameform.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/read/index.html` & `lute3-3.3.2b1/lute/templates/read/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/read/page_content.html` & `lute3-3.3.2b1/lute/templates/read/page_content.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/read/page_edit_form.html` & `lute3-3.3.2b1/lute/templates/read/page_edit_form.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/read/reading_menu.html` & `lute3-3.3.2b1/lute/templates/read/reading_menu.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/read/termpopup.html` & `lute3-3.3.2b1/lute/templates/read/termpopup.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/read/updated.html` & `lute3-3.3.2b1/lute/templates/read/updated.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/settings/form.html` & `lute3-3.3.2b1/lute/templates/settings/form.html`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
           title="Click for details"
           onclick="$('#custom_styles_help').toggle();"
           />
         <blockquote id="custom_styles_help" style="width:60%; display: none;">
           <p>Use this field to define custom styles to be applied to
           Lute.</p>
           <p>See examples
-          in <a href="https://jzohrab.github.io/lute-manual/usage/themes/custom-styles.html"
+          in <a href="https://luteorg.github.io/lute-manual/usage/themes/custom-styles.html"
           target="_blank">the manual</a>.</p>
         </blockquote>
       </td>
       </td>
       <td>
         {{ form.custom_styles(class="form-largetextarea") }}
       </td>
@@ -110,21 +110,21 @@
           src="{{ url_for('static', filename='icn/question-balloon.png') }}"
           title="Click for details"
           onclick="$('#mecab_path_help').toggle();"
           />
         <blockquote id="mecab_path_help" style="width:60%; display: none;">
           <p>Lute uses MeCab to parse Japanese, so MeCab needs to be
             installed on your machine (see notes
-            in <a href="https://jzohrab.github.io/lute-manual/install/mecab.html"
+            in <a href="https://luteorg.github.io/lute-manual/install/mecab.html"
             target="_blank">the manual</a>).</p>
           <p>Lute includes the Python
             library <a href="https://github.com/buruzaemon/natto-py">natto-py</a>
             to interact with MeCab.  natto-py can usually find MeCab
             automatically, but you <i>may</i> need to set the MECAB_PATH, per
-            <a href="https://jzohrab.github.io/lute-manual/install/mecab.html#lute-configuration"
+            <a href="https://luteorg.github.io/lute-manual/install/mecab.html#lute-configuration"
             target="_blank">the manual</a>.</p>
           <p>Try different values for MECAB_PATH, including leaving
             the field blank, until clicking the &quot;test&quot;
             button returns a &quot;success&quot; message.</p>
         </blockquote>
       </td>
       <td>{{ form.mecab_path(class="form-control") }}</td>
```

### Comparing `lute3-3.3.1/lute/templates/stats/index.html` & `lute3-3.3.2b1/lute/templates/stats/index.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/term/_form.html` & `lute3-3.3.2b1/lute/templates/term/_form.html`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         {% endif %}>
         {{ form.language_id(class="form-control") }}
         <button id="load-dicts-btn" title="Load dictionaries for the new term" type="button"></button>
       </div>
   
       {{ form.original_text }}
 
-      <div>{{ form.text(class="form-control", value=(form.original_text.data or ''), autofocus=(not form.original_text.data)) }}</div>
+      <div>{{ form.text(class="form-control", value=(form.original_text.data or '')) }}</div>
 
       <div>{{ form.parentslist(class="form-control") }}</div>
   
       <div {% if hide_pronunciation %}style="display:none;"{% endif %}>
         {{ form.romanization(class="form-control") }}
       </div>
 
@@ -295,40 +295,44 @@
       autoComplete: { enabled: true, rightKey: true, tabKey: true },
       dropdown: { enabled: 1 },
       enforceWhitelist: false,
       whitelist: TAGS
     });  // end tagify
   };
 
-  // TODO zzfuture fix: check term autofocus
-  // lute.js should send an "autofocus" flag, I believe.
-  let handleAutofocus = function() {
-    const wordfield = $('#text');
-    const transfield = $('#translation');
-
-    if ($('#autofocus').val() != 'false') {
-      if (wordfield.val()) {
-        transfield.focus();
-      }
-      else {
-        wordfield.focus();
-      }
-    }
-  };
-
   $(document).ready(function () {
 
     // "Save" shortcut
     $(document).keydown(function(event) {
       console.log(event);
       if (event.ctrlKey && event.key === "Enter") {
         $("#submit").click();
       }
     });
 
+    /*
+    // Set term form focus
+    // DISABLING THIS: with this change, the term edit form pulls focus,
+    // so the left-and-right arrows don't work within the reading pane.
+    // The reading pane arrows are more important than the focus being set, IMO.
+    // Perhaps this can be changed later to set the focus if the form is opened
+    // from the term listing (i.e. move this to templates/term/formframes.html).
+    const langId = $("#language_id")
+    const text = $("#text")
+    const translation = $("#translation")
+
+    if(langId.val() == "0"){
+      langId.focus();
+    }else if(text.val() == ""){
+      text.focus();
+    }else{
+      translation.focus();
+    }
+    */
+
     // Term image events.
     var term_image = $("#term_image");
 
     term_image.hover(
       function(){ $(this).attr("title", "Click and hit Delete to remove, then Save."); },
       function(){ $(this).removeClass('clickedZoomableImage') }
     );
```

### Comparing `lute3-3.3.1/lute/templates/term/formframes.html` & `lute3-3.3.2b1/lute/templates/term/formframes.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/term/index.html` & `lute3-3.3.2b1/lute/templates/term/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
       layout: {
         topStart: 'pageLength',
         topEnd: 'search',
         bottomStart: ['info', 'buttons'],
         bottomEnd: 'paging'
       },
       responsive: true,
-      select: true,
+      select: false,
       lengthMenu: [ 25, 50, 100, 500, 1000 ],
 
       // The button is included but the div.dt-buttons is hidden,
       // so that the button actions can be trigged by a link
       // in the "Actions" list.
       buttons: [
          {
```

### Comparing `lute3-3.3.1/lute/templates/term/sentences.html` & `lute3-3.3.2b1/lute/templates/term/sentences.html`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   <body>
 
     {% if no_references %}
     <p>No references found for "{{ text }}":</p>
     <ul>
       <li>This may be a new term.</li>
       <li>The page containing this word may not be marked as "read" (see
-        <a href="https://jzohrab.github.io/lute-manual/faq/terms/sentences-only-shown-when-page-is-read.html"
+        <a href="https://luteorg.github.io/lute-manual/faq/terms/sentences-only-shown-when-page-is-read.html"
            target="_blank">the manual</a>
         ).
       </li>
       <li>Books containing this term may have been deleted.</li>
     </ul>
     {% endif %}
```

### Comparing `lute3-3.3.1/lute/templates/termimport/index.html` & `lute3-3.3.2b1/lute/templates/termimport/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends 'base.html' %}
 
 {% block title %}Import Terms{% endblock %}
 {% block header %}Import Terms{% endblock %}
 
 {% block body %}
 
-<p>See <a href="https://jzohrab.github.io/lute-manual/usage/terms/bulk-term-import.html" target="_blank">"Bulk Term Import"</a> in the Lute manual for notes about the CSV file format and data.</p>
+<p>See <a href="https://luteorg.github.io/lute-manual/usage/terms/bulk-term-import.html" target="_blank">"Bulk Term Import"</a> in the Lute manual for notes about the CSV file format and data.</p>
 <br />
 
 {% for field_name, field_errors in form.errors.items() %}
 {% for error in field_errors %}
 <div class="flash-notice">{{ error }}</div>
 {% endfor %}
 <br />
```

### Comparing `lute3-3.3.1/lute/templates/termtag/_form.html` & `lute3-3.3.2b1/lute/templates/termtag/_form.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/templates/termtag/index.html` & `lute3-3.3.2b1/lute/templates/termtag/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 </form>
 
 <script>
   
   let setup_datatable = function() {
     var table = $('#termtagtable').DataTable({
       responsive: true,
-      select: true,
+      select: false,
       lengthMenu: [ 10, 25, 50 ],
       paging: true,
       info: true,
       searching: true,
       processing: true,
       serverSide: true,
       stateSave: true,
```

### Comparing `lute3-3.3.1/lute/templates/version.html` & `lute3-3.3.2b1/lute/templates/version.html`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/term/datatables.py` & `lute3-3.3.2b1/lute/term/datatables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/term/forms.py` & `lute3-3.3.2b1/lute/term/forms.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/term/model.py` & `lute3-3.3.2b1/lute/term/model.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/term/routes.py` & `lute3-3.3.2b1/lute/term/routes.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     Blueprint,
     request,
     jsonify,
     render_template,
     redirect,
     current_app,
     send_file,
-    flash,
 )
 from lute.models.language import Language
 from lute.models.term import Term as DBTerm
 from lute.models.setting import UserSetting
 from lute.utils.data_tables import DataTablesFlaskParamParser
 from lute.term.datatables import get_data_tables_list
 from lute.term.model import Repository, Term
@@ -323,22 +322,7 @@
     Delete a term.
     """
     repo = Repository(db)
     term = repo.load(termid)
     repo.delete(term)
     repo.commit()
     return redirect("/term/index", 302)
-
-
-@bp.route("/delete_all_status_0_terms", methods=["GET"])
-def delete_all_status_0():
-    """
-    Delete all status 0 terms.
-
-    This route can only be called directly in the browser, it doesn't have a URL.
-
-    ref https://github.com/jzohrab/lute-v3/issues/99
-    Need to remove all status 0 terms if reverting from the alpha release.
-    """
-    deleted = DBTerm.delete_all_status_0_terms()
-    flash(f"Clean up: deleted {deleted} status 0 terms.")
-    return redirect("/", 302)
```

### Comparing `lute3-3.3.1/lute/term_parent_map/routes.py` & `lute3-3.3.2b1/lute/term_parent_map/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/term_parent_map/service.py` & `lute3-3.3.2b1/lute/term_parent_map/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/termimport/routes.py` & `lute3-3.3.2b1/lute/termimport/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/termimport/service.py` & `lute3-3.3.2b1/lute/termimport/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -204,16 +204,24 @@
     "Set the term parents."
     t = repo.find(lang.id, rec["term"])
     parents = list(map(str.strip, rec["parent"].split(",")))
     t.parents = [p for p in parents if p != ""]
     if "link_status" in rec and len(parents) == 1:
         sync_status = rec["link_status"] or ""
         t.sync_status = sync_status.strip().lower() == "y"
-    if len(parents) != 1:
+    if len(t.parents) != 1:
         t.sync_status = False
+
+    # If syncing to parent, and the term status was not explicitly set,
+    # then "inherit" the parent status.
+    if t.sync_status and len(t.parents) == 1 and "status" not in rec:
+        p = repo.find(lang.id, t.parents[0])
+        if p is not None:
+            t.status = p.status
+
     repo.add(t)
 
 
 def _do_import(
     import_data, create_terms=True, update_terms=True, new_as_unknowns=False
 ):
     """
```

### Comparing `lute3-3.3.1/lute/termtag/datatables.py` & `lute3-3.3.2b1/lute/termtag/datatables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/termtag/routes.py` & `lute3-3.3.2b1/lute/termtag/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/themes/css/Apple_Books.css` & `lute3-3.3.2b1/lute/themes/css/Apple_Books.css`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/themes/css/Dark_slate.css` & `lute3-3.3.2b1/lute/themes/css/Dark_slate.css`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/themes/css/LWT.css` & `lute3-3.3.2b1/lute/themes/css/LWT.css`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/themes/css/LingQ.css` & `lute3-3.3.2b1/lute/themes/css/LingQ.css`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/themes/css/Night.css` & `lute3-3.3.2b1/lute/themes/css/Night.css`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/themes/routes.py` & `lute3-3.3.2b1/lute/themes/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/themes/service.py` & `lute3-3.3.2b1/lute/themes/service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/useraudio/routes.py` & `lute3-3.3.2b1/lute/useraudio/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/userimage/routes.py` & `lute3-3.3.2b1/lute/userimage/routes.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/utils/data_tables.py` & `lute3-3.3.2b1/lute/utils/data_tables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/utils/debug_helpers.py` & `lute3-3.3.2b1/lute/utils/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/lute/utils/formutils.py` & `lute3-3.3.2b1/lute/utils/formutils.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/pyproject.toml` & `lute3-3.3.2b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   "jaconv>=0.3.4,<1",
   "platformdirs>=3.10.0,<4",
   "requests>=2.31.0,<3",
   "beautifulsoup4>=4.12.2,<5",
   "PyYAML>=6.0.1,<7",
   "toml>=0.10.2,<1",
   "waitress>=2.1.2,<3",
-  "openepub>=0.0.6,<1",
+  "openepub>=0.0.8,<1",
   "pypdf>=3.17.4",
   "subtitle-parser>=1.3.0"
 ]
 
 [project.scripts]
 lute = "lute.main:start"
 
@@ -52,8 +52,8 @@
   "pytest-bdd>=7.0.0,<8",
   "pytest-splinter>=3.3.2,<4",
   "pre-commit>=3.5.0,<4",
   "black>=23.10.1,<24",
 ]
 
 [project.urls]
-Home = "https://github.com/jzohrab/lute-v3"
+Home = "https://github.com/luteorg/lute-v3"
```

### Comparing `lute3-3.3.1/requirements.txt` & `lute3-3.3.2b1/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 lazy-object-proxy==1.9.0
 Mako==1.2.4
 MarkupSafe==2.1.3
 mccabe==0.7.0
 mypy-extensions==1.0.0
 natto-py==1.0.1
 nodeenv==1.8.0
-openepub==0.0.6
+openepub==0.0.8
 outcome==1.3.0.post0
 packaging==23.1
 parse==1.19.1
 parse-type==0.6.2
 pathspec==0.11.2
 pipdeptree==2.13.0
 platformdirs==3.10.0
```

### Comparing `lute3-3.3.1/tasks.py` & `lute3-3.3.2b1/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,22 +101,28 @@
 
 
 @task(
     pre=[_ensure_test_db],
     help={
         "port": "optional port to run on; creates server if needed.",
         "show": "print data",
-        "headless": "run as headless",
+        "noheadless": "run as non-headless (default is headless, i.e. not shown)",
         "kflag": "optional -k flag argument",
         "exitfirst": "exit on first failure",
         "verbose": "make verbose",
     },
 )
 def accept(  # pylint: disable=too-many-arguments
-    c, port=5000, show=False, headless=False, kflag=None, exitfirst=False, verbose=False
+    c,
+    port=5000,
+    show=False,
+    noheadless=False,
+    kflag=None,
+    exitfirst=False,
+    verbose=False,
 ):
     """
     Start lute, run tests/acceptance tests, screenshot fails.
 
     If no port specified, use default 5000.
 
     If Lute's not running on specified port, start a server.
@@ -127,15 +133,15 @@
         "--splinter-screenshot-dir=tests/acceptance/failure_screenshots",
         "--splinter-webdriver=chrome",
         f"--port={port}",
     ]
 
     if show:
         run_test.append("-s")
-    if headless:
+    if not noheadless:
         run_test.append("--headless")
     if kflag:
         run_test.append("-k")
         run_test.append(kflag)
     if exitfirst:
         run_test.append("--exitfirst")
     if verbose:
```

### Comparing `lute3-3.3.1/tests/acceptance/book.feature` & `lute3-3.3.2b1/tests/acceptance/book.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/acceptance/conftest.py` & `lute3-3.3.2b1/tests/acceptance/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,15 @@
 # Books
 
 
 @given(parsers.parse('a {lang} book "{title}" with content:\n{c}'))
 def given_book(luteclient, lang, title, c):
     "Make a book."
     luteclient.make_book(title, c, lang)
+    _sleep(1)  # Hack!
 
 
 @given(parsers.parse('a {lang} book "{title}" from file {filename}'))
 def given_book_from_file(luteclient, lang, title, filename):
     "Book is made from file in sample_files dir."
     thisdir = os.path.dirname(os.path.realpath(__file__))
     fullpath = os.path.join(thisdir, "sample_files", filename)
```

### Comparing `lute3-3.3.1/tests/acceptance/lute_test_client.py` & `lute3-3.3.2b1/tests/acceptance/lute_test_client.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/acceptance/reading.feature` & `lute3-3.3.2b1/tests/acceptance/reading.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/acceptance/sample_files/Hola.epub` & `lute3-3.3.2b1/tests/acceptance/sample_files/Hola.epub`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/acceptance/sample_files/Hola.pdf` & `lute3-3.3.2b1/tests/acceptance/sample_files/Hola.pdf`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/acceptance/sample_files/invalid_empty.epub` & `lute3-3.3.2b1/tests/acceptance/sample_files/invalid_empty.epub`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/acceptance/smoke.feature` & `lute3-3.3.2b1/tests/acceptance/smoke.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/acceptance/start_acceptance_app.py` & `lute3-3.3.2b1/tests/acceptance/start_acceptance_app.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/acceptance/sync_status.feature` & `lute3-3.3.2b1/tests/acceptance/sync_status.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/acceptance/term.feature` & `lute3-3.3.2b1/tests/acceptance/term.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/acceptance/unsupported_parser.feature` & `lute3-3.3.2b1/tests/acceptance/unsupported_parser.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/conftest.py` & `lute3-3.3.2b1/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import os
 import yaml
 import pytest
 
 from lute.config.app_config import AppConfig
 from lute.db import db
+from lute.language.service import get_language_def
 import lute.db.demo
 from lute.app_factory import create_app
 
 from lute.models.language import Language
 
 
 def pytest_sessionstart(session):  # pylint: disable=unused-argument
@@ -94,78 +95,52 @@
 def fixture_demo_client(app):
     """
     Client using demo-data-loaded application.
     """
     return app.test_client()
 
 
-@pytest.fixture(name="demo_yaml_folder")
-def fixture_yaml_folder():
-    "Path to the demo files."
-    return os.path.join(lute.db.demo.demo_data_path(), "languages")
-
-
-def _get_language(f):
+def _get_test_language(lang_name):
     """
     Return language from the db if it already exists,
     or create it from the file.
     """
-    lang = lute.db.demo.get_demo_language(f)
-    db_language = db.session.query(Language).filter(Language.name == lang.name).first()
-    if db_language is None:
+    lang = db.session.query(Language).filter(Language.name == lang_name).first()
+    if lang is not None:
         return lang
-    return db_language
-
-
-@pytest.fixture(name="test_languages")
-def fixture_test_languages(app_context, demo_yaml_folder):
-    "Dict of available languages for tests."
-    # Hardcoded = good enough.
-    langs = [
-        "spanish",
-        "english",
-        "japanese",
-        "turkish",
-        "classical_chinese",
-        "german",
-        "hindi",
-    ]
-    ret = {}
-    for lang in langs:
-        f = os.path.join(demo_yaml_folder, f"{lang}.yaml")
-        ret[lang] = _get_language(f)
-    yield ret
+    lang = get_language_def(lang_name)["language"]
+    return lang
 
 
 @pytest.fixture(name="spanish")
-def fixture_spanish(test_languages):
-    return test_languages["spanish"]
+def fixture_spanish(app_context):
+    return _get_test_language("Spanish")
 
 
 @pytest.fixture(name="english")
-def fixture_english(test_languages):
-    return test_languages["english"]
+def fixture_english(app_context):
+    return _get_test_language("English")
 
 
 @pytest.fixture(name="japanese")
-def fixture_japanese(test_languages):
-    return test_languages["japanese"]
+def fixture_japanese(app_context):
+    return _get_test_language("Japanese")
 
 
 @pytest.fixture(name="turkish")
-def fixture_turkish(test_languages):
-    return test_languages["turkish"]
+def fixture_turkish(app_context):
+    return _get_test_language("Turkish")
 
 
 @pytest.fixture(name="classical_chinese")
-def fixture_cl_chinese(test_languages):
-    return test_languages["classical_chinese"]
+def fixture_cl_chinese(app_context):
+    return _get_test_language("Classical Chinese")
 
 
 @pytest.fixture(name="german")
-def fixture_german(test_languages):
-    return test_languages["german"]
+def fixture_german(app_context):
+    return _get_test_language("German")
 
 
 @pytest.fixture(name="hindi")
-def fixture_hindi(test_languages):
-    return test_languages["hindi"]
+def fixture_hindi(app_context):
+    return _get_test_language("Hindi")
```

### Comparing `lute3-3.3.1/tests/dbasserts.py` & `lute3-3.3.2b1/tests/dbasserts.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/features/README.md` & `lute3-3.3.2b1/tests/features/README.md`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/features/rendering.feature` & `lute3-3.3.2b1/tests/features/rendering.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/features/term_import.feature` & `lute3-3.3.2b1/tests/features/term_import.feature`

 * *Files 12% similar despite different names*

```diff
@@ -337,14 +337,77 @@
         And sql "select WoText, WoStatus, WoSyncStatus from words order by WoText" should return:
             a; 3; 0
             b; 3; 1
             c; 3; 1
             d; 4; 0
 
 
+    Scenario: Issue 387 child without status inherits parent status if linked
+        Given import file:
+            language,term,status
+            Spanish,a,3
+        When import with create true, update false
+        Then import should succeed with 1 created, 0 updated, 0 skipped
+        And sql "select WoText, WoStatus, WoSyncStatus from words order by WoText" should return:
+            a; 3; 0
+
+        Given import file:
+            language,term,parent,link_status
+            Spanish,achild,a,y
+        When import with create true, update false
+        Then import should succeed with 1 created, 0 updated, 0 skipped
+        And sql "select WoText, WoStatus, WoSyncStatus from words order by WoText" should return:
+            a; 3; 0
+            achild; 3; 1
+
+
+    Scenario: Issue 387 child with status overrides parent status if linked
+        Given import file:
+            language,term,status
+            Spanish,a,3
+        When import with create true, update false
+        Then import should succeed with 1 created, 0 updated, 0 skipped
+        And sql "select WoText, WoStatus, WoSyncStatus from words order by WoText" should return:
+            a; 3; 0
+
+        Given import file:
+            language,term,parent,status,link_status
+            Spanish,achild,a,2,y
+        When import with create true, update false
+        Then import should succeed with 1 created, 0 updated, 0 skipped
+        And sql "select WoText, WoStatus, WoSyncStatus from words order by WoText" should return:
+            a; 2; 0
+            achild; 2; 1
+
+
+    Scenario: Issue 387 importing an unknown child of a parent sets its status to parent
+        Given import file:
+            language,term,status
+            Spanish,a,3
+        When import with create true, update false
+        Then import should succeed with 1 created, 0 updated, 0 skipped
+        And sql "select WoText, WoStatus, WoSyncStatus from words order by WoText" should return:
+            a; 3; 0
+
+        # Importing a term as "unknown" really imports it as "known" (with non-0 status)
+        # if it's associated with a known parent!
+        # This may seem counter-intuitive, but it's really the only thing that makes sense.
+        # The parent is "known" (non-0 status), so if the child is associated with that
+        # parent then really it's known too.  Having such a child be an exception to the
+        # parent-status following rules is so hairy that I'm not going to bother doing it.
+        Given import file:
+            language,term,parent,link_status
+            Spanish,achild,a,y
+        When import with create true, update false, new as unknown true
+        Then import should succeed with 1 created, 0 updated, 0 skipped
+        And sql "select WoText, WoStatus, WoSyncStatus from words order by WoText" should return:
+            a; 3; 0
+            achild; 3; 1
+
+    
     Scenario: Import file fields can be in any order
         Given import file:
             language,translation,term,parent,status,tags,pronunciation
             Spanish,,gatos,gato,1,,
             Spanish,CAT,gato,,1,animal,GAH-toh
         When import with create true, update false
         Then import should succeed with 2 created, 0 updated, 0 skipped
```

### Comparing `lute3-3.3.1/tests/features/term_import_status_0.feature` & `lute3-3.3.2b1/tests/features/term_import_status_0.feature`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/features/test_rendering.py` & `lute3-3.3.2b1/tests/features/test_rendering.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/features/test_term_import.py` & `lute3-3.3.2b1/tests/features/test_term_import.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/integration/test_main.py` & `lute3-3.3.2b1/tests/integration/test_main.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/orm/test_Book.py` & `lute3-3.3.2b1/tests/orm/test_Book.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/orm/test_Language.py` & `lute3-3.3.2b1/tests/orm/test_Language.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/orm/test_Term.py` & `lute3-3.3.2b1/tests/orm/test_Term.py`

 * *Files 3% similar despite different names*

```diff
@@ -301,38 +301,7 @@
 
 
 @pytest.mark.term_case
 def test_changing_text_of_non_saved_Term_is_ok(english):
     "Changing text should not throw if not saved."
     term = Term(english, "ABC")
     term.text = "DEF"
-
-
-## Status 0 alpha release data cleanup.
-# ref https://github.com/jzohrab/lute-v3/issues/99
-# Need to remove all status 0 terms if reverting from the alpha release.
-
-
-def test_delete_all_status_0_terms(spanish):
-    "Non-status-0 terms are left as-is."
-    term = Term(spanish, "HOLA")
-    term.set_flash_message("hello")
-    term.set_current_image("hello.png")
-    term.status = 0
-    db.session.add(term)
-
-    term2 = Term(spanish, "GATO")
-    term2.status = 0
-    db.session.add(term2)
-
-    other = Term(spanish, "other")
-    other.status = 1
-    db.session.add(other)
-
-    db.session.commit()
-
-    sql_list = "select WoText from words order by WoText"
-    assert_sql_result(sql_list, ["GATO", "HOLA", "other"], "both exist")
-
-    deleted = Term.delete_all_status_0_terms()
-    assert deleted == 2, "2 deleted"
-    assert_sql_result(sql_list, ["other"], "GATO, HOLA del")
```

### Comparing `lute3-3.3.1/tests/orm/test_Text.py` & `lute3-3.3.2b1/tests/orm/test_Text.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/playwright/playwright.py` & `lute3-3.3.2b1/tests/playwright/playwright.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     # print("-" * 50)
     def _print(s):
         print(s)
 
     _print("Opening browser.")
     browser = p.chromium.launch(headless=not showbrowser)
     context = browser.new_context()
-    context.set_default_timeout(3000)
+    context.set_default_timeout(30000)
     page = context.new_page()
 
     _print("Reset db.")
     page.goto("http://localhost:5000/dev_api/load_demo")
 
     # Hardcoded port will cause problems ...
     page.goto("http://localhost:5000/")
```

### Comparing `lute3-3.3.1/tests/unit/backup/test_backup.py` & `lute3-3.3.2b1/tests/unit/backup/test_backup.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/book/test_Repository.py` & `lute3-3.3.2b1/tests/unit/book/test_Repository.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,33 @@
     assert b.texts[0].text == "greeting"
 
     book = repo.load(b.id)
     assert book.title == new_book.title, "found book"
     assert book.book_tags == ["tag1", "tag2"], "tags filled"
 
 
+def test_can_save_new_book_by_language_name(app_context, new_book, repo):
+    """
+    Can save a book with language name, useful for api access.
+    """
+    sql = "select BkTitle from books where BkTitle = 'HELLO'"
+    assert_sql_result(sql, [], "empty table")
+
+    new_book.language_id = None
+    new_book.language_name = "English"
+    b = repo.add(new_book)
+    repo.commit()
+    assert_sql_result(sql, ["HELLO"], "Saved")
+    assert b.texts[0].text == "greeting"
+
+    book = repo.load(b.id)
+    assert book.title == new_book.title, "found book"
+    assert book.book_tags == ["tag1", "tag2"], "tags filled"
+
+
 def test_save_new_respects_book_words_per_page_count(app_context, new_book, repo):
     """
     Saving a simple Book object loads the database.
     """
     sql = "select BkTitle from books where BkTitle = 'HELLO'"
     assert_sql_result(sql, [], "empty table")
```

### Comparing `lute3-3.3.1/tests/unit/book/test_datatables.py` & `lute3-3.3.2b1/tests/unit/book/test_datatables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/book/test_stats.py` & `lute3-3.3.2b1/tests/unit/book/test_stats.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/cli/test_language_term_export.py` & `lute3-3.3.2b1/tests/unit/cli/test_language_term_export.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/config/test_app_config.py` & `lute3-3.3.2b1/tests/unit/config/test_app_config.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/db/setup/test_BackupManager.py` & `lute3-3.3.2b1/tests/unit/db/setup/test_BackupManager.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/db/setup/test_Setup.py` & `lute3-3.3.2b1/tests/unit/db/setup/test_Setup.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/db/setup/test_SqliteMigrator.py` & `lute3-3.3.2b1/tests/unit/db/setup/test_SqliteMigrator.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/db/test_management.py` & `lute3-3.3.2b1/tests/unit/db/test_management.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/models/test_Book.py` & `lute3-3.3.2b1/tests/unit/models/test_Book.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/models/test_Book_add_remove_pages.py` & `lute3-3.3.2b1/tests/unit/models/test_Book_add_remove_pages.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/models/test_Language.py` & `lute3-3.3.2b1/tests/unit/models/test_Language.py`

 * *Files 17% similar despite different names*

```diff
@@ -59,7 +59,20 @@
 
     This needs to be converted to the python equivalent, e.g.
 
     u0600-u06FFuFE70-uFEFC  (where u = backslash-u)
     """
     a = Language.find_by_name("Arabic")
     assert a.word_characters == r"\u0600-\u06FF\uFE70-\uFEFC"
+
+
+def test_lang_to_dict_from_dict_returns_same_thing(app_context):
+    """
+    Lang can be exported to yaml and imported from yaml.
+    A dictionary is used as the intermediary form, so the
+    same language should return the same data.
+    """
+    e = Language.find_by_name("English")
+    e_dict = e.to_dict()
+    e_from_dict = Language.from_dict(e_dict)
+    e_back_to_dict = e_from_dict.to_dict()
+    assert e_dict == e_back_to_dict, "Same thing returned"
```

### Comparing `lute3-3.3.1/tests/unit/models/test_Setting.py` & `lute3-3.3.2b1/tests/unit/models/test_Setting.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/models/test_Term.py` & `lute3-3.3.2b1/tests/unit/models/test_Term.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/models/test_TermTag.py` & `lute3-3.3.2b1/tests/unit/models/test_TermTag.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/models/test_Text.py` & `lute3-3.3.2b1/tests/unit/models/test_Text.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/parse/test_ClassicalChineseParser.py` & `lute3-3.3.2b1/tests/unit/parse/test_ClassicalChineseParser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/parse/test_JapaneseParser.py` & `lute3-3.3.2b1/tests/unit/parse/test_JapaneseParser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/parse/test_SentenceGroupIterator.py` & `lute3-3.3.2b1/tests/unit/parse/test_SentenceGroupIterator.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/parse/test_SpaceDelimitedParser.py` & `lute3-3.3.2b1/tests/unit/parse/test_SpaceDelimitedParser.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/parse/test_registry.py` & `lute3-3.3.2b1/tests/unit/parse/test_registry.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/read/render/test_RenderableCalculator.py` & `lute3-3.3.2b1/tests/unit/read/render/test_RenderableCalculator.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/read/render/test_TokenLocator.py` & `lute3-3.3.2b1/tests/unit/read/render/test_TokenLocator.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/read/test_service.py` & `lute3-3.3.2b1/tests/unit/read/test_service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/read/test_service_popup_data.py` & `lute3-3.3.2b1/tests/unit/read/test_service_popup_data.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/stats/test_service.py` & `lute3-3.3.2b1/tests/unit/stats/test_service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/term/test_Repository.py` & `lute3-3.3.2b1/tests/unit/term/test_Repository.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/term/test_TermForm.py` & `lute3-3.3.2b1/tests/unit/term/test_TermForm.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/term/test_Term_status_follow.py` & `lute3-3.3.2b1/tests/unit/term/test_Term_status_follow.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/term/test_datatables.py` & `lute3-3.3.2b1/tests/unit/term/test_datatables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/term_parent_map/test_service.py` & `lute3-3.3.2b1/tests/unit/term_parent_map/test_service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/termtag/test_datatables.py` & `lute3-3.3.2b1/tests/unit/termtag/test_datatables.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/themes/test_service.py` & `lute3-3.3.2b1/tests/unit/themes/test_service.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/utils/test_DataTablesSqliteQuery.py` & `lute3-3.3.2b1/tests/unit/utils/test_DataTablesSqliteQuery.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/unit/utils/test_formutils.py` & `lute3-3.3.2b1/tests/unit/utils/test_formutils.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/tests/utils.py` & `lute3-3.3.2b1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/utils/dump_changelog.sh` & `lute3-3.3.2b1/utils/dump_changelog.sh`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/utils/findstring.sh` & `lute3-3.3.2b1/utils/findstring.sh`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/utils/todos.py` & `lute3-3.3.2b1/utils/todos.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/utils/verify.py` & `lute3-3.3.2b1/utils/verify.py`

 * *Files identical despite different names*

### Comparing `lute3-3.3.1/PKG-INFO` & `lute3-3.3.2b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 Metadata-Version: 2.1
 Name: lute3
-Version: 3.3.1
+Version: 3.3.2b1
 Summary: Learning Using Texts
 Author-email: Jeff Zohrab <jzohrab@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: Flask-SQLAlchemy>=3.1.1,<4
 Requires-Dist: Flask-WTF>=1.2.1,<2
 Requires-Dist: natto-py>=1.0.1,<2
 Requires-Dist: jaconv>=0.3.4,<1
 Requires-Dist: platformdirs>=3.10.0,<4
 Requires-Dist: requests>=2.31.0,<3
 Requires-Dist: beautifulsoup4>=4.12.2,<5
 Requires-Dist: PyYAML>=6.0.1,<7
 Requires-Dist: toml>=0.10.2,<1
 Requires-Dist: waitress>=2.1.2,<3
-Requires-Dist: openepub>=0.0.6,<1
+Requires-Dist: openepub>=0.0.8,<1
 Requires-Dist: pypdf>=3.17.4
 Requires-Dist: subtitle-parser>=1.3.0
 Requires-Dist: coverage>=7.3.1,<8 ; extra == "dev"
 Requires-Dist: invoke>=2.2.0,<3 ; extra == "dev"
 Requires-Dist: pip>=23.0.1 ; extra == "dev"
 Requires-Dist: pipdeptree>=2.13.0,<3 ; extra == "dev"
 Requires-Dist: pylint>=2.17.5,<3 ; extra == "dev"
 Requires-Dist: pytest-bdd>=7.0.0,<8 ; extra == "dev"
 Requires-Dist: pytest-splinter>=3.3.2,<4 ; extra == "dev"
 Requires-Dist: pre-commit>=3.5.0,<4 ; extra == "dev"
 Requires-Dist: black>=23.10.1,<24 ; extra == "dev"
-Project-URL: Home, https://github.com/jzohrab/lute-v3
+Project-URL: Home, https://github.com/luteorg/lute-v3
 Provides-Extra: dev
 
 # `lute3`
 
 Learning Using Texts v3.
 
-Lute is for learning foreign languages through reading.  `lute3` is a rewrite of the original Lute PHP application in Python and Flask.
-
+Lute is for learning foreign languages through reading.  `lute3` is a rewrite of the original Lute PHP application in Python and Flask.  See the [Lute manual](https://luteorg.github.io/lute-manual/) for more detail, and notes about installation.
 
 
 ## Requirements
 
 Python 3.8+ (tested with python 3.8 through 3.11)
 
 Japanese learners will also need to install MeCab.
```

