# Comparing `tmp/sastadev-0.1.5.tar.gz` & `tmp/sastadev-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sastadev-0.1.5.tar", last modified: Wed Apr 24 10:56:23 2024, max compression
+gzip compressed data, was "sastadev-0.2.0.tar", last modified: Fri Apr 26 09:02:22 2024, max compression
```

## Comparing `sastadev-0.1.5.tar` & `sastadev-0.2.0.tar`

### file list

```diff
@@ -1,160 +1,183 @@
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.171971 sastadev-0.1.5/
--rw-r--r--   0 a3248526   (502) staff       (20)     1533 2023-05-09 07:39:30.000000 sastadev-0.1.5/LICENSE
--rw-r--r--   0 a3248526   (502) staff       (20)     3440 2024-04-24 10:56:23.171633 sastadev-0.1.5/PKG-INFO
--rw-r--r--   0 a3248526   (502) staff       (20)     3048 2023-12-06 08:36:28.000000 sastadev-0.1.5/README.md
--rw-r--r--   0 a3248526   (502) staff       (20)      328 2024-04-24 10:50:43.000000 sastadev-0.1.5/pyproject.toml
--rw-r--r--   0 a3248526   (502) staff       (20)       38 2024-04-24 10:56:23.172180 sastadev-0.1.5/setup.cfg
--rw-r--r--   0 a3248526   (502) staff       (20)      976 2024-04-24 10:52:29.000000 sastadev-0.1.5/setup.py
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.073829 sastadev-0.1.5/src/
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.094940 sastadev-0.1.5/src/sastadev/
--rw-r--r--   0 a3248526   (502) staff       (20)    13390 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/ASTApostfunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)    43480 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/CHAT_Annotation.py
--rw-r--r--   0 a3248526   (502) staff       (20)    24123 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/SAFreader.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1591 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/SRFreader.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1037 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/STAPpostfunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)     7260 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/Sziplus.py
--rw-r--r--   0 a3248526   (502) staff       (20)    10335 2023-11-09 09:41:57.000000 sastadev-0.1.5/src/sastadev/TARSPpostfunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)     5863 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/TARSPscreening.py
--rw-r--r--   0 a3248526   (502) staff       (20)       64 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/__init__.py
--rw-r--r--   0 a3248526   (502) staff       (20)    59205 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/__main__.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1338 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/allresults.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3108 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/alpino.py
--rw-r--r--   0 a3248526   (502) staff       (20)     4850 2023-11-09 09:41:57.000000 sastadev-0.1.5/src/sastadev/alpinoparsing.py
--rw-r--r--   0 a3248526   (502) staff       (20)    13788 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/asta_neo.py
--rw-r--r--   0 a3248526   (502) staff       (20)    12520 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/asta_queries.py
--rw-r--r--   0 a3248526   (502) staff       (20)    13102 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/astaforms.py
--rw-r--r--   0 a3248526   (502) staff       (20)      415 2024-03-27 15:52:57.000000 sastadev-0.1.5/src/sastadev/auchannsettings.py
--rw-r--r--   0 a3248526   (502) staff       (20)    19783 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/basicreplacements.py
--rw-r--r--   0 a3248526   (502) staff       (20)    11294 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/celexlexicon.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3667 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/checkcorrection.py
--rw-r--r--   0 a3248526   (502) staff       (20)     9634 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/cleanCHILDEStokens.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3613 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/compounds.py
--rw-r--r--   0 a3248526   (502) staff       (20)      739 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/conf.py
--rw-r--r--   0 a3248526   (502) staff       (20)      415 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/constants.py
--rw-r--r--   0 a3248526   (502) staff       (20)    57750 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/corrector.py
--rw-r--r--   0 a3248526   (502) staff       (20)    44070 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/correcttreebank.py
--rw-r--r--   0 a3248526   (502) staff       (20)      770 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/counterfunctions.py
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.096447 sastadev-0.1.5/src/sastadev/data/
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.074038 sastadev-0.1.5/src/sastadev/data/celexlexicon/
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.120083 sastadev-0.1.5/src/sastadev/data/celexlexicon/dutch/
--rw-r--r--   0 a3248526   (502) staff       (20) 10433870 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/celexlexicon/dutch/DMLCD.txt
--rw-r--r--   0 a3248526   (502) staff       (20) 11540324 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/celexlexicon/dutch/DMWCDOK.txt
--rw-r--r--   0 a3248526   (502) staff       (20)  4092534 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/celexlexicon/dutch/DSLCD.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.138367 sastadev-0.1.5/src/sastadev/data/compoundfiles/
--rw-r--r--   0 a3248526   (502) staff       (20)  4216927 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/compoundfiles/Ncompounds-attempt1.txt
--rw-r--r--   0 a3248526   (502) staff       (20)  1403658 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/compoundfiles/Ncompounds-attempt2.txt
--rw-r--r--   0 a3248526   (502) staff       (20)   332732 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/compoundfiles/Ncompounds-attempt2.zip
--rw-r--r--   0 a3248526   (502) staff       (20)      390 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/expandedqueries.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.141275 sastadev-0.1.5/src/sastadev/data/filledpauseslexicon/
--rw-r--r--   0 a3248526   (502) staff       (20)      145 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/filledpauseslexicon/filledpauseslexicon.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.142794 sastadev-0.1.5/src/sastadev/data/form_templates/
--rw-r--r--   0 a3248526   (502) staff       (20)    48437 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/form_templates/STAP Excel VUmc 2018.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    13350 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/form_templates/TARSP Form Current.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)   111180 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/data/inflectioncorrection.tsv.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.144955 sastadev-0.1.5/src/sastadev/data/macros/
--rw-r--r--   0 a3248526   (502) staff       (20)    10249 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/data/macros/newimperatives.txt
--rw-r--r--   0 a3248526   (502) staff       (20)    21148 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/data/macros/sastamacros1.txt
--rw-r--r--   0 a3248526   (502) staff       (20)    10375 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/macros/sastamacros2.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.149948 sastadev-0.1.5/src/sastadev/data/methods/
--rw-r--r--   0 a3248526   (502) staff       (20)    12471 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/methods/ASTA_07062021.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    12808 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/data/methods/ASTA_Index_Current.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    17518 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/methods/STAP_07062021.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    17695 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/data/methods/STAP_Index_Current.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    25892 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/methods/TARSP Index 2022-01-07.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    26134 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/data/methods/TARSP Index Current.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    26318 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/methods/TARSP_07062021.xlsx
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.151737 sastadev-0.1.5/src/sastadev/data/names/
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.159413 sastadev-0.1.5/src/sastadev/data/names/Woonplaatsen/
--rw-r--r--   0 a3248526   (502) staff       (20)   406828 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/names/Woonplaatsen/83958NED_TypedDataSet_19062020_173530.csv
--rw-r--r--   0 a3248526   (502) staff       (20)   406828 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/names/Woonplaatsen/83958NED_UntypedDataSet_19062020_173456.csv
--rw-r--r--   0 a3248526   (502) staff       (20)    66586 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/names/Woonplaatsen/83958NED_metadata.csv
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.162182 sastadev-0.1.5/src/sastadev/data/names/fn10k_versie1/
--rw-r--r--   0 a3248526   (502) staff       (20)  1088716 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/names/fn10k_versie1/fn_10kw.xml
--rw-r--r--   0 a3248526   (502) staff       (20)     1442 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/names/fn10k_versie1/fn_10kw.xsl
--rw-r--r--   0 a3248526   (502) staff       (20)   134136 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/names/fn10k_versie1.zip
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.163529 sastadev-0.1.5/src/sastadev/data/names/hoofdsteden/
--rw-r--r--   0 a3248526   (502) staff       (20)     8762 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden.csv
--rw-r--r--   0 a3248526   (502) staff       (20)     7950 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden_raw.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.164135 sastadev-0.1.5/src/sastadev/data/names/nameparts/
--rw-r--r--   0 a3248526   (502) staff       (20)   104652 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/names/nameparts/namepartlexicon.csv
--rw-r--r--   0 a3248526   (502) staff       (20)  2160410 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/data/names/voornamentop10000.xml
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.164863 sastadev-0.1.5/src/sastadev/data/top3000/
--rw-r--r--   0 a3248526   (502) staff       (20)   186224 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/data/top3000/Woordenlijsten Current.xlsx
--rw-r--r--   0 a3248526   (502) staff       (20)    35888 2023-11-09 09:41:57.000000 sastadev-0.1.5/src/sastadev/dedup.py
--rw-r--r--   0 a3248526   (502) staff       (20)    23956 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/deregularise.py
--rw-r--r--   0 a3248526   (502) staff       (20)     7380 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/exampletrees.py
--rw-r--r--   0 a3248526   (502) staff       (20)      993 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/expandquery.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3652 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/external_functions.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1630 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/filefunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)     9032 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/find_ngram.py
--rw-r--r--   0 a3248526   (502) staff       (20)      473 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/forms.py
--rw-r--r--   0 a3248526   (502) staff       (20)     6814 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/generatemacros.py
--rw-r--r--   0 a3248526   (502) staff       (20)     5251 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/goldcountreader.py
--rw-r--r--   0 a3248526   (502) staff       (20)    17456 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/iedims.py
--rw-r--r--   0 a3248526   (502) staff       (20)     5275 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/imperatives.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1366 2024-04-16 10:12:10.000000 sastadev-0.1.5/src/sastadev/imply.py
--rw-r--r--   0 a3248526   (502) staff       (20)     5485 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/lexicon.py
--rw-r--r--   0 a3248526   (502) staff       (20)    18574 2024-03-27 15:55:43.000000 sastadev-0.1.5/src/sastadev/longqueries.py
--rw-r--r--   0 a3248526   (502) staff       (20)      959 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/macrolength.py
--rw-r--r--   0 a3248526   (502) staff       (20)     2831 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/macros.py
--rw-r--r--   0 a3248526   (502) staff       (20)      321 2024-04-16 09:53:39.000000 sastadev-0.1.5/src/sastadev/memoize.py
--rw-r--r--   0 a3248526   (502) staff       (20)     6445 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/metadata.py
--rw-r--r--   0 a3248526   (502) staff       (20)      583 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/methodinfo.py
--rw-r--r--   0 a3248526   (502) staff       (20)     5541 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/methods.py
--rw-r--r--   0 a3248526   (502) staff       (20)    11651 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/mismatches.py
--rw-r--r--   0 a3248526   (502) staff       (20)     9027 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/mksilver.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1542 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/mwe2pep.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1462 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/namepartlexicon.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1028 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/phonetics.py
--rw-r--r--   0 a3248526   (502) staff       (20)        0 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/py.typed
--rw-r--r--   0 a3248526   (502) staff       (20)     2154 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/query.py
--rw-r--r--   0 a3248526   (502) staff       (20)     5735 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/queryfunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3254 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/rawalpinoparsing.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1718 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/readcsv.py
--rw-r--r--   0 a3248526   (502) staff       (20)     7724 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/readmethod.py
--rw-r--r--   0 a3248526   (502) staff       (20)     7608 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/reduceresults.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1954 2024-03-27 15:58:14.000000 sastadev-0.1.5/src/sastadev/resultsbyutterance.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1599 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/rpf1.py
--rw-r--r--   0 a3248526   (502) staff       (20)    14042 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/sasta_explanation.py
--rw-r--r--   0 a3248526   (502) staff       (20)     2973 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/sastatok.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1975 2024-04-16 08:16:53.000000 sastadev-0.1.5/src/sastadev/sastatoken.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3470 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/sastatypes.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1329 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/sentence_parser.py
--rw-r--r--   0 a3248526   (502) staff       (20)    13468 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/smallclauses.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3912 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/smartcompoundcomparison.py
--rw-r--r--   0 a3248526   (502) staff       (20)     3358 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/stapforms.py
--rw-r--r--   0 a3248526   (502) staff       (20)    16358 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/stringfunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)    31189 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/sva.py
--rw-r--r--   0 a3248526   (502) staff       (20)     6535 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/syllablecount.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1614 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/targets.py
--rw-r--r--   0 a3248526   (502) staff       (20)     4692 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/tarspform.py
--rw-r--r--   0 a3248526   (502) staff       (20)     6434 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/tblex.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1475 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/tokeniseCHILDES.py
--rw-r--r--   0 a3248526   (502) staff       (20)      880 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/tokenmd.py
--rw-r--r--   0 a3248526   (502) staff       (20)     4341 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/top3000.py
--rw-r--r--   0 a3248526   (502) staff       (20)    78257 2024-04-24 10:50:43.000000 sastadev-0.1.5/src/sastadev/treebankfunctions.py
--rw-r--r--   0 a3248526   (502) staff       (20)     2117 2024-04-24 10:52:29.000000 sastadev-0.1.5/src/sastadev/xenx.py
--rw-r--r--   0 a3248526   (502) staff       (20)     5144 2023-08-29 13:46:10.000000 sastadev-0.1.5/src/sastadev/xlsx.py
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.096002 sastadev-0.1.5/src/sastadev.egg-info/
--rw-r--r--   0 a3248526   (502) staff       (20)     3440 2024-04-24 10:56:23.000000 sastadev-0.1.5/src/sastadev.egg-info/PKG-INFO
--rw-r--r--   0 a3248526   (502) staff       (20)     4378 2024-04-24 10:56:23.000000 sastadev-0.1.5/src/sastadev.egg-info/SOURCES.txt
--rw-r--r--   0 a3248526   (502) staff       (20)        1 2024-04-24 10:56:23.000000 sastadev-0.1.5/src/sastadev.egg-info/dependency_links.txt
--rw-r--r--   0 a3248526   (502) staff       (20)       52 2024-04-24 10:56:23.000000 sastadev-0.1.5/src/sastadev.egg-info/entry_points.txt
--rw-r--r--   0 a3248526   (502) staff       (20)       51 2024-04-24 10:56:23.000000 sastadev-0.1.5/src/sastadev.egg-info/requires.txt
--rw-r--r--   0 a3248526   (502) staff       (20)        9 2024-04-24 10:56:23.000000 sastadev-0.1.5/src/sastadev.egg-info/top_level.txt
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:23.807681 sastadev-0.1.5/tests/
-drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-24 10:56:26.035742 sastadev-0.1.5/tests/__pycache__/
--rw-r--r--   0 a3248526   (502) staff       (20)    15132 2024-04-24 10:56:23.812023 sastadev-0.1.5/tests/__pycache__/test_adjacency.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)     1317 2024-04-24 10:56:23.835137 sastadev-0.1.5/tests/__pycache__/test_explanation.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)     2655 2024-04-24 10:56:25.452252 sastadev-0.1.5/tests/__pycache__/test_hyphens.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)     7255 2024-04-24 10:56:25.453285 sastadev-0.1.5/tests/__pycache__/test_indexexpansion.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)     6907 2024-04-24 10:56:25.455009 sastadev-0.1.5/tests/__pycache__/test_lxml.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)     2145 2024-04-24 10:56:25.457678 sastadev-0.1.5/tests/__pycache__/test_smallclauses.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)    15020 2024-04-24 10:56:26.035570 sastadev-0.1.5/tests/__pycache__/test_vobij.cpython-38-pytest-7.4.0.pyc
--rw-r--r--   0 a3248526   (502) staff       (20)    13386 2023-08-29 13:46:10.000000 sastadev-0.1.5/tests/test_adjacency.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1345 2024-04-24 10:50:43.000000 sastadev-0.1.5/tests/test_explanation.py
--rw-r--r--   0 a3248526   (502) staff       (20)      634 2023-08-29 13:46:10.000000 sastadev-0.1.5/tests/test_hyphens.py
--rw-r--r--   0 a3248526   (502) staff       (20)     6946 2023-08-29 13:46:10.000000 sastadev-0.1.5/tests/test_indexexpansion.py
--rw-r--r--   0 a3248526   (502) staff       (20)     7187 2023-08-29 13:46:10.000000 sastadev-0.1.5/tests/test_lxml.py
--rw-r--r--   0 a3248526   (502) staff       (20)     1971 2023-08-29 13:46:10.000000 sastadev-0.1.5/tests/test_smallclauses.py
--rw-r--r--   0 a3248526   (502) staff       (20)    14153 2023-08-29 13:46:10.000000 sastadev-0.1.5/tests/test_vobij.py
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.631200 sastadev-0.2.0/
+-rw-r--r--   0 a3248526   (502) staff       (20)     1533 2023-05-09 07:39:30.000000 sastadev-0.2.0/LICENSE
+-rw-r--r--   0 a3248526   (502) staff       (20)     3440 2024-04-26 09:02:22.630978 sastadev-0.2.0/PKG-INFO
+-rw-r--r--   0 a3248526   (502) staff       (20)     3048 2023-12-06 08:36:28.000000 sastadev-0.2.0/README.md
+-rw-r--r--   0 a3248526   (502) staff       (20)      375 2024-04-26 09:00:24.000000 sastadev-0.2.0/pyproject.toml
+-rw-r--r--   0 a3248526   (502) staff       (20)       38 2024-04-26 09:02:22.631264 sastadev-0.2.0/setup.cfg
+-rw-r--r--   0 a3248526   (502) staff       (20)      976 2024-04-26 09:00:36.000000 sastadev-0.2.0/setup.py
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.579544 sastadev-0.2.0/src/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.594257 sastadev-0.2.0/src/sastadev/
+-rw-r--r--   0 a3248526   (502) staff       (20)    11603 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/ASTApostfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    43549 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/CHAT_Annotation.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    22704 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/SAFreader.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     2303 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/SRFreader.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1163 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/STAPpostfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7260 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/Sziplus.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    10335 2023-11-09 09:41:57.000000 sastadev-0.2.0/src/sastadev/TARSPpostfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5863 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/TARSPscreening.py
+-rw-r--r--   0 a3248526   (502) staff       (20)       64 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/__init__.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    62496 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/__main__.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3381 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/allresults.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3108 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/alpino.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     4850 2023-11-09 09:41:57.000000 sastadev-0.2.0/src/sastadev/alpinoparsing.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1480 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/anonymization.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    13788 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/asta_neo.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    14736 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/asta_queries.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    15340 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/astaforms.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      415 2024-03-27 15:52:57.000000 sastadev-0.2.0/src/sastadev/auchannsettings.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    25155 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/basicreplacements.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    11294 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/celexlexicon.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     8474 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/chatundo.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3667 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/checkcorrection.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     9671 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/cleanCHILDEStokens.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3613 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/compounds.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      783 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/conf.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      494 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/constants.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    60201 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/corrector.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    44303 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/correcttreebank.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      770 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/counterfunctions.py
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.596117 sastadev-0.2.0/src/sastadev/data/
+-rw-r--r--   0 a3248526   (502) staff       (20)     5819 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/DutchIrregularVerbs.tsv
+-rw-r--r--   0 a3248526   (502) staff       (20)     1562 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/anonymization.json
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.579852 sastadev-0.2.0/src/sastadev/data/celexlexicon/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.610416 sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/
+-rw-r--r--   0 a3248526   (502) staff       (20) 10433870 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/DMLCD.txt
+-rw-r--r--   0 a3248526   (502) staff       (20) 11540324 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/DMWCDOK.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)  4092534 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/DSLCD.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.617302 sastadev-0.2.0/src/sastadev/data/compoundfiles/
+-rw-r--r--   0 a3248526   (502) staff       (20)  4216927 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/compoundfiles/Ncompounds-attempt1.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)  1403658 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/compoundfiles/Ncompounds-attempt2.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)   332732 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/compoundfiles/Ncompounds-attempt2.zip
+-rw-r--r--   0 a3248526   (502) staff       (20)      390 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/expandedqueries.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.620892 sastadev-0.2.0/src/sastadev/data/filledpauseslexicon/
+-rw-r--r--   0 a3248526   (502) staff       (20)      145 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/filledpauseslexicon/filledpauseslexicon.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)      495 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/filledpauseslexicon/notanalyzewords.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)      113 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/filledpauseslexicon/oldfilledpauseslexicon.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)       60 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/filledpauseslexicon/vuwordslexicon.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.621409 sastadev-0.2.0/src/sastadev/data/form_templates/
+-rw-r--r--   0 a3248526   (502) staff       (20)    48437 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/form_templates/STAP Excel VUmc 2018.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    13350 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/form_templates/TARSP Form Current.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)   159165 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/inflectioncorrection.tsv.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.622289 sastadev-0.2.0/src/sastadev/data/macros/
+-rw-r--r--   0 a3248526   (502) staff       (20)    12994 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/macros/newimperatives.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)      388 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/macros/newrobusthwwi.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)    23141 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/macros/sastamacros1.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)    10375 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/macros/sastamacros2.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.623706 sastadev-0.2.0/src/sastadev/data/methods/
+-rw-r--r--   0 a3248526   (502) staff       (20)    12471 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/methods/ASTA_07062021.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    12824 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/methods/ASTA_Index_Current.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    12808 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/methods/ASTA_Index_Current_old.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    17518 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/methods/STAP_07062021.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    17537 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/methods/STAP_Index_Current.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    25892 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/methods/TARSP Index 2022-01-07.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    26318 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/methods/TARSP_07062021.xlsx
+-rw-r--r--   0 a3248526   (502) staff       (20)    25871 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/methods/TARSP_Index_Current.xlsx
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.624636 sastadev-0.2.0/src/sastadev/data/names/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.626880 sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/
+-rw-r--r--   0 a3248526   (502) staff       (20)   406828 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/83958NED_TypedDataSet_19062020_173530.csv
+-rw-r--r--   0 a3248526   (502) staff       (20)   406828 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/83958NED_UntypedDataSet_19062020_173456.csv
+-rw-r--r--   0 a3248526   (502) staff       (20)    66586 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/83958NED_metadata.csv
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.627905 sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1/
+-rw-r--r--   0 a3248526   (502) staff       (20)  1088716 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1/fn_10kw.xml
+-rw-r--r--   0 a3248526   (502) staff       (20)     1442 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1/fn_10kw.xsl
+-rw-r--r--   0 a3248526   (502) staff       (20)   134136 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1.zip
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.628229 sastadev-0.2.0/src/sastadev/data/names/hoofdsteden/
+-rw-r--r--   0 a3248526   (502) staff       (20)     8762 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden.csv
+-rw-r--r--   0 a3248526   (502) staff       (20)     7950 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden_raw.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.628387 sastadev-0.2.0/src/sastadev/data/names/nameparts/
+-rw-r--r--   0 a3248526   (502) staff       (20)   104652 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/nameparts/namepartlexicon.csv
+-rw-r--r--   0 a3248526   (502) staff       (20)  2160410 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/data/names/voornamentop10000.xml
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.628611 sastadev-0.2.0/src/sastadev/data/nochildwords/
+-rw-r--r--   0 a3248526   (502) staff       (20)        5 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/nochildwords/nochildwords.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)   108483 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/old_inflectioncorrection.tsv.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.628755 sastadev-0.2.0/src/sastadev/data/top3000/
+-rw-r--r--   0 a3248526   (502) staff       (20)   187619 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/top3000/Woordenlijsten Current.xlsx
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.629015 sastadev-0.2.0/src/sastadev/data/wordsunknowntoalpino/
+-rw-r--r--   0 a3248526   (502) staff       (20)      140 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/data/wordsunknowntoalpino/wordsunknowntoalpino.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)    35888 2023-11-09 09:41:57.000000 sastadev-0.2.0/src/sastadev/dedup.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    24636 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/deregularise.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7380 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/exampletrees.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      993 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/expandquery.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3793 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/external_functions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1630 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/filefunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     9032 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/find_ngram.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      473 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/forms.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6814 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/generatemacros.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5251 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/goldcountreader.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    17456 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/iedims.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5607 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/imperatives.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1366 2024-04-16 10:12:10.000000 sastadev-0.2.0/src/sastadev/imply.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6653 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/lexicon.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    18574 2024-03-27 15:55:43.000000 sastadev-0.2.0/src/sastadev/longqueries.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      959 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/macrolength.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     2831 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/macros.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      321 2024-04-16 09:53:39.000000 sastadev-0.2.0/src/sastadev/memoize.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6478 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/metadata.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      583 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/methodinfo.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7016 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/methods.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    14928 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/mismatches.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     9027 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/mksilver.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1542 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/mwe2pep.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    60916 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/mysastadev.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1462 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/namepartlexicon.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    17785 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/normalise_lemma.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1028 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/phonetics.py
+-rw-r--r--   0 a3248526   (502) staff       (20)        0 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/py.typed
+-rw-r--r--   0 a3248526   (502) staff       (20)     2276 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/query.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6157 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/queryfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3281 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/rawalpinoparsing.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1718 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/readcsv.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7826 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/readmethod.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7720 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/reduceresults.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1954 2024-03-27 15:58:14.000000 sastadev-0.2.0/src/sastadev/resultsbyutterance.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1599 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/rpf1.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    14312 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/sasta_explanation.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    13568 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/sastacore.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     2988 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/sastatok.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1975 2024-04-16 08:16:53.000000 sastadev-0.2.0/src/sastadev/sastatoken.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3243 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/sastatypes.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1329 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/sentence_parser.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    13555 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/smallclauses.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3869 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/smartcompoundcomparison.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     3540 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/stapforms.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    16421 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/stringfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    31189 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/sva.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6564 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/syllablecount.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1614 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/targets.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     4846 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/tarspform.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6435 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/tblex.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1475 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/tokeniseCHILDES.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      880 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/tokenmd.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     4341 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/top3000.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    81828 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/treebankfunctions.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      299 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/tryderegularize.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1108 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/tryexcelfilter.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      561 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/trygaatie.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1076 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/update_inflectioncorrection.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1994 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/vuandnonwords.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1523 2024-04-26 09:00:24.000000 sastadev-0.2.0/src/sastadev/vunonwordlexicons.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     2117 2024-04-24 10:52:29.000000 sastadev-0.2.0/src/sastadev/xenx.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     5144 2023-08-29 13:46:10.000000 sastadev-0.2.0/src/sastadev/xlsx.py
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:22.594992 sastadev-0.2.0/src/sastadev.egg-info/
+-rw-r--r--   0 a3248526   (502) staff       (20)     3440 2024-04-26 09:02:22.000000 sastadev-0.2.0/src/sastadev.egg-info/PKG-INFO
+-rw-r--r--   0 a3248526   (502) staff       (20)     5234 2024-04-26 09:02:22.000000 sastadev-0.2.0/src/sastadev.egg-info/SOURCES.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)        1 2024-04-26 09:02:22.000000 sastadev-0.2.0/src/sastadev.egg-info/dependency_links.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)       52 2024-04-26 09:02:22.000000 sastadev-0.2.0/src/sastadev.egg-info/entry_points.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)       51 2024-04-26 09:02:22.000000 sastadev-0.2.0/src/sastadev.egg-info/requires.txt
+-rw-r--r--   0 a3248526   (502) staff       (20)        9 2024-04-26 09:02:22.000000 sastadev-0.2.0/src/sastadev.egg-info/top_level.txt
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:23.202918 sastadev-0.2.0/tests/
+drwxr-xr-x   0 a3248526   (502) staff       (20)        0 2024-04-26 09:02:25.294840 sastadev-0.2.0/tests/__pycache__/
+-rw-r--r--   0 a3248526   (502) staff       (20)    15132 2024-04-26 09:02:23.206920 sastadev-0.2.0/tests/__pycache__/test_adjacency.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     1316 2024-04-26 09:02:23.235139 sastadev-0.2.0/tests/__pycache__/test_explanation.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     2655 2024-04-26 09:02:24.739838 sastadev-0.2.0/tests/__pycache__/test_hyphens.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     7255 2024-04-26 09:02:24.740787 sastadev-0.2.0/tests/__pycache__/test_indexexpansion.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     6907 2024-04-26 09:02:24.742413 sastadev-0.2.0/tests/__pycache__/test_lxml.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)     2145 2024-04-26 09:02:24.744441 sastadev-0.2.0/tests/__pycache__/test_smallclauses.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)    15020 2024-04-26 09:02:25.294693 sastadev-0.2.0/tests/__pycache__/test_vobij.cpython-38-pytest-7.4.0.pyc
+-rw-r--r--   0 a3248526   (502) staff       (20)    13386 2023-08-29 13:46:10.000000 sastadev-0.2.0/tests/test_adjacency.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1438 2024-04-26 09:00:24.000000 sastadev-0.2.0/tests/test_explanation.py
+-rw-r--r--   0 a3248526   (502) staff       (20)      634 2023-08-29 13:46:10.000000 sastadev-0.2.0/tests/test_hyphens.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     6946 2023-08-29 13:46:10.000000 sastadev-0.2.0/tests/test_indexexpansion.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     7187 2023-08-29 13:46:10.000000 sastadev-0.2.0/tests/test_lxml.py
+-rw-r--r--   0 a3248526   (502) staff       (20)     1971 2023-08-29 13:46:10.000000 sastadev-0.2.0/tests/test_smallclauses.py
+-rw-r--r--   0 a3248526   (502) staff       (20)    14153 2023-08-29 13:46:10.000000 sastadev-0.2.0/tests/test_vobij.py
```

### Comparing `sastadev-0.1.5/LICENSE` & `sastadev-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/PKG-INFO` & `sastadev-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sastadev
-Version: 0.1.5
+Version: 0.2.0
 Summary: Linguistic functions for SASTA tool
 Home-page: https://github.com/UUDigitalHumanitieslab/sastadev
 Author: Research Software Lab - Centre for Digital Humanities - Utrecht University
 Author-email: digitalhumanities@uu.nl
 License: BSD-3-Clause
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `sastadev-0.1.5/README.md` & `sastadev-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/setup.py` & `sastadev-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 
 setup(
     name='sastadev',
-    version='0.1.5',
+    version='0.2.0',
     description='Linguistic functions for SASTA tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/UUDigitalHumanitieslab/sastadev',
     author='Research Software Lab - Centre for Digital Humanities - Utrecht University',
     author_email='digitalhumanities@uu.nl',
     package_dir={'': 'src'},
```

### Comparing `sastadev-0.1.5/src/sastadev/ASTApostfunctions.py` & `sastadev-0.2.0/src/sastadev/ASTApostfunctions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import Counter
 from copy import deepcopy
 from typing import Dict, List, Optional, Tuple
 
-from sastadev.allresults import AllResults
+from sastadev.allresults import AllResults, ResultsKey, mkresultskey
 from sastadev.lexicon import getwordinfo, getwordposinfo
-from sastadev.sastatypes import Position, QId, SynTree, UttId
+from sastadev.sastatypes import Position, SynTree, UttId
 from sastadev.stringfunctions import getallrealwords, realwordstring
 from sastadev.treebankfunctions import getattval, getnodeyield
 
 lpad = 3
 zero = '0'
 astamaxwordcount = 300
 
@@ -21,16 +21,31 @@
 pvqid = 'A024'
 delpvqid = 'A009'
 subpvqid = 'A032'
 kqid = 'A013'
 mqid = 'A020'
 tijdfoutpvqid = 'A041'
 nounlemmaqid = 'A046'
+formqid = 'A047'
 verblemmaqid = 'A049'
 
+nounreskey = mkresultskey(nounqid)
+lexreskey = mkresultskey(lexqid)
+
+samplesizereskey = mkresultskey(samplesizeqid)
+mluxreskey = mkresultskey(mluxqid)
+
+pvreskey = mkresultskey(pvqid)
+delpvreskey = mkresultskey(delpvqid)
+subpvreskey = mkresultskey(subpvqid)
+tijdfoutpvreskey = mkresultskey(tijdfoutpvqid)
+kreskey = mkresultskey(kqid)
+mreskey = mkresultskey(mqid)
+formreskey = mkresultskey(formqid)
+
 specialform = 'Special Form'
 errormarking = 'Error Marking'
 
 #: The varibale (constant) *mdnamemdxpathtemplate* is an Xpath template to find
 #: metadata (xmeta) with  name=*mdname* and value=*mdvalue*
 mdnamemdxpathtemplate = """.//xmeta[@name="{mdname}" and @value="{mdvalue}"]"""
 
@@ -104,17 +119,17 @@
 
 
 def wordcountperutt(allresults):
     lemmas = getalllemmas(allresults)
     wordcounts = {uttid: sum(ctr.values()) for uttid, ctr in lemmas.items()}
     ignorewordcounts = deepcopy(
         allresults.coreresults[
-            samplesizeqid]) if samplesizeqid in allresults.coreresults else Counter()  # samplesize
+            samplesizereskey]) if samplesizereskey in allresults.coreresults else Counter()  # samplesize
     ignorewordcounts += allresults.coreresults[
-        mluxqid] if mluxqid in allresults.coreresults else Counter()  # mlux
+        mluxreskey] if mluxreskey in allresults.coreresults else Counter()  # mlux
     # ignorewordcounts += allresults.coreresults['A050'] if 'A050' in allresults.coreresults else Counter() # echolalie covered by mlux
     result = {}
     for uttid in wordcounts:
         tosubtract = ignorewordcounts[uttid] if uttid in ignorewordcounts else 0
         result[uttid] = wordcounts[uttid] - tosubtract
     # remove uttids which have 0 words
     result = {uttid: ctr for uttid, ctr in result.items() if ctr != 0}
@@ -152,47 +167,47 @@
     return result
 
 
 def getcutoffpoint(allresults: AllResults, uttid: UttId, diff: int) -> int:
     theutt = allresults.allutts[uttid]
     final = diff
     for i, w in enumerate(theutt):
-        if (uttid, i + 1) in allresults.exactresults[samplesizeqid]:
+        if (uttid, i + 1) in allresults.exactresults[samplesizereskey]:
             final += 1
         if i + 1 == final:
             break
     return final
 
 
 def finietheidsindex(allresults, _):
     allpvs = allresults.coreresults[
-        pvqid] if pvqid in allresults.coreresults else Counter()
+        pvreskey] if pvreskey in allresults.coreresults else Counter()
     subpvs = allresults.coreresults[
-        subpvqid] if subpvqid in allresults.coreresults else Counter()
+        subpvreskey] if subpvreskey in allresults.coreresults else Counter()
     delpvs = allresults.coreresults[
-        delpvqid] if delpvqid in allresults.coreresults else Counter()
+        delpvreskey] if delpvreskey in allresults.coreresults else Counter()
     tijdfoutpvs = allresults.coreresults[
-        tijdfoutpvqid] if tijdfoutpvqid in allresults.coreresults else Counter()
+        tijdfoutpvreskey] if tijdfoutpvreskey in allresults.coreresults else Counter()
     foutepvs = subpvs + delpvs + tijdfoutpvs
     allpvcount = sumctr(allpvs)
     foutepvcount = sumctr(foutepvs)
     okpvcount = allpvcount - foutepvcount
     if allpvcount == 0:
         result = 0
     else:
         result = okpvcount / allpvcount
     return result
 
 
 def countwordsandcutoff(allresults, _):
     # @@to be adapted
     result = (None, 0)
-    if 'A047' in allresults.postresults:
+    if formreskey in allresults.postresults:
         paddedlist = []
-        for key, val in allresults.postresults['A047'].items():
+        for key, val in allresults.postresults[formreskey].items():
             paddedkey = key.rjust(lpad, zero)
             paddedlist.append((paddedkey, val))
         sortedlist = sorted(paddedlist)
         wc = 0
         for key, val in sortedlist:
             if wc + val > astamaxwordcount:
                 result = (key, wc)
@@ -201,61 +216,48 @@
                 wc += val
                 result = (None, wc)
     return result
 
 
 def KMcount(allresults, _):
     Kcount = sumctr(
-        allresults.coreresults[kqid]) if kqid in allresults.coreresults else 0
+        allresults.coreresults[kreskey]) if kreskey in allresults.coreresults else 0
     Mcount = sumctr(
         allresults.coreresults[mqid]) if mqid in allresults.coreresults else 0
     result = Kcount + Mcount
     return result
 
 
-def old_old_getlemmas(allresults, _):
-    allmatches = allresults.allmatches
-    allresults.postresults['A046'] = Counter()
-    for el in allmatches:
-        (qid, uttid) = el
-        if qid in ['A021', 'A018']:
-            for amatch in allmatches[el]:
-                # theword = normalizedword(amatch[0])
-                theword = getattval(amatch[0], 'lemma')
-                allresults.postresults['A046'].update([(theword, uttid)])
-    return allresults
-
-
-def getlemmas(allresults, _):
-    result = getcondlemmas(allresults, _, lambda qid: qid in [nounqid, lexqid])
-    return result
+# def getlemmas(allresults, _):
+#    result = getcondlemmas(allresults, _, lambda reskey: reskey in [nounreskey, lexreskey])
+#    return result
 
 
 def getnounlemmas(allresults, _):
     '''
     The function *getnounlemmas* uses the function *getposlemmas* applied to
     *allresults* and the query identifier for nouns to obtain the lemmas
     for nouns.
 
     .. autofunction:: ASTApostfunctions::getposlemmas
 
     '''
-    result = getposlemmas(allresults, nounqid)
+    result = getposlemmas(allresults, nounreskey)
     return result
 
 
 def getlexlemmas(allresults, _):
     '''
     The function *getlexlemmas* uses the function *getposlemmas* applied to
     *allresults* and the query identifier for lexical verbs to obtain the lemmas
     for lexical verbs.
 
     .. autofunction:: ASTApostfunctions::getposlemmas
     '''
-    result = getposlemmas(allresults, lexqid)
+    result = getposlemmas(allresults, lexreskey)
     return result
 
 
 def realword(node):
     result = getattval(node, 'pt') not in ['let']
     return result
 
@@ -272,99 +274,45 @@
             # uttid = getuttid(syntree)
             lemmas = [getattval(node, 'lemma') for node in getnodeyield(syntree) if
                       realword(node)]
             result[uttid] = Counter(lemmas)
     return result
 
 
-def old_getlemmas(allresults, _):
-    allmatches = allresults.allmatches
-    result = Counter()
-    for el in allmatches:
-        (qid, uttid) = el
-        if qid in ['A021', 'A018']:
-            for amatch in allmatches[el]:
-                # theword = normalizedword(amatch[0])
-                theword = getattval(amatch[0], 'lemma')
-                result.update([(theword, uttid)])
-    return result
-
-
-def oldgetcondlemmas(allresults, _, cond):
-    allmatches = allresults.allmatches
-    result = Counter()
-    for el in allmatches:
-        (qid, uttid) = el
-        if cond(qid):
-            for amatch in allmatches[el]:
-                # theword = normalizedword(amatch[0])
-                theword = getattval(amatch[0], 'lemma')
-                result.update([(theword, uttid)])
-    return result
-
-
-# not used anymore, contains an error
-def getcondlemmas(allresults, _, cond):
-    result = Counter()
-    if allresults.annotationinput:
-        for qid in allresults.exactresults:
-            if cond(qid):
-                for (uttid, position) in allresults.exactresults[qid]:
-                    word = allresults.allutts[uttid][position - 1]
-                    if qid == 'A021':
-                        pos = 'n'
-                    elif qid == 'A018':
-                        pos = 'ww'
-                    else:
-                        pos = None
-                    lemma = bgetlemma(word, pos)
-                    result.update([(lemma, qid, uttid)])
-
-    else:
-        allmatches = allresults.allmatches
-        for el in allmatches:
-            (qid, uttid) = el
-            if cond(qid):
-                for amatch in allmatches[el]:
-                    # theword = normalizedword(amatch[0])
-                    theword = getattval(amatch[0], 'lemma')
-                    result.update([(theword, uttid)])
-    return result
-
-
 def getposfromqid(qid):
     if qid == 'A021':
         pos = 'n'
     elif qid == 'A018':
         pos = 'ww'
     else:
         pos = None
     return pos
 
 
-def getposlemmas(allresults: AllResults, posqid: QId) -> List[Tuple[str, UttId]]:
+def getposlemmas(allresults: AllResults, posreskey: ResultsKey) -> List[Tuple[str, UttId]]:
     '''
     The function *getposlemmas* obtains the lemmas from *allresults* that have been
-    found by a query with identifier *posqid*.
+    found by a query with identifier *posreskey*.
 
     The lemma is obtained from the parse tree if there is one, otherwise (in case the
     input was an annotation form) from the lexicon (CELEX).
     '''
     result = Counter()
     if allresults.annotationinput:
-        for (uttid, position) in allresults.exactresults[posqid]:
+        for (uttid, position) in allresults.exactresults[posreskey]:
             word = allresults.allutts[uttid][position - 1]
+            posqid = posreskey[0]
             pos = getposfromqid(posqid)
             lemma = bgetlemma(word, pos)
             result.update([(lemma, uttid)])
     else:
         allmatches = allresults.allmatches
         for el in allmatches:
-            (qid, uttid) = el
-            if qid == posqid:
+            (reskey, uttid) = el
+            if reskey == posreskey:
                 for amatch in allmatches[el]:
                     # theword = normalizedword(amatch[0])
                     theword = getattval(amatch[0], 'lemma')
                     result.update([(theword, uttid)])
     return result
```

### Comparing `sastadev-0.1.5/src/sastadev/CHAT_Annotation.py` & `sastadev-0.2.0/src/sastadev/CHAT_Annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 
 from sastadev import cleanCHILDEStokens
+# import sastadev.cleanCHILDEStokens
 from sastadev.conf import settings
 from sastadev.metadata import Meta, bpl_delete, bpl_replacement
 from sastadev.sastatoken import Token, show
 
 CHAT = 'CHAT'
 
 CHAT_explanation = 'Explanation'
@@ -58,16 +59,17 @@
     r'[\w:\^\+_~\'\-\(\)' + \
     u'\u2019\u02C8\u02CC\u0329\u02de\u21AB\u2260' + r']*'
 simplewordpat = r'\w+'
 fullwordpat = fullre(wordpat)
 wordre = re.compile(fullwordpat)
 # interpunction = r'(:?' + r'[!\?\.,;]' + '|' + u'[\u201C\u201D\u2039\u203A]' + r'|' + r'(?<=\s):' + r')'
 interpunction = r'\-\-\-|\-\-|\-|\-' + r'|' + \
-    r'[!\?\.,;]' + '|' + \
-    u'[\u2013\u2014\u2015\u201C\u201D\u2039\u203A]' + r'|' + r'(?<=\s):'
+                r'[!\?\.,;]' + '|' + \
+                u'[\u2013\u2014\u2015\u201C\u201D\u2039\u203A]' + \
+    r'|' + r'(?<=\s):'
 filenamepat = r'[\w\.]+'
 fullfilenamepat = fullre(filenamepat)
 fullfilenamere = re.compile(fullfilenamepat)
 
 wordorpuncpat = r'(:?' + wordpat + '|' + interpunction + ')'
 
 specialformpat = wordpat + r'(?:@z:\w\w\w|@\w\w?\w?)'
```

### Comparing `sastadev-0.1.5/src/sastadev/SAFreader.py` & `sastadev-0.2.0/src/sastadev/SAFreader.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,44 +11,49 @@
 # =codes written without spaces?
 
 import re
 from collections import Counter, defaultdict
 from typing import Any, Dict, List, Match, Optional, Pattern, Tuple
 
 from sastadev import xlsx
+from sastadev.allresults import ResultsKey, mkresultskey
+from sastadev.anonymization import getname
 from sastadev.conf import settings
+from sastadev.methods import Method
 from sastadev.readmethod import itemseppattern
-from sastadev.sastatypes import (FileName, Item, Level, Position, QId,
-                                 QueryDict, UttId, UttWordDict)
+from sastadev.sastatypes import (ExactResults, FileName, Item, Level, Position,
+                                 QId, QueryDict, UttId, UttWordDict)
 
 varitem = ''
 
 txtext = ".txt"
 comma = ","
 space = ' '
 tsvext = '.tsv'
 commaspace = ', '
 tab = '\t'
 all_levels = set()
-literallevels = ['lemma']
+
+# @@next must be made dependent on the method
+literallevels = ['literal', 'lemma']
 
 semicolon = ';'
 labelsep = semicolon
 
 wordcolheaderpattern = r'^\s*word\d+\s*$'
 wordcolheaderre = re.compile(wordcolheaderpattern)
 firstwordcolheaderpattern = r'^\s*word0*1\s*$'
 firstwordcolheaderre = re.compile(firstwordcolheaderpattern)
 
 speakerheaders = ['speaker', 'spreker', 'spk']
-uttidheaders = ['id', 'utt', 'uttid', 'uiting']
+uttidheaders = ['uiting', 'id', 'utt', 'uttid', ]
 levelheaders = ['level']
 stagesheaders = ['fases', 'stages']
-commentsheaders = ['comments', 'commentaar']
-unalignedheaders = ['unaligned', 'hele zin', 'hele uiting']
+commentsheaders = ['opmerkingen', 'comments', 'commentaar']
+unalignedheaders = ['hele uiting', 'unaligned', 'hele zin']
 
 
 def nested_dict(n: int,
                 type: type):  # I do not know how to characterize the result type Dict n times deep endin gwith values of type type
     if n == 1:
         return defaultdict(type)
     else:
@@ -59,30 +64,51 @@
     result = label
     result = result.lstrip()
     result = result.rstrip()
     result = result.lower()
     return result
 
 
-def getlabels(labelstr: str, patterns: Tuple[Pattern, Pattern]) -> List[str]:
+def getlabels(labelstr: str, allvaliditems: List[str], themethod: Method) -> List[str]:
+    separators = themethod.separators
+    rawlabels = re.split(separators, labelstr)
+    labels = [rawlabel.strip() for rawlabel in rawlabels]
+    validlabels = []
+    for label in labels:
+        if label in allvaliditems:
+            validlabels.append(label)
+        elif label == '':
+            pass
+        else:
+            settings.LOGGER.warning(
+                f'Cannot interpret {label} in {labelstr}; ignored')
+    return validlabels
+
+
+def oldgetlabels(labelstr: str, patterns: Tuple[Pattern, Pattern]) -> List[str]:
     results = []
     (pattern, fullpattern) = patterns
     if fullpattern.match(labelstr):
         ms = pattern.finditer(labelstr)
         results = [m.group(0) for m in ms if m.group(0) not in ' ;,-/']
     else:
         results = []
         ms = pattern.finditer(labelstr)
         logstr = str([m.group(0) for m in ms if m.group(0) not in ' ;,-'])
         # print('Cannot interpret {};  found items: {}'.format(labelstr,logstr), file=sys.stderr)
-        settings.LOGGER.warning('Cannot interpret %s; found items: %s', labelstr, logstr)
+        settings.LOGGER.warning(
+            'Cannot interpret %s; found items: %s', labelstr, logstr)
         # exit(-1)
     return results
 
 
+def isuttlevel(level: str) -> bool:
+    return level.lower() in uttidheaders
+
+
 def iswordcolumn(str: str) -> Optional[Match[str]]:
     result = wordcolheaderre.match(str.lower())
     return result
 
 
 def isfirstwordcolumn(str: str) -> Optional[Match[str]]:
     result = firstwordcolheaderre.match(str.lower())
@@ -98,15 +124,15 @@
             newlabels.append(lcprefix + ":" + cleanlabel)
         else:
             newlabels.append(cleanlabel)
     result = labelsep.join(newlabels)
     return result
 
 
-def getcleanlevelsandlabels(thelabelstr: str, thelevel: str, prefix: str, patterns: Tuple[Pattern, Pattern]) \
+def oldgetcleanlevelsandlabels(thelabelstr: str, thelevel: str, prefix: str, patterns: Tuple[Pattern, Pattern]) \
         -> List[Tuple[str, str]]:
     results: List[Tuple[str, str]] = []
     lcthelabelstr = thelabelstr.lower()
     lcprefix = prefix.lower().strip()
     lcthelabelstr = enrich(lcthelabelstr, lcprefix)
     thelabels = getlabels(lcthelabelstr, patterns)
     for thelabel in thelabels:
@@ -115,200 +141,32 @@
             cleanlevel = clean(thelevel)
             result = (cleanlevel, cleanlabel)
             results.append(result)
 
     return results
 
 
-# def oldget_annotations(infilename, patterns):
-#     '''
-#     Reads the file with name filename in SASTA Annotation Format
-#     :param infilename:
-#     :param patterns
-#     :return: a dictionary  with as  key a tuple (level, item) and as value a Counter  with key uttid and value its count
-#     '''
-#
-#     thedata = defaultdict(list)
-#     exactdata = defaultdict(list)
-#     cdata = {}
-#
-#     # To open Workbook
-#     wb = xlrd.open_workbook(infilename)
-#     sheet = wb.sheet_by_index(0)
-#
-#     startrow = 0
-#     startcol = 0
-#     headerrow = 0
-#     headers = {}
-#     lastrow = sheet.nrows
-#     lastcol = sheet.ncols
-#     #    firstwordcol = 2
-#     #    lastwordcol = lastcol - 4
-#     levelcol = 1
-#     uttidcol = 0
-#     stagescol = -1
-#     commentscol = -1
-#
-#     uttlevel = 'utt'
-#
-#     for rowctr in range(startrow, lastrow):
-#         if rowctr == headerrow:
-#             for colctr in range(startcol, lastcol):
-#                 headers[colctr] = sheet.cell_value(rowctr, colctr)
-#                 if iswordcolumn(headers[colctr]):
-#                     lastwordcol = colctr
-#                     if isfirstwordcolumn(headers[colctr]):
-#                         firstwordcol = colctr
-#                 elif clean(headers[colctr]) in speakerheaders:
-#                     spkcol = colctr
-#                 elif clean(headers[colctr]) in uttidheaders:
-#                     uttidcol = colctr
-#                 elif clean(headers[colctr]) in levelheaders:
-#                     levelcol = colctr
-#                 elif clean(headers[colctr]) in stagesheaders:
-#                     stagescol = colctr
-#                 elif clean(headers[colctr]) in commentsheaders:
-#                     commentscol = colctr
-#         else:
-#             if sheet.cell_value(rowctr, uttidcol) != "":
-#                 uttid = str(int(sheet.cell_value(rowctr, uttidcol)))
-#             thelevel = sheet.cell_value(rowctr, levelcol)
-#             thelevel = clean(thelevel)
-#             all_levels.add(thelevel)
-#             for colctr in range(firstwordcol, sheet.ncols):
-#                 if thelevel in literallevels and colctr != stagescol and colctr != commentscol:
-#                     thelabel = sheet.cell_value(rowctr, colctr)
-#                     if colctr > lastwordcol:
-#                         tokenposition = 0
-#                     else:
-#                         tokenposition = colctr - firstwordcol + 1
-#                     thedata[(thelevel, thelabel)].append(uttid)
-#                     exactdata[(cleanlevel, cleanlabel)].append((uttid, tokenposition))
-#                 elif thelevel != uttlevel and colctr != stagescol and colctr != commentscol:
-#                     thelabelstr = sheet.cell_value(rowctr, colctr)
-#                     thelevel = sheet.cell_value(rowctr, levelcol)
-#                     if lastwordcol + 1 <= colctr < sheet.ncols:
-#                         # prefix = headers[colctr] aangepast om het simpeler te houden
-#                         prefix = ""
-#                     else:
-#                         prefix = ""
-#                     cleanlevelsandlabels = getcleanlevelsandlabels(thelabelstr, thelevel, prefix, patterns)
-#                     if colctr > lastwordcol:
-#                         tokenposition = 0
-#                     else:
-#                         tokenposition = colctr - firstwordcol + 1
-#                     for (cleanlevel, cleanlabel) in cleanlevelsandlabels:
-#                         thedata[(cleanlevel, cleanlabel)].append(uttid)
-#                         exactdata[(cleanlevel, cleanlabel)].append((uttid, tokenposition))
-#     # wb.close() there is no way to close the workbook
-#     for atuple in thedata:
-#         cdata[atuple] = Counter(thedata[atuple])
-#     return cdata
-#
-#
-# def old2get_annotations(infilename: FileName, patterns: Tuple[Pattern, Pattern]) \
-#         -> Tuple[UttWordDict, Dict[Tuple[Level, Item], List[Tuple[UttId, Position]]]]:
-#     '''
-#     Reads the file with name filename in SASTA Annotation Format
-#     :param infilename:
-#     :param patterns
-#     :return: a dictionary  with as  key a tuple (level, item) and as value a list of (uttid, tokenposition) pairs
-#     '''
-#
-#     thedata = defaultdict(list)
-#     #cdata = {}
-#
-#     allutts = {}
-#
-#     # To open Workbook
-#     wb = xlrd.open_workbook(infilename)
-#     sheet = wb.sheet_by_index(0)
-#
-#     startrow = 0
-#     startcol = 0
-#     headerrow = 0
-#     headers = {}
-#     lastrow = sheet.nrows
-#     lastcol = sheet.ncols
-#     #    firstwordcol = 2
-#     #    lastwordcol = lastcol - 4
-#     levelcol = 1
-#     uttidcol = 0
-#     stagescol = -1
-#     commentscol = -1
-#
-#     uttlevel = 'utt'
-#
-#     uttcount = 0
-#
-#     for rowctr in range(startrow, lastrow):
-#         if rowctr == headerrow:
-#             for colctr in range(startcol, lastcol):
-#                 headers[colctr] = sheet.cell_value(rowctr, colctr)
-#                 if iswordcolumn(headers[colctr]):
-#                     lastwordcol = colctr
-#                     if isfirstwordcolumn(headers[colctr]):
-#                         firstwordcol = colctr
-#                 elif clean(headers[colctr]) in speakerheaders:
-#                     spkcol = colctr
-#                 elif clean(headers[colctr]) in uttidheaders:
-#                     uttidcol = colctr
-#                 elif clean(headers[colctr]) in levelheaders:
-#                     levelcol = colctr
-#                 elif clean(headers[colctr]) in stagesheaders:
-#                     stagescol = colctr
-#                 elif clean(headers[colctr]) in commentsheaders:
-#                     commentscol = colctr
-#         else:
-#             if sheet.cell_value(rowctr, uttidcol) != "":
-#                 uttid = str(int(sheet.cell_value(rowctr, uttidcol)))
-#             thelevel = sheet.cell_value(rowctr, levelcol)
-#             thelevel = clean(thelevel)
-#             all_levels.add(thelevel)
-#             # if thelevel == uttlevel:
-#             #    uttcount += 1
-#             curuttwlist = []
-#             for colctr in range(firstwordcol, sheet.ncols):
-#                 if thelevel == uttlevel:
-#                     curcellval = sheet.cell_value(rowctr, colctr)
-#                     if curcellval != '':
-#                         curuttwlist.append(curcellval)
-#                 elif thelevel in literallevels and colctr != stagescol and colctr != commentscol:
-#                     thelabel = sheet.cell_value(rowctr, colctr)
-#                     if colctr > lastwordcol:
-#                         tokenposition = 0
-#                     else:
-#                         tokenposition = colctr - firstwordcol + 1
-#                     # thedata[(thelevel, thelabel)].append(uttid)
-#                     cleanlevel = thelevel
-#                     cleanlabel = thelabel
-#                     if cleanlabel != '':
-#                         thedata[(cleanlevel, cleanlabel)].append((uttid, tokenposition))
-#                 elif thelevel != uttlevel and colctr != stagescol and colctr != commentscol:
-#                     thelabelstr = sheet.cell_value(rowctr, colctr)
-#                     thelevel = sheet.cell_value(rowctr, levelcol)
-#                     if lastwordcol + 1 <= colctr < sheet.ncols:
-#                         # prefix = headers[colctr] aangepast om het simpeler te houden
-#                         prefix = ""
-#                     else:
-#                         prefix = ""
-#                     cleanlevelsandlabels = getcleanlevelsandlabels(thelabelstr, thelevel, prefix, patterns)
-#                     if colctr > lastwordcol:
-#                         tokenposition = 0
-#                     else:
-#                         tokenposition = colctr - firstwordcol + 1
-#                     for (cleanlevel, cleanlabel) in cleanlevelsandlabels:
-#                         thedata[(cleanlevel, cleanlabel)].append((uttid, tokenposition))
-#             if curuttwlist != []:
-#                 allutts[uttid] = curuttwlist
-#     # wb.close() there is no way to close the workbook
-#     return allutts, thedata
+def getcleanlevelsandlabels(thelabelstr: str, thelevel: str, prefix: str, allvaliditems: List[str], themethod: Method) \
+        -> List[Tuple[str, str]]:
+    results: List[Tuple[str, str]] = []
+    lcthelabelstr = thelabelstr.lower()
+    lcprefix = prefix.lower().strip()
+    lcthelabelstr = enrich(lcthelabelstr, lcprefix)
+    thelabels = getlabels(lcthelabelstr, allvaliditems, themethod)
+    for thelabel in thelabels:
+        if thelabel != "":
+            cleanlabel = thelabel
+            cleanlevel = clean(thelevel)
+            result = (cleanlevel, cleanlabel)
+            results.append(result)
+
+    return results
 
 
-def get_annotations(infilename: FileName, patterns: Tuple[Pattern, Pattern]) \
+def oldget_annotations(infilename: FileName, patterns: Tuple[Pattern, Pattern]) \
         -> Tuple[UttWordDict, Dict[Tuple[Level, Item], List[Tuple[UttId, Position]]]]:
     '''
     Reads the file with name filename in SASTA Annotation Format
     :param infilename:
     :param patterns
     :return: a dictionary  with as  key a tuple (level, item) and as value a list of (uttid, tokenposition) pairs
     '''
@@ -322,15 +180,114 @@
 
     levelcol = 1
     uttidcol = 0
     stagescol = -1
     commentscol = -1
     unalignedcol = -1
 
-    uttlevel = 'utt'
+    # uttlevel = 'utt'
+
+    uttcount = 0
+
+    for col, val in enumerate(header):
+        if iswordcolumn(val):
+            lastwordcol = col
+            if isfirstwordcolumn(val):
+                firstwordcol = col
+        elif clean(val) in speakerheaders:
+            spkcol = col
+        elif clean(val) in uttidheaders:
+            uttidcol = col
+        elif clean(val) in levelheaders:
+            levelcol = col
+        elif clean(val) in stagesheaders:
+            stagescol = col
+        elif clean(val) in commentsheaders:
+            commentscol = col
+        elif clean(val) in unalignedheaders:
+            unalignedcol = col
+        else:
+            pass  # maybe warn here that an unknow column header has been encountered?
+
+    for row in data:
+        if row[uttidcol] != "":
+            # this might go wrong if there is no integer there @@make it robust
+            uttid = str(int(row[uttidcol]))
+        thelevel = row[levelcol]
+        thelevel = clean(thelevel)
+        all_levels.add(thelevel)
+        # if thelevel == uttlevel:
+        #    uttcount += 1
+        curuttwlist = []
+        for colctr in range(firstwordcol, len(row)):
+            if thelevel.lower() in uttidheaders:
+                rawcurcellval = str(row[colctr])
+                curcellval = getname(rawcurcellval)
+                if curcellval != '':
+                    curuttwlist.append(curcellval)
+            elif thelevel in literallevels and colctr != stagescol and colctr != commentscol:
+                rawthelabel = str(row[colctr])
+                thelabel = getname(rawthelabel)
+                if colctr > lastwordcol:
+                    tokenposition = 0
+                else:
+                    tokenposition = colctr - firstwordcol + 1
+                cleanlevel = thelevel
+                cleanlabel = thelabel
+                if cleanlabel != '':
+                    thedata[(cleanlevel, cleanlabel)].append(
+                        (uttid, tokenposition))
+            elif not isuttlevel(thelevel) and colctr != stagescol and colctr != commentscol:
+                thelabelstr = row[colctr]
+                thelevel = row[levelcol]
+                if colctr == unalignedcol:
+                    prefix = ''
+                if lastwordcol + 1 <= colctr < len(row):
+                    # prefix = headers[colctr] aangepast om het simpeler te houden
+                    prefix = ""
+                else:
+                    prefix = ""
+                cleanlevelsandlabels = getcleanlevelsandlabels(
+                    thelabelstr, thelevel, prefix, patterns)
+                if colctr > lastwordcol or colctr == unalignedcol:
+                    tokenposition = 0
+                else:
+                    tokenposition = colctr - firstwordcol + 1
+                for (cleanlevel, cleanlabel) in cleanlevelsandlabels:
+                    thedata[(cleanlevel, cleanlabel)].append(
+                        (uttid, tokenposition))
+        if curuttwlist != []:
+            allutts[uttid] = curuttwlist
+    return allutts, thedata
+
+
+def get_annotations(infilename: FileName, allitems: List[str], themethod: Method) \
+        -> Tuple[UttWordDict, Dict[Tuple[Level, Item], List[Tuple[UttId, Position]]]]:
+    '''
+    Reads the file with name filename in SASTA Annotation Format
+    :param infilename:
+    :param allitems: list of all valid items
+    :param themethod: the method
+    :return: a dictionary  with as  key a tuple (level, item) and as value a list of (uttid, tokenposition) pairs
+    '''
+
+    thedata = defaultdict(list)
+
+    allutts = {}
+
+    # To open Workbook
+    header, data = xlsx.getxlsxdata(infilename)
+
+    levelcol = 1
+    uttidcol = 0
+    stagescol = -1
+    commentscol = -1
+    unalignedcol = -1
+
+    # uttlevel = 'utt'
 
     uttcount = 0
 
     for col, val in enumerate(header):
         if iswordcolumn(val):
             lastwordcol = col
             if isfirstwordcolumn(val):
@@ -348,66 +305,72 @@
         elif clean(val) in unalignedheaders:
             unalignedcol = col
         else:
             pass  # maybe warn here that an unknow column header has been encountered?
 
     for row in data:
         if row[uttidcol] != "":
+            # this might go wrong if there is no integer there @@make it robust
             uttid = str(int(row[uttidcol]))
         thelevel = row[levelcol]
         thelevel = clean(thelevel)
         all_levels.add(thelevel)
         # if thelevel == uttlevel:
         #    uttcount += 1
         curuttwlist = []
         for colctr in range(firstwordcol, len(row)):
-            if thelevel == uttlevel:
-                curcellval = str(row[colctr])
+            if thelevel.lower() in uttidheaders:
+                rawcurcellval = str(row[colctr])
+                curcellval = getname(rawcurcellval)
                 if curcellval != '':
                     curuttwlist.append(curcellval)
             elif thelevel in literallevels and colctr != stagescol and colctr != commentscol:
-                thelabel = str(row[colctr])
+                rawthelabel = str(row[colctr])
+                thelabel = getname(rawthelabel)
                 if colctr > lastwordcol:
                     tokenposition = 0
                 else:
                     tokenposition = colctr - firstwordcol + 1
                 cleanlevel = thelevel
                 cleanlabel = thelabel
                 if cleanlabel != '':
-                    thedata[(cleanlevel, cleanlabel)].append((uttid, tokenposition))
-            elif thelevel != uttlevel and colctr != stagescol and colctr != commentscol:
+                    thedata[(cleanlevel, cleanlabel)].append(
+                        (uttid, tokenposition))
+            elif not isuttlevel(thelevel) and colctr != stagescol and colctr != commentscol:
                 thelabelstr = row[colctr]
                 thelevel = row[levelcol]
                 if colctr == unalignedcol:
                     prefix = ''
                 if lastwordcol + 1 <= colctr < len(row):
                     # prefix = headers[colctr] aangepast om het simpeler te houden
                     prefix = ""
                 else:
                     prefix = ""
-                cleanlevelsandlabels = getcleanlevelsandlabels(thelabelstr, thelevel, prefix, patterns)
+                cleanlevelsandlabels = getcleanlevelsandlabels(
+                    thelabelstr, thelevel, prefix, allitems, themethod)
                 if colctr > lastwordcol or colctr == unalignedcol:
                     tokenposition = 0
                 else:
                     tokenposition = colctr - firstwordcol + 1
                 for (cleanlevel, cleanlabel) in cleanlevelsandlabels:
-                    thedata[(cleanlevel, cleanlabel)].append((uttid, tokenposition))
+                    thedata[(cleanlevel, cleanlabel)].append(
+                        (uttid, tokenposition))
         if curuttwlist != []:
             allutts[uttid] = curuttwlist
     return allutts, thedata
 
 
-def update(thedict: Dict[QId, Tuple[Level, Item, List[Tuple[UttId, Position]]]], qid: QId,
-           goldtuple: Tuple[Level, Item, List[Tuple[UttId, Position]]]):
+def update(thedict: Dict[ResultsKey, Tuple[Level, Item, ExactResults]], reskey: ResultsKey,
+           goldtuple: Tuple[Level, Item, ExactResults]):
     (level, item, thecounter) = goldtuple
-    if qid in thedict:
-        (oldlevel, olditem, oldcounter) = thedict[qid]
-        thedict[qid] = (oldlevel, olditem, oldcounter + thecounter)
+    if reskey in thedict:
+        (oldlevel, olditem, oldcounter) = thedict[reskey]
+        thedict[reskey] = (oldlevel, olditem, oldcounter + thecounter)
     else:
-        thedict[qid] = goldtuple
+        thedict[reskey] = goldtuple
 
 
 def oldgetitem2levelmap(mapping: Dict[Tuple[Item, Level], Any]) -> Dict[Item, List[Level]]:
     resultmap: Dict[Item, List[Level]] = {}
     for (item, level) in mapping:
         if item in resultmap:
             resultmap[item].append(level)
@@ -444,106 +407,125 @@
     sortedallcodes = sorted(allcodes, key=len, reverse=True)
     adaptedcodes = [codeadapt(c) for c in sortedallcodes]
     basepattern = r'' + '|'.join(adaptedcodes) + '|' + itemseppattern
     fullpattern = r'^(' + basepattern + r')*$'
     return (re.compile(basepattern), re.compile(fullpattern))
 
 
-def get_golddata(filename: FileName, mapping: Dict[Tuple[Item, Level], QId],
-                 altcodes: Dict[Tuple[Item, Level], Tuple[Item, Level]],
-                 queries: QueryDict, includeimplies: bool = False) \
+# def get_golddata(filename: FileName, mapping: Dict[Tuple[Item, Level], QId],
+#                  altcodes: Dict[Tuple[Item, Level], Tuple[Item, Level]],
+#                  queries: QueryDict, includeimplies: bool = False) \
+#         -> Tuple[UttWordDict, Dict[QId, Tuple[Level, Item, List[Tuple[UttId, Position]]]]]:
+def get_golddata(filename: FileName, themethod: Method, includeimplies: bool = False) \
         -> Tuple[UttWordDict, Dict[QId, Tuple[Level, Item, List[Tuple[UttId, Position]]]]]:
+
     # item2levelmap = {}
+    mapping: Dict[Tuple[Item, Level], QId] = themethod.item2idmap
+    altcodes: Dict[Tuple[Item, Level], Tuple[Item, Level]] = themethod.altcodes
+    queries: QueryDict = themethod.queries
+    includeimplies = False  # temporarily put off to test different implementation
     mappingitem2levelmap = getitem2levelmap(mapping)
     altcodesitem2levelmap = getitem2levelmap(altcodes)
     allmappingitems = [item for (item, _) in mapping]
     allaltcodesitems = [item for (item, _) in altcodes]
     allitems = allmappingitems + allaltcodesitems
     patterns = mkpatterns(allitems)
-    allutts, basicdata = get_annotations(filename, patterns)
-    results: Dict[QId, Tuple[Level, Item, List[Tuple[UttId, Position]]]] = {}
+    allutts, basicdata = get_annotations(filename, allitems, themethod)
+    results: Dict[ResultsKey, Tuple[Level, Item, ExactResults]] = {}
     for thelevel, theitem in basicdata:
         thecounter = basicdata[(thelevel, theitem)]
         # unclear why this below here is needed
         #        if (theitem, thelevel) in mapping:
         #            mappingitem = theitem
         #        elif (varitem, thelevel) in mapping:
         #            mappingitem = varitem
         #        else:
         #            mappingitem = theitem
-        if thelevel in literallevels:
-            # we still have to determine how to deal with this
-            pass
+        if thelevel in literallevels and (thelevel, thelevel) in mapping:
+            # we still have to determine how to deal with this this is an attempt
+            qid = mapping[thelevel, thelevel]
+            reskey = mkresultskey(qid, theitem)
+            update(results, reskey, (thelevel, theitem, thecounter))
         elif (theitem, thelevel) in mapping:
             qid = mapping[(theitem, thelevel)]
-            update(results, qid, (thelevel, theitem, thecounter))
+            reskey = mkresultskey(qid)
+            update(results, reskey, (thelevel, theitem, thecounter))
             if includeimplies:
                 for implieditem in queries[qid].implies:
                     impliedlevel = mappingitem2levelmap[implieditem]
                     if (implieditem, impliedlevel) in mapping:
                         impliedqid = mapping[(implieditem, impliedlevel)]
-                        update(results, impliedqid, (impliedlevel, implieditem, thecounter))
+                        update(results, mkresultskey(impliedqid),
+                               (impliedlevel, implieditem, thecounter))
                     else:
                         settings.LOGGER.error(
                             'Implied Item ({},{}) not found in mapping'.format(implieditem, impliedlevel))
         elif (theitem, thelevel) in altcodes:
             (altitem, altlevel) = altcodes[(theitem, thelevel)]
             qid = mapping[(altitem, altlevel)]
-            update(results, qid, (altlevel, altitem, thecounter))
+            reskey = mkresultskey(qid)
+            update(results, reskey, (altlevel, altitem, thecounter))
             settings.LOGGER.info(
                 '{} of level {} invalid code replaced by {} of level {}'.format(theitem, thelevel, altitem, altlevel))
             if includeimplies:
                 for implieditem in queries[qid].implies:
                     impliedlevel = mappingitem2levelmap[implieditem]
                     if (implieditem, impliedlevel) in mapping:
                         impliedqid = mapping[(implieditem, impliedlevel)]
-                        update(results, impliedqid, (impliedlevel, implieditem, thecounter))
+                        update(results, mkresultskey(impliedqid),
+                               (impliedlevel, implieditem, thecounter))
                     else:
                         settings.LOGGER.error(
                             'Implied Item ({},{}) not found in mapping'.format(implieditem, impliedlevel))
         elif theitem in mappingitem2levelmap:  # valid item but wrong level
             thecorrectlevel = mappingitem2levelmap[theitem]
             qid = mapping[(theitem, thecorrectlevel)]
-            update(results, qid, (thecorrectlevel, theitem, thecounter))
+            reskey = mkresultskey(qid)
+            update(results, reskey, (thecorrectlevel, theitem, thecounter))
             settings.LOGGER.info(
                 'level {} of item {} replaced by correct level {}'.format(thelevel, theitem, thecorrectlevel))
             if includeimplies:
                 for implieditem in queries[qid].implies:
                     impliedlevel = mappingitem2levelmap[implieditem]
                     if (implieditem, impliedlevel) in mapping:
                         impliedqid = mapping[(implieditem, impliedlevel)]
-                        update(results, impliedqid, (impliedlevel, implieditem, thecounter))
+                        update(results, mkresultskey(impliedqid),
+                               (impliedlevel, implieditem, thecounter))
                     else:
                         settings.LOGGER.error(
                             'Implied Item ({},{}) not found in mapping'.format(implieditem, impliedlevel))
         elif theitem in altcodesitem2levelmap:  # valid alternative item but wrong level
             theitemlevel = altcodesitem2levelmap[theitem]
-            (thecorrectitem, thecorrectlevel) = altcodes[(theitem, theitemlevel)]
+            (thecorrectitem, thecorrectlevel) = altcodes[(
+                theitem, theitemlevel)]
             qid = mapping[(thecorrectitem, thecorrectlevel)]
-            update(results, qid, (thecorrectlevel, thecorrectitem, thecounter))
+            reskey = mkresultskey(qid)
+            update(results, reskey, (thecorrectlevel, thecorrectitem, thecounter))
             settings.LOGGER.info(
-                'level {} of item {} replaced by correct level {} and item {}'.format(
-                    thelevel, theitem, thecorrectlevel, thecorrectitem)
-            )
+                'level {} of item {} replaced by correct level {} and item {}'.format(thelevel, theitem,
+                                                                                      thecorrectlevel,
+                                                                                      thecorrectitem))
             if includeimplies:
                 for implieditem in queries[qid].implies:
                     impliedlevel = mappingitem2levelmap[implieditem]
                     if (implieditem, impliedlevel) in mapping:
                         impliedqid = mapping[(implieditem, impliedlevel)]
-                        update(results, impliedqid, (impliedlevel, implieditem, thecounter))
+                        update(results, mkresultskey(impliedqid),
+                               (impliedlevel, implieditem, thecounter))
                     else:
                         settings.LOGGER.error(
                             'Implied Item ({},{}) not found in mapping'.format(implieditem, thecorrectlevel))
 
         else:
-            settings.LOGGER.error('{} of level {} not a valid coding'.format(theitem, thelevel))
+            settings.LOGGER.error(
+                '{} of level {} not a valid coding'.format(theitem, thelevel))
     return allutts, results
 
 
-def exact2global(thedata: Dict[Tuple[Level, Item], List[Tuple[UttId, Position]]]) -> Dict[Tuple[Level, Item], Counter]:
+def exact2global(thedata: Dict[Tuple[Level, Item], ExactResults]) -> Dict[Tuple[Level, Item], Counter]:
     '''
     turns a dictionary with  as values a list of (uttid, pos) tuples into a dictionary with the same keys and as values a counter of uttid
     :param thedata:
     :return:
     '''
 
     cdata = {}
@@ -565,12 +547,12 @@
     for thekey in thedata:
         (thelevel, theitem, exactlist) = thedata[thekey]
         newvalue = [uttid for (uttid, _) in exactlist]
         cdata[thekey] = (thelevel, theitem, Counter(newvalue))
     return cdata
 
 
-def richscores2scores(richscores: Dict[QId, Tuple[Level, Item, Any]]) -> Dict[QId, Any]:
+def richscores2scores(richscores: Dict[ResultsKey, Tuple[Level, Item, Any]]) -> Dict[QId, Any]:
     scores = {}
-    for queryid in richscores:
-        scores[queryid] = richscores[queryid][2]
+    for reskey in richscores:
+        scores[reskey] = richscores[reskey][2]
     return scores
```

### Comparing `sastadev-0.1.5/src/sastadev/SRFreader.py` & `sastadev-0.2.0/src/sastadev/SRFreader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,69 @@
 from collections import Counter
 
+from sastadev.allresults import ResultsKey, mkresultskey
+from sastadev.conf import settings
+
 qidcolheader = 'id'
 uttcolheader = 'uttids'
 tab = '\t'
 comma = ','
 platinumheaderrows = 0
 
 
+def getreskey(rawcell: str) -> ResultsKey:
+    '''
+    older / manually created versions of a reference file can contain simply a QId here, newer ones have a ResultKey string
+    :param cell:
+    :return:
+    '''
+    cell = rawcell.strip()
+    cellparts = cell.split('/')
+    if len(cellparts) == 2:
+        result = (cellparts[0], cellparts[1])
+    elif len(cellparts) == 1:
+        result = mkresultskey(cell)
+    else:
+        result = cell
+        settings.LOGGER.error(f'Unknown value {cell} encountered')
+    return result
+
+
 def read_referencefile(infilename, logfile):
     '''
     a reference file is tsv file which contains a header with at least two column headers (idcolheader, uttcolheader)
     :param infilename:
-    :return: a dictionary with for each queryid a Counter for the utterance ids
+    :return: a dictionary with for each ResultsKey  a Counter for the utterance ids
     '''
     infile = open(infilename, 'r')
     rowctr = 0
     results = {}
     for line in infile:
         if rowctr == platinumheaderrows:
             rowstr = line.lower()
             rowlist = rowstr.split(tab)
             try:
                 qidcol = rowlist.index(qidcolheader)
             except ValueError:
-                print('Error reading reference file; no ID column header', infilename, file=logfile)
+                print('Error reading reference file; no ID column header',
+                      infilename, file=logfile)
                 exit(-1)
             try:
                 uttcol = rowlist.index(uttcolheader)
             except ValueError:
-                print('Error reading reference file: no uttids column header in', infilename, file=logfile)
+                print('Error reading reference file: no uttids column header in',
+                      infilename, file=logfile)
                 exit(-1)
         elif rowctr > platinumheaderrows:
             rowstr = line[:-1]
             rowlist = rowstr.split(tab)
-            qid = rowlist[qidcol]
+            reskey = getreskey(rowlist[qidcol])
             utts = rowlist[uttcol]
             if utts == '':
                 uttlist = []
             else:
                 rawuttlist = utts.split(comma)
                 uttlist = [uttid.strip() for uttid in rawuttlist]
-            results[qid] = Counter(uttlist)
+            results[reskey] = Counter(uttlist)
         rowctr += 1
     infile.close()
     return results
```

### Comparing `sastadev-0.1.5/src/sastadev/STAPpostfunctions.py` & `sastadev-0.2.0/src/sastadev/STAPpostfunctions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 '''
 defines functions for the STAP post part of the methods
 
 '''
 from collections import Counter
 
+from sastadev.allresults import mkresultskey
+
 BB_ids = ['S010', 'S011', 'S012']
+S013qid = 'S013'
+S013reskey = mkresultskey(S013qid)
 
 
 def BB_totaal(allresults, _):
     scores = []
     for qid in BB_ids:
         if qid in allresults.coreresults:
             scores.append(allresults.coreresults[qid])
@@ -17,22 +21,22 @@
     counts = [len(s) for s in scores]
     result = sum(counts)
     return result
 
 
 def GLVU(allresults, _):
     total_length_VU = 0
-    if 'S013' in allresults.coreresults:
-        for key in allresults.coreresults['S013']:
-            total_length_VU += allresults.coreresults['S013'][key]
+    if S013reskey in allresults.coreresults:
+        for key in allresults.coreresults[S013reskey]:
+            total_length_VU += allresults.coreresults[S013reskey][key]
     result = total_length_VU / allresults.uttcount
     return result
 
 
 def GL5LVU(allresults, _):
     counts = []
-    if 'S013' in allresults.coreresults:
-        for key in allresults.coreresults['S013']:
-            counts.append(allresults.coreresults['S013'][key])
+    if S013reskey in allresults.coreresults:
+        for key in allresults.coreresults[S013reskey]:
+            counts.append(allresults.coreresults[S013reskey][key])
     sorted_counts = counts.sort()
     result = sum(counts[45:50]) / 5
     return result
```

### Comparing `sastadev-0.1.5/src/sastadev/Sziplus.py` & `sastadev-0.2.0/src/sastadev/Sziplus.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/TARSPpostfunctions.py` & `sastadev-0.2.0/src/sastadev/TARSPpostfunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/TARSPscreening.py` & `sastadev-0.2.0/src/sastadev/TARSPscreening.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/__main__.py` & `sastadev-0.2.0/src/sastadev/mysastadev.py`

 * *Files 6% similar despite different names*

```diff
@@ -141,45 +141,50 @@
 import sys
 from collections import Counter, defaultdict
 # from altcodes import altcodes
 from optparse import OptionParser
 from typing import Any, Callable, Dict, List, Pattern, Tuple
 
 import xlsxwriter
+# import xlrd
 from lxml import etree
 
 from sastadev import compounds
-from sastadev.allresults import AllResults, scores2counts
+from sastadev.allresults import (AllResults, ExactResultsDict, MatchesDict,
+                                 ResultsKey, mkresultskey, scores2counts,
+                                 showreskey)
 from sastadev.ASTApostfunctions import getastamaxsamplesizeuttidsandcutoff
 from sastadev.conf import settings
 from sastadev.constants import (bronzefolder, formsfolder, intreebanksfolder,
                                 loggingfolder, outtreebanksfolder,
                                 resultsfolder, silverfolder, silverpermfolder)
 from sastadev.correcttreebank import (correcttreebank, corrn, errorwbheader,
                                       validcorroptions)
 from sastadev.counterfunctions import counter2liststr
 from sastadev.external_functions import str2functionmap
 from sastadev.goldcountreader import get_goldcounts
 from sastadev.macros import expandmacros
 from sastadev.methods import (Method, astamethods, stapmethods,
                               supported_methods, tarspmethods, treatmethod)
-from sastadev.mismatches import exactmismatches, getmarkposition
+from sastadev.mismatches import (exactmismatches, getmarkposition,
+                                 literalmissedmatches)
 from sastadev.mksilver import getsilverannotations, permprefix
-from sastadev.query import (Query, form_process, is_core, is_pre, is_preorcore,
-                            post_process, query_exists, query_inform)
+from sastadev.query import (Query, form_process, is_core, is_literal, is_pre,
+                            is_preorcore, post_process, query_exists,
+                            query_inform)
 from sastadev.readmethod import itemseppattern, read_method
 from sastadev.reduceresults import (exact2results, reduceallresults,
                                     reduceexactgoldscores, reduceresults)
 from sastadev.rpf1 import getevalscores, getscores, sumfreq
 from sastadev.SAFreader import (get_golddata, richexact2global,
                                 richscores2scores)
 from sastadev.sasta_explanation import finalexplanation_adapttreebank
-from sastadev.sastatypes import (AltCodeDict, ExactResultsDict, GoldTuple,
-                                 MatchesDict, MethodName, Position, QId,
-                                 QIdCount, QueryDict, ResultsCounter,
+# import sastatypes
+from sastadev.sastatypes import (AltCodeDict, GoldTuple, MethodName, Position,
+                                 QId, QIdCount, QueryDict, ResultsCounter,
                                  SampleSizeTuple, SynTree, UttId)
 from sastadev.SRFreader import read_referencefile
 from sastadev.stringfunctions import getallrealwords
 from sastadev.targets import get_mustbedone, get_targets
 from sastadev.treebankfunctions import (getattval, getnodeendmap, getuttid,
                                         getxmetatreepositions, getxselseuttid,
                                         getyield, showtree)
@@ -193,15 +198,14 @@
 
 tarsp = 'tarsp'
 stap = 'stap'
 asta = 'asta'
 gramat = 'gramat'
 
 codepath = os.path.dirname(os.path.abspath(__file__))
-methodspath = os.path.join(codepath, 'data', 'methods')
 
 
 # moved to methods.py
 # methodspath = os.path.join(codepath, 'methods')
 
 # supported_methods = {}
 # supported_methods[tarsp] = os.path.join(methodspath, 'TARSP Index Current.xlsx')
@@ -265,23 +269,24 @@
 allmatches: MatchesDict = {}
 altcodes: AltCodeDict = {}
 
 emptycounter: Counter = Counter()
 invalidqueries: Dict[QId, Exception] = {}
 
 
-def checkplatinum(goldscores: Dict[QId, Counter], platinumscores: Dict[QId, Counter], queries: QueryDict) -> None:
-    for qid in goldscores:
-        if qid in platinumscores:
+def checkplatinum(goldscores: Dict[ResultsKey, Counter], platinumscores: Dict[ResultsKey, Counter], queries: QueryDict) -> None:
+    for reskey in goldscores:
+        if reskey in platinumscores:
             # all values of gold must be in platinum
+            qid = reskey[0]
             if query_exists(queries[qid]):
-                diff1 = goldscores[qid] - platinumscores[qid]
+                diff1 = goldscores[reskey] - platinumscores[reskey]
                 if diff1 != Counter():
                     settings.LOGGER.warning(
-                        '{} has goldscores not in platinum: {}'.format(qid, diff1))
+                        '{} has goldscores not in platinum: {}'.format(str(reskey), diff1))
 
 
 def mkerrorreport(errordict, errorreportfilename: str):
     header = ['name', 'count', 'uttid', 'value',
               'source', 'cat', 'subcat', 'origutt', 'parsed_as']
     allrows = []
     for item in errordict:
@@ -317,15 +322,15 @@
 #    counts = {}
 #    for el in scores:
 #        countval = len(scores[el])
 #        counts[el] = countval
 #    return counts
 
 def sf(number):
-    if isinstance(number, float) or isinstance(number, int):
+    if type(number) == float or type(number) == int:
         result = '{0:.1f}'.format(number)
     else:
         result = number
     return result
 
 
 def getmarkedutt(m: SynTree, syntree: SynTree) -> str:
@@ -427,26 +432,38 @@
 
 
 def isxpathquery(query: str) -> bool:
     cleanquery = query.lstrip()
     return cleanquery.startswith('//')
 
 
+def getreskey(qid: QId, m: SynTree, queries: QueryDict) -> ResultsKey:
+    if m is None:
+        return mkresultskey(qid)
+    thequery = queries[qid]
+    if is_literal(thequery):
+        litfunc = str2functionmap[thequery.literal]
+        thevalue = litfunc(m)
+        return mkresultskey(qid, thevalue)
+    else:
+        return mkresultskey(qid)
+
+
 def doqueries(syntree: SynTree, queries: QueryDict, exactresults: ExactResultsDict, allmatches: MatchesDict, criterion: Callable[[Query], bool]):
     global invalidqueries
     uttid = getuttid(syntree)
     # uttid = getuttidorno(syntree)
     omittedwordpositions = getxmetatreepositions(
         syntree, 'Omitted Word', poslistname='annotatedposlist')
     # print(uttid)
     # core queries
     junk = 0
-    for queryid in queries:
-        if queryid not in exactresults:
-            exactresults[queryid] = []
+    for queryid in queries:  # @@ dit aanpassen voor literals en voor Resultskey; check read_referencefile
+        # if queryid not in exactresults: # not needed becaysetaken care of below
+        #     exactresults[queryid] = []
         thequeryobj = queries[queryid]
         if criterion(thequeryobj):
             if query_exists(thequeryobj):
                 thelistedquery = thequeryobj.query
                 if isxpathquery(thelistedquery):
                     expandedquery = expandmacros(thelistedquery)
                     thequery = "." + expandedquery
@@ -456,26 +473,30 @@
                         invalidqueries[queryid] = e
                         matches = []
                 else:
                     thef = str2functionmap[thelistedquery]
                     matches = thef(syntree)
             else:
                 matches = []
-                exactresults[queryid] = []
+                exactresults[mkresultskey(queryid)] = []
             # matchingids = [uttid for x in matches]
             for m in matches:
                 # showtree(m)
+                reskey = getreskey(queryid, m, queries)
                 if m is None:
                     showtree(syntree, text='in doqueries: Nonematch')
-                if (queryid, uttid) in allmatches:
-                    allmatches[(queryid, uttid)].append((m, syntree))
+                if (reskey, uttid) in allmatches:
+                    allmatches[(reskey, uttid)].append((m, syntree))
                 else:
-                    allmatches[(queryid, uttid)] = [(m, syntree)]
+                    allmatches[(reskey, uttid)] = [(m, syntree)]
                 exactresult = (uttid, int(getattval(m, 'begin')) + 1)
-                exactresults[queryid].append(exactresult)
+                if reskey in exactresults:
+                    exactresults[reskey].append(exactresult)
+                else:
+                    exactresults[reskey] = [exactresult]
             # if queryid in results:
             #    results[queryid].update(matchingids)
             # else:
             #    results[queryid] = Counter(matchingids)
 
 
 def docorequeries(syntree: SynTree, queries: QueryDict, results: ExactResultsDict, allmatches: MatchesDict):
@@ -519,16 +540,17 @@
     fullpattern = r'^(' + basepattern + r')*$'
     return (re.compile(basepattern), re.compile(fullpattern))
 
 
 def get_definedfornonemptygold(goldscores, queries: QueryDict) -> Tuple[int, List[QId]]:
     undefinedqueries = []
     definedfornonemptygoldscore = 0
-    for queryid in goldscores:
-        if goldscores[queryid] != emptycounter:
+    for reskey in goldscores:
+        if goldscores[reskey] != emptycounter:
+            queryid = reskey[0]
             if queryid in queries:
                 if queries[queryid].query != '':
                     definedfornonemptygoldscore += 1
                 else:
                     undefinedqueries.append(queryid)
     return (definedfornonemptygoldscore, undefinedqueries)
 
@@ -597,27 +619,29 @@
         newexactresults[qid] = newlist
     return newexactresults
 
 
 def passfilter(rawexactresults: ExactResultsDict, method: Method) -> ExactResultsDict:
     """
     let only those through that satisfy the filter
-    :param rawexactresults: dictionary with queryid as key and a Counter as value, exact results
+    :param rawexactresults: dictionary with ResultsKey as key and a Counter as value, exact results
     :param method: Method object
     :return: a filtered version of rawexactresults: results that pass the filter
     """
-    exactresults: ExactResultsDict = defaultdict(list)
+#    exactresults: ExactResultsDict = defaultdict(list)  # hiermee ontstaat een probleem: dictionary size changed in iteration
+    exactresults: ExactResultsDict = {}
     queries = method.queries
-    for queryid in rawexactresults:
+    for reskey in rawexactresults:
+        queryid = reskey[0]
         query = queries[queryid]
         queryfilter = query.filter
         thefilter = method.defaultfilter if queryfilter is None or queryfilter == '' else str2functionmap[
             queryfilter]
-        exactresults[queryid] = [r for r in rawexactresults[queryid]
-                                 if thefilter(query, rawexactresults, r)]
+        exactresults[reskey] = [r for r in rawexactresults[reskey] if reskey in rawexactresults and
+                                thefilter(query, rawexactresults, r)]
     return exactresults
 
 
 def getmaxsamplesizeuttidsandcutoff(allresults: AllResults) -> Tuple[List[UttId], int, Position]:
     cutoffpoint = None
     words = getallrealwords(allresults)
     cumwordcount = 0
@@ -825,17 +849,17 @@
     else:
         settings.LOGGER.error(
             'Neither an annotationfile nor a goldfile, nor a gold count file specified. Aborting')
         exit(1)
 
     # rawcoreresults = {}
     # exact = True
-    rawexactresults: ExactResultsDict = defaultdict(list)
+    rawexactresults: ExactResultsDict = {}
 
-    # @dit aanpassen , voor al de message-done
+    # @dit aanpassen , vooral de message-done
     if not os.path.exists(options.infilename):
         settings.LOGGER.error(
             'Input treebank or annotationfile {} not found. Aborting'.format(options.infilename))
         exit(1)
 
     # gather remarks on results of earlier runs, write them to a perm_file  and adapt the silverscore file
 
@@ -940,14 +964,16 @@
         errorwb.close()
 
         # analysedtrees consists of (uttid, syntree) pairs in the order in which they come in
         analysedtrees: List[(UttId, SynTree)] = []
         for syntree in treebank:
             temputtid = getuttid(syntree)
             uttcount += 1
+            # if temputtid == '118':
+            #     showtree(syntree, 'tree 118')
             # settings.LOGGER.error('uttcount={}'.format(uttcount))
             mustbedone = get_mustbedone(syntree, targets)
             if mustbedone:
                 # uttid = getuttid(syntree)
                 # analysedtrees consists of (uttid, syntree) pairs in order
                 uttid = getxselseuttid(syntree)
                 analysedtrees.append((uttid, syntree))
@@ -981,28 +1007,28 @@
     # adapt the exactresults  positions to the reference
 
     coreresults = exact2results(exactresults)
 
     platinuminfilefound = False
     if os.path.exists(options.platinuminfilename):
         platinuminfilefound = True
-        platinumresults: Dict[QId, Counter] = read_referencefile(
+        platinumresults: Dict[ResultsKey, Counter] = read_referencefile(
             options.platinuminfilename, logfile)
         checkplatinum(goldscores, platinumresults, themethod.queries)
     else:
         settings.LOGGER.info('Platinum file {} not found.'.format(
             options.platinuminfilename))
         platinumresults = {}
 
     # platinumoutfilename = base + platinumsuffix + txtext
     platinumoutfile = open(platinumoutfilename, 'w', encoding='utf8')
     # platinumcheckfilename = base + platinumchecksuffix + txtext
     platinumcheckfile = open(platinumcheckfilename, 'w', encoding='utf8')
 
-    postresults: Dict[QId, Any] = {}
+    postresults: Dict[ResultsKey, Any] = {}
     allresults = AllResults(uttcount, coreresults, exactresults, postresults, allmatches, options.infilename, analysedtrees,
                             allutts, annotationinput)
 
     samplesizefunction = getsamplesizefunction(options.methodname)
     samplesizetuple: SampleSizeTuple = samplesizefunction(allresults)
 
     postquerylist: List[QId] = [
@@ -1017,15 +1043,15 @@
     # bronze reduction
     exactgoldscores = reduceexactgoldscores(
         exactgoldscores, samplesizetuple, options.methodname)  # ongoing
     goldscores = exact2results(exactgoldscores)  # ongoing
     goldcounts = scores2counts(goldscores)
 
     # silver / platinumreduction
-    platinumresults: Dict[QId, Counter] = reduceresults(
+    platinumresults: Dict[ResultsKey, Counter] = reduceresults(
         platinumresults, samplesizetuple, options.methodname)
 
     dopostqueries(allresults, postquerylist, themethod.queries)
 
     dopostqueries(allresults, formquerylist, themethod.queries)
 
     (base, ext) = os.path.splitext(options.infilename)
@@ -1057,61 +1083,62 @@
     # print the platinumheader
     print(platinumheaderstring, file=platinumoutfile)
 
     # print the results
     qcount = 0
     invalidqcount = 0
     undefinedqcount = 0
-    results: Dict[QId, ResultsCounter] = allresults.coreresults
+    results: Dict[ResultsKey, ResultsCounter] = allresults.coreresults
     # exactresults = getexactresults(allmatches)
     exact = True
 
     pcheaders = [['User1', 'User2', 'User3', 'MoreorLess', 'qid',
                   'cat', 'subcat', 'item', 'uttid', 'pos', 'utt', 'origutt']]
     allrows = []
 
-    for queryid in results:
+    for reskey in results:
         sortedgolduttlist: List[str] = []
         platinumoutresults: Dict[UttId, int] = Counter()
         platinumoutresultsstring = ''
         qcount += 1
-        theresults = results[queryid]
+        theresults = results[reskey]
         resultstr = counter2liststr(theresults)
-        if queryid in goldscores:
+        if reskey in goldscores:
             # (goldlevel, golditem, goldcounter) = goldscores[queryid]
-            goldcounter = goldscores[queryid]
+            goldcounter = goldscores[reskey]
             goldcount = sumfreq(goldcounter)
             sortedgolduttstr = counter2liststr(goldcounter)
         else:
             goldcount = 0
             sortedgolduttstr = ''
+        queryid = reskey[0]
         thequery = themethod.queries[queryid]
         if query_exists(thequery):
             if queryid not in invalidqueries:
                 qex = 'yes'
             else:
                 qex = 'invalid'
                 invalidqcount += 1
         else:
             qex = 'no'
             undefinedqcount += 1
         if query_exists(thequery) and queryid not in invalidqueries:
             # print(queryid, file=logfile)
-            if queryid in goldscores:
-                goldcounter = goldscores[queryid]
+            if reskey in goldscores:
+                goldcounter = goldscores[reskey]
             else:
                 goldcounter = Counter()
             (recall, precision, f1score) = getscores(theresults, goldcounter)
             liststargoldstr = counter2liststr(theresults & goldcounter)
             goldminustheresults = goldcounter - theresults
             goldminusliststr = counter2liststr(goldminustheresults)
             theresultsminusgold = theresults - goldcounter
             listminusgoldstr = counter2liststr(theresultsminusgold)
-            if platinuminfilefound and queryid in platinumresults:
-                theplatinumresults = platinumresults[queryid]
+            if platinuminfilefound and reskey in platinumresults:
+                theplatinumresults = platinumresults[reskey]
                 sortedplatinumliststr = counter2liststr(theplatinumresults)
                 liststarplatinumstr = counter2liststr(
                     theresults & theplatinumresults)
                 platinumminusliststr = counter2liststr(
                     theplatinumresults - theresults)
                 listminusplatinumliststr = counter2liststr(
                     theresults - theplatinumresults)
@@ -1143,16 +1170,17 @@
             theresultsminusgold = {}
             goldminustheresults = {}
             goldstarplatinumstr, platinumminusgoldstr, goldminusplatinumstr = '', '', ''
             (gprecall, gpprecision, gpf1score) = (na, na, na)
 
         platinumoutresults = theresults | goldcounter
         platinumoutresultsstring = counter2liststr(platinumoutresults)
+        reskeystr = showreskey(reskey)
 
-        queryinforow = [queryid, themethod.queries[queryid].cat, themethod.queries[queryid].subcat,
+        queryinforow = [reskeystr, themethod.queries[queryid].cat, themethod.queries[queryid].subcat,
                         themethod.queries[queryid].item]
         queryresultsrow = [str(sumfreq(theresults)), resultstr, str(
             goldcount), sortedgolduttstr, qex]
         queryRGscorerow = [sf(recall), sf(precision), sf(
             f1score), liststargoldstr, goldminusliststr, listminusgoldstr]
         queryRPscorerow = [sortedplatinumliststr, sf(platinumrecall), sf(platinumprecision), sf(platinumf1score),
                            platinumminusliststr, listminusplatinumliststr]
@@ -1161,81 +1189,88 @@
 
         fullresultrow = queryinforow + queryresultsrow + \
             queryRGscorerow + queryRPscorerow + queryGPscorerow
         print(tab.join(fullresultrow), file=outfile)
         outworksheet.write_row(outrowctr, outstartcol, fullresultrow)
         outrowctr += 1
 
-        platinumrow = [queryid, themethod.queries[queryid].cat, themethod.queries[queryid].subcat,
+        platinumrow = [reskeystr, themethod.queries[queryid].cat, themethod.queries[queryid].subcat,
                        themethod.queries[queryid].item, platinumoutresultsstring, listminusgoldstr, '', '']
 
         print(tab.join(platinumrow), file=platinumoutfile)
 
         # @with an annotationfile allmatches is empty so we need to redefine newrows (exactmismatches) markedutt (getmarkedutt)-done
         if exact:
-            newrows = exactmismatches(queryid, themethod.queries, exactresults, exactgoldscores, allmatches, allutts,
+            newrows = exactmismatches(reskey, themethod.queries, exactresults, exactgoldscores, allmatches, allutts,
                                       platinumcheckfile, silverannotationsdict, annotationinput)
             allrows += newrows
         else:
             if theresultsminusgold != {}:
                 print('More examples', file=platinumcheckfile)
             for uttid in theresultsminusgold:
-                if (queryid, uttid) in allmatches:
-                    for (m, syntree) in allmatches[(queryid, uttid)]:
+                if (reskey, uttid) in allmatches:
+                    for (m, syntree) in allmatches[(reskey, uttid)]:
                         markedutt = getmarkedutt(m, syntree)
-                        platinumcheckrow1 = [queryid, themethod.queries[queryid].cat, themethod.queries[queryid].subcat,
+                        platinumcheckrow1 = [reskey, themethod.queries[queryid].cat, themethod.queries[queryid].subcat,
                                              themethod.queries[queryid].item, uttid, markedutt]
                         print(tab.join(platinumcheckrow1),
                               file=platinumcheckfile)
 
             if goldminustheresults != {}:
                 print('Missed examples', file=platinumcheckfile)
             for uttid in goldminustheresults:
                 if uttid in allutts:
                     uttstr = space.join(allutts[uttid])
                 else:
                     settings.LOGGER.warning(
                         'uttid {} not in allutts'.format(uttid))
-                platinumcheckrow2 = [queryid, themethod.queries[queryid].cat, themethod.queries[queryid].subcat,
+                platinumcheckrow2 = [reskey, themethod.queries[queryid].cat, themethod.queries[queryid].subcat,
                                      themethod.queries[queryid].item, uttid, uttstr]
                 print(tab.join(platinumcheckrow2), file=platinumcheckfile)
 
     # platinumcheckfullname = platinumcheckfile.name
     # (base, ext) = os.path.splitext(platinumcheckfilename)
     # platinumcheckxlfullname = base + '.xlsx'
+    # add missed literal hits
+    literalmissedrows = literalmissedmatches(themethod.queries, exactresults, exactgoldscores, allmatches, allutts,
+                                             platinumcheckfile, silverannotationsdict, annotationinput)
+    allrows += literalmissedrows
+
     wb = mkworkbook(platinumcheckxlfullname, pcheaders,
                     allrows, freeze_panes=(1, 9))
     wb.close()
 
     # compute the gold postresults
     goldpostresults: Dict[UttId, int] = {}
     goldcounters: Dict[QId, ResultsCounter] = {}
     allgoldmatches: MatchesDict = {}
-    for qid in goldscores:
-        goldcounters[qid] = goldscores[qid]
+    for reskey in goldscores:
+        goldcounters[reskey] = goldscores[reskey]
     allgoldresults = AllResults(uttcount, goldcounters, exactgoldscores, goldpostresults, allgoldmatches, reffilename, [],
                                 allannutts, annotationinput)
     dopostqueries(allgoldresults, postquerylist, themethod.queries)
 
     # compute the platinum postresults
 
-    platinumpostresults: Dict[QId, Any] = {}
+    platinumpostresults: Dict[ResultsKey, Any] = {}
 
     # print the postresults
     thepostresults = allresults.postresults
     for queryid in postquerylist:
         resultposval = str(getpostval(queryid, thepostresults))
         goldpostval = str(getpostval(queryid, goldpostresults))
         platinumpostval = str(getpostval(queryid, platinumpostresults))
         if themethod.queries[queryid].query != '':
             qex = 'yes'
         else:
             qex = 'no'
 
-        queryinforow = [queryid, themethod.queries[queryid].cat, themethod.queries[queryid].subcat,
+        queryreskey = mkresultskey(queryid)
+        queryreskeystr = showreskey(queryreskey)
+        queryinforow = [queryreskeystr, themethod.queries[queryid].cat, themethod.queries[queryid].subcat,
                         themethod.queries[queryid].item]
         queryresultsrow = ['', resultposval, '', goldpostval,
                            qex] + erow(6) + [platinumpostval] + erow(11)
 
         postrow = queryinforow + queryresultsrow
         postrowstring = tab.join(queryinforow + queryresultsrow)
         print(postrowstring, sep=tab, file=outfile)
@@ -1251,92 +1286,97 @@
                       (3, 'Overall (original pre and core measures with defined queries only)',
                        lambda x: is_preorcore(x) and query_exists(x)),
                       (4, 'Overall (all original pre and core measures)', lambda x: is_preorcore(x))]
 
     logheader = ['datetime', 'treebank', 'scorenr,' 'R', 'P', 'F1', 'P-R', 'P-P', 'P-F1', 'GP-R', 'GP-P', 'GP-F1', 'ref',
                  'method']
     logname = 'sastalog.txt'
-    logpath = os.path.join(codepath, '../../sastalog')
-    os.makedirs(logpath, exist_ok=True)
+    logpath = r'.'
     logfullname = os.path.join(logpath, logname)
     biglogfile = open(logfullname, 'a', encoding='utf8')
 
     exactlynow = datetime.datetime.now()
     now = exactlynow.replace(microsecond=0).isoformat()
 
     for (ctr, message, queryfunction) in overallmethods:
         # gather resultscount
         resultscount = 0
-        for queryid in results:
+        for reskey in results:
+            queryid = reskey[0]
             thequery = themethod.queries[queryid]
             if thequery.original and queryfunction(thequery):
-                resultscount += sum(results[queryid].values())
+                resultscount += sum(results[reskey].values())
 
         # gather goldcount
         goldcount = 0
-        for queryid in goldscores:
+        for reskey in goldscores:
+            queryid = reskey[0]
             thequery = themethod.queries[queryid]
-            goldcounter = goldscores[queryid]
+            goldcounter = goldscores[reskey]
             if thequery.original and queryfunction(thequery):
                 goldcount += sum(goldcounter.values())
 
         # gather platinumcount
         platinumcount = 0
-        for queryid in platinumresults:
+        for reskey in platinumresults:
+            queryid = reskey[0]
             if queryid in themethod.queries:
                 thequery = themethod.queries[queryid]
                 if thequery.original and queryfunction(thequery):
-                    platinumcount += sum(platinumresults[queryid].values())
+                    platinumcount += sum(platinumresults[reskey].values())
             else:
                 settings.LOGGER.warning(
-                    'Query {} found in platinumresults but not in queries'.format(queryid))
+                    f'Query {reskey} found in platinumresults but {queryid} not in queries')
 
         # resultsgoldintersectiocount
         resultsgoldintersectioncount = 0
-        for queryid in results:
+        for reskey in results:
+            queryid = reskey[0]
             thequery = themethod.queries[queryid]
             if thequery.original and queryfunction(thequery):
-                if queryid in goldscores:
-                    goldcounter = goldscores[queryid]
-                    intersection = results[queryid] & goldcounter
+                if reskey in goldscores:
+                    goldcounter = goldscores[reskey]
+                    intersection = results[reskey] & goldcounter
                     resultsgoldintersectioncount += sum(intersection.values())
                 else:
                     pass
-                    # settings.LOGGER.warning('Query {} found in results but not in goldscores'.format(queryid))
+                    # settings.LOGGER.warning(f'Query {reskey} found in results but not in goldscores')
 
         # resultsplatinumintersectioncount
         resultsplatinumintersectioncount = 0
-        for queryid in results:
+        for reskey in results:
+            queryid = reskey[0]
             thequery = themethod.queries[queryid]
             if thequery.original and queryfunction(thequery):
-                if queryid in platinumresults:
-                    intersection = results[queryid] & platinumresults[queryid]
+                if reskey in platinumresults:
+                    intersection = results[reskey] & platinumresults[reskey]
                     resultsplatinumintersectioncount += sum(
                         intersection.values())
                 else:
                     pass
                     # settings.LOGGER.warning('queryid {} not in platinumresults'.format(queryid))
 
         # goldplatinumintersectioncount
         goldplatinumintersectioncount = 0
-        for queryid in platinumresults:
+        for reskey in platinumresults:
+            queryid = reskey[0]
             if queryid in themethod.queries:
                 thequery = themethod.queries[queryid]
                 if thequery.original and queryfunction(thequery):
-                    if queryid in goldscores:
-                        goldcounter = goldscores[queryid]
-                        intersection = goldcounter & platinumresults[queryid]
+                    if reskey in goldscores:
+                        goldcounter = goldscores[reskey]
+                        intersection = goldcounter & platinumresults[reskey]
                         goldplatinumintersectioncount += sum(
                             intersection.values())
                     else:
                         pass
                         # settings.LOGGER.warning('Query {} in platinumresults but not in goldscores'.format(queryid))
             else:
                 settings.LOGGER.warning(
-                    'Query {} in platinumresults but not in queries'.format(queryid))
+                    f'Query {reskey} in platinumresults but {queryid} not in queries')
 
         (recall, precision, f1score) = getevalscores(
             resultscount, goldcount, resultsgoldintersectioncount)
         (platinumrecall, platinumprecision, platinumf1score) = getevalscores(resultscount, platinumcount,
                                                                              resultsplatinumintersectioncount)
         (gprecall, gpprecision, gpf1score) = getevalscores(
             goldcount, platinumcount, goldplatinumintersectioncount)
```

### Comparing `sastadev-0.1.5/src/sastadev/allresults.py` & `sastadev-0.2.0/src/sastadev/allresults.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,100 @@
-from typing import Any, Callable, Counter, Dict, List, Union
+from collections import defaultdict
+from typing import Any, Callable, Counter, Dict, List, Tuple, Union
 
-from sastadev.sastatypes import (ExactResultsDict, FileName, MatchesDict, QId,
-                                 ResultsCounter, SynTree, UttWordDict)
+from sastadev.sastatypes import (ExactResult, ExactResults, FileName, Matches,
+                                 QId, Query, ResultsCounter, SynTree, UttId,
+                                 UttWordDict)
+from sastadev.treebankfunctions import getattval as gav
+
+slash = '/'
+reskeysep = slash
+
+
+ResultsKey = Tuple[QId, str]
+
+# class ResultsKey:  # we do not use it anymore because two instantiations with the same value are dfferent objects
+#     def __init__(self, qid: QId, value: str = None):
+#         self.qid: QId = qid
+#         self.value: str = str(qid) if value is None else value
+#
+#     def __str__(self):
+#         return f'{self.qid}/{self.value}'
+#
+#     def __repr__(self):
+#         return f"ResultsKey('{self.qid}','{self.value}')"
+
+
+def mkresultskey(qid: QId, value: str = None) -> Tuple[QId, str]:
+    if value is None:
+        return (qid, str(qid))
+    else:
+        return (qid, value)
+
+
+def showreskey(reskey):
+    return f'{reskey[0]}{reskeysep}{reskey[1]}'
+
+
+def reskeystr2reskey(reskeystr: str) -> ResultsKey:
+    parts = reskeystr.split(reskeysep)
+    result = tuple(parts)
+    return result
+
+
+def getqueryid(reskeystr: str) -> QId:
+    reskey = reskeystr2reskey(reskeystr)
+    result = reskey[0]
+    return result
 
 
 class AllResults:
     def __init__(self, uttcount, coreresults, exactresults, postresults, allmatches, filename, analysedtrees, allutts, annotationinput=False):
         self.uttcount: int = uttcount
-        self.coreresults: Dict[QId, ResultsCounter] = coreresults
+        self.coreresults: Dict[ResultsKey, ResultsCounter] = coreresults
         self.exactresults: ExactResultsDict = exactresults
-        self.postresults: Dict[QId, Any] = postresults
+        self.postresults: Dict[ResultsKey, Any] = postresults
         self.allmatches: MatchesDict = allmatches
         self.filename: FileName = filename
         self.analysedtrees: List[SynTree] = analysedtrees
         self.allutts: UttWordDict = allutts
         self.annotationinput: bool = annotationinput
 
 
-def scores2counts(scores: Dict[QId, Counter]) -> Dict[QId, int]:
+CoreQueryFunction = Callable[[SynTree], List[SynTree]]
+PostQueryFunction = Callable[[AllResults, SynTree], List[SynTree]]
+QueryFunction = Union[CoreQueryFunction, PostQueryFunction]
+
+
+def scores2counts(scores: Dict[ResultsKey, Counter]) -> Dict[QId, int]:
     '''
     input is a dictionary of Counter()s
     output is a dictionary of ints
     '''
     counts = {}
     for el in scores:
         countval = len(scores[el])
         counts[el] = countval
     return counts
 
 
 CoreQueryFunction = Callable[[SynTree], List[SynTree]]
 PostQueryFunction = Callable[[AllResults, SynTree], List[SynTree]]
 QueryFunction = Union[CoreQueryFunction, PostQueryFunction]
+
+MatchesDict = Dict[Tuple[ResultsKey, UttId], Matches]
+ExactResultsDict = Dict[ResultsKey, ExactResults]  # qid
+ExactResultsFilter = Callable[[Query, ExactResultsDict, ExactResult], bool]
+
+
+def matches2exactresults(matchesdict: MatchesDict) -> ExactResultsDict:
+    exactresultsdict = defaultdict(list)
+    for resultskey, uttid in matchesdict:
+        for match in matchesdict[(resultskey, uttid)]:
+            position = getposition(match[0])
+            exactresultsdict[resultskey].append((uttid, position))
+    return exactresultsdict
+
+
+def getposition(node: SynTree) -> int:
+    result = int(gav(node, 'begin')) + 1
+    return result
```

### Comparing `sastadev-0.1.5/src/sastadev/alpino.py` & `sastadev-0.2.0/src/sastadev/alpino.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/alpinoparsing.py` & `sastadev-0.2.0/src/sastadev/alpinoparsing.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/asta_neo.py` & `sastadev-0.2.0/src/sastadev/asta_neo.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/asta_queries.py` & `sastadev-0.2.0/src/sastadev/asta_queries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from typing import Callable, Dict, List
+from typing import Callable, Dict, List, Optional
 
 from sastadev.conf import settings
 from sastadev.dedup import getposition
 from sastadev.macros import expandmacros
 from sastadev.metadata import (longrep, repeated, repeatedseqtoken, repetition,
                                substringrep)
+from sastadev.normalise_lemma import normaliselemma
 from sastadev.sastatypes import SynTree
 from sastadev.stringfunctions import string2list
 from sastadev.tblex import asta_recognised_lexnode, asta_recognised_nounnode
 from sastadev.treebankfunctions import (clausecats, find1, getattval,
                                         getnodeyield, getyield, showtns)
 
 noun_xpath = './/node[%asta_noun%]'
@@ -21,27 +22,63 @@
 astabijzinquery = expandmacros(astabijzinquerybase)
 
 astacoredelpvquery = './/node[%coredelpv%]'
 expandedastacoredelpvquery = expandmacros(astacoredelpvquery)
 
 dpancestorsquery = 'ancestor::node[@rel="dp"] | self::node[@rel="dp" or @rel="--"]'
 
+lemma_path = './/node[%asta_noun% or %ASTA_LEX%]'
+expandedlemma_path = expandmacros(lemma_path)
+# this covers all repetitions but the short repetitions should not be included
+repetitioncond = f'@subcat="{repetition}"'
+longrepetitioncond = f'@value="{repeated}" or @value="{repeatedseqtoken}" or @value="{longrep}" or @value="{substringrep}"'
+
+
+def astalemmafunction(node: SynTree) -> str:
+    repetitionantecedent = getrepetitionantecedent(node)
+    if repetitionantecedent is not None:
+        result = astalemmafunction(repetitionantecedent)
+    else:
+        rawlemma = getattval(node, 'lemma')
+        rawword = getattval(node, 'word')
+        pt = getattval(node, 'pt')
+        if pt == 'n':
+            result = normaliselemma(rawword, rawlemma)
+        else:
+            resultlist = [c for c in rawlemma if c != '_']
+            result = ''.join(resultlist)
+    return result
+
+
+def getrepetitionantecedent(node: SynTree) -> Optional[SynTree]:
+    topnode = find1(node, 'ancestor::alpino_ds')
+    dupindex = get_dupindex(topnode, longrepetitioncond)
+    nodepos = getattval(node, 'begin')
+    if nodepos in dupindex:
+        antecedentpos = dupindex[nodepos]
+        antecedent = find1(
+            topnode, f'.//node[@word and @begin="{antecedentpos}"]')
+    else:
+        antecedent = None
+    return antecedent
+
 
 def get_dupindex(stree: SynTree, cond: str) -> Dict[str, str]:
     dupindex = {}
     dupxpath = './/xmeta[{cond}]'.format(cond=cond)
     dupmetadatalist = stree.xpath(dupxpath)
     for meta in dupmetadatalist:
         if 'annotatedposlist' in meta.attrib and 'annotationposlist' in meta.attrib:
             keyliststr = meta.attrib['annotatedposlist']
             keylist = string2list(keyliststr)
             valueliststr = meta.attrib['annotationposlist']
             valuelist = string2list(valueliststr)
             if len(keylist) != len(valuelist):
-                settings.LOGGER.error('Error in metadata: {} in sentence {}'.format(meta, getyield(stree)))
+                settings.LOGGER.error(
+                    'Error in metadata: {} in sentence {}'.format(meta, getyield(stree)))
             else:
                 for key, val in zip(keylist, valuelist):
                     dupindex[key] = val
     return dupindex
 
 
 def asta_noun(
@@ -70,40 +107,63 @@
 
     '''
 
     results = asta_x(stree, expanded_lex_xpath, asta_recognised_lexnode)
     return results
 
 
+def asta_recognised_lexicalnode(node: SynTree) -> bool:
+    result = asta_recognised_nounnode(node) or asta_recognised_lexnode(node)
+    return result
+
+
+def asta_lemma(stree: SynTree) -> List[SynTree]:
+    '''The function *asta_lemma* uses the function *asta_x* with parameters *stree*,
+    *lemma_path* and the function *asta_recognised_lexicalnode*.
+
+
+    .. autofunction:: treebankfunctions::asta_recognised_lexicalnode
+         :noindex:
+
+    '''
+    results = asta_x(stree, expandedlemma_path, asta_recognised_lexicalnode)
+    return results
+
+
 def old_asta_noun(stree: SynTree) -> List[SynTree]:
     theyield = getyield(stree)   # for debugging purposes
     thenodeyield = getnodeyield(stree)
-    cond1 = '@value="{}" or @value="{}" or @value="{}" or @value="{}"'.format(repeated, repeatedseqtoken, longrep, substringrep)
+    cond1 = '@value="{}" or @value="{}" or @value="{}" or @value="{}"'.format(
+        repeated, repeatedseqtoken, longrep, substringrep)
     dupindex = get_dupindex(stree, cond1)
     cond2 = '@subcat="{}"'.format(repetition)
     allrepdupindex = get_dupindex(stree, cond2)
     revallrepdupindex = {val: key for key, val in allrepdupindex.items()}
     noun_nodes = stree.xpath(expanded_noun_xpath)
     # print(showtns(noun_nodes))
 
     clean_noun_nodes = noun_nodes
 
     # remove the nodes that should get it from this function
-    clean_noun_nodes = [node for node in clean_noun_nodes if getattval(node, 'begin') not in allrepdupindex]
+    clean_noun_nodes = [node for node in clean_noun_nodes if getattval(
+        node, 'begin') not in allrepdupindex]
 
     # remove words not recognised as nouns; is dit nodig? Ja dit is nodig!!!
-    clean_noun_nodes = [node for node in clean_noun_nodes if asta_recognised_nounnode(node)]
+    clean_noun_nodes = [
+        node for node in clean_noun_nodes if asta_recognised_nounnode(node)]
     # print(showtns(clean_noun_nodes))
 
     additional_nodes = []
     for key in dupindex:
-        keynode = find1(stree, './/node[(@pt or @pos) and @begin="{}"]'.format(key))
+        keynode = find1(
+            stree, './/node[(@pt or @pos) and @begin="{}"]'.format(key))
         if keynode is not None:
             val = dupindex[key]
-            valnode = find1(stree, './/node[(@pt or @pos) and @begin="{}"]'.format(val))
+            valnode = find1(
+                stree, './/node[(@pt or @pos) and @begin="{}"]'.format(val))
             if valnode is not None:
                 if valnode in clean_noun_nodes:
                     additional_nodes.append(keynode)
 
     result = clean_noun_nodes + additional_nodes
     # print(showtns(result))
     return result
@@ -116,47 +176,53 @@
             return True
     return False
 
 
 def asta_delpv(stree: SynTree) -> List[SynTree]:
     coredelpvnodes = stree.xpath(expandedastacoredelpvquery)
     streeleaves = getnodeyield(stree)
-    wwbegins = [getattval(node, 'begin') for node in streeleaves if getattval(node, 'pt') == 'ww']
-    delpvnodes = [node for node in coredelpvnodes if node.xpath(dpancestorsquery) == [] or not (verbleftof(node, wwbegins))]
+    wwbegins = [getattval(node, 'begin')
+                for node in streeleaves if getattval(node, 'pt') == 'ww']
+    delpvnodes = [node for node in coredelpvnodes if node.xpath(
+        dpancestorsquery) == [] or not (verbleftof(node, wwbegins))]
     return delpvnodes
 
 
 def asta_x(stree: SynTree,
            xpathexpr: str,
            recognized_x_f: Callable[[SynTree], bool]) -> List[SynTree]:
     theyield = getyield(stree)   # for debugging purposes
     thenodeyield = getnodeyield(stree)
-    cond1 = '@value="{}" or @value="{}" or @value="{}" or @value="{}"'.format(repeated, repeatedseqtoken, longrep, substringrep)
+    cond1 = '@value="{}" or @value="{}" or @value="{}" or @value="{}"'.format(
+        repeated, repeatedseqtoken, longrep, substringrep)
     dupindex = get_dupindex(stree, cond1)
     cond2 = '@subcat="{}"'.format(repetition)
     allrepdupindex = get_dupindex(stree, cond2)
     revallrepdupindex = {val: key for key, val in allrepdupindex.items()}
     x_nodes = stree.xpath(xpathexpr)
     # print(showtns(noun_nodes))
 
     clean_x_nodes = x_nodes
 
     # remove the nodes that should get it from this function
-    clean_x_nodes = [node for node in clean_x_nodes if getattval(node, 'begin') not in allrepdupindex]
+    clean_x_nodes = [node for node in clean_x_nodes if getattval(
+        node, 'begin') not in allrepdupindex]
 
     # remove words not recognised as nouns; is dit nodig? Ja dit is nodig!!!
     clean_x_nodes = [node for node in clean_x_nodes if recognized_x_f(node)]
     # print(showtns(clean_noun_nodes))
 
     additional_nodes = []
     for key in dupindex:
-        keynode = find1(stree, './/node[(@pt or @pos) and @begin="{}"]'.format(key))
+        keynode = find1(
+            stree, './/node[(@pt or @pos) and @begin="{}"]'.format(key))
         if keynode is not None:
             val = dupindex[key]
-            valnode = find1(stree, './/node[(@pt or @pos) and @begin="{}"]'.format(val))
+            valnode = find1(
+                stree, './/node[(@pt or @pos) and @begin="{}"]'.format(val))
             if valnode is not None:
                 if valnode in clean_x_nodes:
                     additional_nodes.append(keynode)
 
     result = clean_x_nodes + additional_nodes
     # print(showtns(result))
     return result
@@ -188,15 +254,16 @@
     results = [node for node in nodes if getposition(node) == position]
     lresults = len(results)
     if lresults == 0:
         result = None
     elif lresults == 1:
         result = results[0]
     else:
-        settings.LOGGER.warning('Multiple nodes found for position {}: {}, in {}'.format(position, showtns(results), showtns(nodes)))
+        settings.LOGGER.warning('Multiple nodes found for position {}: {}, in {}'.format(
+            position, showtns(results), showtns(nodes)))
         result = results[0]
     return result
 
 
 bijzin_xpath = './/node[%ASTA_Bijzin%]'
 expanded_bijzin_xpath = expandmacros(bijzin_xpath)
 
@@ -214,15 +281,16 @@
     The function *removerepetitions* returns a list of nodes from *ptnodes* that are
     not marked in the metadata as repetitions.
 
     '''
     newptnodes = []
     for ptnode in ptnodes:
         ptnodeend = ptnode.attrib['begin'] if 'begin' in ptnode.attrib else None
-        xmetaxpath = './/xmeta[@subcat="Repetition" and @annotatedposlist="[{}]"]'.format(ptnodeend)
+        xmetaxpath = './/xmeta[@subcat="Repetition" and @annotatedposlist="[{}]"]'.format(
+            ptnodeend)
         repmetas = stree.xpath(xmetaxpath)
         if repmetas == []:
             newptnodes.append(ptnode)
     return newptnodes
 
 
 def asta_bijzin(stree: SynTree) -> List[SynTree]:
@@ -256,28 +324,31 @@
 
     .. autofunction:: asta_queries::removerepetitions
     '''
     theyield = getyield(stree)
     clausenodes = stree.xpath(astabijzinquery)
     ptnodes = [n for n in clausenodes if 'pt' in n.attrib]
     okptnodes = removerepetitions(ptnodes, stree)
-    trueclausenodes = [n for n in clausenodes if getattval(n, 'cat') in clausecats]
+    trueclausenodes = [
+        n for n in clausenodes if getattval(n, 'cat') in clausecats]
     # alternative 1
     # sortedclausenodes = sorted(trueclausenodes, key=lambda x: (int(getattval(x,'begin')), -int(getattval(x, 'end'))))
     # result = sortedclausenodes[1:] + okptnodes
 
     # alternative2 -follows the conventions for ASTA
-    sortedclausenodes = sorted(trueclausenodes, key=lambda x: (int(getattval(x, 'begin')), int(getattval(x, 'end'))))
+    sortedclausenodes = sorted(trueclausenodes, key=lambda x: (
+        int(getattval(x, 'begin')), int(getattval(x, 'end'))))
     if len(sortedclausenodes) > 1:
         cn0 = sortedclausenodes[0]
         cn1 = sortedclausenodes[1]
         if getattval(cn1, 'begin') == getattval(cn0, 'begin'):
             cn0end = getattval(cn0, 'end')
             newbegin = cn0end
-            newokptnodexpath = '//node[@pt and @begin="{newbegin}"]'.format(newbegin=newbegin)
+            newokptnodexpath = '//node[@pt and @begin="{newbegin}"]'.format(
+                newbegin=newbegin)
             newokptnode = find1(cn1, newokptnodexpath)
             result = sortedclausenodes[2:] + okptnodes
             if newokptnode is not None:
                 result += [newokptnode]
         else:
             result = sortedclausenodes[1:] + okptnodes
     else:
```

### Comparing `sastadev-0.1.5/src/sastadev/astaforms.py` & `sastadev-0.2.0/src/sastadev/astaforms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,819 +1,959 @@
 00000000: 0d0a 6672 6f6d 2063 6f6c 6c65 6374 696f  ..from collectio
 00000010: 6e73 2069 6d70 6f72 7420 436f 756e 7465  ns import Counte
 00000020: 722c 2064 6566 6175 6c74 6469 6374 0d0a  r, defaultdict..
 00000030: 6672 6f6d 2069 6f20 696d 706f 7274 2042  from io import B
-00000040: 7974 6573 494f 0d0a 0d0a 696d 706f 7274  ytesIO....import
-00000050: 2078 6c73 7877 7269 7465 720d 0a0d 0a66   xlsxwriter....f
-00000060: 726f 6d20 7361 7374 6164 6576 2e41 5354  rom sastadev.AST
-00000070: 4170 6f73 7466 756e 6374 696f 6e73 2069  Apostfunctions i
-00000080: 6d70 6f72 7420 286e 6f75 6e6c 656d 6d61  mport (nounlemma
-00000090: 7169 642c 2076 6572 626c 656d 6d61 7169  qid, verblemmaqi
-000000a0: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
-000000b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000000c0: 2020 2020 2020 2020 2020 2020 776f 7264              word
-000000d0: 636f 756e 7470 6572 7574 7429 0d0a 6672  countperutt)..fr
+00000040: 7974 6573 494f 0d0a 6672 6f6d 2074 7970  ytesIO..from typ
+00000050: 696e 6720 696d 706f 7274 2044 6963 740d  ing import Dict.
+00000060: 0a0d 0a69 6d70 6f72 7420 786c 7378 7772  ...import xlsxwr
+00000070: 6974 6572 0d0a 0d0a 6672 6f6d 2073 6173  iter....from sas
+00000080: 7461 6465 762e 616c 6c72 6573 756c 7473  tadev.allresults
+00000090: 2069 6d70 6f72 7420 6d6b 7265 7375 6c74   import mkresult
+000000a0: 736b 6579 0d0a 6672 6f6d 2073 6173 7461  skey..from sasta
+000000b0: 6465 762e 4153 5441 706f 7374 6675 6e63  dev.ASTApostfunc
+000000c0: 7469 6f6e 7320 696d 706f 7274 2077 6f72  tions import wor
+000000d0: 6463 6f75 6e74 7065 7275 7474 0d0a 6672  dcountperutt..fr
 000000e0: 6f6d 2073 6173 7461 6465 762e 666f 726d  om sastadev.form
 000000f0: 7320 696d 706f 7274 2067 6574 666f 726d  s import getform
-00000100: 6669 6c65 6e61 6d65 0d0a 0d0a 6772 6565  filename....gree
-00000110: 6e20 3d20 2723 3030 4646 3030 270d 0a72  n = '#00FF00'..r
-00000120: 6564 203d 2027 2346 4630 3030 3027 0d0a  ed = '#FF0000'..
-00000130: 6f72 616e 6765 203d 2027 2346 4642 4239  orange = '#FFBB9
-00000140: 4127 0d0a 6772 6579 203d 2027 2342 3042  A'..grey = '#B0B
-00000150: 3042 3027 0d0a 0d0a 0d0a 2320 6772 6565  0B0'......# gree
-00000160: 6e20 3d20 2767 7265 656e 270d 0a23 2067  n = 'green'..# g
-00000170: 7265 656e 203d 2027 2330 3036 3130 3027  reen = '#006100'
-00000180: 0d0a 2320 7265 6420 3d20 2723 3943 3030  ..# red = '#9C00
-00000190: 3036 270d 0a23 2072 6564 203d 2027 7265  06'..# red = 're
-000001a0: 6427 0d0a 2320 6f72 616e 6765 203d 2027  d'..# orange = '
-000001b0: 2339 4336 3530 3027 0d0a 2320 6f72 616e  #9C6500'..# oran
-000001c0: 6765 203d 2027 7965 6c6c 6f77 270d 0a0d  ge = 'yellow'...
-000001d0: 0a0d 0a63 6c61 7373 2045 7863 656c 466f  ...class ExcelFo
-000001e0: 726d 3a0d 0a20 2020 2064 6566 205f 5f69  rm:..    def __i
-000001f0: 6e69 745f 5f28 7365 6c66 2c20 7461 6265  nit__(self, tabe
-00000200: 6c2c 2073 636f 7265 7329 3a0d 0a20 2020  l, scores):..   
-00000210: 2020 2020 2073 656c 662e 7461 6265 6c20       self.tabel 
-00000220: 3d20 7461 6265 6c0d 0a20 2020 2020 2020  = tabel..       
-00000230: 2073 656c 662e 7363 6f72 6573 203d 2073   self.scores = s
-00000240: 636f 7265 730d 0a0d 0a0d 0a63 6c61 7373  cores......class
-00000250: 2041 7374 6146 6f72 6d44 6174 613a 0d0a   AstaFormData:..
-00000260: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00000270: 2873 656c 662c 206e 6f75 6e64 6963 742c  (self, noundict,
-00000280: 2076 6572 6264 6963 742c 2076 6172 6469   verbdict, vardi
-00000290: 6374 2c20 7574 746c 6973 7429 3a0d 0a20  ct, uttlist):.. 
-000002a0: 2020 2020 2020 2073 656c 662e 6e6f 756e         self.noun
-000002b0: 6469 6374 203d 206e 6f75 6e64 6963 740d  dict = noundict.
-000002c0: 0a20 2020 2020 2020 2073 656c 662e 7665  .        self.ve
-000002d0: 7262 6469 6374 203d 2076 6572 6264 6963  rbdict = verbdic
-000002e0: 740d 0a20 2020 2020 2020 2073 656c 662e  t..        self.
-000002f0: 7661 7264 6963 7420 3d20 7661 7264 6963  vardict = vardic
-00000300: 740d 0a20 2020 2020 2020 2073 656c 662e  t..        self.
-00000310: 7574 746c 6973 7420 3d20 7574 746c 6973  uttlist = uttlis
-00000320: 740d 0a0d 0a0d 0a66 6f72 6d75 6c61 7465  t......formulate
-00000330: 6d70 6c61 7465 3120 3d20 273d 4946 2842  mplate1 = '=IF(B
-00000340: 7b7d 3d22 4e69 6574 2067 6576 756c 6422  {}="Niet gevuld"
-00000350: 2c42 7b7d 2c28 427b 7d2d 5461 6265 6c21  ,B{},(B{}-Tabel!
-00000360: 427b 7d29 2f54 6162 656c 2143 7b7d 2927  B{})/Tabel!C{})'
-00000370: 0d0a 0d0a 0d0a 6465 6620 6170 706c 7974  ......def applyt
-00000380: 656d 706c 6174 6531 2872 6f77 6374 7229  emplate1(rowctr)
-00000390: 3a0d 0a20 2020 2072 6573 756c 7420 3d20  :..    result = 
-000003a0: 666f 726d 756c 6174 656d 706c 6174 6531  formulatemplate1
-000003b0: 2e66 6f72 6d61 7428 726f 7763 7472 2c20  .format(rowctr, 
-000003c0: 726f 7763 7472 2c20 726f 7763 7472 2c20  rowctr, rowctr, 
-000003d0: 726f 7763 7472 202b 2031 2c20 726f 7763  rowctr + 1, rowc
-000003e0: 7472 202b 2031 290d 0a20 2020 2072 6574  tr + 1)..    ret
-000003f0: 7572 6e20 7265 7375 6c74 0d0a 0d0a 0d0a  urn result......
-00000400: 666f 726d 756c 6174 656d 706c 6174 6532  formulatemplate2
-00000410: 203d 2027 3d28 427b 7d2d 5461 6265 6c21   = '=(B{}-Tabel!
-00000420: 427b 7d29 2f54 6162 656c 2143 7b7d 270d  B{})/Tabel!C{}'.
-00000430: 0a0d 0a0d 0a64 6566 2061 7070 6c79 7465  .....def applyte
-00000440: 6d70 6c61 7465 3228 726f 7763 7472 293a  mplate2(rowctr):
-00000450: 0d0a 2020 2020 7265 7375 6c74 203d 2066  ..    result = f
-00000460: 6f72 6d75 6c61 7465 6d70 6c61 7465 322e  ormulatemplate2.
-00000470: 666f 726d 6174 2872 6f77 6374 722c 2072  format(rowctr, r
-00000480: 6f77 6374 7220 2b20 312c 2072 6f77 6374  owctr + 1, rowct
-00000490: 7220 2b20 3129 0d0a 2020 2020 7265 7475  r + 1)..    retu
-000004a0: 726e 2072 6573 756c 740d 0a0d 0a0d 0a66  rn result......f
-000004b0: 6f72 6d75 6c61 7465 6d70 6c61 7465 3320  ormulatemplate3 
-000004c0: 3d20 223d 4946 2849 5345 5252 4f52 2852  = "=IF(ISERROR(R
-000004d0: 4f55 4e44 2827 7b7d 2721 7b7d 332c 3229  OUND('{}'!{}3,2)
-000004e0: 292c 5c22 4e69 6574 2067 6576 756c 645c  ),\"Niet gevuld\
-000004f0: 222c 524f 554e 4428 277b 7d27 217b 7d33  ",ROUND('{}'!{}3
-00000500: 2c32 2929 220d 0a0d 0a0d 0a64 6566 2061  ,2))"......def a
-00000510: 7070 6c79 7465 6d70 6c61 7465 3328 7368  pplytemplate3(sh
-00000520: 6565 742c 2063 6f6c 6368 6172 293a 0d0a  eet, colchar):..
-00000530: 2020 2020 7265 7375 6c74 203d 2066 6f72      result = for
-00000540: 6d75 6c61 7465 6d70 6c61 7465 332e 666f  mulatemplate3.fo
-00000550: 726d 6174 2873 6865 6574 2c20 636f 6c63  rmat(sheet, colc
-00000560: 6861 722c 2073 6865 6574 2c20 636f 6c63  har, sheet, colc
-00000570: 6861 7229 0d0a 2020 2020 7265 7475 726e  har)..    return
-00000580: 2072 6573 756c 740d 0a0d 0a0d 0a66 696e   result......fin
-00000590: 6965 7468 6569 6473 696e 6465 7873 636f  ietheidsindexsco
-000005a0: 7265 203d 2022 3d49 4628 4953 4552 524f  re = "=IF(ISERRO
-000005b0: 5228 524f 554e 4428 5569 7469 6e67 656e  R(ROUND(Uitingen
-000005c0: 2144 332c 3229 292c 5c22 4e69 6574 2067  !D3,2)),\"Niet g
-000005d0: 6576 756c 645c 222c 524f 554e 4428 5569  evuld\",ROUND(Ui
-000005e0: 7469 6e67 656e 2144 332c 3229 2922 0d0a  tingen!D3,2))"..
-000005f0: 7063 7573 636f 7265 203d 2022 3d49 4628  pcuscore = "=IF(
-00000600: 4953 4552 524f 5228 524f 554e 4428 5569  ISERROR(ROUND(Ui
-00000610: 7469 6e67 656e 2142 342f 5569 7469 6e67  tingen!B4/Uiting
-00000620: 656e 2142 312c 3229 292c 5c22 4e69 6574  en!B1,2)),\"Niet
-00000630: 2067 6576 756c 645c 222c 524f 554e 4428   gevuld\",ROUND(
-00000640: 5569 7469 6e67 656e 2142 342f 5569 7469  Uitingen!B4/Uiti
-00000650: 6e67 656e 2142 312c 3229 2922 0d0a 0d0a  ngen!B1,2))"....
-00000660: 7461 6265 6c20 3d20 5b5b 2727 2c20 2747  tabel = [['', 'G
-00000670: 454d 272c 2027 5344 275d 2c0d 0a20 2020  EM', 'SD'],..   
-00000680: 2020 2020 2020 5b27 4161 6e74 616c 207a        ['Aantal z
-00000690: 656c 6673 7461 6e64 6967 6520 6e61 616d  elfstandige naam
-000006a0: 776f 6f72 6465 6e27 2c20 3438 2c20 372e  woorden', 48, 7.
-000006b0: 3838 5d2c 0d0a 2020 2020 2020 2020 205b  88],..         [
-000006c0: 2754 5452 207a 656c 6673 7461 6e64 6967  'TTR zelfstandig
-000006d0: 6520 6e61 616d 776f 6f72 6465 6e27 2c20  e naamwoorden', 
-000006e0: 302e 3736 2c20 302e 3038 5d2c 0d0a 2020  0.76, 0.08],..  
-000006f0: 2020 2020 2020 205b 274c 6578 6963 616c         ['Lexical
-00000700: 6520 7765 726b 776f 6f72 6465 6e27 2c20  e werkwoorden', 
-00000710: 3239 2c20 342e 3134 5d2c 0d0a 2020 2020  29, 4.14],..    
-00000720: 2020 2020 205b 2754 5452 206c 6578 6963       ['TTR lexic
-00000730: 616c 2077 6572 6b77 6f6f 7264 656e 272c  al werkwoorden',
-00000740: 2030 2e36 332c 2030 2e31 315d 2c0d 0a20   0.63, 0.11],.. 
-00000750: 2020 2020 2020 2020 5b27 5365 6d61 6e74          ['Semant
-00000760: 6973 6368 6520 7061 7261 6661 7369 65c3  ische parafasie.
-00000770: ab6e 272c 2030 2c20 302e 3537 5d2c 0d0a  .n', 0, 0.57],..
-00000780: 2020 2020 2020 2020 205b 2746 6f6e 6f6c           ['Fonol
-00000790: 6f67 6973 6368 6520 7061 7261 6661 7369  ogische parafasi
-000007a0: 65c3 ab6e 272c 2030 2c20 302e 3333 5d2c  e..n', 0, 0.33],
-000007b0: 0d0a 2020 2020 2020 2020 205b 274e 656f  ..         ['Neo
-000007c0: 6c6f 6769 736d 656e 272c 2030 2c20 305d  logismen', 0, 0]
-000007d0: 2c0d 0a20 2020 2020 2020 2020 5b27 4161  ,..         ['Aa
-000007e0: 6e74 616c 206b 6f70 7065 6c2f 6d6f 6461  ntal koppel/moda
-000007f0: 616c 7765 726b 776f 6f72 6465 6e27 2c20  alwerkwoorden', 
-00000800: 3132 2c20 342e 3135 5d2c 0d0a 2020 2020  12, 4.15],..    
-00000810: 2020 2020 205b 274d 4c55 272c 2038 2e36       ['MLU', 8.6
-00000820: 332c 2031 2e37 345d 2c0d 0a20 2020 2020  3, 1.74],..     
-00000830: 2020 2020 5b27 5065 7263 656e 7461 6765      ['Percentage
-00000840: 2063 6f72 7265 6374 6520 7569 7469 6e67   correcte uiting
-00000850: 656e 272c 2030 2e39 332c 2030 2e30 365d  en', 0.93, 0.06]
-00000860: 2c0d 0a20 2020 2020 2020 2020 5b27 4669  ,..         ['Fi
-00000870: 6e69 6574 6865 6964 7369 6e64 6578 272c  nietheidsindex',
-00000880: 2030 2e39 392c 2030 2e30 335d 2c0d 0a20   0.99, 0.03],.. 
-00000890: 2020 2020 2020 2020 5b27 4161 6e74 616c          ['Aantal
-000008a0: 2062 696a 7a69 6e6e 656e 272c 2034 2e38   bijzinnen', 4.8
-000008b0: 2c20 322e 3738 5d5d 0d0a 0d0a 7363 6f72  , 2.78]]....scor
-000008c0: 6573 203d 205b 5b27 272c 2027 5363 6f72  es = [['', 'Scor
-000008d0: 6527 2c20 2753 4427 5d2c 0d0a 2020 2020  e', 'SD'],..    
-000008e0: 2020 2020 2020 5b27 4161 6e74 616c 207a        ['Aantal z
-000008f0: 656c 6673 7461 6e64 6967 6520 6e61 616d  elfstandige naam
-00000900: 776f 6f72 6465 6e27 2c20 223d 275a 4e57  woorden', "='ZNW
-00000910: 2026 2057 5727 2142 3122 2c20 223d 2842   & WW'!B1", "=(B
-00000920: 322d 5461 6265 6c21 4233 292f 5461 6265  2-Tabel!B3)/Tabe
-00000930: 6c21 4333 225d 2c0d 0a20 2020 2020 2020  l!C3"],..       
-00000940: 2020 205b 2754 5452 207a 656c 6673 7461     ['TTR zelfsta
-00000950: 6e64 6967 6520 6e61 616d 776f 6f72 6465  ndige naamwoorde
-00000960: 6e27 2c20 6170 706c 7974 656d 706c 6174  n', applytemplat
-00000970: 6533 2827 5a4e 5720 2620 5757 272c 2027  e3('ZNW & WW', '
-00000980: 4227 292c 2061 7070 6c79 7465 6d70 6c61  B'), applytempla
-00000990: 7465 3128 3329 5d2c 0d0a 2020 2020 2020  te1(3)],..      
-000009a0: 2020 2020 5b27 4161 6e74 616c 206c 6578      ['Aantal lex
-000009b0: 6963 616c 6520 7765 726b 776f 6f72 6465  icale werkwoorde
-000009c0: 6e27 2c20 223d 275a 4e57 2026 2057 5727  n', "='ZNW & WW'
-000009d0: 2146 3122 2c20 6170 706c 7974 656d 706c  !F1", applytempl
-000009e0: 6174 6532 2834 295d 2c0d 0a20 2020 2020  ate2(4)],..     
-000009f0: 2020 2020 205b 2754 5452 206c 6578 6963       ['TTR lexic
-00000a00: 616c 6520 7765 726b 776f 6f72 6465 6e27  ale werkwoorden'
-00000a10: 2c20 6170 706c 7974 656d 706c 6174 6533  , applytemplate3
-00000a20: 2827 5a4e 5720 2620 5757 272c 2027 4627  ('ZNW & WW', 'F'
-00000a30: 292c 2061 7070 6c79 7465 6d70 6c61 7465  ), applytemplate
-00000a40: 3128 3529 5d2c 0d0a 2020 2020 2020 2020  1(5)],..        
-00000a50: 2020 5b27 5365 6d61 6e74 6973 6368 6520    ['Semantische 
-00000a60: 7061 7261 6661 7369 65c3 ab6e 272c 2027  parafasie..n', '
-00000a70: 272c 2061 7070 6c79 7465 6d70 6c61 7465  ', applytemplate
-00000a80: 3228 3629 5d2c 0d0a 2020 2020 2020 2020  2(6)],..        
-00000a90: 2020 5b27 466f 6e6f 6c6f 6769 7363 6865    ['Fonologische
-00000aa0: 2070 6172 6166 6173 6965 c3ab 6e27 2c20   parafasie..n', 
-00000ab0: 2727 2c20 6170 706c 7974 656d 706c 6174  '', applytemplat
-00000ac0: 6532 2837 295d 2c0d 0a20 2020 2020 2020  e2(7)],..       
-00000ad0: 2020 205b 274e 656f 6c6f 6769 736d 656e     ['Neologismen
-00000ae0: 272c 2027 272c 2027 3d49 4628 4238 3d30  ', '', '=IF(B8=0
-00000af0: 2c22 4e6f 726d 6161 6c22 2c22 4166 7769  ,"Normaal","Afwi
-00000b00: 6a6b 656e 6422 2927 5d2c 0d0a 2020 2020  jkend")'],..    
-00000b10: 2020 2020 2020 5b27 4161 6e74 616c 206b        ['Aantal k
-00000b20: 6f70 7065 6c2f 6d6f 6461 616c 7765 726b  oppel/modaalwerk
-00000b30: 776f 6f72 6465 6e27 2c20 2727 2c20 6170  woorden', '', ap
-00000b40: 706c 7974 656d 706c 6174 6532 2839 295d  plytemplate2(9)]
-00000b50: 2c0d 0a20 2020 2020 2020 2020 205b 274d  ,..          ['M
-00000b60: 4c55 272c 2061 7070 6c79 7465 6d70 6c61  LU', applytempla
-00000b70: 7465 3328 2755 6974 696e 6765 6e27 2c20  te3('Uitingen', 
-00000b80: 2742 2729 2c20 6170 706c 7974 656d 706c  'B'), applytempl
-00000b90: 6174 6531 2831 3029 5d2c 0d0a 2020 2020  ate1(10)],..    
-00000ba0: 2020 2020 2020 5b27 5065 7263 656e 7461        ['Percenta
-00000bb0: 6765 2063 6f72 7265 6374 6520 7569 7469  ge correcte uiti
-00000bc0: 6e67 656e 272c 2070 6375 7363 6f72 652c  ngen', pcuscore,
-00000bd0: 2061 7070 6c79 7465 6d70 6c61 7465 3128   applytemplate1(
-00000be0: 3131 295d 2c0d 0a20 2020 2020 2020 2020  11)],..         
-00000bf0: 205b 2746 696e 6965 7468 6569 6473 696e   ['Finietheidsin
-00000c00: 6465 7827 2c20 6669 6e69 6574 6865 6964  dex', finietheid
-00000c10: 7369 6e64 6578 7363 6f72 652c 2061 7070  sindexscore, app
-00000c20: 6c79 7465 6d70 6c61 7465 3128 3132 295d  lytemplate1(12)]
-00000c30: 2c0d 0a20 2020 2020 2020 2020 205b 2741  ,..          ['A
-00000c40: 616e 7461 6c20 6269 6a7a 696e 6e65 6e27  antal bijzinnen'
-00000c50: 2c20 273d 5569 7469 6e67 656e 2146 3227  , '=Uitingen!F2'
-00000c60: 2c20 6170 706c 7974 656d 706c 6174 6532  , applytemplate2
-00000c70: 2831 3329 5d5d 0d0a 0d0a 7368 6565 7432  (13)]]....sheet2
-00000c80: 6869 6464 656e 726f 7773 203d 205b 5b27  hiddenrows = [['
-00000c90: 546f 7461 616c 272c 2027 3d53 554d 2844  Totaal', '=SUM(D
-00000ca0: 363a 4431 3035 2927 2c20 2727 2c20 2727  6:D105)', '', ''
-00000cb0: 2c20 2727 2c20 273d 5355 4d28 4836 3a48  , '', '=SUM(H6:H
-00000cc0: 3130 3529 275d 2c0d 0a20 2020 2020 2020  105)'],..       
-00000cd0: 2020 2020 2020 2020 2020 2020 205b 2741               ['A
-00000ce0: 616e 7461 6c20 756e 6965 6b27 2c20 273d  antal uniek', '=
-00000cf0: 434f 554e 5441 2842 363a 4231 3035 2927  COUNTA(B6:B105)'
-00000d00: 2c20 2727 2c20 2727 2c20 2727 2c20 273d  , '', '', '', '=
-00000d10: 434f 554e 5441 2846 363a 4631 3035 2927  COUNTA(F6:F105)'
-00000d20: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00000d30: 2020 2020 2020 2020 5b27 5454 5227 2c20          ['TTR', 
-00000d40: 273d 4232 2f42 3127 2c20 2727 2c20 2727  '=B2/B1', '', ''
-00000d50: 2c20 2727 2c20 273d 4632 2f46 3127 5d2c  , '', '=F2/F1'],
-00000d60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000d70: 2020 2020 2020 5b27 272c 2027 272c 2027        ['', '', '
-00000d80: 272c 2027 272c 2027 272c 2027 275d 0d0a  ', '', '', '']..
-00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000da0: 2020 2020 5d0d 0a0d 0a73 6865 6574 3368      ]....sheet3h
-00000db0: 6964 6465 6e72 6f77 7320 3d20 5b5b 2741  iddenrows = [['A
-00000dc0: 616e 7461 6c27 2c20 273d 434f 554e 5441  antal', '=COUNTA
-00000dd0: 2842 363a 4231 3035 2927 2c20 2727 2c20  (B6:B105)', '', 
-00000de0: 2753 6f6d 272c 2027 536f 6d27 2c20 2753  'Som', 'Som', 'S
-00000df0: 6f6d 275d 2c0d 0a20 2020 2020 2020 2020  om'],..         
-00000e00: 2020 2020 2020 2020 2020 205b 2754 6f74             ['Tot
-00000e10: 6161 6c27 2c20 273d 5355 4d28 4236 3a42  aal', '=SUM(B6:B
-00000e20: 3130 3529 272c 2027 272c 2027 3d53 554d  105)', '', '=SUM
-00000e30: 2844 363a 4431 3035 2927 2c20 273d 5355  (D6:D105)', '=SU
-00000e40: 4d28 4536 3a45 3130 3529 272c 2027 3d53  M(E6:E105)', '=S
-00000e50: 554d 2846 363a 4631 3035 2927 5d2c 0d0a  UM(F6:F105)'],..
-00000e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e70: 2020 2020 5b27 4d4c 5527 2c20 273d 4232      ['MLU', '=B2
-00000e80: 2f42 3127 2c20 2727 2c20 273d 2844 322f  /B1', '', '=(D2/
-00000e90: 2844 322b 4532 2929 272c 2027 272c 2027  (D2+E2))', '', '
-00000ea0: 275d 2c0d 0a20 2020 2020 2020 2020 2020  '],..           
-00000eb0: 2020 2020 2020 2020 205b 2743 6f72 7265           ['Corre
-00000ec0: 6374 272c 2027 3d43 4f55 4e54 4946 2843  ct', '=COUNTIF(C
-00000ed0: 363a 4331 3035 2c22 4a22 2927 2c20 2727  6:C105,"J")', ''
-00000ee0: 2c20 2727 2c20 2727 2c20 2727 5d0d 0a20  , '', '', ''].. 
-00000ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f00: 2020 205d 0d0a 0d0a 7368 6565 7432 6865     ]....sheet2he
-00000f10: 6164 6572 203d 205b 274e 756d 6d65 7227  ader = ['Nummer'
-00000f20: 2c20 275a 656c 6673 7461 6e64 6967 206e  , 'Zelfstandig n
-00000f30: 6161 6d77 6f6f 7264 272c 2027 4865 7268  aamwoord', 'Herh
-00000f40: 616c 696e 6727 2c20 2741 616e 7461 6c27  aling', 'Aantal'
-00000f50: 2c20 2727 2c20 274c 6578 6963 6161 6c20  , '', 'Lexicaal 
-00000f60: 7765 726b 776f 6f72 6427 2c20 2748 6572  werkwoord', 'Her
-00000f70: 6861 6c69 6e67 272c 0d0a 2020 2020 2020  haling',..      
-00000f80: 2020 2020 2020 2020 2020 2741 616e 7461            'Aanta
-00000f90: 6c27 5d0d 0a73 6865 6574 3263 6f6c 7769  l']..sheet2colwi
-00000fa0: 6474 6873 203d 205b 3130 2c20 3235 2c20  dths = [10, 25, 
-00000fb0: 3230 2c20 3130 2c20 352c 2032 352c 2032  20, 10, 5, 25, 2
-00000fc0: 302c 2031 305d 0d0a 7368 6565 7433 6865  0, 10]..sheet3he
-00000fd0: 6164 6572 203d 205b 2755 6974 696e 6773  ader = ['Uitings
-00000fe0: 6e75 6d6d 6572 272c 2027 4161 6e74 616c  nummer', 'Aantal
-00000ff0: 2077 6f6f 7264 656e 272c 2027 436f 7272   woorden', 'Corr
-00001000: 6563 7427 2c20 2247 6f65 6465 2050 5627  ect', "Goede PV'
-00001010: 7322 2c20 2246 6f75 7465 2065 6e20 6f6e  s", "Foute en on
-00001020: 7462 7265 6b65 6e64 6520 5056 2773 222c  tbrekende PV's",
-00001030: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001040: 2020 2241 616e 7461 6c20 6269 6a7a 696e    "Aantal bijzin
-00001050: 6e65 6e22 2c20 2242 696a 7a6f 6e64 6572  nen", "Bijzonder
-00001060: 6865 6465 6e22 5d0d 0a0d 0a0d 0a64 6566  heden"]......def
-00001070: 2077 7269 7465 7461 626c 6528 7461 6265   writetable(tabe
-00001080: 6c2c 2077 732c 2073 7461 7274 726f 773d  l, ws, startrow=
-00001090: 302c 2073 7461 7274 636f 6c3d 302c 2072  0, startcol=0, r
-000010a0: 6866 6f72 6d61 743d 4e6f 6e65 2c20 6368  hformat=None, ch
-000010b0: 666f 726d 6174 3d4e 6f6e 652c 2063 656c  format=None, cel
-000010c0: 6c66 6f72 6d61 743d 4e6f 6e65 293a 0d0a  lformat=None):..
-000010d0: 2020 2020 6375 7263 6f6c 203d 2073 7461      curcol = sta
-000010e0: 7274 636f 6c0d 0a20 2020 2063 7572 726f  rtcol..    curro
-000010f0: 7720 3d20 7374 6172 7472 6f77 0d0a 2020  w = startrow..  
-00001100: 2020 666f 7220 726f 7720 696e 2074 6162    for row in tab
-00001110: 656c 3a0d 0a20 2020 2020 2020 2066 6f72  el:..        for
-00001120: 2065 6c20 696e 2072 6f77 3a0d 0a20 2020   el in row:..   
-00001130: 2020 2020 2020 2020 2069 6620 6375 7272           if curr
-00001140: 6f77 203d 3d20 7374 6172 7472 6f77 3a0d  ow == startrow:.
-00001150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001160: 2074 6865 666f 726d 6174 203d 2072 6866   theformat = rhf
-00001170: 6f72 6d61 740d 0a20 2020 2020 2020 2020  ormat..         
-00001180: 2020 2065 6c69 6620 6375 7263 6f6c 203d     elif curcol =
-00001190: 3d20 7374 6172 7463 6f6c 3a0d 0a20 2020  = startcol:..   
-000011a0: 2020 2020 2020 2020 2020 2020 2074 6865               the
-000011b0: 666f 726d 6174 203d 2063 6866 6f72 6d61  format = chforma
-000011c0: 740d 0a20 2020 2020 2020 2020 2020 2065  t..            e
-000011d0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-000011e0: 2020 2020 2020 7468 6566 6f72 6d61 7420        theformat 
-000011f0: 3d20 6365 6c6c 666f 726d 6174 0d0a 2020  = cellformat..  
-00001200: 2020 2020 2020 2020 2020 7773 2e77 7269            ws.wri
-00001210: 7465 2863 7572 726f 772c 2063 7572 636f  te(currow, curco
-00001220: 6c2c 2065 6c2c 2074 6865 666f 726d 6174  l, el, theformat
-00001230: 290d 0a20 2020 2020 2020 2020 2020 2063  )..            c
-00001240: 7572 636f 6c20 2b3d 2031 0d0a 2020 2020  urcol += 1..    
-00001250: 2020 2020 6375 7272 6f77 202b 3d20 310d      currow += 1.
-00001260: 0a20 2020 2020 2020 2063 7572 636f 6c20  .        curcol 
-00001270: 3d20 7374 6172 7463 6f6c 0d0a 0d0a 0d0a  = startcol......
-00001280: 6465 6620 6d61 6b65 5f61 7374 6166 6f72  def make_astafor
-00001290: 6d28 7468 6566 6f72 6d2c 2061 7374 6164  m(theform, astad
-000012a0: 6174 612c 2074 6172 6765 7429 3a0d 0a20  ata, target):.. 
-000012b0: 2020 2077 6f72 6b62 6f6f 6b20 3d20 786c     workbook = xl
-000012c0: 7378 7772 6974 6572 2e57 6f72 6b62 6f6f  sxwriter.Workboo
-000012d0: 6b28 7461 7267 6574 2c20 7b22 7374 7269  k(target, {"stri
-000012e0: 6e67 735f 746f 5f6e 756d 6265 7273 223a  ngs_to_numbers":
-000012f0: 2054 7275 657d 290d 0a20 2020 2062 6f6c   True})..    bol
-00001300: 6420 3d20 776f 726b 626f 6f6b 2e61 6464  d = workbook.add
-00001310: 5f66 6f72 6d61 7428 7b27 626f 6c64 273a  _format({'bold':
-00001320: 2054 7275 657d 290d 0a20 2020 2064 6432   True})..    dd2
-00001330: 203d 2077 6f72 6b62 6f6f 6b2e 6164 645f   = workbook.add_
-00001340: 666f 726d 6174 287b 276e 756d 5f66 6f72  format({'num_for
-00001350: 6d61 7427 3a20 2730 2e30 3027 7d29 0d0a  mat': '0.00'})..
-00001360: 2020 2020 6f6b 666f 726d 6174 203d 2077      okformat = w
-00001370: 6f72 6b62 6f6f 6b2e 6164 645f 666f 726d  orkbook.add_form
-00001380: 6174 287b 2762 675f 636f 6c6f 7227 3a20  at({'bg_color': 
-00001390: 6772 6565 6e7d 290d 0a20 2020 2077 726f  green})..    wro
-000013a0: 6e67 666f 726d 6174 203d 2077 6f72 6b62  ngformat = workb
-000013b0: 6f6f 6b2e 6164 645f 666f 726d 6174 287b  ook.add_format({
-000013c0: 2762 675f 636f 6c6f 7227 3a20 7265 647d  'bg_color': red}
-000013d0: 290d 0a20 2020 2075 6e66 696c 6c65 6466  )..    unfilledf
-000013e0: 6f72 6d61 7420 3d20 776f 726b 626f 6f6b  ormat = workbook
-000013f0: 2e61 6464 5f66 6f72 6d61 7428 7b27 6267  .add_format({'bg
-00001400: 5f63 6f6c 6f72 273a 206f 7261 6e67 657d  _color': orange}
-00001410: 290d 0a20 2020 2062 6767 7265 7920 3d20  )..    bggrey = 
-00001420: 776f 726b 626f 6f6b 2e61 6464 5f66 6f72  workbook.add_for
-00001430: 6d61 7428 7b27 6267 5f63 6f6c 6f72 273a  mat({'bg_color':
-00001440: 2067 7265 797d 290d 0a0d 0a20 2020 2063   grey})....    c
-00001450: 6f6e 6466 6f72 6d61 7431 6120 3d20 7b27  ondformat1a = {'
-00001460: 7479 7065 273a 2027 6365 6c6c 272c 2027  type': 'cell', '
-00001470: 6372 6974 6572 6961 273a 2027 6265 7477  criteria': 'betw
-00001480: 6565 6e27 2c20 276d 696e 696d 756d 273a  een', 'minimum':
-00001490: 202d 322c 2027 6d61 7869 6d75 6d27 3a20   -2, 'maximum': 
-000014a0: 322c 2027 666f 726d 6174 273a 206f 6b66  2, 'format': okf
-000014b0: 6f72 6d61 747d 0d0a 2020 2020 636f 6e64  ormat}..    cond
-000014c0: 666f 726d 6174 3162 203d 207b 2774 7970  format1b = {'typ
-000014d0: 6527 3a20 2763 656c 6c27 2c20 2763 7269  e': 'cell', 'cri
-000014e0: 7465 7269 6127 3a20 276e 6f74 2062 6574  teria': 'not bet
-000014f0: 7765 656e 272c 2027 6d69 6e69 6d75 6d27  ween', 'minimum'
-00001500: 3a20 2d32 2c20 276d 6178 696d 756d 273a  : -2, 'maximum':
-00001510: 2032 2c20 2766 6f72 6d61 7427 3a20 7772   2, 'format': wr
-00001520: 6f6e 6766 6f72 6d61 747d 0d0a 2020 2020  ongformat}..    
-00001530: 636f 6e64 666f 726d 6174 3163 203d 207b  condformat1c = {
-00001540: 2774 7970 6527 3a20 2763 656c 6c27 2c20  'type': 'cell', 
-00001550: 2763 7269 7465 7269 6127 3a20 2765 7175  'criteria': 'equ
-00001560: 616c 2074 6f27 2c20 2776 616c 7565 273a  al to', 'value':
-00001570: 2027 224e 6965 7420 6765 7675 6c64 2227   '"Niet gevuld"'
-00001580: 2c20 2766 6f72 6d61 7427 3a20 756e 6669  , 'format': unfi
-00001590: 6c6c 6564 666f 726d 6174 7d0d 0a20 2020  lledformat}..   
-000015a0: 2063 6f6e 6466 6f72 6d61 7432 6120 3d20   condformat2a = 
-000015b0: 7b27 7479 7065 273a 2027 666f 726d 756c  {'type': 'formul
-000015c0: 6127 2c20 2763 7269 7465 7269 6127 3a20  a', 'criteria': 
-000015d0: 273d 2442 2438 3c3e 3027 2c20 2766 6f72  '=$B$8<>0', 'for
-000015e0: 6d61 7427 3a20 7772 6f6e 6766 6f72 6d61  mat': wrongforma
-000015f0: 747d 0d0a 2020 2020 636f 6e64 666f 726d  t}..    condform
-00001600: 6174 3262 203d 207b 2774 7970 6527 3a20  at2b = {'type': 
-00001610: 2766 6f72 6d75 6c61 272c 2027 6372 6974  'formula', 'crit
-00001620: 6572 6961 273a 2027 3d24 4224 383d 3027  eria': '=$B$8=0'
-00001630: 2c20 2766 6f72 6d61 7427 3a20 6f6b 666f  , 'format': okfo
-00001640: 726d 6174 7d0d 0a20 2020 2063 6f6e 6466  rmat}..    condf
-00001650: 6f72 6d61 7432 6320 3d20 7b27 7479 7065  ormat2c = {'type
-00001660: 273a 2027 6365 6c6c 272c 2027 6372 6974  ': 'cell', 'crit
-00001670: 6572 6961 273a 2027 6571 7561 6c20 746f  eria': 'equal to
-00001680: 272c 2027 7661 6c75 6527 3a20 2722 4e69  ', 'value': '"Ni
-00001690: 6574 2067 6576 756c 6422 272c 2027 666f  et gevuld"', 'fo
-000016a0: 726d 6174 273a 2075 6e66 696c 6c65 6466  rmat': unfilledf
-000016b0: 6f72 6d61 747d 0d0a 0d0a 2020 2020 776f  ormat}....    wo
-000016c0: 726b 7368 6565 7431 203d 2077 6f72 6b62  rksheet1 = workb
-000016d0: 6f6f 6b2e 6164 645f 776f 726b 7368 6565  ook.add_workshee
-000016e0: 7428 2755 6974 6b6f 6d73 7465 6e74 6162  t('Uitkomstentab
-000016f0: 656c 2729 0d0a 2020 2020 776f 726b 7368  el')..    worksh
-00001700: 6565 7432 203d 2077 6f72 6b62 6f6f 6b2e  eet2 = workbook.
-00001710: 6164 645f 776f 726b 7368 6565 7428 275a  add_worksheet('Z
-00001720: 4e57 2026 2057 5727 290d 0a20 2020 2077  NW & WW')..    w
-00001730: 6f72 6b73 6865 6574 3320 3d20 776f 726b  orksheet3 = work
-00001740: 626f 6f6b 2e61 6464 5f77 6f72 6b73 6865  book.add_workshe
-00001750: 6574 2827 5569 7469 6e67 656e 2729 0d0a  et('Uitingen')..
-00001760: 2020 2020 776f 726b 7368 6565 7434 203d      worksheet4 =
-00001770: 2077 6f72 6b62 6f6f 6b2e 6164 645f 776f   workbook.add_wo
-00001780: 726b 7368 6565 7428 2754 6162 656c 2729  rksheet('Tabel')
-00001790: 0d0a 0d0a 2020 2020 2320 776f 726b 7368  ....    # worksh
-000017a0: 6565 7431 0d0a 2020 2020 776f 726b 7368  eet1..    worksh
-000017b0: 6565 7431 2e73 6574 5f63 6f6c 756d 6e28  eet1.set_column(
-000017c0: 302c 2030 2c20 3330 290d 0a20 2020 2077  0, 0, 30)..    w
-000017d0: 6f72 6b73 6865 6574 312e 7365 745f 636f  orksheet1.set_co
-000017e0: 6c75 6d6e 2831 2c20 322c 2031 3229 0d0a  lumn(1, 2, 12)..
-000017f0: 2020 2020 776f 726b 7368 6565 7431 2e68      worksheet1.h
-00001800: 6964 655f 6772 6964 6c69 6e65 7328 6f70  ide_gridlines(op
-00001810: 7469 6f6e 3d32 290d 0a20 2020 2077 6f72  tion=2)..    wor
-00001820: 6b73 6865 6574 312e 636f 6e64 6974 696f  ksheet1.conditio
-00001830: 6e61 6c5f 666f 726d 6174 2827 2443 2432  nal_format('$C$2
-00001840: 3a24 4324 3727 2c20 636f 6e64 666f 726d  :$C$7', condform
-00001850: 6174 3161 290d 0a20 2020 2077 6f72 6b73  at1a)..    works
-00001860: 6865 6574 312e 636f 6e64 6974 696f 6e61  heet1.conditiona
-00001870: 6c5f 666f 726d 6174 2827 2443 2432 3a24  l_format('$C$2:$
-00001880: 4324 3727 2c20 636f 6e64 666f 726d 6174  C$7', condformat
-00001890: 3162 290d 0a20 2020 2077 6f72 6b73 6865  1b)..    workshe
-000018a0: 6574 312e 636f 6e64 6974 696f 6e61 6c5f  et1.conditional_
-000018b0: 666f 726d 6174 2827 2443 2432 3a24 4324  format('$C$2:$C$
-000018c0: 3727 2c20 636f 6e64 666f 726d 6174 3163  7', condformat1c
-000018d0: 290d 0a20 2020 2077 6f72 6b73 6865 6574  )..    worksheet
-000018e0: 312e 636f 6e64 6974 696f 6e61 6c5f 666f  1.conditional_fo
-000018f0: 726d 6174 2827 2443 2439 272c 2063 6f6e  rmat('$C$9', con
-00001900: 6466 6f72 6d61 7431 6129 0d0a 2020 2020  dformat1a)..    
-00001910: 776f 726b 7368 6565 7431 2e63 6f6e 6469  worksheet1.condi
-00001920: 7469 6f6e 616c 5f66 6f72 6d61 7428 2724  tional_format('$
-00001930: 4324 3927 2c20 636f 6e64 666f 726d 6174  C$9', condformat
-00001940: 3162 290d 0a20 2020 2077 6f72 6b73 6865  1b)..    workshe
-00001950: 6574 312e 636f 6e64 6974 696f 6e61 6c5f  et1.conditional_
-00001960: 666f 726d 6174 2827 2443 2439 272c 2063  format('$C$9', c
-00001970: 6f6e 6466 6f72 6d61 7431 6329 0d0a 2020  ondformat1c)..  
-00001980: 2020 776f 726b 7368 6565 7431 2e63 6f6e    worksheet1.con
-00001990: 6469 7469 6f6e 616c 5f66 6f72 6d61 7428  ditional_format(
-000019a0: 2724 4324 3130 3a24 4324 3133 272c 2063  '$C$10:$C$13', c
-000019b0: 6f6e 6466 6f72 6d61 7431 6129 0d0a 2020  ondformat1a)..  
-000019c0: 2020 776f 726b 7368 6565 7431 2e63 6f6e    worksheet1.con
-000019d0: 6469 7469 6f6e 616c 5f66 6f72 6d61 7428  ditional_format(
-000019e0: 2724 4324 3130 3a24 4324 3133 272c 2063  '$C$10:$C$13', c
-000019f0: 6f6e 6466 6f72 6d61 7431 6229 0d0a 2020  ondformat1b)..  
-00001a00: 2020 776f 726b 7368 6565 7431 2e63 6f6e    worksheet1.con
-00001a10: 6469 7469 6f6e 616c 5f66 6f72 6d61 7428  ditional_format(
-00001a20: 2724 4324 3130 3a24 4324 3133 272c 2063  '$C$10:$C$13', c
-00001a30: 6f6e 6466 6f72 6d61 7431 6329 0d0a 2020  ondformat1c)..  
-00001a40: 2020 776f 726b 7368 6565 7431 2e63 6f6e    worksheet1.con
-00001a50: 6469 7469 6f6e 616c 5f66 6f72 6d61 7428  ditional_format(
-00001a60: 2724 4324 3827 2c20 636f 6e64 666f 726d  '$C$8', condform
-00001a70: 6174 3261 290d 0a20 2020 2077 6f72 6b73  at2a)..    works
-00001a80: 6865 6574 312e 636f 6e64 6974 696f 6e61  heet1.conditiona
-00001a90: 6c5f 666f 726d 6174 2827 2443 2438 272c  l_format('$C$8',
-00001aa0: 2063 6f6e 6466 6f72 6d61 7432 6229 0d0a   condformat2b)..
-00001ab0: 2020 2020 776f 726b 7368 6565 7431 2e63      worksheet1.c
-00001ac0: 6f6e 6469 7469 6f6e 616c 5f66 6f72 6d61  onditional_forma
-00001ad0: 7428 2724 4324 3827 2c20 636f 6e64 666f  t('$C$8', condfo
-00001ae0: 726d 6174 3263 290d 0a0d 0a20 2020 2077  rmat2c)....    w
-00001af0: 7269 7465 7461 626c 6528 7468 6566 6f72  ritetable(thefor
-00001b00: 6d2e 7363 6f72 6573 2c20 776f 726b 7368  m.scores, worksh
-00001b10: 6565 7431 2c20 7268 666f 726d 6174 3d62  eet1, rhformat=b
-00001b20: 6f6c 642c 2063 6866 6f72 6d61 743d 626f  old, chformat=bo
-00001b30: 6c64 2c20 6365 6c6c 666f 726d 6174 3d64  ld, cellformat=d
-00001b40: 6432 290d 0a20 2020 2077 6f72 6b73 6865  d2)..    workshe
-00001b50: 6574 312e 7772 6974 6528 2724 4224 3627  et1.write('$B$6'
-00001b60: 2c20 2727 2c20 6267 6772 6579 290d 0a20  , '', bggrey).. 
-00001b70: 2020 2077 6f72 6b73 6865 6574 312e 7772     worksheet1.wr
-00001b80: 6974 6528 2724 4224 3727 2c20 2727 2c20  ite('$B$7', '', 
-00001b90: 6267 6772 6579 290d 0a20 2020 2077 6f72  bggrey)..    wor
-00001ba0: 6b73 6865 6574 312e 7772 6974 6528 2724  ksheet1.write('$
-00001bb0: 4224 3827 2c20 2727 2c20 6267 6772 6579  B$8', '', bggrey
-00001bc0: 290d 0a20 2020 2077 6f72 6b73 6865 6574  )..    worksheet
-00001bd0: 312e 7772 6974 6528 2724 4224 3927 2c20  1.write('$B$9', 
-00001be0: 2727 2c20 6267 6772 6579 290d 0a0d 0a20  '', bggrey).... 
-00001bf0: 2020 2066 6f72 2028 6c6f 632c 2063 6f75     for (loc, cou
-00001c00: 6e74 2920 696e 2061 7374 6164 6174 612e  nt) in astadata.
-00001c10: 7661 7264 6963 742e 6974 656d 7328 293a  vardict.items():
-00001c20: 0d0a 2020 2020 2020 2020 776f 726b 7368  ..        worksh
-00001c30: 6565 7431 2e77 7269 7465 286c 6f63 2c20  eet1.write(loc, 
-00001c40: 636f 756e 7429 0d0a 0d0a 2020 2020 2320  count)....    # 
-00001c50: 776f 726b 7368 6565 7432 0d0a 2020 2020  worksheet2..    
-00001c60: 7772 6974 6574 6162 6c65 2873 6865 6574  writetable(sheet
-00001c70: 3268 6964 6465 6e72 6f77 732c 2077 6f72  2hiddenrows, wor
-00001c80: 6b73 6865 6574 3229 0d0a 0d0a 2020 2020  ksheet2)....    
-00001c90: 636f 6c63 7472 203d 2030 0d0a 2020 2020  colctr = 0..    
-00001ca0: 666f 7220 2865 6c2c 2077 2920 696e 207a  for (el, w) in z
-00001cb0: 6970 2873 6865 6574 3268 6561 6465 722c  ip(sheet2header,
-00001cc0: 2073 6865 6574 3263 6f6c 7769 6474 6873   sheet2colwidths
-00001cd0: 293a 0d0a 2020 2020 2020 2020 776f 726b  ):..        work
-00001ce0: 7368 6565 7432 2e77 7269 7465 2834 2c20  sheet2.write(4, 
-00001cf0: 636f 6c63 7472 2c20 656c 2c20 626f 6c64  colctr, el, bold
-00001d00: 290d 0a20 2020 2020 2020 2077 6f72 6b73  )..        works
-00001d10: 6865 6574 322e 7365 745f 636f 6c75 6d6e  heet2.set_column
-00001d20: 2863 6f6c 6374 722c 2063 6f6c 6374 722c  (colctr, colctr,
-00001d30: 2077 290d 0a20 2020 2020 2020 2063 6f6c   w)..        col
-00001d40: 6374 7220 2b3d 2031 0d0a 0d0a 2020 2020  ctr += 1....    
-00001d50: 726f 7763 7472 203d 2035 0d0a 2020 2020  rowctr = 5..    
-00001d60: 666f 7220 6920 696e 2072 616e 6765 2831  for i in range(1
-00001d70: 3030 293a 0d0a 2020 2020 2020 2020 776f  00):..        wo
-00001d80: 726b 7368 6565 7432 2e77 7269 7465 2872  rksheet2.write(r
-00001d90: 6f77 6374 722c 2030 2c20 6920 2b20 3129  owctr, 0, i + 1)
-00001da0: 0d0a 2020 2020 2020 2020 726f 7763 7472  ..        rowctr
-00001db0: 202b 3d20 310d 0a0d 0a20 2020 2072 6f77   += 1....    row
-00001dc0: 6374 7220 3d20 350d 0a20 2020 2077 636f  ctr = 5..    wco
-00001dd0: 6c20 3d20 310d 0a20 2020 2066 7265 7163  l = 1..    freqc
-00001de0: 6f6c 203d 2033 0d0a 2020 2020 666f 7220  ol = 3..    for 
-00001df0: 2877 2c20 636e 7429 2069 6e20 6173 7461  (w, cnt) in asta
-00001e00: 6461 7461 2e6e 6f75 6e64 6963 742e 6974  data.noundict.it
-00001e10: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-00001e20: 776f 726b 7368 6565 7432 2e77 7269 7465  worksheet2.write
-00001e30: 2872 6f77 6374 722c 2077 636f 6c2c 2077  (rowctr, wcol, w
-00001e40: 290d 0a20 2020 2020 2020 2077 6f72 6b73  )..        works
-00001e50: 6865 6574 322e 7772 6974 6528 726f 7763  heet2.write(rowc
-00001e60: 7472 2c20 6672 6571 636f 6c2c 2063 6e74  tr, freqcol, cnt
-00001e70: 290d 0a20 2020 2020 2020 2072 6f77 6374  )..        rowct
-00001e80: 7220 2b3d 2031 0d0a 0d0a 2020 2020 726f  r += 1....    ro
-00001e90: 7763 7472 203d 2035 0d0a 2020 2020 7763  wctr = 5..    wc
-00001ea0: 6f6c 203d 2035 0d0a 2020 2020 6672 6571  ol = 5..    freq
-00001eb0: 636f 6c20 3d20 370d 0a20 2020 2066 6f72  col = 7..    for
-00001ec0: 2028 772c 2063 6e74 2920 696e 2061 7374   (w, cnt) in ast
-00001ed0: 6164 6174 612e 7665 7262 6469 6374 2e69  adata.verbdict.i
-00001ee0: 7465 6d73 2829 3a0d 0a20 2020 2020 2020  tems():..       
-00001ef0: 2077 6f72 6b73 6865 6574 322e 7772 6974   worksheet2.writ
-00001f00: 6528 726f 7763 7472 2c20 7763 6f6c 2c20  e(rowctr, wcol, 
-00001f10: 7729 0d0a 2020 2020 2020 2020 776f 726b  w)..        work
-00001f20: 7368 6565 7432 2e77 7269 7465 2872 6f77  sheet2.write(row
-00001f30: 6374 722c 2066 7265 7163 6f6c 2c20 636e  ctr, freqcol, cn
-00001f40: 7429 0d0a 2020 2020 2020 2020 726f 7763  t)..        rowc
-00001f50: 7472 202b 3d20 310d 0a0d 0a20 2020 2066  tr += 1....    f
-00001f60: 6f72 2072 6f77 6374 7220 696e 2072 616e  or rowctr in ran
-00001f70: 6765 2834 293a 0d0a 2020 2020 2020 2020  ge(4):..        
-00001f80: 776f 726b 7368 6565 7432 2e73 6574 5f72  worksheet2.set_r
-00001f90: 6f77 2872 6f77 6374 722c 204e 6f6e 652c  ow(rowctr, None,
-00001fa0: 204e 6f6e 652c 207b 2768 6964 6465 6e27   None, {'hidden'
-00001fb0: 3a20 5472 7565 7d29 0d0a 0d0a 2020 2020  : True})....    
-00001fc0: 2320 776f 726b 6173 6865 6574 330d 0a20  # workasheet3.. 
-00001fd0: 2020 2077 7269 7465 7461 626c 6528 7368     writetable(sh
-00001fe0: 6565 7433 6869 6464 656e 726f 7773 2c20  eet3hiddenrows, 
-00001ff0: 776f 726b 7368 6565 7433 290d 0a0d 0a20  worksheet3).... 
-00002000: 2020 2063 6f6c 6374 7220 3d20 300d 0a20     colctr = 0.. 
-00002010: 2020 2066 6f72 2065 6c20 696e 2073 6865     for el in she
-00002020: 6574 3368 6561 6465 723a 0d0a 2020 2020  et3header:..    
-00002030: 2020 2020 776f 726b 7368 6565 7433 2e77      worksheet3.w
-00002040: 7269 7465 2834 2c20 636f 6c63 7472 2c20  rite(4, colctr, 
-00002050: 656c 2c20 626f 6c64 290d 0a20 2020 2020  el, bold)..     
-00002060: 2020 2063 6f6c 6374 7220 2b3d 2031 0d0a     colctr += 1..
-00002070: 2020 2020 776f 726b 7368 6565 7433 2e73      worksheet3.s
-00002080: 6574 5f63 6f6c 756d 6e28 302c 2063 6f6c  et_column(0, col
-00002090: 6374 722c 2032 3029 0d0a 0d0a 2020 2020  ctr, 20)....    
-000020a0: 726f 7763 7472 203d 2035 0d0a 2020 2020  rowctr = 5..    
-000020b0: 7772 6974 6574 6162 6c65 2861 7374 6164  writetable(astad
-000020c0: 6174 612e 7574 746c 6973 742c 2077 6f72  ata.uttlist, wor
-000020d0: 6b73 6865 6574 332c 2073 7461 7274 726f  ksheet3, startro
-000020e0: 773d 726f 7763 7472 290d 0a0d 0a20 2020  w=rowctr)....   
-000020f0: 2066 6f72 2072 6f77 6374 7220 696e 2072   for rowctr in r
-00002100: 616e 6765 2834 293a 0d0a 2020 2020 2020  ange(4):..      
-00002110: 2020 776f 726b 7368 6565 7433 2e73 6574    worksheet3.set
-00002120: 5f72 6f77 2872 6f77 6374 722c 204e 6f6e  _row(rowctr, Non
-00002130: 652c 204e 6f6e 652c 207b 2768 6964 6465  e, None, {'hidde
-00002140: 6e27 3a20 5472 7565 7d29 0d0a 0d0a 2020  n': True})....  
-00002150: 2020 2320 776f 726b 7368 6565 7434 0d0a    # worksheet4..
-00002160: 2020 2020 776f 726b 7368 6565 7434 2e73      worksheet4.s
-00002170: 6574 5f63 6f6c 756d 6e28 302c 2030 2c20  et_column(0, 0, 
-00002180: 3330 290d 0a0d 0a20 2020 2077 7269 7465  30)....    write
-00002190: 7461 626c 6528 7468 6566 6f72 6d2e 7461  table(theform.ta
-000021a0: 6265 6c2c 2077 6f72 6b73 6865 6574 342c  bel, worksheet4,
-000021b0: 2073 7461 7274 726f 773d 312c 2072 6866   startrow=1, rhf
-000021c0: 6f72 6d61 743d 626f 6c64 290d 0a0d 0a20  ormat=bold).... 
-000021d0: 2020 2072 6574 7572 6e20 776f 726b 626f     return workbo
-000021e0: 6f6b 2c20 7461 7267 6574 0d0a 0d0a 0d0a  ok, target......
-000021f0: 6465 6620 7375 6d63 7472 2863 7472 293a  def sumctr(ctr):
-00002200: 0d0a 2020 2020 7265 7375 6c74 203d 2073  ..    result = s
-00002210: 756d 2863 7472 2e76 616c 7565 7328 2929  um(ctr.values())
-00002220: 0d0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
-00002230: 756c 740d 0a0d 0a0d 0a64 6566 2067 6574  ult......def get
-00002240: 7661 7264 6963 7428 616c 6c72 6573 756c  vardict(allresul
-00002250: 7473 293a 0d0a 2020 2020 7365 6d70 6172  ts):..    sempar
-00002260: 203d 2027 4236 270d 0a20 2020 2070 686f   = 'B6'..    pho
-00002270: 6e70 6172 203d 2027 4237 270d 0a20 2020  npar = 'B7'..   
-00002280: 206e 656f 203d 2027 4238 270d 0a20 2020   neo = 'B8'..   
-00002290: 204b 4d20 3d20 2742 3927 0d0a 2020 2020   KM = 'B9'..    
-000022a0: 7365 6d70 6172 636f 756e 7420 3d20 7375  semparcount = su
-000022b0: 6d63 7472 2861 6c6c 7265 7375 6c74 732e  mctr(allresults.
-000022c0: 636f 7265 7265 7375 6c74 735b 2741 3032  coreresults['A02
-000022d0: 3627 5d29 2069 6620 2741 3032 3627 2069  6']) if 'A026' i
-000022e0: 6e20 616c 6c72 6573 756c 7473 2e63 6f72  n allresults.cor
-000022f0: 6572 6573 756c 7473 2065 6c73 6520 300d  eresults else 0.
-00002300: 0a20 2020 2070 686f 6e70 6172 636f 756e  .    phonparcoun
-00002310: 7420 3d20 7375 6d63 7472 2861 6c6c 7265  t = sumctr(allre
-00002320: 7375 6c74 732e 636f 7265 7265 7375 6c74  sults.coreresult
-00002330: 735b 2741 3030 3827 5d29 2069 6620 2741  s['A008']) if 'A
-00002340: 3030 3827 2069 6e20 616c 6c72 6573 756c  008' in allresul
-00002350: 7473 2e63 6f72 6572 6573 756c 7473 2065  ts.coreresults e
-00002360: 6c73 6520 300d 0a20 2020 206e 656f 636f  lse 0..    neoco
-00002370: 756e 7420 3d20 7375 6d63 7472 2861 6c6c  unt = sumctr(all
-00002380: 7265 7375 6c74 732e 636f 7265 7265 7375  results.coreresu
-00002390: 6c74 735b 2741 3032 3227 5d29 2069 6620  lts['A022']) if 
-000023a0: 2741 3032 3227 2069 6e20 616c 6c72 6573  'A022' in allres
-000023b0: 756c 7473 2e63 6f72 6572 6573 756c 7473  ults.coreresults
-000023c0: 2065 6c73 6520 300d 0a20 2020 204b 636f   else 0..    Kco
-000023d0: 756e 7420 3d20 7375 6d63 7472 2861 6c6c  unt = sumctr(all
-000023e0: 7265 7375 6c74 732e 636f 7265 7265 7375  results.coreresu
-000023f0: 6c74 735b 2741 3031 3327 5d29 2069 6620  lts['A013']) if 
-00002400: 2741 3031 3327 2069 6e20 616c 6c72 6573  'A013' in allres
-00002410: 756c 7473 2e63 6f72 6572 6573 756c 7473  ults.coreresults
-00002420: 2065 6c73 6520 300d 0a20 2020 204d 636f   else 0..    Mco
-00002430: 756e 7420 3d20 7375 6d63 7472 2861 6c6c  unt = sumctr(all
-00002440: 7265 7375 6c74 732e 636f 7265 7265 7375  results.coreresu
-00002450: 6c74 735b 2741 3032 3027 5d29 2069 6620  lts['A020']) if 
-00002460: 2741 3032 3027 2069 6e20 616c 6c72 6573  'A020' in allres
-00002470: 756c 7473 2e63 6f72 6572 6573 756c 7473  ults.coreresults
-00002480: 2065 6c73 6520 300d 0a20 2020 204b 4d63   else 0..    KMc
-00002490: 6f75 6e74 203d 204b 636f 756e 7420 2b20  ount = Kcount + 
-000024a0: 4d63 6f75 6e74 0d0a 2020 2020 7265 7375  Mcount..    resu
-000024b0: 6c74 203d 207b 7365 6d70 6172 3a20 7365  lt = {sempar: se
-000024c0: 6d70 6172 636f 756e 742c 2070 686f 6e70  mparcount, phonp
-000024d0: 6172 3a20 7068 6f6e 7061 7263 6f75 6e74  ar: phonparcount
-000024e0: 2c20 6e65 6f3a 206e 656f 636f 756e 742c  , neo: neocount,
-000024f0: 204b 4d3a 204b 4d63 6f75 6e74 7d0d 0a20   KM: KMcount}.. 
-00002500: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00002510: 0d0a 0d0a 0d0a 6465 6620 7570 6461 7465  ......def update
-00002520: 2872 6573 756c 7464 6963 742c 2063 7472  (resultdict, ctr
-00002530: 6469 6374 2c20 6b65 792c 2070 726f 7029  dict, key, prop)
-00002540: 3a0d 0a20 2020 2069 6620 6b65 7920 696e  :..    if key in
-00002550: 2063 7472 6469 6374 3a0d 0a20 2020 2020   ctrdict:..     
-00002560: 2020 2063 7472 203d 2063 7472 6469 6374     ctr = ctrdict
-00002570: 5b6b 6579 5d0d 0a20 2020 2020 2020 2066  [key]..        f
-00002580: 6f72 2075 7474 6964 2069 6e20 6374 723a  or uttid in ctr:
-00002590: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000025a0: 7375 6c74 6469 6374 5b75 7474 6964 5d5b  sultdict[uttid][
-000025b0: 7072 6f70 5d20 3d20 6374 725b 7574 7469  prop] = ctr[utti
-000025c0: 645d 0d0a 0d0a 0d0a 6465 6620 7570 6461  d]......def upda
-000025d0: 7465 7769 7468 6374 7228 7265 7375 6c74  tewithctr(result
-000025e0: 6469 6374 2c20 6374 722c 2070 726f 7029  dict, ctr, prop)
-000025f0: 3a0d 0a20 2020 2066 6f72 2075 7474 6964  :..    for uttid
-00002600: 2069 6e20 6374 723a 0d0a 2020 2020 2020   in ctr:..      
-00002610: 2020 7265 7375 6c74 6469 6374 5b75 7474    resultdict[utt
-00002620: 6964 5d5b 7072 6f70 5d20 3d20 6374 725b  id][prop] = ctr[
-00002630: 7574 7469 645d 0d0a 0d0a 0d0a 6465 6620  uttid]......def 
-00002640: 696e 7464 6963 7467 6574 2864 6374 2c20  intdictget(dct, 
-00002650: 6b65 796e 616d 6529 3a0d 0a20 2020 2072  keyname):..    r
-00002660: 3120 3d20 6469 6374 6765 7428 6463 742c  1 = dictget(dct,
-00002670: 206b 6579 6e61 6d65 290d 0a20 2020 2069   keyname)..    i
-00002680: 6620 7231 203d 3d20 2727 3a0d 0a20 2020  f r1 == '':..   
-00002690: 2020 2020 2072 6573 756c 7420 3d20 300d       result = 0.
-000026a0: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
-000026b0: 2020 2020 7265 7375 6c74 203d 2069 6e74      result = int
-000026c0: 2872 3129 0d0a 2020 2020 7265 7475 726e  (r1)..    return
-000026d0: 2072 6573 756c 740d 0a0d 0a0d 0a64 6566   result......def
-000026e0: 2064 6963 7467 6574 2864 6374 2c20 6b65   dictget(dct, ke
-000026f0: 796e 616d 6529 3a0d 0a20 2020 2069 6620  yname):..    if 
-00002700: 6b65 796e 616d 6520 696e 2064 6374 3a0d  keyname in dct:.
-00002710: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-00002720: 3d20 6463 745b 6b65 796e 616d 655d 0d0a  = dct[keyname]..
-00002730: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00002740: 2020 2072 6573 756c 7420 3d20 2727 0d0a     result = ''..
-00002750: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00002760: 740d 0a0d 0a0d 0a64 6566 2072 6573 756c  t......def resul
-00002770: 7464 6963 7432 7461 626c 6528 7265 7375  tdict2table(resu
-00002780: 6c74 6469 6374 293a 0d0a 2020 2020 7461  ltdict):..    ta
-00002790: 626c 6520 3d20 5b5d 0d0a 2020 2020 666f  ble = []..    fo
-000027a0: 7220 7574 7469 6420 696e 2072 6573 756c  r uttid in resul
-000027b0: 7464 6963 743a 0d0a 2020 2020 2020 2020  tdict:..        
-000027c0: 7574 7469 645f 6469 6374 203d 2072 6573  uttid_dict = res
-000027d0: 756c 7464 6963 745b 7574 7469 645d 0d0a  ultdict[uttid]..
-000027e0: 2020 2020 2020 2020 7763 203d 2064 6963          wc = dic
-000027f0: 7467 6574 2875 7474 6964 5f64 6963 742c  tget(uttid_dict,
-00002800: 2027 7763 2729 0d0a 2020 2020 2020 2020   'wc')..        
-00002810: 636f 7272 6563 7420 3d20 6469 6374 6765  correct = dictge
-00002820: 7428 7574 7469 645f 6469 6374 2c20 2763  t(uttid_dict, 'c
-00002830: 6f72 7265 6374 2729 0d0a 2020 2020 2020  orrect')..      
-00002840: 2020 6966 2063 6f72 7265 6374 2021 3d20    if correct != 
-00002850: 2727 3a0d 0a20 2020 2020 2020 2020 2020  '':..           
-00002860: 2063 6f72 7265 6374 203d 2027 4a27 0d0a   correct = 'J'..
-00002870: 2020 2020 2020 2020 616c 6c70 7673 203d          allpvs =
-00002880: 2069 6e74 6469 6374 6765 7428 7574 7469   intdictget(utti
-00002890: 645f 6469 6374 2c20 2761 6c6c 7076 7327  d_dict, 'allpvs'
-000028a0: 290d 0a20 2020 2020 2020 2066 6f75 7465  )..        foute
-000028b0: 7076 7320 3d20 696e 7464 6963 7467 6574  pvs = intdictget
-000028c0: 2875 7474 6964 5f64 6963 742c 2027 666f  (uttid_dict, 'fo
-000028d0: 7574 6570 7673 2729 0d0a 2020 2020 2020  utepvs')..      
-000028e0: 2020 6f6b 7076 7320 3d20 6d61 7828 302c    okpvs = max(0,
-000028f0: 2061 6c6c 7076 7320 2d20 666f 7574 6570   allpvs - foutep
-00002900: 7673 290d 0a20 2020 2020 2020 2062 696a  vs)..        bij
-00002910: 7a69 6e63 6f75 6e74 203d 2064 6963 7467  zincount = dictg
-00002920: 6574 2875 7474 6964 5f64 6963 742c 2027  et(uttid_dict, '
-00002930: 6269 6a7a 696e 636f 756e 7427 290d 0a20  bijzincount').. 
-00002940: 2020 2020 2020 2072 656d 6172 6b73 203d         remarks =
-00002950: 2064 6963 7467 6574 2875 7474 6964 5f64   dictget(uttid_d
-00002960: 6963 742c 2027 7265 6d61 726b 7327 290d  ict, 'remarks').
-00002970: 0a20 2020 2020 2020 2070 6164 6465 6475  .        paddedu
-00002980: 7474 6964 203d 2073 7472 2875 7474 6964  ttid = str(uttid
-00002990: 292e 726a 7573 7428 332c 2027 3027 290d  ).rjust(3, '0').
-000029a0: 0a20 2020 2020 2020 206e 6577 726f 7720  .        newrow 
-000029b0: 3d20 5b70 6164 6465 6475 7474 6964 2c20  = [paddeduttid, 
-000029c0: 7763 2c20 636f 7272 6563 742c 206f 6b70  wc, correct, okp
-000029d0: 7673 2c20 666f 7574 6570 7673 2c20 6269  vs, foutepvs, bi
-000029e0: 6a7a 696e 636f 756e 742c 2072 656d 6172  jzincount, remar
-000029f0: 6b73 5d0d 0a20 2020 2020 2020 2074 6162  ks]..        tab
-00002a00: 6c65 2e61 7070 656e 6428 6e65 7772 6f77  le.append(newrow
-00002a10: 290d 0a20 2020 2073 6f72 7465 6474 6162  )..    sortedtab
-00002a20: 6c65 203d 2073 6f72 7465 6428 7461 626c  le = sorted(tabl
-00002a30: 652c 206b 6579 3d6c 616d 6264 6120 726f  e, key=lambda ro
-00002a40: 773a 2072 6f77 5b30 5d29 0d0a 2020 2020  w: row[0])..    
-00002a50: 7265 7475 726e 2073 6f72 7465 6474 6162  return sortedtab
-00002a60: 6c65 0d0a 0d0a 0d0a 6465 6620 6765 7475  le......def getu
-00002a70: 7474 6c69 7374 2861 6c6c 7265 7375 6c74  ttlist(allresult
-00002a80: 7329 3a0d 0a20 2020 2072 6573 756c 7464  s):..    resultd
-00002a90: 6963 7420 3d20 6465 6661 756c 7464 6963  ict = defaultdic
-00002aa0: 7428 6c61 6d62 6461 3a20 6465 6661 756c  t(lambda: defaul
-00002ab0: 7464 6963 7428 696e 7429 290d 0a20 2020  tdict(int))..   
-00002ac0: 2077 6f72 6463 6f75 6e74 6469 6374 203d   wordcountdict =
-00002ad0: 2077 6f72 6463 6f75 6e74 7065 7275 7474   wordcountperutt
-00002ae0: 2861 6c6c 7265 7375 6c74 7329 0d0a 2020  (allresults)..  
-00002af0: 2020 666f 7220 7574 7469 6420 696e 2077    for uttid in w
-00002b00: 6f72 6463 6f75 6e74 6469 6374 3a0d 0a20  ordcountdict:.. 
-00002b10: 2020 2020 2020 2072 6573 756c 7464 6963         resultdic
-00002b20: 745b 7574 7469 645d 5b27 7763 275d 203d  t[uttid]['wc'] =
-00002b30: 2077 6f72 6463 6f75 6e74 6469 6374 5b75   wordcountdict[u
-00002b40: 7474 6964 5d0d 0a20 2020 2023 2075 7064  ttid]..    # upd
-00002b50: 6174 6528 7265 7375 6c74 6469 6374 2c20  ate(resultdict, 
-00002b60: 616c 6c72 6573 756c 7473 2e70 6f73 7472  allresults.postr
-00002b70: 6573 756c 7473 2c20 2741 3034 3627 2c20  esults, 'A046', 
-00002b80: 2777 6327 290d 0a20 2020 2075 7064 6174  'wc')..    updat
-00002b90: 6528 7265 7375 6c74 6469 6374 2c20 616c  e(resultdict, al
-00002ba0: 6c72 6573 756c 7473 2e63 6f72 6572 6573  lresults.coreres
-00002bb0: 756c 7473 2c20 2741 3030 3427 2c20 2763  ults, 'A004', 'c
-00002bc0: 6f72 7265 6374 2729 0d0a 2020 2020 7570  orrect')..    up
-00002bd0: 6461 7465 2872 6573 756c 7464 6963 742c  date(resultdict,
-00002be0: 2061 6c6c 7265 7375 6c74 732e 636f 7265   allresults.core
-00002bf0: 7265 7375 6c74 732c 2027 4130 3234 272c  results, 'A024',
-00002c00: 2027 616c 6c70 7673 2729 0d0a 2020 2020   'allpvs')..    
-00002c10: 7375 6270 7673 203d 2061 6c6c 7265 7375  subpvs = allresu
-00002c20: 6c74 732e 636f 7265 7265 7375 6c74 735b  lts.coreresults[
-00002c30: 2741 3033 3227 5d20 6966 2027 4130 3332  'A032'] if 'A032
-00002c40: 2720 696e 2061 6c6c 7265 7375 6c74 732e  ' in allresults.
-00002c50: 636f 7265 7265 7375 6c74 7320 656c 7365  coreresults else
-00002c60: 2043 6f75 6e74 6572 2829 0d0a 2020 2020   Counter()..    
-00002c70: 6465 6c70 7673 203d 2061 6c6c 7265 7375  delpvs = allresu
-00002c80: 6c74 732e 636f 7265 7265 7375 6c74 735b  lts.coreresults[
-00002c90: 2741 3030 3927 5d20 6966 2027 4130 3039  'A009'] if 'A009
-00002ca0: 2720 696e 2061 6c6c 7265 7375 6c74 732e  ' in allresults.
-00002cb0: 636f 7265 7265 7375 6c74 7320 656c 7365  coreresults else
-00002cc0: 2043 6f75 6e74 6572 2829 0d0a 2020 2020   Counter()..    
-00002cd0: 7469 6a64 666f 7574 7076 7320 3d20 616c  tijdfoutpvs = al
-00002ce0: 6c72 6573 756c 7473 2e63 6f72 6572 6573  lresults.coreres
-00002cf0: 756c 7473 5b27 4130 3431 275d 2069 6620  ults['A041'] if 
-00002d00: 2741 3034 3127 2069 6e20 616c 6c72 6573  'A041' in allres
-00002d10: 756c 7473 2e63 6f72 6572 6573 756c 7473  ults.coreresults
-00002d20: 2065 6c73 6520 436f 756e 7465 7228 290d   else Counter().
-00002d30: 0a20 2020 2066 6f75 7465 7076 7320 3d20  .    foutepvs = 
-00002d40: 7375 6270 7673 202b 2064 656c 7076 7320  subpvs + delpvs 
-00002d50: 2b20 7469 6a64 666f 7574 7076 730d 0a20  + tijdfoutpvs.. 
-00002d60: 2020 2075 7064 6174 6577 6974 6863 7472     updatewithctr
-00002d70: 2872 6573 756c 7464 6963 742c 2066 6f75  (resultdict, fou
-00002d80: 7465 7076 732c 2027 666f 7574 6570 7673  tepvs, 'foutepvs
-00002d90: 2729 0d0a 2020 2020 7570 6461 7465 2872  ')..    update(r
-00002da0: 6573 756c 7464 6963 742c 2061 6c6c 7265  esultdict, allre
-00002db0: 7375 6c74 732e 636f 7265 7265 7375 6c74  sults.coreresult
-00002dc0: 732c 2027 4130 3033 272c 2027 6269 6a7a  s, 'A003', 'bijz
-00002dd0: 696e 636f 756e 7427 290d 0a0d 0a20 2020  incount')....   
-00002de0: 2072 6573 756c 7420 3d20 7265 7375 6c74   result = result
-00002df0: 6469 6374 3274 6162 6c65 2872 6573 756c  dict2table(resul
-00002e00: 7464 6963 7429 0d0a 2020 2020 7265 7475  tdict)..    retu
-00002e10: 726e 2072 6573 756c 740d 0a0d 0a0d 0a64  rn result......d
-00002e20: 6566 2061 7374 6166 6f72 6d28 616c 6c72  ef astaform(allr
-00002e30: 6573 756c 7473 2c20 5f2c 2069 6e5f 6d65  esults, _, in_me
-00002e40: 6d6f 7279 3d46 616c 7365 293a 0d0a 2020  mory=False):..  
-00002e50: 2020 6e6f 756e 6469 6374 203d 2064 6566    noundict = def
-00002e60: 6175 6c74 6469 6374 2869 6e74 290d 0a20  aultdict(int).. 
-00002e70: 2020 2076 6572 6264 6963 7420 3d20 6465     verbdict = de
-00002e80: 6661 756c 7464 6963 7428 696e 7429 0d0a  faultdict(int)..
-00002e90: 2020 2020 616c 6c6d 6174 6368 6573 203d      allmatches =
-00002ea0: 2061 6c6c 7265 7375 6c74 732e 616c 6c6d   allresults.allm
-00002eb0: 6174 6368 6573 0d0a 2020 2020 2320 666f  atches..    # fo
-00002ec0: 7220 656c 2069 6e20 616c 6c6d 6174 6368  r el in allmatch
-00002ed0: 6573 3a0d 0a20 2020 2023 2020 2020 2028  es:..    #     (
-00002ee0: 7169 642c 2075 7474 6964 2920 3d20 656c  qid, uttid) = el
-00002ef0: 0d0a 2020 2020 2320 2020 2020 6966 2071  ..    #     if q
-00002f00: 6964 203d 3d20 2741 3032 3127 3a0d 0a20  id == 'A021':.. 
-00002f10: 2020 2023 2020 2020 2020 2020 2066 6f72     #         for
-00002f20: 2061 6d61 7463 6820 696e 2061 6c6c 6d61   amatch in allma
-00002f30: 7463 6865 735b 656c 5d3a 0d0a 2020 2020  tches[el]:..    
-00002f40: 2320 2020 2020 2020 2020 2020 2020 2320  #             # 
-00002f50: 7468 6577 6f72 6420 3d20 6e6f 726d 616c  theword = normal
-00002f60: 697a 6564 776f 7264 2861 6d61 7463 685b  izedword(amatch[
-00002f70: 305d 290d 0a20 2020 2023 2020 2020 2020  0])..    #      
-00002f80: 2020 2020 2020 2074 6865 776f 7264 203d         theword =
-00002f90: 2067 6574 6174 7476 616c 2861 6d61 7463   getattval(amatc
-00002fa0: 685b 305d 2c20 276c 656d 6d61 2729 0d0a  h[0], 'lemma')..
-00002fb0: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-00002fc0: 2020 6e6f 756e 6469 6374 5b74 6865 776f    noundict[thewo
-00002fd0: 7264 5d20 2b3d 2031 0d0a 2020 2020 2320  rd] += 1..    # 
-00002fe0: 2020 2020 6966 2071 6964 203d 3d20 2741      if qid == 'A
-00002ff0: 3031 3827 3a0d 0a20 2020 2023 2020 2020  018':..    #    
-00003000: 2020 2020 2066 6f72 2061 6d61 7463 6820       for amatch 
-00003010: 696e 2061 6c6c 6d61 7463 6865 735b 656c  in allmatches[el
-00003020: 5d3a 0d0a 2020 2020 2320 2020 2020 2020  ]:..    #       
-00003030: 2020 2020 2020 2320 7468 6577 6f72 6420        # theword 
-00003040: 3d20 6e6f 726d 616c 697a 6564 776f 7264  = normalizedword
-00003050: 2861 6d61 7463 685b 305d 290d 0a20 2020  (amatch[0])..   
-00003060: 2023 2020 2020 2020 2020 2020 2020 2074   #             t
-00003070: 6865 776f 7264 203d 2067 6574 6174 7476  heword = getattv
-00003080: 616c 2861 6d61 7463 685b 305d 2c20 276c  al(amatch[0], 'l
-00003090: 656d 6d61 2729 0d0a 2020 2020 2320 2020  emma')..    #   
-000030a0: 2020 2020 2020 2020 2020 7665 7262 6469            verbdi
-000030b0: 6374 5b74 6865 776f 7264 5d20 2b3d 2031  ct[theword] += 1
-000030c0: 0d0a 2020 2020 666f 7220 286c 656d 6d61  ..    for (lemma
-000030d0: 2c20 7574 7469 6429 2069 6e20 616c 6c72  , uttid) in allr
-000030e0: 6573 756c 7473 2e70 6f73 7472 6573 756c  esults.postresul
-000030f0: 7473 5b6e 6f75 6e6c 656d 6d61 7169 645d  ts[nounlemmaqid]
-00003100: 3a0d 0a20 2020 2020 2020 206e 6f75 6e64  :..        nound
-00003110: 6963 745b 6c65 6d6d 615d 202b 3d20 310d  ict[lemma] += 1.
-00003120: 0a20 2020 2066 6f72 2028 6c65 6d6d 612c  .    for (lemma,
-00003130: 2075 7474 6964 2920 696e 2061 6c6c 7265   uttid) in allre
-00003140: 7375 6c74 732e 706f 7374 7265 7375 6c74  sults.postresult
-00003150: 735b 7665 7262 6c65 6d6d 6171 6964 5d3a  s[verblemmaqid]:
-00003160: 0d0a 2020 2020 2020 2020 7665 7262 6469  ..        verbdi
-00003170: 6374 5b6c 656d 6d61 5d20 2b3d 2031 0d0a  ct[lemma] += 1..
-00003180: 2020 2020 7661 7264 6963 7420 3d20 6765      vardict = ge
-00003190: 7476 6172 6469 6374 2861 6c6c 7265 7375  tvardict(allresu
-000031a0: 6c74 7329 0d0a 2020 2020 7574 746c 6973  lts)..    uttlis
-000031b0: 7420 3d20 6765 7475 7474 6c69 7374 2861  t = getuttlist(a
-000031c0: 6c6c 7265 7375 6c74 7329 0d0a 2020 2020  llresults)..    
-000031d0: 6173 7461 6461 7461 203d 2041 7374 6146  astadata = AstaF
-000031e0: 6f72 6d44 6174 6128 6e6f 756e 6469 6374  ormData(noundict
-000031f0: 2c20 7665 7262 6469 6374 2c20 7661 7264  , verbdict, vard
-00003200: 6963 742c 2075 7474 6c69 7374 290d 0a20  ict, uttlist).. 
-00003210: 2020 2074 6865 666f 726d 203d 2045 7863     theform = Exc
-00003220: 656c 466f 726d 2874 6162 656c 2c20 7363  elForm(tabel, sc
-00003230: 6f72 6573 290d 0a0d 0a20 2020 2069 6620  ores)....    if 
-00003240: 696e 5f6d 656d 6f72 793a 0d0a 2020 2020  in_memory:..    
-00003250: 2020 2020 7461 7267 6574 203d 2042 7974      target = Byt
-00003260: 6573 494f 2829 0d0a 2020 2020 656c 7365  esIO()..    else
-00003270: 3a0d 0a20 2020 2020 2020 2074 6172 6765  :..        targe
-00003280: 7420 3d20 6765 7466 6f72 6d66 696c 656e  t = getformfilen
-00003290: 616d 6528 616c 6c72 6573 756c 7473 2e66  ame(allresults.f
-000032a0: 696c 656e 616d 652c 2027 5f61 7374 6166  ilename, '_astaf
-000032b0: 6f72 6d75 6c69 6572 2729 0d0a 0d0a 2020  ormulier')....  
-000032c0: 2020 7468 6577 6f72 6b62 6f6f 6b2c 2074    theworkbook, t
-000032d0: 6172 6765 7420 3d20 6d61 6b65 5f61 7374  arget = make_ast
-000032e0: 6166 6f72 6d28 7468 6566 6f72 6d2c 2061  aform(theform, a
-000032f0: 7374 6164 6174 612c 2074 6172 6765 7429  stadata, target)
-00003300: 0d0a 2020 2020 7468 6577 6f72 6b62 6f6f  ..    theworkboo
-00003310: 6b2e 636c 6f73 6528 290d 0a20 2020 2072  k.close()..    r
-00003320: 6574 7572 6e20 7461 7267 6574 0d0a       eturn target..
+00000100: 6669 6c65 6e61 6d65 0d0a 0d0a 6269 6a7a  filename....bijz
+00000110: 696e 7169 6420 3d20 2741 3030 3327 0d0a  inqid = 'A003'..
+00000120: 636f 7272 6563 7471 6964 203d 2027 4130  correctqid = 'A0
+00000130: 3034 270d 0a66 6f6e 7061 7271 6964 203d  04'..fonparqid =
+00000140: 2027 4130 3038 270d 0a64 656c 7076 7169   'A008'..delpvqi
+00000150: 6420 3d20 2741 3030 3927 0d0a 6b6f 7071  d = 'A009'..kopq
+00000160: 6964 203d 2027 4130 3133 270d 0a6c 6578  id = 'A013'..lex
+00000170: 7169 6420 3d20 2741 3031 3827 0d0a 6d6f  qid = 'A018'..mo
+00000180: 6461 6c71 6964 203d 2027 4130 3230 270d  dalqid = 'A020'.
+00000190: 0a6e 6f75 6e71 6964 203d 2027 4130 3231  .nounqid = 'A021
+000001a0: 270d 0a6e 656f 7169 6420 3d20 2741 3032  '..neoqid = 'A02
+000001b0: 3227 0d0a 7076 7169 6420 3d20 2741 3032  2'..pvqid = 'A02
+000001c0: 3427 0d0a 7365 6d70 6172 7169 6420 3d20  4'..semparqid = 
+000001d0: 2741 3032 3627 0d0a 7375 6270 7671 6964  'A026'..subpvqid
+000001e0: 203d 2027 4130 3332 270d 0a74 696a 6466   = 'A032'..tijdf
+000001f0: 6f75 7470 7671 6964 203d 2027 4130 3431  outpvqid = 'A041
+00000200: 270d 0a6c 656d 6d61 7169 6420 3d20 2741  '..lemmaqid = 'A
+00000210: 3035 3127 0d0a 0d0a 6269 6a7a 696e 7169  051'....bijzinqi
+00000220: 6420 3d20 2741 3030 3327 0d0a 636f 7272  d = 'A003'..corr
+00000230: 6563 7471 6964 203d 2027 4130 3034 270d  ectqid = 'A004'.
+00000240: 0a66 6f6e 7061 7271 6964 203d 2027 4130  .fonparqid = 'A0
+00000250: 3038 270d 0a64 656c 7076 7169 6420 3d20  08'..delpvqid = 
+00000260: 2741 3030 3927 0d0a 6b6f 7071 6964 203d  'A009'..kopqid =
+00000270: 2027 4130 3133 270d 0a6c 6578 7169 6420   'A013'..lexqid 
+00000280: 3d20 2741 3031 3827 0d0a 6d6f 6461 6c71  = 'A018'..modalq
+00000290: 6964 203d 2027 4130 3230 270d 0a6e 6f75  id = 'A020'..nou
+000002a0: 6e71 6964 203d 2027 4130 3231 270d 0a6e  nqid = 'A021'..n
+000002b0: 656f 7169 6420 3d20 2741 3032 3227 0d0a  eoqid = 'A022'..
+000002c0: 7076 7169 6420 3d20 2741 3032 3427 0d0a  pvqid = 'A024'..
+000002d0: 7365 6d70 6172 7169 6420 3d20 2741 3032  semparqid = 'A02
+000002e0: 3627 0d0a 7375 6270 7671 6964 203d 2027  6'..subpvqid = '
+000002f0: 4130 3332 270d 0a74 696a 6466 6f75 7470  A032'..tijdfoutp
+00000300: 7671 6964 203d 2027 4130 3431 270d 0a6c  vqid = 'A041'..l
+00000310: 656d 6d61 7169 6420 3d20 2741 3035 3127  emmaqid = 'A051'
+00000320: 0d0a 0d0a 6269 6a7a 696e 7265 736b 6579  ....bijzinreskey
+00000330: 203d 206d 6b72 6573 756c 7473 6b65 7928   = mkresultskey(
+00000340: 6269 6a7a 696e 7169 6429 0d0a 636f 7272  bijzinqid)..corr
+00000350: 6563 7472 6573 6b65 7920 3d20 6d6b 7265  ectreskey = mkre
+00000360: 7375 6c74 736b 6579 2863 6f72 7265 6374  sultskey(correct
+00000370: 7169 6429 0d0a 666f 6e70 6172 7265 736b  qid)..fonparresk
+00000380: 6579 203d 206d 6b72 6573 756c 7473 6b65  ey = mkresultske
+00000390: 7928 666f 6e70 6172 7169 6429 0d0a 6465  y(fonparqid)..de
+000003a0: 6c70 7672 6573 6b65 7920 3d20 6d6b 7265  lpvreskey = mkre
+000003b0: 7375 6c74 736b 6579 2864 656c 7076 7169  sultskey(delpvqi
+000003c0: 6429 0d0a 6b6f 7072 6573 6b65 7920 3d20  d)..kopreskey = 
+000003d0: 6d6b 7265 7375 6c74 736b 6579 286b 6f70  mkresultskey(kop
+000003e0: 7169 6429 0d0a 6c65 7872 6573 6b65 7920  qid)..lexreskey 
+000003f0: 3d20 6d6b 7265 7375 6c74 736b 6579 286c  = mkresultskey(l
+00000400: 6578 7169 6429 0d0a 6d6f 6461 6c72 6573  exqid)..modalres
+00000410: 6b65 7920 3d20 6d6b 7265 7375 6c74 736b  key = mkresultsk
+00000420: 6579 286d 6f64 616c 7169 6429 0d0a 6e6f  ey(modalqid)..no
+00000430: 756e 7265 736b 6579 203d 206d 6b72 6573  unreskey = mkres
+00000440: 756c 7473 6b65 7928 6e6f 756e 7169 6429  ultskey(nounqid)
+00000450: 0d0a 6e65 6f72 6573 6b65 7920 3d20 6d6b  ..neoreskey = mk
+00000460: 7265 7375 6c74 736b 6579 286e 656f 7169  resultskey(neoqi
+00000470: 6429 0d0a 7076 7265 736b 6579 203d 206d  d)..pvreskey = m
+00000480: 6b72 6573 756c 7473 6b65 7928 7076 7169  kresultskey(pvqi
+00000490: 6429 0d0a 7365 6d70 6172 7265 736b 6579  d)..semparreskey
+000004a0: 203d 206d 6b72 6573 756c 7473 6b65 7928   = mkresultskey(
+000004b0: 7365 6d70 6172 7169 6429 0d0a 7375 6270  semparqid)..subp
+000004c0: 7672 6573 6b65 7920 3d20 6d6b 7265 7375  vreskey = mkresu
+000004d0: 6c74 736b 6579 2873 7562 7076 7169 6429  ltskey(subpvqid)
+000004e0: 0d0a 7469 6a64 666f 7574 7076 7265 736b  ..tijdfoutpvresk
+000004f0: 6579 203d 206d 6b72 6573 756c 7473 6b65  ey = mkresultske
+00000500: 7928 7469 6a64 666f 7574 7076 7169 6429  y(tijdfoutpvqid)
+00000510: 0d0a 6c65 6d6d 6172 6573 6b65 7920 3d20  ..lemmareskey = 
+00000520: 6d6b 7265 7375 6c74 736b 6579 286c 656d  mkresultskey(lem
+00000530: 6d61 7169 6429 0d0a 0d0a 0d0a 6772 6565  maqid)......gree
+00000540: 6e20 3d20 2723 3030 4646 3030 270d 0a72  n = '#00FF00'..r
+00000550: 6564 203d 2027 2346 4630 3030 3027 0d0a  ed = '#FF0000'..
+00000560: 6f72 616e 6765 203d 2027 2346 4642 4239  orange = '#FFBB9
+00000570: 4127 0d0a 6772 6579 203d 2027 2342 3042  A'..grey = '#B0B
+00000580: 3042 3027 0d0a 0d0a 0d0a 2320 6772 6565  0B0'......# gree
+00000590: 6e20 3d20 2767 7265 656e 270d 0a23 2067  n = 'green'..# g
+000005a0: 7265 656e 203d 2027 2330 3036 3130 3027  reen = '#006100'
+000005b0: 0d0a 2320 7265 6420 3d20 2723 3943 3030  ..# red = '#9C00
+000005c0: 3036 270d 0a23 2072 6564 203d 2027 7265  06'..# red = 're
+000005d0: 6427 0d0a 2320 6f72 616e 6765 203d 2027  d'..# orange = '
+000005e0: 2339 4336 3530 3027 0d0a 2320 6f72 616e  #9C6500'..# oran
+000005f0: 6765 203d 2027 7965 6c6c 6f77 270d 0a0d  ge = 'yellow'...
+00000600: 0a0d 0a64 6566 2063 6f6e 646e 6f75 6e28  ...def condnoun(
+00000610: 6c65 6d6d 6170 6f73 6974 696f 6e73 2c20  lemmapositions, 
+00000620: 6578 6163 7472 6573 756c 7473 293a 0d0a  exactresults):..
+00000630: 2020 2020 6e6f 756e 706f 7369 7469 6f6e      nounposition
+00000640: 7320 3d20 6578 6163 7472 6573 756c 7473  s = exactresults
+00000650: 5b6e 6f75 6e72 6573 6b65 795d 0d0a 2020  [nounreskey]..  
+00000660: 2020 7265 7375 6c74 203d 206c 656d 6d61    result = lemma
+00000670: 706f 7369 7469 6f6e 7320 696e 206e 6f75  positions in nou
+00000680: 6e70 6f73 6974 696f 6e73 2020 2023 2073  npositions   # s
+00000690: 6f6d 6574 6869 6e67 2069 7320 7772 6f6e  omething is wron
+000006a0: 6720 6865 7265 204a 4f0d 0a20 2020 2072  g here JO..    r
+000006b0: 6574 7572 6e20 7265 7375 6c74 0d0a 0d0a  eturn result....
+000006c0: 0d0a 636c 6173 7320 4578 6365 6c46 6f72  ..class ExcelFor
+000006d0: 6d3a 0d0a 2020 2020 6465 6620 5f5f 696e  m:..    def __in
+000006e0: 6974 5f5f 2873 656c 662c 2074 6162 656c  it__(self, tabel
+000006f0: 2c20 7363 6f72 6573 293a 0d0a 2020 2020  , scores):..    
+00000700: 2020 2020 7365 6c66 2e74 6162 656c 203d      self.tabel =
+00000710: 2074 6162 656c 0d0a 2020 2020 2020 2020   tabel..        
+00000720: 7365 6c66 2e73 636f 7265 7320 3d20 7363  self.scores = sc
+00000730: 6f72 6573 0d0a 0d0a 0d0a 636c 6173 7320  ores......class 
+00000740: 4173 7461 466f 726d 4461 7461 3a0d 0a20  AstaFormData:.. 
+00000750: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000760: 7365 6c66 2c20 6e6f 756e 6469 6374 2c20  self, noundict, 
+00000770: 7665 7262 6469 6374 2c20 7661 7264 6963  verbdict, vardic
+00000780: 742c 2075 7474 6c69 7374 293a 0d0a 2020  t, uttlist):..  
+00000790: 2020 2020 2020 7365 6c66 2e6e 6f75 6e64        self.nound
+000007a0: 6963 7420 3d20 6e6f 756e 6469 6374 0d0a  ict = noundict..
+000007b0: 2020 2020 2020 2020 7365 6c66 2e76 6572          self.ver
+000007c0: 6264 6963 7420 3d20 7665 7262 6469 6374  bdict = verbdict
+000007d0: 0d0a 2020 2020 2020 2020 7365 6c66 2e76  ..        self.v
+000007e0: 6172 6469 6374 203d 2076 6172 6469 6374  ardict = vardict
+000007f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e75  ..        self.u
+00000800: 7474 6c69 7374 203d 2075 7474 6c69 7374  ttlist = uttlist
+00000810: 0d0a 0d0a 0d0a 666f 726d 756c 6174 656d  ......formulatem
+00000820: 706c 6174 6531 203d 2027 3d49 4628 427b  plate1 = '=IF(B{
+00000830: 7d3d 224e 6965 7420 6765 7675 6c64 222c  }="Niet gevuld",
+00000840: 427b 7d2c 2842 7b7d 2d54 6162 656c 2142  B{},(B{}-Tabel!B
+00000850: 7b7d 292f 5461 6265 6c21 437b 7d29 270d  {})/Tabel!C{})'.
+00000860: 0a0d 0a0d 0a64 6566 2061 7070 6c79 7465  .....def applyte
+00000870: 6d70 6c61 7465 3128 726f 7763 7472 293a  mplate1(rowctr):
+00000880: 0d0a 2020 2020 7265 7375 6c74 203d 2066  ..    result = f
+00000890: 6f72 6d75 6c61 7465 6d70 6c61 7465 312e  ormulatemplate1.
+000008a0: 666f 726d 6174 280d 0a20 2020 2020 2020  format(..       
+000008b0: 2072 6f77 6374 722c 2072 6f77 6374 722c   rowctr, rowctr,
+000008c0: 2072 6f77 6374 722c 2072 6f77 6374 7220   rowctr, rowctr 
+000008d0: 2b20 312c 2072 6f77 6374 7220 2b20 3129  + 1, rowctr + 1)
+000008e0: 0d0a 2020 2020 7265 7475 726e 2072 6573  ..    return res
+000008f0: 756c 740d 0a0d 0a0d 0a66 6f72 6d75 6c61  ult......formula
+00000900: 7465 6d70 6c61 7465 3220 3d20 273d 2842  template2 = '=(B
+00000910: 7b7d 2d54 6162 656c 2142 7b7d 292f 5461  {}-Tabel!B{})/Ta
+00000920: 6265 6c21 437b 7d27 0d0a 0d0a 0d0a 6465  bel!C{}'......de
+00000930: 6620 6170 706c 7974 656d 706c 6174 6532  f applytemplate2
+00000940: 2872 6f77 6374 7229 3a0d 0a20 2020 2072  (rowctr):..    r
+00000950: 6573 756c 7420 3d20 666f 726d 756c 6174  esult = formulat
+00000960: 656d 706c 6174 6532 2e66 6f72 6d61 7428  emplate2.format(
+00000970: 726f 7763 7472 2c20 726f 7763 7472 202b  rowctr, rowctr +
+00000980: 2031 2c20 726f 7763 7472 202b 2031 290d   1, rowctr + 1).
+00000990: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
+000009a0: 6c74 0d0a 0d0a 0d0a 666f 726d 756c 6174  lt......formulat
+000009b0: 656d 706c 6174 6533 203d 2022 3d49 4628  emplate3 = "=IF(
+000009c0: 4953 4552 524f 5228 524f 554e 4428 277b  ISERROR(ROUND('{
+000009d0: 7d27 217b 7d33 2c32 2929 2c5c 224e 6965  }'!{}3,2)),\"Nie
+000009e0: 7420 6765 7675 6c64 5c22 2c52 4f55 4e44  t gevuld\",ROUND
+000009f0: 2827 7b7d 2721 7b7d 332c 3229 2922 0d0a  ('{}'!{}3,2))"..
+00000a00: 0d0a 0d0a 6465 6620 6170 706c 7974 656d  ....def applytem
+00000a10: 706c 6174 6533 2873 6865 6574 2c20 636f  plate3(sheet, co
+00000a20: 6c63 6861 7229 3a0d 0a20 2020 2072 6573  lchar):..    res
+00000a30: 756c 7420 3d20 666f 726d 756c 6174 656d  ult = formulatem
+00000a40: 706c 6174 6533 2e66 6f72 6d61 7428 7368  plate3.format(sh
+00000a50: 6565 742c 2063 6f6c 6368 6172 2c20 7368  eet, colchar, sh
+00000a60: 6565 742c 2063 6f6c 6368 6172 290d 0a20  eet, colchar).. 
+00000a70: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00000a80: 0d0a 0d0a 0d0a 6669 6e69 6574 6865 6964  ......finietheid
+00000a90: 7369 6e64 6578 7363 6f72 6520 3d20 223d  sindexscore = "=
+00000aa0: 4946 2849 5345 5252 4f52 2852 4f55 4e44  IF(ISERROR(ROUND
+00000ab0: 2855 6974 696e 6765 6e21 4433 2c32 2929  (Uitingen!D3,2))
+00000ac0: 2c5c 224e 6965 7420 6765 7675 6c64 5c22  ,\"Niet gevuld\"
+00000ad0: 2c52 4f55 4e44 2855 6974 696e 6765 6e21  ,ROUND(Uitingen!
+00000ae0: 4433 2c32 2929 220d 0a70 6375 7363 6f72  D3,2))"..pcuscor
+00000af0: 6520 3d20 223d 4946 2849 5345 5252 4f52  e = "=IF(ISERROR
+00000b00: 2852 4f55 4e44 2855 6974 696e 6765 6e21  (ROUND(Uitingen!
+00000b10: 4234 2f55 6974 696e 6765 6e21 4231 2c32  B4/Uitingen!B1,2
+00000b20: 2929 2c5c 224e 6965 7420 6765 7675 6c64  )),\"Niet gevuld
+00000b30: 5c22 2c52 4f55 4e44 2855 6974 696e 6765  \",ROUND(Uitinge
+00000b40: 6e21 4234 2f55 6974 696e 6765 6e21 4231  n!B4/Uitingen!B1
+00000b50: 2c32 2929 220d 0a0d 0a74 6162 656c 203d  ,2))"....tabel =
+00000b60: 205b 5b27 272c 2027 4745 4d27 2c20 2753   [['', 'GEM', 'S
+00000b70: 4427 5d2c 0d0a 2020 2020 2020 2020 205b  D'],..         [
+00000b80: 2741 616e 7461 6c20 7a65 6c66 7374 616e  'Aantal zelfstan
+00000b90: 6469 6765 206e 6161 6d77 6f6f 7264 656e  dige naamwoorden
+00000ba0: 272c 2034 382c 2037 2e38 385d 2c0d 0a20  ', 48, 7.88],.. 
+00000bb0: 2020 2020 2020 2020 5b27 5454 5220 7a65          ['TTR ze
+00000bc0: 6c66 7374 616e 6469 6765 206e 6161 6d77  lfstandige naamw
+00000bd0: 6f6f 7264 656e 272c 2030 2e37 362c 2030  oorden', 0.76, 0
+00000be0: 2e30 385d 2c0d 0a20 2020 2020 2020 2020  .08],..         
+00000bf0: 5b27 4c65 7869 6361 6c65 2077 6572 6b77  ['Lexicale werkw
+00000c00: 6f6f 7264 656e 272c 2032 392c 2034 2e31  oorden', 29, 4.1
+00000c10: 345d 2c0d 0a20 2020 2020 2020 2020 5b27  4],..         ['
+00000c20: 5454 5220 6c65 7869 6361 6c20 7765 726b  TTR lexical werk
+00000c30: 776f 6f72 6465 6e27 2c20 302e 3633 2c20  woorden', 0.63, 
+00000c40: 302e 3131 5d2c 0d0a 2020 2020 2020 2020  0.11],..        
+00000c50: 205b 2753 656d 616e 7469 7363 6865 2070   ['Semantische p
+00000c60: 6172 6166 6173 6965 c3ab 6e27 2c20 302c  arafasie..n', 0,
+00000c70: 2030 2e35 375d 2c0d 0a20 2020 2020 2020   0.57],..       
+00000c80: 2020 5b27 466f 6e6f 6c6f 6769 7363 6865    ['Fonologische
+00000c90: 2070 6172 6166 6173 6965 c3ab 6e27 2c20   parafasie..n', 
+00000ca0: 302c 2030 2e33 335d 2c0d 0a20 2020 2020  0, 0.33],..     
+00000cb0: 2020 2020 5b27 4e65 6f6c 6f67 6973 6d65      ['Neologisme
+00000cc0: 6e27 2c20 302c 2030 5d2c 0d0a 2020 2020  n', 0, 0],..    
+00000cd0: 2020 2020 205b 2741 616e 7461 6c20 6b6f       ['Aantal ko
+00000ce0: 7070 656c 2f6d 6f64 6161 6c77 6572 6b77  ppel/modaalwerkw
+00000cf0: 6f6f 7264 656e 272c 2031 322c 2034 2e31  oorden', 12, 4.1
+00000d00: 355d 2c0d 0a20 2020 2020 2020 2020 5b27  5],..         ['
+00000d10: 4d4c 5527 2c20 382e 3633 2c20 312e 3734  MLU', 8.63, 1.74
+00000d20: 5d2c 0d0a 2020 2020 2020 2020 205b 2750  ],..         ['P
+00000d30: 6572 6365 6e74 6167 6520 636f 7272 6563  ercentage correc
+00000d40: 7465 2075 6974 696e 6765 6e27 2c20 302e  te uitingen', 0.
+00000d50: 3933 2c20 302e 3036 5d2c 0d0a 2020 2020  93, 0.06],..    
+00000d60: 2020 2020 205b 2746 696e 6965 7468 6569       ['Finiethei
+00000d70: 6473 696e 6465 7827 2c20 302e 3939 2c20  dsindex', 0.99, 
+00000d80: 302e 3033 5d2c 0d0a 2020 2020 2020 2020  0.03],..        
+00000d90: 205b 2741 616e 7461 6c20 6269 6a7a 696e   ['Aantal bijzin
+00000da0: 6e65 6e27 2c20 342e 382c 2032 2e37 385d  nen', 4.8, 2.78]
+00000db0: 5d0d 0a0d 0a73 636f 7265 7320 3d20 5b5b  ]....scores = [[
+00000dc0: 2727 2c20 2753 636f 7265 272c 2027 5344  '', 'Score', 'SD
+00000dd0: 275d 2c0d 0a20 2020 2020 2020 2020 205b  '],..          [
+00000de0: 2741 616e 7461 6c20 7a65 6c66 7374 616e  'Aantal zelfstan
+00000df0: 6469 6765 206e 6161 6d77 6f6f 7264 656e  dige naamwoorden
+00000e00: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00000e10: 2020 223d 275a 4e57 2026 2057 5727 2142    "='ZNW & WW'!B
+00000e20: 3122 2c20 223d 2842 322d 5461 6265 6c21  1", "=(B2-Tabel!
+00000e30: 4233 292f 5461 6265 6c21 4333 225d 2c0d  B3)/Tabel!C3"],.
+00000e40: 0a20 2020 2020 2020 2020 205b 2754 5452  .          ['TTR
+00000e50: 207a 656c 6673 7461 6e64 6967 6520 6e61   zelfstandige na
+00000e60: 616d 776f 6f72 6465 6e27 2c20 6170 706c  amwoorden', appl
+00000e70: 7974 656d 706c 6174 6533 280d 0a20 2020  ytemplate3(..   
+00000e80: 2020 2020 2020 2020 2020 2027 5a4e 5720             'ZNW 
+00000e90: 2620 5757 272c 2027 4227 292c 2061 7070  & WW', 'B'), app
+00000ea0: 6c79 7465 6d70 6c61 7465 3128 3329 5d2c  lytemplate1(3)],
+00000eb0: 0d0a 2020 2020 2020 2020 2020 5b27 4161  ..          ['Aa
+00000ec0: 6e74 616c 206c 6578 6963 616c 6520 7765  ntal lexicale we
+00000ed0: 726b 776f 6f72 6465 6e27 2c20 223d 275a  rkwoorden', "='Z
+00000ee0: 4e57 2026 2057 5727 2146 3122 2c20 6170  NW & WW'!F1", ap
+00000ef0: 706c 7974 656d 706c 6174 6532 2834 295d  plytemplate2(4)]
+00000f00: 2c0d 0a20 2020 2020 2020 2020 205b 2754  ,..          ['T
+00000f10: 5452 206c 6578 6963 616c 6520 7765 726b  TR lexicale werk
+00000f20: 776f 6f72 6465 6e27 2c20 6170 706c 7974  woorden', applyt
+00000f30: 656d 706c 6174 6533 280d 0a20 2020 2020  emplate3(..     
+00000f40: 2020 2020 2020 2020 2027 5a4e 5720 2620           'ZNW & 
+00000f50: 5757 272c 2027 4627 292c 2061 7070 6c79  WW', 'F'), apply
+00000f60: 7465 6d70 6c61 7465 3128 3529 5d2c 0d0a  template1(5)],..
+00000f70: 2020 2020 2020 2020 2020 5b27 5365 6d61            ['Sema
+00000f80: 6e74 6973 6368 6520 7061 7261 6661 7369  ntische parafasi
+00000f90: 65c3 ab6e 272c 2027 272c 2061 7070 6c79  e..n', '', apply
+00000fa0: 7465 6d70 6c61 7465 3228 3629 5d2c 0d0a  template2(6)],..
+00000fb0: 2020 2020 2020 2020 2020 5b27 466f 6e6f            ['Fono
+00000fc0: 6c6f 6769 7363 6865 2070 6172 6166 6173  logische parafas
+00000fd0: 6965 c3ab 6e27 2c20 2727 2c20 6170 706c  ie..n', '', appl
+00000fe0: 7974 656d 706c 6174 6532 2837 295d 2c0d  ytemplate2(7)],.
+00000ff0: 0a20 2020 2020 2020 2020 205b 274e 656f  .          ['Neo
+00001000: 6c6f 6769 736d 656e 272c 2027 272c 2027  logismen', '', '
+00001010: 3d49 4628 4238 3d30 2c22 4e6f 726d 6161  =IF(B8=0,"Normaa
+00001020: 6c22 2c22 4166 7769 6a6b 656e 6422 2927  l","Afwijkend")'
+00001030: 5d2c 0d0a 2020 2020 2020 2020 2020 5b27  ],..          ['
+00001040: 4161 6e74 616c 206b 6f70 7065 6c2f 6d6f  Aantal koppel/mo
+00001050: 6461 616c 7765 726b 776f 6f72 6465 6e27  daalwerkwoorden'
+00001060: 2c20 2727 2c20 6170 706c 7974 656d 706c  , '', applytempl
+00001070: 6174 6532 2839 295d 2c0d 0a20 2020 2020  ate2(9)],..     
+00001080: 2020 2020 205b 274d 4c55 272c 2061 7070       ['MLU', app
+00001090: 6c79 7465 6d70 6c61 7465 3328 2755 6974  lytemplate3('Uit
+000010a0: 696e 6765 6e27 2c20 2742 2729 2c20 6170  ingen', 'B'), ap
+000010b0: 706c 7974 656d 706c 6174 6531 2831 3029  plytemplate1(10)
+000010c0: 5d2c 0d0a 2020 2020 2020 2020 2020 5b27  ],..          ['
+000010d0: 5065 7263 656e 7461 6765 2063 6f72 7265  Percentage corre
+000010e0: 6374 6520 7569 7469 6e67 656e 272c 2070  cte uitingen', p
+000010f0: 6375 7363 6f72 652c 2061 7070 6c79 7465  cuscore, applyte
+00001100: 6d70 6c61 7465 3128 3131 295d 2c0d 0a20  mplate1(11)],.. 
+00001110: 2020 2020 2020 2020 205b 2746 696e 6965           ['Finie
+00001120: 7468 6569 6473 696e 6465 7827 2c20 6669  theidsindex', fi
+00001130: 6e69 6574 6865 6964 7369 6e64 6578 7363  nietheidsindexsc
+00001140: 6f72 652c 2061 7070 6c79 7465 6d70 6c61  ore, applytempla
+00001150: 7465 3128 3132 295d 2c0d 0a20 2020 2020  te1(12)],..     
+00001160: 2020 2020 205b 2741 616e 7461 6c20 6269       ['Aantal bi
+00001170: 6a7a 696e 6e65 6e27 2c20 273d 5569 7469  jzinnen', '=Uiti
+00001180: 6e67 656e 2146 3227 2c20 6170 706c 7974  ngen!F2', applyt
+00001190: 656d 706c 6174 6532 2831 3329 5d5d 0d0a  emplate2(13)]]..
+000011a0: 0d0a 7368 6565 7432 6869 6464 656e 726f  ..sheet2hiddenro
+000011b0: 7773 203d 205b 5b27 546f 7461 616c 272c  ws = [['Totaal',
+000011c0: 2027 3d53 554d 2844 363a 4431 3035 2927   '=SUM(D6:D105)'
+000011d0: 2c20 2727 2c20 2727 2c20 2727 2c20 273d  , '', '', '', '=
+000011e0: 5355 4d28 4836 3a48 3130 3529 275d 2c0d  SUM(H6:H105)'],.
+000011f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001200: 2020 2020 205b 2741 616e 7461 6c20 756e       ['Aantal un
+00001210: 6965 6b27 2c20 273d 434f 554e 5441 2842  iek', '=COUNTA(B
+00001220: 363a 4231 3035 2927 2c0d 0a20 2020 2020  6:B105)',..     
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 2727 2c20 2727 2c20 2727 2c20 273d 434f  '', '', '', '=CO
+00001250: 554e 5441 2846 363a 4631 3035 2927 5d2c  UNTA(F6:F105)'],
+00001260: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001270: 2020 2020 2020 5b27 5454 5227 2c20 273d        ['TTR', '=
+00001280: 4232 2f42 3127 2c20 2727 2c20 2727 2c20  B2/B1', '', '', 
+00001290: 2727 2c20 273d 4632 2f46 3127 5d2c 0d0a  '', '=F2/F1'],..
+000012a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012b0: 2020 2020 5b27 272c 2027 272c 2027 272c      ['', '', '',
+000012c0: 2027 272c 2027 272c 2027 275d 0d0a 2020   '', '', '']..  
+000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012e0: 2020 5d0d 0a0d 0a73 6865 6574 3368 6964    ]....sheet3hid
+000012f0: 6465 6e72 6f77 7320 3d20 5b5b 2741 616e  denrows = [['Aan
+00001300: 7461 6c27 2c20 273d 434f 554e 5441 2842  tal', '=COUNTA(B
+00001310: 363a 4231 3035 2927 2c20 2727 2c20 2753  6:B105)', '', 'S
+00001320: 6f6d 272c 2027 536f 6d27 2c20 2753 6f6d  om', 'Som', 'Som
+00001330: 275d 2c0d 0a20 2020 2020 2020 2020 2020  '],..           
+00001340: 2020 2020 2020 2020 205b 2754 6f74 6161           ['Totaa
+00001350: 6c27 2c20 273d 5355 4d28 4236 3a42 3130  l', '=SUM(B6:B10
+00001360: 3529 272c 2027 272c 2027 3d53 554d 2844  5)', '', '=SUM(D
+00001370: 363a 4431 3035 2927 2c0d 0a20 2020 2020  6:D105)',..     
+00001380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001390: 273d 5355 4d28 4536 3a45 3130 3529 272c  '=SUM(E6:E105)',
+000013a0: 2027 3d53 554d 2846 363a 4631 3035 2927   '=SUM(F6:F105)'
+000013b0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+000013c0: 2020 2020 2020 2020 5b27 4d4c 5527 2c20          ['MLU', 
+000013d0: 273d 4232 2f42 3127 2c20 2727 2c20 273d  '=B2/B1', '', '=
+000013e0: 2844 322f 2844 322b 4532 2929 272c 2027  (D2/(D2+E2))', '
+000013f0: 272c 2027 275d 2c0d 0a20 2020 2020 2020  ', ''],..       
+00001400: 2020 2020 2020 2020 2020 2020 205b 2743               ['C
+00001410: 6f72 7265 6374 272c 2027 3d43 4f55 4e54  orrect', '=COUNT
+00001420: 4946 2843 363a 4331 3035 2c22 4a22 2927  IF(C6:C105,"J")'
+00001430: 2c20 2727 2c20 2727 2c20 2727 2c20 2727  , '', '', '', ''
+00001440: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00001450: 2020 2020 2020 205d 0d0a 0d0a 7368 6565         ]....shee
+00001460: 7432 6865 6164 6572 203d 205b 274e 756d  t2header = ['Num
+00001470: 6d65 7227 2c20 275a 656c 6673 7461 6e64  mer', 'Zelfstand
+00001480: 6967 206e 6161 6d77 6f6f 7264 272c 2027  ig naamwoord', '
+00001490: 4865 7268 616c 696e 6727 2c20 2741 616e  Herhaling', 'Aan
+000014a0: 7461 6c27 2c20 2727 2c20 274c 6578 6963  tal', '', 'Lexic
+000014b0: 6161 6c20 7765 726b 776f 6f72 6427 2c20  aal werkwoord', 
+000014c0: 2748 6572 6861 6c69 6e67 272c 0d0a 2020  'Herhaling',..  
+000014d0: 2020 2020 2020 2020 2020 2020 2020 2741                'A
+000014e0: 616e 7461 6c27 5d0d 0a73 6865 6574 3263  antal']..sheet2c
+000014f0: 6f6c 7769 6474 6873 203d 205b 3130 2c20  olwidths = [10, 
+00001500: 3235 2c20 3230 2c20 3130 2c20 352c 2032  25, 20, 10, 5, 2
+00001510: 352c 2032 302c 2031 305d 0d0a 7368 6565  5, 20, 10]..shee
+00001520: 7433 6865 6164 6572 203d 205b 2755 6974  t3header = ['Uit
+00001530: 696e 6773 6e75 6d6d 6572 272c 2027 4161  ingsnummer', 'Aa
+00001540: 6e74 616c 2077 6f6f 7264 656e 272c 2027  ntal woorden', '
+00001550: 436f 7272 6563 7427 2c20 2247 6f65 6465  Correct', "Goede
+00001560: 2050 5627 7322 2c20 2246 6f75 7465 2065   PV's", "Foute e
+00001570: 6e20 6f6e 7462 7265 6b65 6e64 6520 5056  n ontbrekende PV
+00001580: 2773 222c 0d0a 2020 2020 2020 2020 2020  's",..          
+00001590: 2020 2020 2020 2241 616e 7461 6c20 6269        "Aantal bi
+000015a0: 6a7a 696e 6e65 6e22 2c20 2242 696a 7a6f  jzinnen", "Bijzo
+000015b0: 6e64 6572 6865 6465 6e22 5d0d 0a0d 0a0d  nderheden"].....
+000015c0: 0a64 6566 2077 7269 7465 7461 626c 6528  .def writetable(
+000015d0: 7461 6265 6c2c 2077 732c 2073 7461 7274  tabel, ws, start
+000015e0: 726f 773d 302c 2073 7461 7274 636f 6c3d  row=0, startcol=
+000015f0: 302c 2072 6866 6f72 6d61 743d 4e6f 6e65  0, rhformat=None
+00001600: 2c20 6368 666f 726d 6174 3d4e 6f6e 652c  , chformat=None,
+00001610: 2063 656c 6c66 6f72 6d61 743d 4e6f 6e65   cellformat=None
+00001620: 293a 0d0a 2020 2020 6375 7263 6f6c 203d  ):..    curcol =
+00001630: 2073 7461 7274 636f 6c0d 0a20 2020 2063   startcol..    c
+00001640: 7572 726f 7720 3d20 7374 6172 7472 6f77  urrow = startrow
+00001650: 0d0a 2020 2020 666f 7220 726f 7720 696e  ..    for row in
+00001660: 2074 6162 656c 3a0d 0a20 2020 2020 2020   tabel:..       
+00001670: 2066 6f72 2065 6c20 696e 2072 6f77 3a0d   for el in row:.
+00001680: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00001690: 6375 7272 6f77 203d 3d20 7374 6172 7472  currow == startr
+000016a0: 6f77 3a0d 0a20 2020 2020 2020 2020 2020  ow:..           
+000016b0: 2020 2020 2074 6865 666f 726d 6174 203d       theformat =
+000016c0: 2072 6866 6f72 6d61 740d 0a20 2020 2020   rhformat..     
+000016d0: 2020 2020 2020 2065 6c69 6620 6375 7263         elif curc
+000016e0: 6f6c 203d 3d20 7374 6172 7463 6f6c 3a0d  ol == startcol:.
+000016f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001700: 2074 6865 666f 726d 6174 203d 2063 6866   theformat = chf
+00001710: 6f72 6d61 740d 0a20 2020 2020 2020 2020  ormat..         
+00001720: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00001730: 2020 2020 2020 2020 2020 7468 6566 6f72            thefor
+00001740: 6d61 7420 3d20 6365 6c6c 666f 726d 6174  mat = cellformat
+00001750: 0d0a 2020 2020 2020 2020 2020 2020 7773  ..            ws
+00001760: 2e77 7269 7465 2863 7572 726f 772c 2063  .write(currow, c
+00001770: 7572 636f 6c2c 2065 6c2c 2074 6865 666f  urcol, el, thefo
+00001780: 726d 6174 290d 0a20 2020 2020 2020 2020  rmat)..         
+00001790: 2020 2063 7572 636f 6c20 2b3d 2031 0d0a     curcol += 1..
+000017a0: 2020 2020 2020 2020 6375 7272 6f77 202b          currow +
+000017b0: 3d20 310d 0a20 2020 2020 2020 2063 7572  = 1..        cur
+000017c0: 636f 6c20 3d20 7374 6172 7463 6f6c 0d0a  col = startcol..
+000017d0: 0d0a 0d0a 6465 6620 6d61 6b65 5f61 7374  ....def make_ast
+000017e0: 6166 6f72 6d28 7468 6566 6f72 6d2c 2061  aform(theform, a
+000017f0: 7374 6164 6174 612c 2074 6172 6765 7429  stadata, target)
+00001800: 3a0d 0a20 2020 2077 6f72 6b62 6f6f 6b20  :..    workbook 
+00001810: 3d20 786c 7378 7772 6974 6572 2e57 6f72  = xlsxwriter.Wor
+00001820: 6b62 6f6f 6b28 7461 7267 6574 2c20 7b22  kbook(target, {"
+00001830: 7374 7269 6e67 735f 746f 5f6e 756d 6265  strings_to_numbe
+00001840: 7273 223a 2054 7275 657d 290d 0a20 2020  rs": True})..   
+00001850: 2062 6f6c 6420 3d20 776f 726b 626f 6f6b   bold = workbook
+00001860: 2e61 6464 5f66 6f72 6d61 7428 7b27 626f  .add_format({'bo
+00001870: 6c64 273a 2054 7275 657d 290d 0a20 2020  ld': True})..   
+00001880: 2064 6432 203d 2077 6f72 6b62 6f6f 6b2e   dd2 = workbook.
+00001890: 6164 645f 666f 726d 6174 287b 276e 756d  add_format({'num
+000018a0: 5f66 6f72 6d61 7427 3a20 2730 2e30 3027  _format': '0.00'
+000018b0: 7d29 0d0a 2020 2020 6f6b 666f 726d 6174  })..    okformat
+000018c0: 203d 2077 6f72 6b62 6f6f 6b2e 6164 645f   = workbook.add_
+000018d0: 666f 726d 6174 287b 2762 675f 636f 6c6f  format({'bg_colo
+000018e0: 7227 3a20 6772 6565 6e7d 290d 0a20 2020  r': green})..   
+000018f0: 2077 726f 6e67 666f 726d 6174 203d 2077   wrongformat = w
+00001900: 6f72 6b62 6f6f 6b2e 6164 645f 666f 726d  orkbook.add_form
+00001910: 6174 287b 2762 675f 636f 6c6f 7227 3a20  at({'bg_color': 
+00001920: 7265 647d 290d 0a20 2020 2075 6e66 696c  red})..    unfil
+00001930: 6c65 6466 6f72 6d61 7420 3d20 776f 726b  ledformat = work
+00001940: 626f 6f6b 2e61 6464 5f66 6f72 6d61 7428  book.add_format(
+00001950: 7b27 6267 5f63 6f6c 6f72 273a 206f 7261  {'bg_color': ora
+00001960: 6e67 657d 290d 0a20 2020 2062 6767 7265  nge})..    bggre
+00001970: 7920 3d20 776f 726b 626f 6f6b 2e61 6464  y = workbook.add
+00001980: 5f66 6f72 6d61 7428 7b27 6267 5f63 6f6c  _format({'bg_col
+00001990: 6f72 273a 2067 7265 797d 290d 0a0d 0a20  or': grey}).... 
+000019a0: 2020 2063 6f6e 6466 6f72 6d61 7431 6120     condformat1a 
+000019b0: 3d20 7b27 7479 7065 273a 2027 6365 6c6c  = {'type': 'cell
+000019c0: 272c 2027 6372 6974 6572 6961 273a 2027  ', 'criteria': '
+000019d0: 6265 7477 6565 6e27 2c0d 0a20 2020 2020  between',..     
+000019e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000019f0: 6d69 6e69 6d75 6d27 3a20 2d32 2c20 276d  minimum': -2, 'm
+00001a00: 6178 696d 756d 273a 2032 2c20 2766 6f72  aximum': 2, 'for
+00001a10: 6d61 7427 3a20 6f6b 666f 726d 6174 7d0d  mat': okformat}.
+00001a20: 0a20 2020 2063 6f6e 6466 6f72 6d61 7431  .    condformat1
+00001a30: 6220 3d20 7b27 7479 7065 273a 2027 6365  b = {'type': 'ce
+00001a40: 6c6c 272c 2027 6372 6974 6572 6961 273a  ll', 'criteria':
+00001a50: 2027 6e6f 7420 6265 7477 6565 6e27 2c0d   'not between',.
+00001a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001a70: 2020 2020 2027 6d69 6e69 6d75 6d27 3a20       'minimum': 
+00001a80: 2d32 2c20 276d 6178 696d 756d 273a 2032  -2, 'maximum': 2
+00001a90: 2c20 2766 6f72 6d61 7427 3a20 7772 6f6e  , 'format': wron
+00001aa0: 6766 6f72 6d61 747d 0d0a 2020 2020 636f  gformat}..    co
+00001ab0: 6e64 666f 726d 6174 3163 203d 207b 2774  ndformat1c = {'t
+00001ac0: 7970 6527 3a20 2763 656c 6c27 2c20 2763  ype': 'cell', 'c
+00001ad0: 7269 7465 7269 6127 3a20 2765 7175 616c  riteria': 'equal
+00001ae0: 2074 6f27 2c0d 0a20 2020 2020 2020 2020   to',..         
+00001af0: 2020 2020 2020 2020 2020 2027 7661 6c75             'valu
+00001b00: 6527 3a20 2722 4e69 6574 2067 6576 756c  e': '"Niet gevul
+00001b10: 6422 272c 2027 666f 726d 6174 273a 2075  d"', 'format': u
+00001b20: 6e66 696c 6c65 6466 6f72 6d61 747d 0d0a  nfilledformat}..
+00001b30: 2020 2020 636f 6e64 666f 726d 6174 3261      condformat2a
+00001b40: 203d 207b 2774 7970 6527 3a20 2766 6f72   = {'type': 'for
+00001b50: 6d75 6c61 272c 0d0a 2020 2020 2020 2020  mula',..        
+00001b60: 2020 2020 2020 2020 2020 2020 2763 7269              'cri
+00001b70: 7465 7269 6127 3a20 273d 2442 2438 3c3e  teria': '=$B$8<>
+00001b80: 3027 2c20 2766 6f72 6d61 7427 3a20 7772  0', 'format': wr
+00001b90: 6f6e 6766 6f72 6d61 747d 0d0a 2020 2020  ongformat}..    
+00001ba0: 636f 6e64 666f 726d 6174 3262 203d 207b  condformat2b = {
+00001bb0: 2774 7970 6527 3a20 2766 6f72 6d75 6c61  'type': 'formula
+00001bc0: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00001bd0: 2020 2020 2020 2020 2763 7269 7465 7269          'criteri
+00001be0: 6127 3a20 273d 2442 2438 3d30 272c 2027  a': '=$B$8=0', '
+00001bf0: 666f 726d 6174 273a 206f 6b66 6f72 6d61  format': okforma
+00001c00: 747d 0d0a 2020 2020 636f 6e64 666f 726d  t}..    condform
+00001c10: 6174 3263 203d 207b 2774 7970 6527 3a20  at2c = {'type': 
+00001c20: 2763 656c 6c27 2c20 2763 7269 7465 7269  'cell', 'criteri
+00001c30: 6127 3a20 2765 7175 616c 2074 6f27 2c0d  a': 'equal to',.
+00001c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c50: 2020 2020 2027 7661 6c75 6527 3a20 2722       'value': '"
+00001c60: 4e69 6574 2067 6576 756c 6422 272c 2027  Niet gevuld"', '
+00001c70: 666f 726d 6174 273a 2075 6e66 696c 6c65  format': unfille
+00001c80: 6466 6f72 6d61 747d 0d0a 0d0a 2020 2020  dformat}....    
+00001c90: 776f 726b 7368 6565 7431 203d 2077 6f72  worksheet1 = wor
+00001ca0: 6b62 6f6f 6b2e 6164 645f 776f 726b 7368  kbook.add_worksh
+00001cb0: 6565 7428 2755 6974 6b6f 6d73 7465 6e74  eet('Uitkomstent
+00001cc0: 6162 656c 2729 0d0a 2020 2020 776f 726b  abel')..    work
+00001cd0: 7368 6565 7432 203d 2077 6f72 6b62 6f6f  sheet2 = workboo
+00001ce0: 6b2e 6164 645f 776f 726b 7368 6565 7428  k.add_worksheet(
+00001cf0: 275a 4e57 2026 2057 5727 290d 0a20 2020  'ZNW & WW')..   
+00001d00: 2077 6f72 6b73 6865 6574 3320 3d20 776f   worksheet3 = wo
+00001d10: 726b 626f 6f6b 2e61 6464 5f77 6f72 6b73  rkbook.add_works
+00001d20: 6865 6574 2827 5569 7469 6e67 656e 2729  heet('Uitingen')
+00001d30: 0d0a 2020 2020 776f 726b 7368 6565 7434  ..    worksheet4
+00001d40: 203d 2077 6f72 6b62 6f6f 6b2e 6164 645f   = workbook.add_
+00001d50: 776f 726b 7368 6565 7428 2754 6162 656c  worksheet('Tabel
+00001d60: 2729 0d0a 0d0a 2020 2020 2320 776f 726b  ')....    # work
+00001d70: 7368 6565 7431 0d0a 2020 2020 776f 726b  sheet1..    work
+00001d80: 7368 6565 7431 2e73 6574 5f63 6f6c 756d  sheet1.set_colum
+00001d90: 6e28 302c 2030 2c20 3330 290d 0a20 2020  n(0, 0, 30)..   
+00001da0: 2077 6f72 6b73 6865 6574 312e 7365 745f   worksheet1.set_
+00001db0: 636f 6c75 6d6e 2831 2c20 322c 2031 3229  column(1, 2, 12)
+00001dc0: 0d0a 2020 2020 776f 726b 7368 6565 7431  ..    worksheet1
+00001dd0: 2e68 6964 655f 6772 6964 6c69 6e65 7328  .hide_gridlines(
+00001de0: 6f70 7469 6f6e 3d32 290d 0a20 2020 2077  option=2)..    w
+00001df0: 6f72 6b73 6865 6574 312e 636f 6e64 6974  orksheet1.condit
+00001e00: 696f 6e61 6c5f 666f 726d 6174 2827 2443  ional_format('$C
+00001e10: 2432 3a24 4324 3727 2c20 636f 6e64 666f  $2:$C$7', condfo
+00001e20: 726d 6174 3161 290d 0a20 2020 2077 6f72  rmat1a)..    wor
+00001e30: 6b73 6865 6574 312e 636f 6e64 6974 696f  ksheet1.conditio
+00001e40: 6e61 6c5f 666f 726d 6174 2827 2443 2432  nal_format('$C$2
+00001e50: 3a24 4324 3727 2c20 636f 6e64 666f 726d  :$C$7', condform
+00001e60: 6174 3162 290d 0a20 2020 2077 6f72 6b73  at1b)..    works
+00001e70: 6865 6574 312e 636f 6e64 6974 696f 6e61  heet1.conditiona
+00001e80: 6c5f 666f 726d 6174 2827 2443 2432 3a24  l_format('$C$2:$
+00001e90: 4324 3727 2c20 636f 6e64 666f 726d 6174  C$7', condformat
+00001ea0: 3163 290d 0a20 2020 2077 6f72 6b73 6865  1c)..    workshe
+00001eb0: 6574 312e 636f 6e64 6974 696f 6e61 6c5f  et1.conditional_
+00001ec0: 666f 726d 6174 2827 2443 2439 272c 2063  format('$C$9', c
+00001ed0: 6f6e 6466 6f72 6d61 7431 6129 0d0a 2020  ondformat1a)..  
+00001ee0: 2020 776f 726b 7368 6565 7431 2e63 6f6e    worksheet1.con
+00001ef0: 6469 7469 6f6e 616c 5f66 6f72 6d61 7428  ditional_format(
+00001f00: 2724 4324 3927 2c20 636f 6e64 666f 726d  '$C$9', condform
+00001f10: 6174 3162 290d 0a20 2020 2077 6f72 6b73  at1b)..    works
+00001f20: 6865 6574 312e 636f 6e64 6974 696f 6e61  heet1.conditiona
+00001f30: 6c5f 666f 726d 6174 2827 2443 2439 272c  l_format('$C$9',
+00001f40: 2063 6f6e 6466 6f72 6d61 7431 6329 0d0a   condformat1c)..
+00001f50: 2020 2020 776f 726b 7368 6565 7431 2e63      worksheet1.c
+00001f60: 6f6e 6469 7469 6f6e 616c 5f66 6f72 6d61  onditional_forma
+00001f70: 7428 2724 4324 3130 3a24 4324 3133 272c  t('$C$10:$C$13',
+00001f80: 2063 6f6e 6466 6f72 6d61 7431 6129 0d0a   condformat1a)..
+00001f90: 2020 2020 776f 726b 7368 6565 7431 2e63      worksheet1.c
+00001fa0: 6f6e 6469 7469 6f6e 616c 5f66 6f72 6d61  onditional_forma
+00001fb0: 7428 2724 4324 3130 3a24 4324 3133 272c  t('$C$10:$C$13',
+00001fc0: 2063 6f6e 6466 6f72 6d61 7431 6229 0d0a   condformat1b)..
+00001fd0: 2020 2020 776f 726b 7368 6565 7431 2e63      worksheet1.c
+00001fe0: 6f6e 6469 7469 6f6e 616c 5f66 6f72 6d61  onditional_forma
+00001ff0: 7428 2724 4324 3130 3a24 4324 3133 272c  t('$C$10:$C$13',
+00002000: 2063 6f6e 6466 6f72 6d61 7431 6329 0d0a   condformat1c)..
+00002010: 2020 2020 776f 726b 7368 6565 7431 2e63      worksheet1.c
+00002020: 6f6e 6469 7469 6f6e 616c 5f66 6f72 6d61  onditional_forma
+00002030: 7428 2724 4324 3827 2c20 636f 6e64 666f  t('$C$8', condfo
+00002040: 726d 6174 3261 290d 0a20 2020 2077 6f72  rmat2a)..    wor
+00002050: 6b73 6865 6574 312e 636f 6e64 6974 696f  ksheet1.conditio
+00002060: 6e61 6c5f 666f 726d 6174 2827 2443 2438  nal_format('$C$8
+00002070: 272c 2063 6f6e 6466 6f72 6d61 7432 6229  ', condformat2b)
+00002080: 0d0a 2020 2020 776f 726b 7368 6565 7431  ..    worksheet1
+00002090: 2e63 6f6e 6469 7469 6f6e 616c 5f66 6f72  .conditional_for
+000020a0: 6d61 7428 2724 4324 3827 2c20 636f 6e64  mat('$C$8', cond
+000020b0: 666f 726d 6174 3263 290d 0a0d 0a20 2020  format2c)....   
+000020c0: 2077 7269 7465 7461 626c 6528 7468 6566   writetable(thef
+000020d0: 6f72 6d2e 7363 6f72 6573 2c20 776f 726b  orm.scores, work
+000020e0: 7368 6565 7431 2c20 7268 666f 726d 6174  sheet1, rhformat
+000020f0: 3d62 6f6c 642c 0d0a 2020 2020 2020 2020  =bold,..        
+00002100: 2020 2020 2020 2063 6866 6f72 6d61 743d         chformat=
+00002110: 626f 6c64 2c20 6365 6c6c 666f 726d 6174  bold, cellformat
+00002120: 3d64 6432 290d 0a20 2020 2077 6f72 6b73  =dd2)..    works
+00002130: 6865 6574 312e 7772 6974 6528 2724 4224  heet1.write('$B$
+00002140: 3627 2c20 2727 2c20 6267 6772 6579 290d  6', '', bggrey).
+00002150: 0a20 2020 2077 6f72 6b73 6865 6574 312e  .    worksheet1.
+00002160: 7772 6974 6528 2724 4224 3727 2c20 2727  write('$B$7', ''
+00002170: 2c20 6267 6772 6579 290d 0a20 2020 2077  , bggrey)..    w
+00002180: 6f72 6b73 6865 6574 312e 7772 6974 6528  orksheet1.write(
+00002190: 2724 4224 3827 2c20 2727 2c20 6267 6772  '$B$8', '', bggr
+000021a0: 6579 290d 0a20 2020 2077 6f72 6b73 6865  ey)..    workshe
+000021b0: 6574 312e 7772 6974 6528 2724 4224 3927  et1.write('$B$9'
+000021c0: 2c20 2727 2c20 6267 6772 6579 290d 0a0d  , '', bggrey)...
+000021d0: 0a20 2020 2066 6f72 2028 6c6f 632c 2063  .    for (loc, c
+000021e0: 6f75 6e74 2920 696e 2061 7374 6164 6174  ount) in astadat
+000021f0: 612e 7661 7264 6963 742e 6974 656d 7328  a.vardict.items(
+00002200: 293a 0d0a 2020 2020 2020 2020 776f 726b  ):..        work
+00002210: 7368 6565 7431 2e77 7269 7465 286c 6f63  sheet1.write(loc
+00002220: 2c20 636f 756e 7429 0d0a 0d0a 2020 2020  , count)....    
+00002230: 2320 776f 726b 7368 6565 7432 0d0a 2020  # worksheet2..  
+00002240: 2020 7772 6974 6574 6162 6c65 2873 6865    writetable(she
+00002250: 6574 3268 6964 6465 6e72 6f77 732c 2077  et2hiddenrows, w
+00002260: 6f72 6b73 6865 6574 3229 0d0a 0d0a 2020  orksheet2)....  
+00002270: 2020 636f 6c63 7472 203d 2030 0d0a 2020    colctr = 0..  
+00002280: 2020 666f 7220 2865 6c2c 2077 2920 696e    for (el, w) in
+00002290: 207a 6970 2873 6865 6574 3268 6561 6465   zip(sheet2heade
+000022a0: 722c 2073 6865 6574 3263 6f6c 7769 6474  r, sheet2colwidt
+000022b0: 6873 293a 0d0a 2020 2020 2020 2020 776f  hs):..        wo
+000022c0: 726b 7368 6565 7432 2e77 7269 7465 2834  rksheet2.write(4
+000022d0: 2c20 636f 6c63 7472 2c20 656c 2c20 626f  , colctr, el, bo
+000022e0: 6c64 290d 0a20 2020 2020 2020 2077 6f72  ld)..        wor
+000022f0: 6b73 6865 6574 322e 7365 745f 636f 6c75  ksheet2.set_colu
+00002300: 6d6e 2863 6f6c 6374 722c 2063 6f6c 6374  mn(colctr, colct
+00002310: 722c 2077 290d 0a20 2020 2020 2020 2063  r, w)..        c
+00002320: 6f6c 6374 7220 2b3d 2031 0d0a 0d0a 2020  olctr += 1....  
+00002330: 2020 726f 7763 7472 203d 2035 0d0a 2020    rowctr = 5..  
+00002340: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00002350: 2831 3030 293a 0d0a 2020 2020 2020 2020  (100):..        
+00002360: 776f 726b 7368 6565 7432 2e77 7269 7465  worksheet2.write
+00002370: 2872 6f77 6374 722c 2030 2c20 6920 2b20  (rowctr, 0, i + 
+00002380: 3129 0d0a 2020 2020 2020 2020 726f 7763  1)..        rowc
+00002390: 7472 202b 3d20 310d 0a0d 0a20 2020 2072  tr += 1....    r
+000023a0: 6f77 6374 7220 3d20 350d 0a20 2020 2077  owctr = 5..    w
+000023b0: 636f 6c20 3d20 310d 0a20 2020 2066 7265  col = 1..    fre
+000023c0: 7163 6f6c 203d 2033 0d0a 2020 2020 666f  qcol = 3..    fo
+000023d0: 7220 2877 2c20 636e 7429 2069 6e20 6173  r (w, cnt) in as
+000023e0: 7461 6461 7461 2e6e 6f75 6e64 6963 742e  tadata.noundict.
+000023f0: 6974 656d 7328 293a 0d0a 2020 2020 2020  items():..      
+00002400: 2020 776f 726b 7368 6565 7432 2e77 7269    worksheet2.wri
+00002410: 7465 2872 6f77 6374 722c 2077 636f 6c2c  te(rowctr, wcol,
+00002420: 2077 290d 0a20 2020 2020 2020 2077 6f72   w)..        wor
+00002430: 6b73 6865 6574 322e 7772 6974 6528 726f  ksheet2.write(ro
+00002440: 7763 7472 2c20 6672 6571 636f 6c2c 2063  wctr, freqcol, c
+00002450: 6e74 290d 0a20 2020 2020 2020 2072 6f77  nt)..        row
+00002460: 6374 7220 2b3d 2031 0d0a 0d0a 2020 2020  ctr += 1....    
+00002470: 726f 7763 7472 203d 2035 0d0a 2020 2020  rowctr = 5..    
+00002480: 7763 6f6c 203d 2035 0d0a 2020 2020 6672  wcol = 5..    fr
+00002490: 6571 636f 6c20 3d20 370d 0a20 2020 2066  eqcol = 7..    f
+000024a0: 6f72 2028 772c 2063 6e74 2920 696e 2061  or (w, cnt) in a
+000024b0: 7374 6164 6174 612e 7665 7262 6469 6374  stadata.verbdict
+000024c0: 2e69 7465 6d73 2829 3a0d 0a20 2020 2020  .items():..     
+000024d0: 2020 2077 6f72 6b73 6865 6574 322e 7772     worksheet2.wr
+000024e0: 6974 6528 726f 7763 7472 2c20 7763 6f6c  ite(rowctr, wcol
+000024f0: 2c20 7729 0d0a 2020 2020 2020 2020 776f  , w)..        wo
+00002500: 726b 7368 6565 7432 2e77 7269 7465 2872  rksheet2.write(r
+00002510: 6f77 6374 722c 2066 7265 7163 6f6c 2c20  owctr, freqcol, 
+00002520: 636e 7429 0d0a 2020 2020 2020 2020 726f  cnt)..        ro
+00002530: 7763 7472 202b 3d20 310d 0a0d 0a20 2020  wctr += 1....   
+00002540: 2066 6f72 2072 6f77 6374 7220 696e 2072   for rowctr in r
+00002550: 616e 6765 2834 293a 0d0a 2020 2020 2020  ange(4):..      
+00002560: 2020 776f 726b 7368 6565 7432 2e73 6574    worksheet2.set
+00002570: 5f72 6f77 2872 6f77 6374 722c 204e 6f6e  _row(rowctr, Non
+00002580: 652c 204e 6f6e 652c 207b 2768 6964 6465  e, None, {'hidde
+00002590: 6e27 3a20 5472 7565 7d29 0d0a 0d0a 2020  n': True})....  
+000025a0: 2020 2320 776f 726b 6173 6865 6574 330d    # workasheet3.
+000025b0: 0a20 2020 2077 7269 7465 7461 626c 6528  .    writetable(
+000025c0: 7368 6565 7433 6869 6464 656e 726f 7773  sheet3hiddenrows
+000025d0: 2c20 776f 726b 7368 6565 7433 290d 0a0d  , worksheet3)...
+000025e0: 0a20 2020 2063 6f6c 6374 7220 3d20 300d  .    colctr = 0.
+000025f0: 0a20 2020 2066 6f72 2065 6c20 696e 2073  .    for el in s
+00002600: 6865 6574 3368 6561 6465 723a 0d0a 2020  heet3header:..  
+00002610: 2020 2020 2020 776f 726b 7368 6565 7433        worksheet3
+00002620: 2e77 7269 7465 2834 2c20 636f 6c63 7472  .write(4, colctr
+00002630: 2c20 656c 2c20 626f 6c64 290d 0a20 2020  , el, bold)..   
+00002640: 2020 2020 2063 6f6c 6374 7220 2b3d 2031       colctr += 1
+00002650: 0d0a 2020 2020 776f 726b 7368 6565 7433  ..    worksheet3
+00002660: 2e73 6574 5f63 6f6c 756d 6e28 302c 2063  .set_column(0, c
+00002670: 6f6c 6374 722c 2032 3029 0d0a 0d0a 2020  olctr, 20)....  
+00002680: 2020 726f 7763 7472 203d 2035 0d0a 2020    rowctr = 5..  
+00002690: 2020 7772 6974 6574 6162 6c65 2861 7374    writetable(ast
+000026a0: 6164 6174 612e 7574 746c 6973 742c 2077  adata.uttlist, w
+000026b0: 6f72 6b73 6865 6574 332c 2073 7461 7274  orksheet3, start
+000026c0: 726f 773d 726f 7763 7472 290d 0a0d 0a20  row=rowctr).... 
+000026d0: 2020 2066 6f72 2072 6f77 6374 7220 696e     for rowctr in
+000026e0: 2072 616e 6765 2834 293a 0d0a 2020 2020   range(4):..    
+000026f0: 2020 2020 776f 726b 7368 6565 7433 2e73      worksheet3.s
+00002700: 6574 5f72 6f77 2872 6f77 6374 722c 204e  et_row(rowctr, N
+00002710: 6f6e 652c 204e 6f6e 652c 207b 2768 6964  one, None, {'hid
+00002720: 6465 6e27 3a20 5472 7565 7d29 0d0a 0d0a  den': True})....
+00002730: 2020 2020 2320 776f 726b 7368 6565 7434      # worksheet4
+00002740: 0d0a 2020 2020 776f 726b 7368 6565 7434  ..    worksheet4
+00002750: 2e73 6574 5f63 6f6c 756d 6e28 302c 2030  .set_column(0, 0
+00002760: 2c20 3330 290d 0a0d 0a20 2020 2077 7269  , 30)....    wri
+00002770: 7465 7461 626c 6528 7468 6566 6f72 6d2e  tetable(theform.
+00002780: 7461 6265 6c2c 2077 6f72 6b73 6865 6574  tabel, worksheet
+00002790: 342c 2073 7461 7274 726f 773d 312c 2072  4, startrow=1, r
+000027a0: 6866 6f72 6d61 743d 626f 6c64 290d 0a0d  hformat=bold)...
+000027b0: 0a20 2020 2072 6574 7572 6e20 776f 726b  .    return work
+000027c0: 626f 6f6b 2c20 7461 7267 6574 0d0a 0d0a  book, target....
+000027d0: 0d0a 6465 6620 7375 6d63 7472 2863 7472  ..def sumctr(ctr
+000027e0: 293a 0d0a 2020 2020 7265 7375 6c74 203d  ):..    result =
+000027f0: 2073 756d 2863 7472 2e76 616c 7565 7328   sum(ctr.values(
+00002800: 2929 0d0a 2020 2020 7265 7475 726e 2072  ))..    return r
+00002810: 6573 756c 740d 0a0d 0a0d 0a64 6566 2067  esult......def g
+00002820: 6574 7661 7264 6963 7428 616c 6c72 6573  etvardict(allres
+00002830: 756c 7473 293a 0d0a 2020 2020 7365 6d70  ults):..    semp
+00002840: 6172 203d 2027 4236 270d 0a20 2020 2070  ar = 'B6'..    p
+00002850: 686f 6e70 6172 203d 2027 4237 270d 0a20  honpar = 'B7'.. 
+00002860: 2020 206e 656f 203d 2027 4238 270d 0a20     neo = 'B8'.. 
+00002870: 2020 204b 4d20 3d20 2742 3927 0d0a 2020     KM = 'B9'..  
+00002880: 2020 7365 6d70 6172 636f 756e 7420 3d20    semparcount = 
+00002890: 7375 6d63 7472 280d 0a20 2020 2020 2020  sumctr(..       
+000028a0: 2061 6c6c 7265 7375 6c74 732e 636f 7265   allresults.core
+000028b0: 7265 7375 6c74 735b 7365 6d70 6172 7265  results[semparre
+000028c0: 736b 6579 5d29 2069 6620 7365 6d70 6172  skey]) if sempar
+000028d0: 7265 736b 6579 2069 6e20 616c 6c72 6573  reskey in allres
+000028e0: 756c 7473 2e63 6f72 6572 6573 756c 7473  ults.coreresults
+000028f0: 2065 6c73 6520 300d 0a20 2020 2070 686f   else 0..    pho
+00002900: 6e70 6172 636f 756e 7420 3d20 7375 6d63  nparcount = sumc
+00002910: 7472 280d 0a20 2020 2020 2020 2061 6c6c  tr(..        all
+00002920: 7265 7375 6c74 732e 636f 7265 7265 7375  results.coreresu
+00002930: 6c74 735b 666f 6e70 6172 7265 736b 6579  lts[fonparreskey
+00002940: 5d29 2069 6620 666f 6e70 6172 7265 736b  ]) if fonparresk
+00002950: 6579 2069 6e20 616c 6c72 6573 756c 7473  ey in allresults
+00002960: 2e63 6f72 6572 6573 756c 7473 2065 6c73  .coreresults els
+00002970: 6520 300d 0a20 2020 206e 656f 636f 756e  e 0..    neocoun
+00002980: 7420 3d20 7375 6d63 7472 280d 0a20 2020  t = sumctr(..   
+00002990: 2020 2020 2061 6c6c 7265 7375 6c74 732e       allresults.
+000029a0: 636f 7265 7265 7375 6c74 735b 6e65 6f72  coreresults[neor
+000029b0: 6573 6b65 795d 2920 6966 206e 656f 7265  eskey]) if neore
+000029c0: 736b 6579 2069 6e20 616c 6c72 6573 756c  skey in allresul
+000029d0: 7473 2e63 6f72 6572 6573 756c 7473 2065  ts.coreresults e
+000029e0: 6c73 6520 300d 0a20 2020 204b 636f 756e  lse 0..    Kcoun
+000029f0: 7420 3d20 7375 6d63 7472 280d 0a20 2020  t = sumctr(..   
+00002a00: 2020 2020 2061 6c6c 7265 7375 6c74 732e       allresults.
+00002a10: 636f 7265 7265 7375 6c74 735b 6b6f 7072  coreresults[kopr
+00002a20: 6573 6b65 795d 2920 6966 206b 6f70 7265  eskey]) if kopre
+00002a30: 736b 6579 2069 6e20 616c 6c72 6573 756c  skey in allresul
+00002a40: 7473 2e63 6f72 6572 6573 756c 7473 2065  ts.coreresults e
+00002a50: 6c73 6520 300d 0a20 2020 204d 636f 756e  lse 0..    Mcoun
+00002a60: 7420 3d20 7375 6d63 7472 280d 0a20 2020  t = sumctr(..   
+00002a70: 2020 2020 2061 6c6c 7265 7375 6c74 732e       allresults.
+00002a80: 636f 7265 7265 7375 6c74 735b 6d6f 6461  coreresults[moda
+00002a90: 6c72 6573 6b65 795d 2920 6966 206d 6f64  lreskey]) if mod
+00002aa0: 616c 7265 736b 6579 2069 6e20 616c 6c72  alreskey in allr
+00002ab0: 6573 756c 7473 2e63 6f72 6572 6573 756c  esults.coreresul
+00002ac0: 7473 2065 6c73 6520 300d 0a20 2020 204b  ts else 0..    K
+00002ad0: 4d63 6f75 6e74 203d 204b 636f 756e 7420  Mcount = Kcount 
+00002ae0: 2b20 4d63 6f75 6e74 0d0a 2020 2020 7265  + Mcount..    re
+00002af0: 7375 6c74 203d 207b 7365 6d70 6172 3a20  sult = {sempar: 
+00002b00: 7365 6d70 6172 636f 756e 742c 2070 686f  semparcount, pho
+00002b10: 6e70 6172 3a20 7068 6f6e 7061 7263 6f75  npar: phonparcou
+00002b20: 6e74 2c0d 0a20 2020 2020 2020 2020 2020  nt,..           
+00002b30: 2020 206e 656f 3a20 6e65 6f63 6f75 6e74     neo: neocount
+00002b40: 2c20 4b4d 3a20 4b4d 636f 756e 747d 0d0a  , KM: KMcount}..
+00002b50: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+00002b60: 740d 0a0d 0a0d 0a64 6566 2075 7064 6174  t......def updat
+00002b70: 6528 7265 7375 6c74 6469 6374 2c20 6374  e(resultdict, ct
+00002b80: 7264 6963 742c 206b 6579 2c20 7072 6f70  rdict, key, prop
+00002b90: 293a 0d0a 2020 2020 6966 206b 6579 2069  ):..    if key i
+00002ba0: 6e20 6374 7264 6963 743a 0d0a 2020 2020  n ctrdict:..    
+00002bb0: 2020 2020 6374 7220 3d20 6374 7264 6963      ctr = ctrdic
+00002bc0: 745b 6b65 795d 0d0a 2020 2020 2020 2020  t[key]..        
+00002bd0: 666f 7220 7574 7469 6420 696e 2063 7472  for uttid in ctr
+00002be0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00002bf0: 6573 756c 7464 6963 745b 7574 7469 645d  esultdict[uttid]
+00002c00: 5b70 726f 705d 203d 2063 7472 5b75 7474  [prop] = ctr[utt
+00002c10: 6964 5d0d 0a0d 0a0d 0a64 6566 2075 7064  id]......def upd
+00002c20: 6174 6577 6974 6863 7472 2872 6573 756c  atewithctr(resul
+00002c30: 7464 6963 742c 2063 7472 2c20 7072 6f70  tdict, ctr, prop
+00002c40: 293a 0d0a 2020 2020 666f 7220 7574 7469  ):..    for utti
+00002c50: 6420 696e 2063 7472 3a0d 0a20 2020 2020  d in ctr:..     
+00002c60: 2020 2072 6573 756c 7464 6963 745b 7574     resultdict[ut
+00002c70: 7469 645d 5b70 726f 705d 203d 2063 7472  tid][prop] = ctr
+00002c80: 5b75 7474 6964 5d0d 0a0d 0a0d 0a64 6566  [uttid]......def
+00002c90: 2069 6e74 6469 6374 6765 7428 6463 742c   intdictget(dct,
+00002ca0: 206b 6579 6e61 6d65 293a 0d0a 2020 2020   keyname):..    
+00002cb0: 7231 203d 2064 6963 7467 6574 2864 6374  r1 = dictget(dct
+00002cc0: 2c20 6b65 796e 616d 6529 0d0a 2020 2020  , keyname)..    
+00002cd0: 6966 2072 3120 3d3d 2027 273a 0d0a 2020  if r1 == '':..  
+00002ce0: 2020 2020 2020 7265 7375 6c74 203d 2030        result = 0
+00002cf0: 0d0a 2020 2020 656c 7365 3a0d 0a20 2020  ..    else:..   
+00002d00: 2020 2020 2072 6573 756c 7420 3d20 696e       result = in
+00002d10: 7428 7231 290d 0a20 2020 2072 6574 7572  t(r1)..    retur
+00002d20: 6e20 7265 7375 6c74 0d0a 0d0a 0d0a 6465  n result......de
+00002d30: 6620 6469 6374 6765 7428 6463 742c 206b  f dictget(dct, k
+00002d40: 6579 6e61 6d65 293a 0d0a 2020 2020 6966  eyname):..    if
+00002d50: 206b 6579 6e61 6d65 2069 6e20 6463 743a   keyname in dct:
+00002d60: 0d0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00002d70: 203d 2064 6374 5b6b 6579 6e61 6d65 5d0d   = dct[keyname].
+00002d80: 0a20 2020 2065 6c73 653a 0d0a 2020 2020  .    else:..    
+00002d90: 2020 2020 7265 7375 6c74 203d 2027 270d      result = ''.
+00002da0: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
+00002db0: 6c74 0d0a 0d0a 0d0a 6465 6620 7265 7375  lt......def resu
+00002dc0: 6c74 6469 6374 3274 6162 6c65 2872 6573  ltdict2table(res
+00002dd0: 756c 7464 6963 7429 3a0d 0a20 2020 2074  ultdict):..    t
+00002de0: 6162 6c65 203d 205b 5d0d 0a20 2020 2066  able = []..    f
+00002df0: 6f72 2075 7474 6964 2069 6e20 7265 7375  or uttid in resu
+00002e00: 6c74 6469 6374 3a0d 0a20 2020 2020 2020  ltdict:..       
+00002e10: 2075 7474 6964 5f64 6963 7420 3d20 7265   uttid_dict = re
+00002e20: 7375 6c74 6469 6374 5b75 7474 6964 5d0d  sultdict[uttid].
+00002e30: 0a20 2020 2020 2020 2077 6320 3d20 6469  .        wc = di
+00002e40: 6374 6765 7428 7574 7469 645f 6469 6374  ctget(uttid_dict
+00002e50: 2c20 2777 6327 290d 0a20 2020 2020 2020  , 'wc')..       
+00002e60: 2063 6f72 7265 6374 203d 2064 6963 7467   correct = dictg
+00002e70: 6574 2875 7474 6964 5f64 6963 742c 2027  et(uttid_dict, '
+00002e80: 636f 7272 6563 7427 290d 0a20 2020 2020  correct')..     
+00002e90: 2020 2069 6620 636f 7272 6563 7420 213d     if correct !=
+00002ea0: 2027 273a 0d0a 2020 2020 2020 2020 2020   '':..          
+00002eb0: 2020 636f 7272 6563 7420 3d20 274a 270d    correct = 'J'.
+00002ec0: 0a20 2020 2020 2020 2061 6c6c 7076 7320  .        allpvs 
+00002ed0: 3d20 696e 7464 6963 7467 6574 2875 7474  = intdictget(utt
+00002ee0: 6964 5f64 6963 742c 2027 616c 6c70 7673  id_dict, 'allpvs
+00002ef0: 2729 0d0a 2020 2020 2020 2020 666f 7574  ')..        fout
+00002f00: 6570 7673 203d 2069 6e74 6469 6374 6765  epvs = intdictge
+00002f10: 7428 7574 7469 645f 6469 6374 2c20 2766  t(uttid_dict, 'f
+00002f20: 6f75 7465 7076 7327 290d 0a20 2020 2020  outepvs')..     
+00002f30: 2020 206f 6b70 7673 203d 206d 6178 2830     okpvs = max(0
+00002f40: 2c20 616c 6c70 7673 202d 2066 6f75 7465  , allpvs - foute
+00002f50: 7076 7329 0d0a 2020 2020 2020 2020 6269  pvs)..        bi
+00002f60: 6a7a 696e 636f 756e 7420 3d20 6469 6374  jzincount = dict
+00002f70: 6765 7428 7574 7469 645f 6469 6374 2c20  get(uttid_dict, 
+00002f80: 2762 696a 7a69 6e63 6f75 6e74 2729 0d0a  'bijzincount')..
+00002f90: 2020 2020 2020 2020 7265 6d61 726b 7320          remarks 
+00002fa0: 3d20 6469 6374 6765 7428 7574 7469 645f  = dictget(uttid_
+00002fb0: 6469 6374 2c20 2772 656d 6172 6b73 2729  dict, 'remarks')
+00002fc0: 0d0a 2020 2020 2020 2020 7061 6464 6564  ..        padded
+00002fd0: 7574 7469 6420 3d20 7374 7228 7574 7469  uttid = str(utti
+00002fe0: 6429 2e72 6a75 7374 2833 2c20 2730 2729  d).rjust(3, '0')
+00002ff0: 0d0a 2020 2020 2020 2020 6e65 7772 6f77  ..        newrow
+00003000: 203d 205b 7061 6464 6564 7574 7469 642c   = [paddeduttid,
+00003010: 2077 632c 2063 6f72 7265 6374 2c0d 0a20   wc, correct,.. 
+00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003030: 206f 6b70 7673 2c20 666f 7574 6570 7673   okpvs, foutepvs
+00003040: 2c20 6269 6a7a 696e 636f 756e 742c 2072  , bijzincount, r
+00003050: 656d 6172 6b73 5d0d 0a20 2020 2020 2020  emarks]..       
+00003060: 2074 6162 6c65 2e61 7070 656e 6428 6e65   table.append(ne
+00003070: 7772 6f77 290d 0a20 2020 2073 6f72 7465  wrow)..    sorte
+00003080: 6474 6162 6c65 203d 2073 6f72 7465 6428  dtable = sorted(
+00003090: 7461 626c 652c 206b 6579 3d6c 616d 6264  table, key=lambd
+000030a0: 6120 726f 773a 2072 6f77 5b30 5d29 0d0a  a row: row[0])..
+000030b0: 2020 2020 7265 7475 726e 2073 6f72 7465      return sorte
+000030c0: 6474 6162 6c65 0d0a 0d0a 0d0a 6465 6620  dtable......def 
+000030d0: 6765 7475 7474 6c69 7374 2861 6c6c 7265  getuttlist(allre
+000030e0: 7375 6c74 7329 3a0d 0a20 2020 2072 6573  sults):..    res
+000030f0: 756c 7464 6963 7420 3d20 6465 6661 756c  ultdict = defaul
+00003100: 7464 6963 7428 6c61 6d62 6461 3a20 6465  tdict(lambda: de
+00003110: 6661 756c 7464 6963 7428 696e 7429 290d  faultdict(int)).
+00003120: 0a20 2020 2077 6f72 6463 6f75 6e74 6469  .    wordcountdi
+00003130: 6374 203d 2077 6f72 6463 6f75 6e74 7065  ct = wordcountpe
+00003140: 7275 7474 2861 6c6c 7265 7375 6c74 7329  rutt(allresults)
+00003150: 0d0a 2020 2020 666f 7220 7574 7469 6420  ..    for uttid 
+00003160: 696e 2077 6f72 6463 6f75 6e74 6469 6374  in wordcountdict
+00003170: 3a0d 0a20 2020 2020 2020 2072 6573 756c  :..        resul
+00003180: 7464 6963 745b 7574 7469 645d 5b27 7763  tdict[uttid]['wc
+00003190: 275d 203d 2077 6f72 6463 6f75 6e74 6469  '] = wordcountdi
+000031a0: 6374 5b75 7474 6964 5d0d 0a20 2020 2023  ct[uttid]..    #
+000031b0: 2075 7064 6174 6528 7265 7375 6c74 6469   update(resultdi
+000031c0: 6374 2c20 616c 6c72 6573 756c 7473 2e70  ct, allresults.p
+000031d0: 6f73 7472 6573 756c 7473 2c20 2741 3034  ostresults, 'A04
+000031e0: 3627 2c20 2777 6327 290d 0a20 2020 2075  6', 'wc')..    u
+000031f0: 7064 6174 6528 7265 7375 6c74 6469 6374  pdate(resultdict
+00003200: 2c20 616c 6c72 6573 756c 7473 2e63 6f72  , allresults.cor
+00003210: 6572 6573 756c 7473 2c20 636f 7272 6563  eresults, correc
+00003220: 7472 6573 6b65 792c 2027 636f 7272 6563  treskey, 'correc
+00003230: 7427 290d 0a20 2020 2075 7064 6174 6528  t')..    update(
+00003240: 7265 7375 6c74 6469 6374 2c20 616c 6c72  resultdict, allr
+00003250: 6573 756c 7473 2e63 6f72 6572 6573 756c  esults.coreresul
+00003260: 7473 2c20 7076 7265 736b 6579 2c20 2761  ts, pvreskey, 'a
+00003270: 6c6c 7076 7327 290d 0a20 2020 2073 7562  llpvs')..    sub
+00003280: 7076 7320 3d20 616c 6c72 6573 756c 7473  pvs = allresults
+00003290: 2e63 6f72 6572 6573 756c 7473 5b73 7562  .coreresults[sub
+000032a0: 7076 7265 736b 6579 5d20 6966 2073 7562  pvreskey] if sub
+000032b0: 7076 7265 736b 6579 2069 6e20 616c 6c72  pvreskey in allr
+000032c0: 6573 756c 7473 2e63 6f72 6572 6573 756c  esults.coreresul
+000032d0: 7473 2065 6c73 6520 436f 756e 7465 7228  ts else Counter(
+000032e0: 0d0a 2020 2020 290d 0a20 2020 2064 656c  ..    )..    del
+000032f0: 7076 7320 3d20 616c 6c72 6573 756c 7473  pvs = allresults
+00003300: 2e63 6f72 6572 6573 756c 7473 5b64 656c  .coreresults[del
+00003310: 7076 7265 736b 6579 5d20 6966 2064 656c  pvreskey] if del
+00003320: 7076 7265 736b 6579 2069 6e20 616c 6c72  pvreskey in allr
+00003330: 6573 756c 7473 2e63 6f72 6572 6573 756c  esults.coreresul
+00003340: 7473 2065 6c73 6520 436f 756e 7465 7228  ts else Counter(
+00003350: 0d0a 2020 2020 290d 0a20 2020 2074 696a  ..    )..    tij
+00003360: 6466 6f75 7470 7673 203d 2061 6c6c 7265  dfoutpvs = allre
+00003370: 7375 6c74 732e 636f 7265 7265 7375 6c74  sults.coreresult
+00003380: 735b 7469 6a64 666f 7574 7076 7265 736b  s[tijdfoutpvresk
+00003390: 6579 5d20 6966 2074 696a 6466 6f75 7470  ey] if tijdfoutp
+000033a0: 7672 6573 6b65 7920 696e 2061 6c6c 7265  vreskey in allre
+000033b0: 7375 6c74 732e 636f 7265 7265 7375 6c74  sults.coreresult
+000033c0: 7320 656c 7365 2043 6f75 6e74 6572 280d  s else Counter(.
+000033d0: 0a20 2020 2029 0d0a 2020 2020 666f 7574  .    )..    fout
+000033e0: 6570 7673 203d 2073 7562 7076 7320 2b20  epvs = subpvs + 
+000033f0: 6465 6c70 7673 202b 2074 696a 6466 6f75  delpvs + tijdfou
+00003400: 7470 7673 0d0a 2020 2020 7570 6461 7465  tpvs..    update
+00003410: 7769 7468 6374 7228 7265 7375 6c74 6469  withctr(resultdi
+00003420: 6374 2c20 666f 7574 6570 7673 2c20 2766  ct, foutepvs, 'f
+00003430: 6f75 7465 7076 7327 290d 0a20 2020 2075  outepvs')..    u
+00003440: 7064 6174 6528 7265 7375 6c74 6469 6374  pdate(resultdict
+00003450: 2c20 616c 6c72 6573 756c 7473 2e63 6f72  , allresults.cor
+00003460: 6572 6573 756c 7473 2c20 6269 6a7a 696e  eresults, bijzin
+00003470: 7265 736b 6579 2c20 2762 696a 7a69 6e63  reskey, 'bijzinc
+00003480: 6f75 6e74 2729 0d0a 0d0a 2020 2020 7265  ount')....    re
+00003490: 7375 6c74 203d 2072 6573 756c 7464 6963  sult = resultdic
+000034a0: 7432 7461 626c 6528 7265 7375 6c74 6469  t2table(resultdi
+000034b0: 6374 290d 0a20 2020 2072 6574 7572 6e20  ct)..    return 
+000034c0: 7265 7375 6c74 0d0a 0d0a 0d0a 6465 6620  result......def 
+000034d0: 6173 7461 666f 726d 2861 6c6c 7265 7375  astaform(allresu
+000034e0: 6c74 732c 205f 2c20 696e 5f6d 656d 6f72  lts, _, in_memor
+000034f0: 793d 4661 6c73 6529 3a0d 0a20 2020 206e  y=False):..    n
+00003500: 6f75 6e64 6963 7420 3d20 6465 6661 756c  oundict = defaul
+00003510: 7464 6963 7428 696e 7429 0d0a 2020 2020  tdict(int)..    
+00003520: 7665 7262 6469 6374 203d 2064 6566 6175  verbdict = defau
+00003530: 6c74 6469 6374 2869 6e74 290d 0a20 2020  ltdict(int)..   
+00003540: 2061 6c6c 6d61 7463 6865 7320 3d20 616c   allmatches = al
+00003550: 6c72 6573 756c 7473 2e61 6c6c 6d61 7463  lresults.allmatc
+00003560: 6865 730d 0a20 2020 2023 2066 6f72 2065  hes..    # for e
+00003570: 6c20 696e 2061 6c6c 6d61 7463 6865 733a  l in allmatches:
+00003580: 0d0a 2020 2020 2320 2020 2020 2871 6964  ..    #     (qid
+00003590: 2c20 7574 7469 6429 203d 2065 6c0d 0a20  , uttid) = el.. 
+000035a0: 2020 2023 2020 2020 2069 6620 7169 6420     #     if qid 
+000035b0: 3d3d 2027 4130 3231 273a 0d0a 2020 2020  == 'A021':..    
+000035c0: 2320 2020 2020 2020 2020 666f 7220 616d  #         for am
+000035d0: 6174 6368 2069 6e20 616c 6c6d 6174 6368  atch in allmatch
+000035e0: 6573 5b65 6c5d 3a0d 0a20 2020 2023 2020  es[el]:..    #  
+000035f0: 2020 2020 2020 2020 2020 2023 2074 6865             # the
+00003600: 776f 7264 203d 206e 6f72 6d61 6c69 7a65  word = normalize
+00003610: 6477 6f72 6428 616d 6174 6368 5b30 5d29  dword(amatch[0])
+00003620: 0d0a 2020 2020 2320 2020 2020 2020 2020  ..    #         
+00003630: 2020 2020 7468 6577 6f72 6420 3d20 6765      theword = ge
+00003640: 7461 7474 7661 6c28 616d 6174 6368 5b30  tattval(amatch[0
+00003650: 5d2c 2027 6c65 6d6d 6127 290d 0a20 2020  ], 'lemma')..   
+00003660: 2023 2020 2020 2020 2020 2020 2020 206e   #             n
+00003670: 6f75 6e64 6963 745b 7468 6577 6f72 645d  oundict[theword]
+00003680: 202b 3d20 310d 0a20 2020 2023 2020 2020   += 1..    #    
+00003690: 2069 6620 7169 6420 3d3d 2027 4130 3138   if qid == 'A018
+000036a0: 273a 0d0a 2020 2020 2320 2020 2020 2020  ':..    #       
+000036b0: 2020 666f 7220 616d 6174 6368 2069 6e20    for amatch in 
+000036c0: 616c 6c6d 6174 6368 6573 5b65 6c5d 3a0d  allmatches[el]:.
+000036d0: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
+000036e0: 2020 2023 2074 6865 776f 7264 203d 206e     # theword = n
+000036f0: 6f72 6d61 6c69 7a65 6477 6f72 6428 616d  ormalizedword(am
+00003700: 6174 6368 5b30 5d29 0d0a 2020 2020 2320  atch[0])..    # 
+00003710: 2020 2020 2020 2020 2020 2020 7468 6577              thew
+00003720: 6f72 6420 3d20 6765 7461 7474 7661 6c28  ord = getattval(
+00003730: 616d 6174 6368 5b30 5d2c 2027 6c65 6d6d  amatch[0], 'lemm
+00003740: 6127 290d 0a20 2020 2023 2020 2020 2020  a')..    #      
+00003750: 2020 2020 2020 2076 6572 6264 6963 745b         verbdict[
+00003760: 7468 6577 6f72 645d 202b 3d20 310d 0a20  theword] += 1.. 
+00003770: 2020 206e 6f75 6e64 6963 7420 3d20 6765     noundict = ge
+00003780: 746c 656d 6d61 6672 6571 7328 616c 6c72  tlemmafreqs(allr
+00003790: 6573 756c 7473 2c20 6e6f 756e 7265 736b  esults, nounresk
+000037a0: 6579 290d 0a20 2020 2023 2066 6f72 2028  ey)..    # for (
+000037b0: 6c65 6d6d 612c 2075 7474 6964 2920 696e  lemma, uttid) in
+000037c0: 2061 6c6c 7265 7375 6c74 732e 706f 7374   allresults.post
+000037d0: 7265 7375 6c74 735b 6e6f 756e 6c65 6d6d  results[nounlemm
+000037e0: 6171 6964 5d3a 0d0a 2020 2020 2320 2020  aqid]:..    #   
+000037f0: 206e 6f75 6e64 6963 745b 6c65 6d6d 615d   noundict[lemma]
+00003800: 202b 3d20 310d 0a20 2020 2076 6572 6264   += 1..    verbd
+00003810: 6963 7420 3d20 6765 746c 656d 6d61 6672  ict = getlemmafr
+00003820: 6571 7328 616c 6c72 6573 756c 7473 2c20  eqs(allresults, 
+00003830: 6c65 7872 6573 6b65 7929 0d0a 2020 2020  lexreskey)..    
+00003840: 2320 666f 7220 286c 656d 6d61 2c20 7574  # for (lemma, ut
+00003850: 7469 6429 2069 6e20 616c 6c72 6573 756c  tid) in allresul
+00003860: 7473 2e70 6f73 7472 6573 756c 7473 5b76  ts.postresults[v
+00003870: 6572 626c 656d 6d61 7169 645d 3a0d 0a20  erblemmaqid]:.. 
+00003880: 2020 2023 2020 2020 7665 7262 6469 6374     #    verbdict
+00003890: 5b6c 656d 6d61 5d20 2b3d 2031 0d0a 2020  [lemma] += 1..  
+000038a0: 2020 7661 7264 6963 7420 3d20 6765 7476    vardict = getv
+000038b0: 6172 6469 6374 2861 6c6c 7265 7375 6c74  ardict(allresult
+000038c0: 7329 0d0a 2020 2020 7574 746c 6973 7420  s)..    uttlist 
+000038d0: 3d20 6765 7475 7474 6c69 7374 2861 6c6c  = getuttlist(all
+000038e0: 7265 7375 6c74 7329 0d0a 2020 2020 6173  results)..    as
+000038f0: 7461 6461 7461 203d 2041 7374 6146 6f72  tadata = AstaFor
+00003900: 6d44 6174 6128 6e6f 756e 6469 6374 2c20  mData(noundict, 
+00003910: 7665 7262 6469 6374 2c20 7661 7264 6963  verbdict, vardic
+00003920: 742c 2075 7474 6c69 7374 290d 0a20 2020  t, uttlist)..   
+00003930: 2074 6865 666f 726d 203d 2045 7863 656c   theform = Excel
+00003940: 466f 726d 2874 6162 656c 2c20 7363 6f72  Form(tabel, scor
+00003950: 6573 290d 0a0d 0a20 2020 2069 6620 696e  es)....    if in
+00003960: 5f6d 656d 6f72 793a 0d0a 2020 2020 2020  _memory:..      
+00003970: 2020 7461 7267 6574 203d 2042 7974 6573    target = Bytes
+00003980: 494f 2829 0d0a 2020 2020 656c 7365 3a0d  IO()..    else:.
+00003990: 0a20 2020 2020 2020 2074 6172 6765 7420  .        target 
+000039a0: 3d20 6765 7466 6f72 6d66 696c 656e 616d  = getformfilenam
+000039b0: 6528 616c 6c72 6573 756c 7473 2e66 696c  e(allresults.fil
+000039c0: 656e 616d 652c 2027 5f61 7374 6166 6f72  ename, '_astafor
+000039d0: 6d75 6c69 6572 2729 0d0a 0d0a 2020 2020  mulier')....    
+000039e0: 7468 6577 6f72 6b62 6f6f 6b2c 2074 6172  theworkbook, tar
+000039f0: 6765 7420 3d20 6d61 6b65 5f61 7374 6166  get = make_astaf
+00003a00: 6f72 6d28 7468 6566 6f72 6d2c 2061 7374  orm(theform, ast
+00003a10: 6164 6174 612c 2074 6172 6765 7429 0d0a  adata, target)..
+00003a20: 2020 2020 7468 6577 6f72 6b62 6f6f 6b2e      theworkbook.
+00003a30: 636c 6f73 6528 290d 0a20 2020 2072 6574  close()..    ret
+00003a40: 7572 6e20 7461 7267 6574 0d0a 0d0a 0d0a  urn target......
+00003a50: 6465 6620 6765 746c 656d 6d61 6672 6571  def getlemmafreq
+00003a60: 7328 616c 6c72 6573 756c 7473 2c20 6c65  s(allresults, le
+00003a70: 7869 6361 6c72 6573 6b65 7929 202d 3e20  xicalreskey) -> 
+00003a80: 4469 6374 5b73 7472 2c20 696e 745d 3a0d  Dict[str, int]:.
+00003a90: 0a20 2020 2064 6963 7420 3d20 6465 6661  .    dict = defa
+00003aa0: 756c 7464 6963 7428 696e 7429 0d0a 2020  ultdict(int)..  
+00003ab0: 2020 666f 7220 7265 736b 6579 2069 6e20    for reskey in 
+00003ac0: 616c 6c72 6573 756c 7473 2e65 7861 6374  allresults.exact
+00003ad0: 7265 7375 6c74 733a 0d0a 2020 2020 2020  results:..      
+00003ae0: 2020 7169 6420 3d20 7265 736b 6579 5b30    qid = reskey[0
+00003af0: 5d0d 0a20 2020 2020 2020 2069 6620 7169  ]..        if qi
+00003b00: 6420 3d3d 206c 656d 6d61 7169 643a 0d0a  d == lemmaqid:..
+00003b10: 2020 2020 2020 2020 2020 2020 6c65 6d6d              lemm
+00003b20: 6120 3d20 7265 736b 6579 5b31 5d0d 0a20  a = reskey[1].. 
+00003b30: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
+00003b40: 6f73 6974 696f 6e20 696e 2061 6c6c 7265  osition in allre
+00003b50: 7375 6c74 732e 6578 6163 7472 6573 756c  sults.exactresul
+00003b60: 7473 5b72 6573 6b65 795d 3a0d 0a20 2020  ts[reskey]:..   
+00003b70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00003b80: 706f 7369 7469 6f6e 2069 6e20 616c 6c72  position in allr
+00003b90: 6573 756c 7473 2e65 7861 6374 7265 7375  esults.exactresu
+00003ba0: 6c74 735b 6c65 7869 6361 6c72 6573 6b65  lts[lexicalreske
+00003bb0: 795d 3a0d 0a20 2020 2020 2020 2020 2020  y]:..           
+00003bc0: 2020 2020 2020 2020 2064 6963 745b 6c65           dict[le
+00003bd0: 6d6d 615d 202b 3d20 310d 0a20 2020 2072  mma] += 1..    r
+00003be0: 6574 7572 6e20 6469 6374 0d0a            eturn dict..
```

### Comparing `sastadev-0.1.5/src/sastadev/basicreplacements.py` & `sastadev-0.2.0/src/sastadev/basicreplacements.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,14 +41,24 @@
 redpron = 'reduced pronunciation'
 emphasis = 'emphasis'
 prefixdrop = 'prefix drop'
 voweldup = 'vowel duplication'
 erdrop = 'er drop'
 closedvow = 'closed vowel'
 vzdevoicing = 'v/z devoicing'
+missingapostrophe = apomiss
+finalschwadrop = 'Finals schwa dropped'
+u4schwa = 'u usewd for the schwa sound'
+inithdrop = 'Initial h drop'
+finaldevoicing = 'Final devoicing'
+assimilation = 'Assimilation'
+reduction = 'Reduction'
+intervocalicd2j = 'Intervocalic d -> j'
+dial = 'Dialectical variation'
+vowellaxing = 'Vowel laxing'
 
 #: The constant *Rvzlist* contains a list of adpositions that can combine with *er* into
 #: a so-called pronominal adverb. Example: *van*, since *er* + * van* = *ervan*.
 #:
 Rvzlist = ['aan', 'achter', 'achteraan', 'achterin', 'achterop', 'af', 'beneden', 'benevens', 'bij', 'binnen',
            'binnenuit', 'boven', 'bovenaan', 'bovenin', 'bovenop', 'buiten', 'dichtbij', 'door', 'doorheen', 'heen',
            'in', 'langs', 'langsheen', 'langszij', 'mede', 'mee', 'middendoor', 'na', 'naar', 'naartoe', 'naast',
@@ -82,14 +92,19 @@
                     ('vanne', 'van', pron, wrongpron, emphasis, dp3),
                     ]
 #: The constant *innureplacements* is derived from the constant *innereplacements* by replacing the final *e* of the
 #: first word in each tuple by an *u*.
 #:
 innureplacements = [(w1[:-1] + 'u', w2, c, n, v, p) for (w1, w2, c, n, v, p) in innereplacements]
 
+#@@to add@:zn, dr. wa, tie, mn, zun, dur, se, dese, naartoe, maa(r), isda -> is dat, wi(l), goe(d), datte shwa+n. sij,
+# dez, eeft, 'savonds, tisda ('t is dat), jamaar, jahoor, oeveel, geten-> gegeten/ vergeten,
+# tzelfde-> hetelfde, neehoor, elemaal, annere -> andere, zteen -> zometeen, hunnie-> hun, hep -> heb, oera -> hoera,
+# rijje
+
 #: The constant *basicreplacementlist* contains 6-tuples of strings with:
 #:
 #: * frequent deviant spelling of a word, usually to indicate how the word was (incorrectly) pronounced. together with (e.g. "as", "effe")
 #: * the correct spelling of the word ("als", "even")
 #: * linguistic level (e.g Pronunciation, Orthography)
 #: * characterisation of the deviancy, e.g. "Informal Pronunciation", "Wrong Pronunciation"
 #: * details about the deviation, e.g. "Coda Reduction", "Initial Devoicing"
@@ -126,49 +141,91 @@
                                                 ('il', 'wil', pron, pronerr, onsetred, dp),
                                                 ('tee', 'twee', pron, pronerr, onsetred, dp),
                                                 ('nie', 'niet', pron, infpron, codared, dp),
                                                 ('s', 'is', orth, spellerr, apomiss, dp),
                                                 ('ooke', 'ook', pron, infpron, addschwa, dp),
                                                 ('it', 'dit', pron, pronerr, onsetred, dp),
                                                 ('da', 'dat', pron, infpron, codared, dp),
+                                                ('wa', 'wat', pron, infpron, codared, dp),
                                                 ('si', 'zit', pron, infpron, codared, dp),  # and zdev
                                                 ('ieduleen', 'iedereen', pron, wrongpron, phonrepl.format(wrong='l', correct='r'), dp),
                                                 ('allemaaw', 'allemaal', pron, wrongpron, phonrepl.format(wrong='w', correct='l'), dp),
                                                 ('amaal', 'allemaal', pron, infpron, varpron, dp),
                                                 ('wiw', 'wil', pron, wrongpron, phonrepl.format(wrong='w', correct='l'), dp),
                                                 ('annug', 'ander', pron, wrongpron, phonrepl.format(wrong='nug', correct='der'), dp),
                                                 ('nohug', 'nodig', pron, wrongpron, phonrepl.format(wrong='hu', correct='di'), dp),
-                                                ('magge', 'mogen', morph, wronginfl, '{} & {}'.format(overgen, infpron), dp),
+                                                ('magge', 'mogen', morph, wronginfl, '{} & {}'.format(overgen, infpron), dp-5),
+                                                ('magge', 'mag', pron, infpron, emphasis, dp),
                                                 ('maggen', 'mogen', morph, wronginfl, overgen, dp),
-                                                ('aleen', 'alleen', orth, typo, typorepl.format(wrong='alleen', correct='alleen'), dp),
+                                                ('aleen', 'alleen', orth, typo, typorepl.format(wrong='aleen', correct='alleen'), dp),
                                                 ('heef', 'heeft', pron, infpron, codared, dp),
                                                 ('saan', 'staan', pron, wrongpron, onsetred, dp),
                                                 ('saan', 'gaan', pron, wrongpron, wrongpron, dp + 2),
                                                 ('jerke', 'werken', pron, wrongpron, wrongpron, dp),
                                                 ('taan', 'staan', pron, wrongpron, onsetred, dp),
                                                 ("a'maal", 'allemaal', pron, infpron, redpron, dp),
                                                 ('taan', 'staan', pron, wrongpron, onsetred, dp),
                                                 ('beurt', 'gebeurt', pron, wrongpron, prefixdrop, dp),
                                                 ('dahaar', 'daar', pron, emphasis, voweldup, dp),
                                                 ('desu', 'deze', pron, infpron, vzdevoicing, dp),
                                                 ('tan', 'dan', pron, infpron, initdev, dp),
                                                 ('tat', 'dat', pron, infpron, initdev, dp),
                                                 ('tit', 'dit', pron, infpron, initdev, dp),
+                                                ('tie', 'ie', pron, infpron, initdev, dp),
                                                 ('lape', 'slapen', pron, infpron, f'{onsetred}+{fndrop}', dp),
                                                 ('vas', 'vast', pron, infpron, codared, dp),
                                                 ('datte', 'dat', pron, infpron, emphasis, dp),
-                                                ('omdatte', 'dat', pron, infpron, emphasis, dp),
-                                                ('cirtus', 'circus', pron, wrongpron, typorepl.format(wrong='t', correct='c'), dp)
-
+                                                ('omdatte', 'omdat', pron, infpron, emphasis, dp),
+                                                ('ditte', 'dit', pron, infpron, emphasis, dp),
+                                                ('datte', 'dat', pron, infpron, emphasis, dp),
+                                                ('disse', 'deze', pron, infpron, emphasis, dp),
+                                                ('deez', 'deze', pron, infpron, finalschwadrop, dp),
+                                                ('dez', 'deze', pron, infpron, finalschwadrop, dp),
+                                                ('dees', 'deze', pron, infpron, finalschwadrop, dp),
+                                                ('dese', 'deze', pron, infpron, vzdevoicing, dp),
+                                                ('hunnie', "hun", pron, infpron, emphasis, dp),
+                                                ('mn', "m'n", pron, infpron, missingapostrophe, dp),
+                                                ('zn', "z'n", pron, infpron, missingapostrophe, dp),
+                                                ('dr', "d'r", pron, infpron, missingapostrophe, dp),
+                                                ('zun', "z'n", pron, infpron, u4schwa , dp),
+                                                ('dur', "d'r", pron, infpron, u4schwa, dp),
+                                                ('se', "z'n", pron, infpron, initdev, dp),
+                                                ('maa', 'maar', pron, infpron, codared, dp),
+                                                ('wi', 'wil', pron, infpron, codared, dp),
+                                                ('sij', 'zijn', pron, infpron, f'{codared}/{initdev}', dp),
+                                                ('eeft', 'heeft', pron, infpron, inithdrop, dp),
+                                                ('oeveel', 'hoeveel', pron, infpron, inithdrop, dp),
+                                                ('elemaal', 'helemaal', pron, infpron, inithdrop, dp),
+                                                ('oera', 'hoera', pron, infpron, inithdrop, dp),
+                                                ('tzelfde', 'hetzelfde', pron, infpron, typo, dp),
+                                                ('hep', 'heb', pron, infpron, finaldevoicing, dp),
+                                                ('annere', 'andere', pron, infpron, assimilation, dp),
+                                                ('zteen', 'zometeen', pron, infpron, reduction, dp),
+                                                ('rijje', 'rijden', pron, infpron, intervocalicd2j, dp),
+                                                ('rije', 'rijden', pron, infpron, intervocalicd2j, dp),
+                                                ('naartoe', 'ernaartoe', pron, infpron, erdrop, dp),
+                                                ('goe', 'goed', pron, infpron, codared, dp),
+                                                ('geten', 'gegeten', morph, infpron, prefixdrop, dp),
+                                                ('geten', 'vergeten', morph, infpron, prefixdrop, dp + 2),
+                                                ('cirtus', 'circus', pron, wrongpron, typorepl.format(wrong='t', correct='c'), dp),
+                                                ('ken', 'kan', pron, infpron, dial, dp),
+                                                ('an', 'aan', pron, infpron, vowellaxing, dp),
+                                                ('an', 'kan', pron, infpron, onsetred, dp),
+                                                ('hoeve', 'hoef', pron, infpron, emphasis, dp),
+                                                ('hoeve', 'hoeft', pron, infpron, emphasis, dp+2),
+                                                ('hebbe', 'heb', pron, infpron, emphasis, dp+2),
+                                                ('kane', 'andere', pron, wrongpron, wrongpron, dp)
                                                 ] + \
     ervzvariants + \
     innereplacements + \
     innureplacements
 
 
+
+
 #: The dictionary *basicreplacements* maps a word with deviant orthography to a list of
 #: 5-tuples containing the correct orthography, 3 strings to encode metadata, and an integer for the associated penalty. The
 #: dictionary is derived from the constant *basicreplacementlist*
 #:
 #: .. autodata:: basicreplacements::basicreplacementlist
 #:       :no-value:
 #:
@@ -219,24 +276,35 @@
 #:
 #: * the constant *innuclosesyllshortprepexpansions*:
 #:   * .. autodata:: basicreplacements::innuclosesyllshortprepexpansions
 #:
 basicexpansionlist: List[BasicExpansion] = \
     [('dis', ['dit', 'is'], pron, infpron, contract, dp),
      ('das', ['dat', 'is'], pron, infpron, contract, dp),
+     ("di's", ['dit' 'is'], pron, infpron, contract, dp),
+     ("da's", ['dat' 'is'], pron, infpron, contract, dp),
      ('tis', ['dit', 'is'], pron, infpron, contract, dp),
      ('waas', ['waar', 'is'], pron, infpron, contract, dp),
      ('is-t-ie', ['is', 'ie'], pron, infpron, t_ie, dp),
      ('als-t-ie', ['als', 'ie'], pron, infpron, t_ie, dp),
      ('of-t-ie', ['of', 'ie'], pron, infpron, t_ie, dp),
      ('as-t-ie', ['als', 'ie'], pron, infpron, t_ie, dp),
      ("dit's", ["dit", "is"], pron, infpron, contract, dp),
      ("dat's", ["dat", "is"], pron, infpron, contract, dp),
      ("datte", ['dat', 'ie'], pron, infpron, contract, dp + 2),
-     ("omdatte", ['omdat', 'ie'], pron, infpron, contract, dp + 2)
+     ("omdatte", ['omdat', 'ie'], pron, infpron, contract, dp + 2),
+     ("isda", ['is', 'dat'], pron, infpron, contract, dp + 2),
+     ("tisda", ['het',  'is', 'dat'], pron, infpron, contract, dp + 2),
+     ("'savonds", ["'s", 'avonds'], pron, infpron, typo, dp + 2),
+     ("savonds", ["'s", 'avonds'], pron, infpron, typo, dp + 2),
+     ("jamaar", ['ja', 'maar'], pron, infpron, typo, dp + 2),
+     ("jahoor", ['ja', 'hoor'], pron, infpron, typo, dp + 2),
+     ("neehoor", ['nee', 'hoor'], pron, infpron, typo, dp + 2),
+     ("kanne", ['kan', 'er'], pron, infpron, codared, dp + 2),
+     ("moek", ['moet', "'k"], pron, infpron, contract, dp)
      ]
 # + closesyllshortprepexpansions # put off does not lead to improvement
 # + innuclosedsyllshortprepexpansions # put off does not lead to improvement
 
 
 #: The dictionary *basicexpansions* maps a contracted word form to a list of 4-tuples
 #: containing its expansion as a list of words, plus 3 strings to encode metadata. The
```

### Comparing `sastadev-0.1.5/src/sastadev/celexlexicon.py` & `sastadev-0.2.0/src/sastadev/celexlexicon.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/checkcorrection.py` & `sastadev-0.2.0/src/sastadev/checkcorrection.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/cleanCHILDEStokens.py` & `sastadev-0.2.0/src/sastadev/cleanCHILDEStokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 * ..autofunction:: cleantext
 
 '''
 import re
 from copy import deepcopy
 from typing import List, Optional, Pattern, TextIO, Tuple, Union
 
-from sastadev import CHAT_Annotation, sastatok
+import sastadev
+# from sastadev import CHAT_Annotation, sastatok
 from sastadev.conf import settings
 from sastadev.metadata import Meta, Metadata, bpl_none
 from sastadev.sastatoken import Token, show
 from sastadev.sastatypes import IntSpan
 
 hexformat = '\\u{0:04X}'
 
@@ -115,15 +116,15 @@
 
     :param utt:
     :param repkeep:
     :param tokenoutput:
     :return:
     '''
     newutt = robustness(utt)
-    tokens = sastatok.sasta_tokenize(newutt)
+    tokens = sastadev.sastatok.sasta_tokenize(newutt)
     inwordlist = [t.word for t in tokens]
     intokenstrings = [str(token) for token in tokens]
     # print(space.join(intokenstrings))
     (newtokens, metadata) = cleantokens(tokens, repkeep)
     #remove symbol tokens that should not be there anymore
     newtokens = purifytokens(newtokens)
     resultwordlist = [t.word for t in newtokens]
@@ -144,15 +145,15 @@
 def cleantokens(tokens: List[Token], repkeep: bool) -> Tuple[List[Token], Metadata]:
     newtokens = deepcopy(tokens)
     metadata = []
 
     (newtokens, nestingmetadata) = clearnesting(newtokens, repkeep)
     metadata += nestingmetadata
 
-    for annotation in CHAT_Annotation.annotations:
+    for annotation in sastadev.CHAT_Annotation.annotations:
         (newtokens, annotationmetadata) = annotation.apply(newtokens, repkeep)
         metadata += annotationmetadata
         tokenstrings = [str(token) for token in newtokens]
         # print(space.join(tokenstrings))
 
     return (newtokens, metadata)
```

### Comparing `sastadev-0.1.5/src/sastadev/compounds.py` & `sastadev-0.2.0/src/sastadev/compounds.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/corrector.py` & `sastadev-0.2.0/src/sastadev/corrector.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                             getunwantedtokens, nodesfindjaneenou)
 from sastadev.deregularise import correctinflection
 from sastadev.find_ngram import (Ngram, findmatches, ngram1, ngram2, ngram7,
                                  ngram10, ngram11, ngram16, ngram17)
 from sastadev.iedims import getjeforms
 from sastadev.lexicon import (WordInfo, de, dets, getwordinfo, het,
                               informlexicon, isa_namepart, known_word,
-                              tswnouns)
+                              tswnouns, wordsunknowntoalpinolexicondict)
 from sastadev.macros import expandmacros
 from sastadev.metadata import (Meta, bpl_indeze, bpl_node, bpl_none, bpl_word,
                                bpl_wordlemma, defaultbackplacement,
                                defaultpenalty, filled_pause, fstoken, intj,
                                janeenou, longrep, mkSASTAMeta, repeated,
                                repeatedjaneenou, repeatedseqtoken, shortrep,
                                substringrep, unknownsymbol)
@@ -100,14 +100,16 @@
 
 # duppattern = r'(.)\1{2,}'
 # dupre = re.compile(duppattern)
 #: The pattern *gaatiepattern* identifies words ending in *tie* preceded by at least a
 #: vowel and optionally a consonant.
 gaatiepattern = r'^.*' + anychars(vowels) + opt(anychars(consonants)) + 'tie$'
 gaatiere = re.compile(gaatiepattern)
+gaattiepattern = r'^.*' + anychars(vowels) + 'ttie$'
+gaattiere = re.compile(gaattiepattern)
 neutersgnoun = 'boekje'  # select here an unambiguous neuter noun
 
 
 def skiptokens(tokenlist: List[Token], skiptokenlist: List[Token]) -> List[Token]:
     '''
 
     :param tokenlist:
@@ -491,15 +493,14 @@
         themetadata = allmetadata + ctmd.metadata
         results.append((correction, themetadata))
     return results
 
 
 # def getalternatives(origtokensmd, method, llremovedtokens, tree, uttid):
 def getalternatives(origtokensmd: TokenListMD, method: MethodName, tree: SynTree, uttid: UttId):
-
     newtokensmd = explanationasreplacement(origtokensmd, tree)
     if newtokensmd is not None:
         tokensmd = newtokensmd
     else:
         tokensmd = origtokensmd
 
     tokens = tokensmd.tokens
@@ -768,15 +769,15 @@
     else:
         headresults = getsingleitemexpansions(tokenlist[0], intokenposlist)
         for headresult in headresults:
             tailresults = getexpansions2(tokenlist[1:], headresult[1])
             results = [combine(headresult, tailresult)
                        for tailresult in tailresults]
             finalresults += [(TokenListMD(result[0].tokens,
-                              result[0].metadata), result[1]) for result in results]
+                                          result[0].metadata), result[1]) for result in results]
     return finalresults
 
 
 def gettokenyield(tokens: List[Token]) -> str:
     words = [token.word for token in tokens]
     result = space.join(words)
     return result
@@ -963,17 +964,18 @@
     #     wordnode = find1(tree, f'.//node[@pt="ww" and @begin="{beginval}"]')
     #     if wordnode is not None:
     #         newwords = ['ietsjes']
     #         newtokenmds = updatenewtokenmds(newtokenmds, token, newwords, beginmetadata,
     #                                         name='Disambiguation', value='Avoid unknown reading',
     #                                         cat='Lexicon', backplacement=bpl_wordlemma)
 
-    moemoetxpath = './/node[@lemma="moe" and @pt!="n" and not(%onlywordinutt%) and (@rel="--" or @rel="dp" or @rel="predm" or @rel="nucl")]'
+    moemoetxpath = './/node[@lemma="moe" and @pt!="n" and not(%onlywordinutt%)]'
     expanded_moemoetxpath = expandmacros(moemoetxpath)
-    if token.word.lower() == 'moe' and tree.xpath(expanded_moemoetxpath) != []:
+    if token.word.lower() == 'moe' and tree.xpath(expanded_moemoetxpath) != [] and (
+            tokenctr == 0 or tokens[tokenctr - 1].word.lower() != 'beetje'):
         newwords = ['moet']
         newtokenmds = updatenewtokenmds(newtokenmds, token, newwords, beginmetadata,
                                         name='Informal pronunciation', value='Final t-deletion', cat='Pronunciation',
                                         backplacement=bpl_word)
 
     # dee -> deze of deed
     if token.word.lower() == 'dee':
@@ -982,14 +984,33 @@
                                         name='Wrong pronunciation', value='Coda reduction', cat='Pronunciation',
                                         backplacement=bpl_word, penalty=5)
         newwords = ['deed']
         newtokenmds = updatenewtokenmds(newtokenmds, token, newwords, beginmetadata,
                                         name='Informal pronunciation', value='Final t-deletion', cat='Pronunciation',
                                         backplacement=bpl_word)
 
+    # beurt -> gebeurt
+    if token.word.lower() == 'beurt':
+        newwords = ['gebeurt']
+        newtokenmds = updatenewtokenmds(newtokenmds, token, newwords, beginmetadata,
+                                        name='Wrong pronunciation', value='Unstressed syllable drop', cat='Pronunciation',
+                                        backplacement=bpl_word, penalty=5)
+        newwords = ['deed']
+        newtokenmds = updatenewtokenmds(newtokenmds, token, newwords, beginmetadata,
+                                        name='Informal pronunciation', value='Final t-deletion', cat='Pronunciation',
+                                        backplacement=bpl_word)
+
+    # words unknown to Alpino e.g *gymmen* is replaced by *trainen*
+    if token.word.lower() in wordsunknowntoalpinolexicondict:
+        newwords = [wordsunknowntoalpinolexicondict[token.word.lower()]]
+        newtokenmds = updatenewtokenmds(newtokenmds, token, newwords, beginmetadata,
+                                    name='Word unknown to Alpino', value='Unknown word', cat='lexicon',
+                                    backplacement=bpl_wordlemma)
+
+
     # find document specific replacements
 
     # find organisation specific replacements
 
     # find childes replacements, preferably with vocabulary from the same age
 
     # gaatie
@@ -1085,16 +1106,45 @@
     validnewtokenmds = [
         tokenmd for tokenmd in newtokenmds if known_word(tokenmd.token.word)]
     # and now we add the original tokenmd
     validnewtokenmds += [tokenmd]
     return validnewtokenmds
 
 
+
 def gaatie(word: str) -> List[str]:
     '''
+    The function *gaatie*
+    * replaces a word of the form *X-ie* by the string f'{X} ie' if X is a verb form
+    * replaces a word of the form *XVttie* by the string f'{X}{V}t ie where V is vowel and XVt is a verb form
+    * replaces  a word that matches with  *gaatiepattern*  (e.g.
+    *gaatie*) by a sequence of two words where the first word equals word[:-2] (
+    *gaat*) and is a known word and the second word equals word[-2:] (*ie*).
+
+    .. autodata:: corrector::gaatiepattern
+    '''
+    results = []
+    # kan-ie, moet-ie, gaat-ie, wil-ie
+    if word.endswith('-ie') and informlexicon(word[:-3]):
+        result = space.join([word[:-3], 'ie'])
+        results.append(result)
+    # moettie, gaattie,
+    if gaattiere.match(word) and informlexicon(word[:-3]):
+        result = space.join([word[:-3], 'ie'])
+        results.append(result)
+    if gaatiere.match(word):
+        # and if it is a verb this is essential because now tie is also split into t ie
+        if informlexicon(word[:-2]):
+            result = space.join([word[:-2], word[-2:]])
+            results.append(result)
+    return results
+
+
+def oldgaatie(word: str) -> List[str]:
+    '''
     The function *gaatie* replaces  a word that matches with  *gaatiepattern*  (e.g.
     *gaatie*) by a sequence of two words where the first word equals word[:-2] (
     *gaat*) and is a known word and the second word equals word[-2:] (*ie*).
 
     .. autodata:: corrector::gaatiepattern
     '''
     results = []
```

### Comparing `sastadev-0.1.5/src/sastadev/correcttreebank.py` & `sastadev-0.2.0/src/sastadev/correcttreebank.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from lxml import etree
 
 from sastadev.basicreplacements import basicreplacements
 from sastadev.cleanCHILDEStokens import cleantext
 from sastadev.conf import settings
 from sastadev.corrector import (Correction, disambiguationdict, getcorrections,
                                 mkuttwithskips)
-from sastadev.lexicon import de, dets, known_word
+from sastadev.lexicon import de, dets, known_word, nochildwords
 from sastadev.macros import expandmacros
 from sastadev.metadata import (Meta, bpl_delete, bpl_indeze, bpl_node,
                                bpl_none, bpl_replacement, bpl_word,
                                bpl_wordlemma, insertion)
 from sastadev.sastatoken import Token, insertinflate, tokenlist2stringlist
 from sastadev.sastatypes import (AltId, CorrectionMode, ErrorDict, MetaElement,
                                  MethodName, Penalty, Position, PositionStr,
@@ -56,25 +56,25 @@
                        'compoundcount', 'unknownwordcount', 'sucount', 'svaokcount', 'deplusneutcount', 'badcatcount',
                        'hyphencount', 'basicreplaceecount', 'ambigcount', 'subjunctivecount', 'unknownnouncount',
                        'unknownnamecount', 'dezebwcount']
 
 errorwbheader = ['Sample', 'User1', 'User2', 'User3'] + \
                 ['Status', 'Uttid', 'Origutt', 'Origsent'] + \
                 ['altid', 'altsent', 'score'] + \
-    altpropertiesheader
-
+                altpropertiesheader
 
 smartreplacepairs = [('me', 'mijn'), ('ze', 'zijn')]
 smartreplacedict = {w1: w2 for w1, w2 in smartreplacepairs}
 
 
 class Alternative():
     def __init__(self, stree, altid, altsent, penalty, dpcount, dhyphencount, complsucount, dimcount,
                  compcount, supcount, compoundcount, unknownwordcount, sucount, svaok, deplusneutcount, badcatcount,
-                 hyphencount, basicreplaceecount, ambigcount, subjunctivecount, unknownnouncount, unknownnamecount, dezebwcount):
+                 hyphencount, basicreplaceecount, ambigcount, subjunctivecount, unknownnouncount, unknownnamecount,
+                 dezebwcount):
         self.stree: SynTree = stree
         self.altid: AltId = altid
         self.altsent: str = altsent
         self.penalty: Penalty = int(penalty)
         self.dpcount: int = int(dpcount)
         self.dhyphencount: int = int(dhyphencount)
         self.complsucount: int = int(complsucount)
@@ -162,15 +162,15 @@
         altsrows = [
             self.alts[altid].alt2row(
                 self.orig.uttid, base, user1, user2, user3, bestaltids, self.selected, origsent)
             for altid in self.alts]
         laltsrows = len(altsrows)
         selectedrow = [base, user1, user2, user3] + \
                       ['Selected', self.orig.uttid, '',
-                          self.alts[self.selected].altsent, str(self.selected)]
+                       self.alts[self.selected].altsent, str(self.selected)]
         if laltsrows > 1:
             rows = [origrow] + altsrows + [selectedrow]
         else:
             rows = []
         return rows
 
 
@@ -225,25 +225,31 @@
         node.attrib['pvagr'] = 'mv'
         node.attrib['pvtijd'] = 'tgw'
         node.attrib['postag'] = 'WW(pv,tgw,mv)'
 
 
 def smartreplace(node: SynTree, word: str) -> SynTree:
     '''
-    replaces *node* by a different node if the parse of *word* yields a node with a valid word and the same word class, otherwise by
+    replaces *node* by a different node if the parse of *word* yields a node with a valid word and the same word class and
+     if it does not occur in nochildwords;  otherwise by
     a node with *word* and *lemma* attributes replaced by *word*
     :param node:
     :param word:
     :return:
     '''
+
     wordtree = settings.PARSE_FUNC(word)
     newnode = find1(wordtree, './/node[@pt]')
     newnodept = getattval(newnode, 'pt')
     nodept = getattval(node, 'pt')
-    if isvalidword(word) and issamewordclass(node, newnode) and not isrobustnoun(newnode):
+    newnodelemma = getattval(newnode, 'lemma')
+    if isvalidword(word) and \
+            issamewordclass(node, newnode) and \
+            not isrobustnoun(newnode) and \
+            newnodelemma not in nochildwords:
         result = newnode
         result.attrib['begin'] = getattval(node, 'begin')
         result.attrib['end'] = getattval(node, 'end')
         result.attrib['rel'] = getattval(node, 'rel')
         if 'index' in node.attrib:
             result.attrib['index'] = getattval(node, 'index')
         if infpvpair(newnode, node):
@@ -252,16 +258,15 @@
         result = copy(node)
         result.attrib['word'] = word
         if '_' in node.attrib['lemma'] and countsyllables(word) == 1:
             result.attrib['lemma'] = word
     return result
 
 
-def mkmetarecord(meta: MetaElement, origutt: Optional[str], parsed_as: Optional[str]) -> Tuple[
-        Optional[str], List[str]]:
+def mkmetarecord(meta: MetaElement, origutt: Optional[str], parsed_as: Optional[str]) -> Tuple[Optional[str], List[str]]:
     if meta is None:
         return None, []
     key = meta.attrib['name']
     if meta.tag == 'xmeta':
         if meta.attrib['source'] in ['CHAT', 'SASTA']:
             newmetarecord = [meta.attrib['name'], meta.attrib['value'], meta.attrib['source'], meta.attrib['cat'],
                              meta.attrib['subcat'], origutt, parsed_as]
@@ -743,15 +748,15 @@
                 # else:
                 #    newnode.attrib['lemma'] = wprop[3]
                 substnode = smartreplace(newnode, oldword)
 
                 newnodeparent = newnode.getparent()
                 newnodeparent.remove(newnode)
                 newnodeparent.append(substnode)
-                # showtree(thetree, 'thetree after smart replace')
+        # showtree(thetree, 'thetree after smart replace')
 
         elif curbackplacement in [bpl_word, bpl_wordlemma]:
             nodeend = meta.annotationposlist[-1] + 1
             nodexpath = './/node[@pt and @begin="{}" and @end="{}"]'.format(
                 nodeend - 1, nodeend)
             newnode = myfind(thetree, nodexpath)
             oldnode = myfind(fatstree, nodexpath)
@@ -893,15 +898,15 @@
     if meta is not None and meta.name in ['cleanedtokenisation', 'cleanedtokenpositions']:
         sortedbegins = sorted(begins, key=lambda x: int(x), reverse=True)
         newmeta = copy(meta)
         for begin in sortedbegins:
             intbegin = int(begin)
             beginindex = cleantokpos.index(intbegin)
             newmeta.annotationwordlist = newmeta.annotationwordlist[:beginindex] \
-                + newmeta.annotationwordlist[beginindex + 1:]
+                                         + newmeta.annotationwordlist[beginindex + 1:]
         newmeta.value = newmeta.annotationwordlist
         return newmeta
     else:
         return meta
 
 
 def oldgetuttid(stree: SynTree) -> UttId:
@@ -920,15 +925,16 @@
         origutt = None
     else:
         origutt = origuttlist[0]
     return origutt
 
 
 def scorefunction(obj: Alternative) -> TupleNint:
-    return (-obj.unknownwordcount, -obj.unknownnouncount, -obj.unknownnamecount, -obj.ambigcount, -obj.dpcount, -obj.dhyphencount,
+    return (-obj.unknownwordcount, -obj.unknownnouncount, -obj.unknownnamecount, -obj.ambigcount, -obj.dpcount,
+            -obj.dhyphencount,
             -obj.complsucount, -obj.badcatcount,
             -obj.basicreplaceecount, -obj.ambigcount, -obj.hyphencount,
             -obj.subjunctivecount, obj.dimcount,
             obj.compcount, obj.supcount, obj.compoundcount, obj.sucount, obj.svaok,
             -obj.deplusneutcount,
             -obj.dezebwcount, -obj.penalty)
 
@@ -995,21 +1001,21 @@
     result = len(ambignodes)
     return result
 
 
 def getunknownwordcount(nt: SynTree) -> int:
     words = [w for w in nt.xpath('.//node[@pt!="tsw"]/@word')]
     unknownwords = [w for w in words if not (
-        isvalidword(w.lower()) or isvalidword(w.title()))]
+            isvalidword(w.lower()) or isvalidword(w.title()))]
     result = len(unknownwords)
     return result
 
 
 def selectcorrection(stree: SynTree, ptmds: List[ParsedCorrection], corr: CorrectionMode) -> Tuple[
-        ParsedCorrection, OrigandAlts]:
+    ParsedCorrection, OrigandAlts]:
     # to be implemented@@
     # it is presupposed that ptmds is not []
 
     uttid = getuttid(stree)
     orig = Original(uttid, stree)
 
     altid: AltId = 0
```

### Comparing `sastadev-0.1.5/src/sastadev/counterfunctions.py` & `sastadev-0.2.0/src/sastadev/counterfunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/celexlexicon/dutch/DMLCD.txt` & `sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/DMLCD.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/celexlexicon/dutch/DMWCDOK.txt` & `sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/DMWCDOK.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/celexlexicon/dutch/DSLCD.txt` & `sastadev-0.2.0/src/sastadev/data/celexlexicon/dutch/DSLCD.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/compoundfiles/Ncompounds-attempt1.txt` & `sastadev-0.2.0/src/sastadev/data/compoundfiles/Ncompounds-attempt1.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/compoundfiles/Ncompounds-attempt2.txt` & `sastadev-0.2.0/src/sastadev/data/compoundfiles/Ncompounds-attempt2.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/compoundfiles/Ncompounds-attempt2.zip` & `sastadev-0.2.0/src/sastadev/data/compoundfiles/Ncompounds-attempt2.zip`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/form_templates/STAP Excel VUmc 2018.xlsx` & `sastadev-0.2.0/src/sastadev/data/form_templates/STAP Excel VUmc 2018.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/form_templates/TARSP Form Current.xlsx` & `sastadev-0.2.0/src/sastadev/data/form_templates/TARSP Form Current.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/inflectioncorrection.tsv.txt` & `sastadev-0.2.0/src/sastadev/data/old_inflectioncorrection.tsv.txt`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,2697 +1,2697 @@
-gebakt	gebakken	Overgeneralisation
-ebakt	gebakken	Overgeneralisation
-bakt	gebakken	Overgeneralisation
-gebakte	gebakkene	Overgeneralisation+
-ebakte	gebakkene	Overgeneralisation+Prefix ge without onset
-ebakken	gebakken	Prefix ge without onset
-bakken	gebakken	Lacking ge prefix
-geband	gebannen	Overgeneralisation
-eband	gebannen	Overgeneralisation+Prefix ge without onset
-band	gebannen	Overgeneralisation+Lacking ge prefix
-gebande	gebannene	Overgeneralisation+
-ebande	gebannene	Overgeneralisation+Prefix ge without onset
-gebant	gebannen	Overgeneralisation
-ebant	gebannen	Overgeneralisation
-bant	gebannen	Overgeneralisation
-ebannen	gebannen	Prefix ge without onset
-bannen	gebannen	Lacking ge prefix
-gebarst	gebarsten	Overgeneralisation
-ebarst	gebarsten	Overgeneralisation
-barst	gebarsten	Overgeneralisation
-gebarste	gebarstene	Overgeneralisation+
-ebarste	gebarstene	Overgeneralisation+Prefix ge without onset
-ebarsten	gebarsten	Prefix ge without onset
-barsten	gebarsten	Lacking ge prefix
-bederfde	bedorvene	Overgeneralisation
-bederfden	bedierven	Overgeneralisation
-bedierfde	bedierf	Irregular form plus regular suffix
-bedierfden	bedierven	Irregular form plus regular suffix
-bederfd	bedorven	Overgeneralisation
-bederft	bedorven	Overgeneralisation
-bederfen	bedorven	Wrong -en suffix
-bedorfd	bedorven	Overgeneralisation
-bedorft	bedorven	Overgeneralisation
-bedriegde	bedrogene	Overgeneralisation
-bedriegden	bedrogen	Overgeneralisation
-bedroogde	bedroog	Irregular form plus regular suffix
-bedroogden	bedrogen	Irregular form plus regular suffix
-bedriegd	bedrogen	Overgeneralisation
-bedriegt	bedrogen	Overgeneralisation
-bedriegen	bedrogen	Wrong -en suffix
-bedroogt	bedrogen	Overgeneralisation
-beginde	begonnene	Overgeneralisation
-beginden	begonnen	Overgeneralisation
-begonde	begon	Irregular form plus regular suffix
-begonden	begonnen	Irregular form plus regular suffix
-begind	begonnen	Overgeneralisation
-begint	begonnen	Overgeneralisation
-beginnen	begonnen	Wrong -en suffix
-begont	begonnen	Overgeneralisation
-behangde	behangene	Overgeneralisation
-behangden	behingen	Overgeneralisation
-behingde	behing	Irregular form plus regular suffix
-behingden	behingen	Irregular form plus regular suffix
-behangd	behangen	Overgeneralisation
-behangt	behangen	Overgeneralisation
-bergde	borg	Overgeneralisation
-bergden	borgen	Overgeneralisation
-borgde	borg	Irregular form plus regular suffix
-borgden	borgen	Irregular form plus regular suffix
-gebergd	geborgen	Overgeneralisation+
-ebergd	geborgen	Overgeneralisation+Prefix ge without onset
-bergd	geborgen	Overgeneralisation+Lacking ge prefix
-gebergde	geborgene	Overgeneralisation+
-ebergde	geborgene	Overgeneralisation+Prefix ge without onset
-gebergt	geborgen	Overgeneralisation
-ebergt	geborgen	Overgeneralisation
-bergt	geborgen	Overgeneralisation
-gebergen	geborgen	Wrong -en suffix
-ebergen	geborgen	Wrong -en suffix
-bergen	geborgen	Wrong -en suffix
-geborgd	geborgen	Overgeneralisation
-geborgt	geborgen	Overgeneralisation
-eborgen	geborgen	Prefix ge without onset
-borgen	geborgen	Lacking ge prefix
-beveelde	bevolene	Overgeneralisation
-beveelden	bevalen	Overgeneralisation
-bevalde	beval	Irregular form plus regular suffix
-bevalden	bevalen	Irregular form plus regular suffix
-beveeld	bevolen	Overgeneralisation
-beveelt	bevolen	Overgeneralisation
-bevelen	bevolen	Wrong -en suffix
-bevoolt	bevolen	Overgeneralisation
-bezwijkte	bezwekene	Overgeneralisation
-bezwijkten	bezweken	Overgeneralisation
-bezweekte	bezweek	Irregular form plus regular suffix
-bezweekten	bezweken	Irregular form plus regular suffix
-bezwijkt	bezweken	Overgeneralisation
-bezwijken	bezweken	Wrong -en suffix
-bezweekt	bezweken	Overgeneralisation
-bidde	bad	Overgeneralisation
-bidden	gebeden	Wrong -en suffix
-badde	bad	Irregular form plus regular suffix
-badden	baden	Irregular form plus regular suffix
-gebid	gebeden	Overgeneralisation
-ebid	gebeden	Overgeneralisation
-bid	gebeden	Overgeneralisation
-gebidde	gebedene	Overgeneralisation+
-ebidde	gebedene	Overgeneralisation+Prefix ge without onset
-gebidden	gebeden	Wrong -en suffix
-ebidden	gebeden	Wrong -en suffix
-gebeed	gebeden	Overgeneralisation
-ebeden	gebeden	Prefix ge without onset
-beden	gebeden	Lacking ge prefix
-biedde	bood	Overgeneralisation
-biedden	boden	Overgeneralisation
-boodde	bood	Irregular form plus regular suffix
-boodden	boden	Irregular form plus regular suffix
-gebied	geboden	Overgeneralisation
-ebied	geboden	Overgeneralisation
-bied	geboden	Overgeneralisation
-gebiede	gebodene	Overgeneralisation+
-ebiede	gebodene	Overgeneralisation+Prefix ge without onset
-gebieden	geboden	Wrong -en suffix
-ebieden	geboden	Wrong -en suffix
-bieden	geboden	Wrong -en suffix
-geboodt	geboden	Overgeneralisation
-gebood	geboden	Overgeneralisation
-eboden	geboden	Prefix ge without onset
-boden	geboden	Lacking ge prefix
-bijtte	beet	Overgeneralisation
-bijtten	beten	Overgeneralisation
-beette	beet	Irregular form plus regular suffix
-beetten	beten	Irregular form plus regular suffix
-gebijt	gebeten	Overgeneralisation
-ebijt	gebeten	Overgeneralisation
-bijt	gebeten	Overgeneralisation
-gebijte	gebetene	Overgeneralisation+
-ebijte	gebetene	Overgeneralisation+Prefix ge without onset
-gebijten	gebeten	Wrong -en suffix
-ebijten	gebeten	Wrong -en suffix
-bijten	gebeten	Wrong -en suffix
-gebeet	gebeten	Overgeneralisation
-ebeten	gebeten	Prefix ge without onset
-beten	gebeten	Lacking ge prefix
-bindde	bond	Overgeneralisation
-bindden	bonden	Overgeneralisation
-bondde	bond	Irregular form plus regular suffix
-bondden	bonden	Irregular form plus regular suffix
-gebind	gebonden	Overgeneralisation
-ebind	gebonden	Overgeneralisation
-bind	gebonden	Overgeneralisation
-gebinde	gebondene	Overgeneralisation+
-ebinde	gebondene	Overgeneralisation+Prefix ge without onset
-gebinden	gebonden	Wrong -en suffix
-ebinden	gebonden	Wrong -en suffix
-binden	gebonden	Wrong -en suffix
-gebond	gebonden	Overgeneralisation
-ebonden	gebonden	Prefix ge without onset
-bonden	gebonden	Lacking ge prefix
-blaasde	blies	Overgeneralisation
-blaasden	bliezen	Overgeneralisation
-bliesde	blies	Irregular form plus regular suffix
-bliesden	bliezen	Irregular form plus regular suffix
-geblaasd	geblazen	Overgeneralisation
-eblaasd	geblazen	Overgeneralisation+Prefix ge without onset
-blaasd	geblazen	Overgeneralisation+Lacking ge prefix
-geblaasde	geblazene	Overgeneralisation+
-eblaasde	geblazene	Overgeneralisation+Prefix ge without onset
-geblaast	geblazen	Overgeneralisation
-eblaast	geblazen	Overgeneralisation
-blaast	geblazen	Overgeneralisation
-geblasen	geblazen	Wrong -en suffix
-eblasen	geblazen	Wrong -en suffix
-blasen	geblazen	Wrong -en suffix
-eblazen	geblazen	Prefix ge without onset
-blazen	geblazen	Lacking ge prefix
-blijkte	bleek	Overgeneralisation
-blijkten	bleken	Overgeneralisation
-bleekte	bleek	Irregular form plus regular suffix
-bleekten	bleken	Irregular form plus regular suffix
-geblijkt	gebleken	Overgeneralisation
-eblijkt	gebleken	Overgeneralisation
-blijkt	gebleken	Overgeneralisation
-geblijkte	geblekene	Overgeneralisation+
-eblijkte	geblekene	Overgeneralisation+Prefix ge without onset
-geblijken	gebleken	Wrong -en suffix
-eblijken	gebleken	Wrong -en suffix
-blijken	gebleken	Wrong -en suffix
-gebleekt	gebleken	Overgeneralisation
-ebleken	gebleken	Prefix ge without onset
-bleken	gebleken	Lacking ge prefix
-blijfde	bleef	Overgeneralisation
-blijfden	bleven	Overgeneralisation
-bleefde	bleef	Irregular form plus regular suffix
-bleefden	bleven	Irregular form plus regular suffix
-geblijfd	gebleven	Overgeneralisation+
-eblijfd	gebleven	Overgeneralisation+Prefix ge without onset
-blijfd	gebleven	Overgeneralisation+Lacking ge prefix
-geblijfde	geblevene	Overgeneralisation+
-eblijfde	geblevene	Overgeneralisation+Prefix ge without onset
-geblijft	gebleven	Overgeneralisation
-eblijft	gebleven	Overgeneralisation
-blijft	gebleven	Overgeneralisation
-geblijfen	gebleven	Wrong -en suffix
-eblijfen	gebleven	Wrong -en suffix
-blijfen	gebleven	Wrong -en suffix
-gebleefd	gebleven	Overgeneralisation
-gebleeft	gebleven	Overgeneralisation
-ebleven	gebleven	Prefix ge without onset
-bleven	gebleven	Lacking ge prefix
-blinkte	blonk	Overgeneralisation
-blinkten	blonken	Overgeneralisation
-blonkte	blonk	Irregular form plus regular suffix
-blonkten	blonken	Irregular form plus regular suffix
-geblinkt	geblonken	Overgeneralisation
-eblinkt	geblonken	Overgeneralisation
-blinkt	geblonken	Overgeneralisation
-geblinkte	geblonkene	Overgeneralisation+
-eblinkte	geblonkene	Overgeneralisation+Prefix ge without onset
-geblinken	geblonken	Wrong -en suffix
-eblinken	geblonken	Wrong -en suffix
-blinken	geblonken	Wrong -en suffix
-geblonkt	geblonken	Overgeneralisation
-eblonken	geblonken	Prefix ge without onset
-blonken	geblonken	Lacking ge prefix
-gebraad	gebraden	Overgeneralisation
-ebraad	gebraden	Overgeneralisation
-braad	gebraden	Overgeneralisation
-gebrade	gebradene	Overgeneralisation+
-ebrade	gebradene	Overgeneralisation+Prefix ge without onset
-ebraden	gebraden	Prefix ge without onset
-braden	gebraden	Lacking ge prefix
-breekte	brak	Overgeneralisation
-breekten	braken	Overgeneralisation
-brakte	brak	Irregular form plus regular suffix
-brakten	braken	Irregular form plus regular suffix
-gebreekt	gebroken	Overgeneralisation
-ebreekt	gebroken	Overgeneralisation
-breekt	gebroken	Overgeneralisation
-gebreekte	gebrokene	Overgeneralisation+
-ebreekte	gebrokene	Overgeneralisation+Prefix ge without onset
-gebreken	gebroken	Wrong -en suffix
-ebreken	gebroken	Wrong -en suffix
-breken	gebroken	Wrong -en suffix
-gebrookt	gebroken	Overgeneralisation
-ebroken	gebroken	Prefix ge without onset
-broken	gebroken	Lacking ge prefix
-brengde	bracht	Overgeneralisation
-brengden	brachten	Overgeneralisation
-brachtde	bracht	Irregular form plus regular suffix
-brachtden	brachten	Irregular form plus regular suffix
-gebrengd	gebracht	Overgeneralisation+
-ebrengd	gebracht	Overgeneralisation+Prefix ge without onset
-brengd	gebracht	Overgeneralisation+Lacking ge prefix
-gebrengde	gebrachte	Overgeneralisation+
-ebrengde	gebrachte	Overgeneralisation+Prefix ge without onset
-gebrengt	gebracht	Overgeneralisation
-ebrengt	gebracht	Overgeneralisation
-brengt	gebracht	Overgeneralisation
-gebrengen	gebracht	Wrong -en suffix
-ebrengen	gebracht	Wrong -en suffix
-brengen	gebracht	Wrong -en suffix
-ebracht	gebracht	Prefix ge without onset
-bracht	gebracht	Lacking ge prefix
-gebrouwd	gebrouwen	Overgeneralisation
-ebrouwd	gebrouwen	Overgeneralisation+Prefix ge without onset
-brouwd	gebrouwen	Overgeneralisation+Lacking ge prefix
-gebrouwde	gebrouwene	Overgeneralisation+
-ebrouwde	gebrouwene	Overgeneralisation+Prefix ge without onset
-gebrouwt	gebrouwen	Overgeneralisation
-ebrouwt	gebrouwen	Overgeneralisation
-brouwt	gebrouwen	Overgeneralisation
-ebrouwen	gebrouwen	Prefix ge without onset
-brouwen	gebrouwen	Lacking ge prefix
-buigde	boog	Overgeneralisation
-buigden	bogen	Overgeneralisation
-boogde	boog	Irregular form plus regular suffix
-boogden	bogen	Irregular form plus regular suffix
-gebuigd	gebogen	Overgeneralisation+
-ebuigd	gebogen	Overgeneralisation+Prefix ge without onset
-buigd	gebogen	Overgeneralisation+Lacking ge prefix
-gebuigde	gebogene	Overgeneralisation+
-ebuigde	gebogene	Overgeneralisation+Prefix ge without onset
-gebuigt	gebogen	Overgeneralisation
-ebuigt	gebogen	Overgeneralisation
-buigt	gebogen	Overgeneralisation
-gebuigen	gebogen	Wrong -en suffix
-ebuigen	gebogen	Wrong -en suffix
-buigen	gebogen	Wrong -en suffix
-geboogt	gebogen	Overgeneralisation
-ebogen	gebogen	Prefix ge without onset
-bogen	gebogen	Lacking ge prefix
-denkte	dacht	Overgeneralisation
-denkten	dachten	Overgeneralisation
-dachtte	dacht	Irregular form plus regular suffix
-dachtten	dachten	Irregular form plus regular suffix
-gedenkt	gedacht	Overgeneralisation
-edenkt	gedacht	Overgeneralisation
-denkt	gedacht	Overgeneralisation
-gedenkte	gedachte	Overgeneralisation+
-edenkte	gedachte	Overgeneralisation+Prefix ge without onset
-gedenken	gedacht	Wrong -en suffix
-edenken	gedacht	Wrong -en suffix
-denken	gedacht	Wrong -en suffix
-edacht	gedacht	Prefix ge without onset
-dacht	gedacht	Lacking ge prefix
-dingde	dong	Overgeneralisation
-dingden	dongen	Overgeneralisation
-dongde	dong	Irregular form plus regular suffix
-dongden	dongen	Irregular form plus regular suffix
-gedingd	gedongen	Overgeneralisation+
-edingd	gedongen	Overgeneralisation+Prefix ge without onset
-dingd	gedongen	Overgeneralisation+Lacking ge prefix
-gedingde	gedongene	Overgeneralisation+
-edingde	gedongene	Overgeneralisation+Prefix ge without onset
-gedingt	gedongen	Overgeneralisation
-edingt	gedongen	Overgeneralisation
-dingt	gedongen	Overgeneralisation
-gedingen	gedongen	Wrong -en suffix
-edingen	gedongen	Wrong -en suffix
-dingen	gedongen	Wrong -en suffix
-gedongd	gedongen	Overgeneralisation
-gedongt	gedongen	Overgeneralisation
-edongen	gedongen	Prefix ge without onset
-dongen	gedongen	Lacking ge prefix
-doete	deed	Overgeneralisation
-doeten	deden	Overgeneralisation
-deedte	deed	Irregular form plus regular suffix
-deedten	deden	Irregular form plus regular suffix
-gedoet	gedaan	Overgeneralisation
-edoet	gedaan	Overgeneralisation
-doet	gedaan	Overgeneralisation
-gedoete	gedaane	Overgeneralisation+
-edoete	gedaane	Overgeneralisation+Prefix ge without onset
-gedoen	gedaan	Wrong -en suffix
-edoen	gedaan	Wrong -en suffix
-doen	gedaan	Wrong -en suffix
-edaan	gedaan	Prefix ge without onset
-daan	gedaan	Lacking ge prefix
-draagde	droeg	Overgeneralisation
-draagden	droegen	Overgeneralisation
-droegde	droeg	Irregular form plus regular suffix
-droegden	droegen	Irregular form plus regular suffix
-gedraagd	gedragen	Overgeneralisation
-edraagd	gedragen	Overgeneralisation+Prefix ge without onset
-draagd	gedragen	Overgeneralisation+Lacking ge prefix
-gedraagde	gedragene	Overgeneralisation+
-edraagde	gedragene	Overgeneralisation+Prefix ge without onset
-gedraagt	gedragen	Overgeneralisation
-edraagt	gedragen	Overgeneralisation
-draagt	gedragen	Overgeneralisation
-edragen	gedragen	Prefix ge without onset
-dragen	gedragen	Lacking ge prefix
-drijfde	dreef	Overgeneralisation
-drijfden	dreven	Overgeneralisation
-dreefde	dreef	Irregular form plus regular suffix
-dreefden	dreven	Irregular form plus regular suffix
-gedrijfd	gedreven	Overgeneralisation+
-edrijfd	gedreven	Overgeneralisation+Prefix ge without onset
-drijfd	gedreven	Overgeneralisation+Lacking ge prefix
-gedrijfde	gedrevene	Overgeneralisation+
-edrijfde	gedrevene	Overgeneralisation+Prefix ge without onset
-gedrijft	gedreven	Overgeneralisation
-edrijft	gedreven	Overgeneralisation
-drijft	gedreven	Overgeneralisation
-gedrijfen	gedreven	Wrong -en suffix
-edrijfen	gedreven	Wrong -en suffix
-drijfen	gedreven	Wrong -en suffix
-gedreefd	gedreven	Overgeneralisation
-gedreeft	gedreven	Overgeneralisation
-edreven	gedreven	Prefix ge without onset
-dreven	gedreven	Lacking ge prefix
-dringde	drong	Overgeneralisation
-dringden	drongen	Overgeneralisation
-drongde	drong	Irregular form plus regular suffix
-drongden	drongen	Irregular form plus regular suffix
-gedringd	gedrongen	Overgeneralisation+
-edringd	gedrongen	Overgeneralisation+Prefix ge without onset
-dringd	gedrongen	Overgeneralisation+Lacking ge prefix
-gedringde	gedrongene	Overgeneralisation+
-edringde	gedrongene	Overgeneralisation+Prefix ge without onset
-gedringt	gedrongen	Overgeneralisation
-edringt	gedrongen	Overgeneralisation
-dringt	gedrongen	Overgeneralisation
-gedringen	gedrongen	Wrong -en suffix
-edringen	gedrongen	Wrong -en suffix
-dringen	gedrongen	Wrong -en suffix
-gedrongd	gedrongen	Overgeneralisation
-gedrongt	gedrongen	Overgeneralisation
-edrongen	gedrongen	Prefix ge without onset
-drongen	gedrongen	Lacking ge prefix
-drinkte	dronk	Overgeneralisation
-drinkten	dronken	Overgeneralisation
-dronkte	dronk	Irregular form plus regular suffix
-dronkten	dronken	Irregular form plus regular suffix
-gedrinkt	gedronken	Overgeneralisation
-edrinkt	gedronken	Overgeneralisation
-drinkt	gedronken	Overgeneralisation
-gedrinkte	gedronkene	Overgeneralisation+
-edrinkte	gedronkene	Overgeneralisation+Prefix ge without onset
-gedrinken	gedronken	Wrong -en suffix
-edrinken	gedronken	Wrong -en suffix
-drinken	gedronken	Wrong -en suffix
-gedronkt	gedronken	Overgeneralisation
-edronken	gedronken	Prefix ge without onset
-dronken	gedronken	Lacking ge prefix
-druipte	droop	Overgeneralisation
-druipten	dropen	Overgeneralisation
-droopte	droop	Irregular form plus regular suffix
-droopten	dropen	Irregular form plus regular suffix
-gedruipt	gedropen	Overgeneralisation
-edruipt	gedropen	Overgeneralisation
-druipt	gedropen	Overgeneralisation
-gedruipte	gedropene	Overgeneralisation+
-edruipte	gedropene	Overgeneralisation+Prefix ge without onset
-gedruipen	gedropen	Wrong -en suffix
-edruipen	gedropen	Wrong -en suffix
-druipen	gedropen	Wrong -en suffix
-gedroopt	gedropen	Overgeneralisation
-edropen	gedropen	Prefix ge without onset
-dropen	gedropen	Lacking ge prefix
-duikte	dook	Overgeneralisation
-duikten	doken	Overgeneralisation
-dookte	dook	Irregular form plus regular suffix
-dookten	doken	Irregular form plus regular suffix
-geduikt	gedoken	Overgeneralisation
-eduikt	gedoken	Overgeneralisation
-duikt	gedoken	Overgeneralisation
-geduikte	gedokene	Overgeneralisation+
-eduikte	gedokene	Overgeneralisation+Prefix ge without onset
-geduiken	gedoken	Wrong -en suffix
-eduiken	gedoken	Wrong -en suffix
-duiken	gedoken	Wrong -en suffix
-gedookt	gedoken	Overgeneralisation
-edoken	gedoken	Prefix ge without onset
-doken	gedoken	Lacking ge prefix
-dwingde	dwong	Overgeneralisation
-dwingden	dwongen	Overgeneralisation
-dwongde	dwong	Irregular form plus regular suffix
-dwongden	dwongen	Irregular form plus regular suffix
-gedwingd	gedwongen	Overgeneralisation+
-edwingd	gedwongen	Overgeneralisation+Prefix ge without onset
-dwingd	gedwongen	Overgeneralisation+Lacking ge prefix
-gedwingde	gedwongene	Overgeneralisation+
-edwingde	gedwongene	Overgeneralisation+Prefix ge without onset
-gedwingt	gedwongen	Overgeneralisation
-edwingt	gedwongen	Overgeneralisation
-dwingt	gedwongen	Overgeneralisation
-gedwingen	gedwongen	Wrong -en suffix
-edwingen	gedwongen	Wrong -en suffix
-dwingen	gedwongen	Wrong -en suffix
-gedwongd	gedwongen	Overgeneralisation
-gedwongt	gedwongen	Overgeneralisation
-edwongen	gedwongen	Prefix ge without onset
-dwongen	gedwongen	Lacking ge prefix
-eette	at	Overgeneralisation
-eetten	aten	Overgeneralisation
-atte	at	Irregular form plus regular suffix
-atten	aten	Irregular form plus regular suffix
-geeet	gegeten	Overgeneralisation+
-eeet	gegeten	Overgeneralisation+Prefix ge without onset
-eet	gegeten	Overgeneralisation
-geete	gegetene	Overgeneralisation+
-eete	gegetene	Overgeneralisation+Prefix ge without onset
-geëet	gegeten	Overgeneralisation
-eëet	gegeten	Overgeneralisation
-geëten	gegeten	Wrong -en suffix
-eëten	gegeten	Wrong -en suffix
-eten	gegeten	Wrong -en suffix
-gegeet	gegeten	Overgeneralisation
-egeten	gegeten	Prefix ge without onset
-geten	gegeten	Lacking ge prefix
-fluitte	floot	Overgeneralisation
-fluitten	floten	Overgeneralisation
-flootte	floot	Irregular form plus regular suffix
-flootten	floten	Irregular form plus regular suffix
-gefluit	gefloten	Overgeneralisation
-efluit	gefloten	Overgeneralisation
-fluit	gefloten	Overgeneralisation
-gefluite	geflotene	Overgeneralisation+
-efluite	geflotene	Overgeneralisation+Prefix ge without onset
-gefluiten	gefloten	Wrong -en suffix
-efluiten	gefloten	Wrong -en suffix
-fluiten	gefloten	Wrong -en suffix
-gefloot	gefloten	Overgeneralisation
-efloten	gefloten	Prefix ge without onset
-floten	gefloten	Lacking ge prefix
-gade	ging	Overgeneralisation
-gaden	gingen	Overgeneralisation
-gingde	ging	Irregular form plus regular suffix
-gingden	gingen	Irregular form plus regular suffix
-gegaad	gegaan	Overgeneralisation+
-egaad	gegaan	Overgeneralisation+Prefix ge without onset
-gaad	gegaan	Overgeneralisation+Lacking ge prefix
-gegade	gegaane	Overgeneralisation+
-egade	gegaane	Overgeneralisation+Prefix ge without onset
-gegaat	gegaan	Overgeneralisation
-egaat	gegaan	Overgeneralisation
-gaat	gegaan	Overgeneralisation
-egaan	gegaan	Prefix ge without onset
-gaan	gegaan	Lacking ge prefix
-geldde	gold	Overgeneralisation
-geldden	golden	Overgeneralisation
-goldde	gold	Irregular form plus regular suffix
-goldden	golden	Irregular form plus regular suffix
-gegeld	gegolden	Overgeneralisation
-egeld	gegolden	Overgeneralisation
-geld	gegolden	Overgeneralisation
-gegelde	gegoldene	Overgeneralisation+
-egelde	gegoldene	Overgeneralisation+Prefix ge without onset
-gegelden	gegolden	Wrong -en suffix
-egelden	gegolden	Wrong -en suffix
-gelden	gegolden	Wrong -en suffix
-gegold	gegolden	Overgeneralisation
-egolden	gegolden	Prefix ge without onset
-golden	gegolden	Lacking ge prefix
-geneesde	genezene	Overgeneralisation
-geneesden	genazen	Overgeneralisation
-genasde	genas	Irregular form plus regular suffix
-genasden	genazen	Irregular form plus regular suffix
-geneesd	genezen	Overgeneralisation
-geneest	genezen	Overgeneralisation
-genesen	genezen	Wrong -en suffix
-enezen	genezen	Prefix ge without onset
-nezen	genezen	Lacking ge prefix
-geniette	genoot	Overgeneralisation
-genietten	genoten	Overgeneralisation
-genootte	genoot	Irregular form plus regular suffix
-genootten	genoten	Irregular form plus regular suffix
-geniet	genoten	Overgeneralisation
-geniete	genotene	Overgeneralisation
-genieten	genoten	Wrong -en suffix
-genoot	genoten	Overgeneralisation
-enoten	genoten	Prefix ge without onset
-noten	genoten	Lacking ge prefix
-geefde	gaf	Overgeneralisation
-geefden	gaven	Overgeneralisation
-gafde	gaf	Irregular form plus regular suffix
-gafden	gaven	Irregular form plus regular suffix
-gegeefd	gegeven	Overgeneralisation
-egeefd	gegeven	Overgeneralisation+Prefix ge without onset
-geefd	gegeven	Overgeneralisation+Lacking ge prefix
-gegeefde	gegevene	Overgeneralisation+
-egeefde	gegevene	Overgeneralisation+Prefix ge without onset
-gegeeft	gegeven	Overgeneralisation
-egeeft	gegeven	Overgeneralisation
-geeft	gegeven	Overgeneralisation
-gegefen	gegeven	Wrong -en suffix
-egefen	gegeven	Wrong -en suffix
-gefen	gegeven	Wrong -en suffix
-egeven	gegeven	Prefix ge without onset
-geven	gegeven	Lacking ge prefix
-giette	goot	Overgeneralisation
-gietten	goten	Overgeneralisation
-gootte	goot	Irregular form plus regular suffix
-gootten	goten	Irregular form plus regular suffix
-gegiet	gegoten	Overgeneralisation
-egiet	gegoten	Overgeneralisation
-giet	gegoten	Overgeneralisation
-gegiete	gegotene	Overgeneralisation+
-egiete	gegotene	Overgeneralisation+Prefix ge without onset
-gegieten	gegoten	Wrong -en suffix
-egieten	gegoten	Wrong -en suffix
-gieten	gegoten	Wrong -en suffix
-gegoot	gegoten	Overgeneralisation
-egoten	gegoten	Prefix ge without onset
-goten	gegoten	Lacking ge prefix
-glijdde	gleed	Overgeneralisation
-glijdden	gleden	Overgeneralisation
-gleedde	gleed	Irregular form plus regular suffix
-gleedden	gleden	Irregular form plus regular suffix
-geglijd	gegleden	Overgeneralisation
-eglijd	gegleden	Overgeneralisation
-glijd	gegleden	Overgeneralisation
-geglijde	gegledene	Overgeneralisation+
-eglijde	gegledene	Overgeneralisation+Prefix ge without onset
-geglijden	gegleden	Wrong -en suffix
-eglijden	gegleden	Wrong -en suffix
-glijden	gegleden	Wrong -en suffix
-gegleed	gegleden	Overgeneralisation
-egleden	gegleden	Prefix ge without onset
-gleden	gegleden	Lacking ge prefix
-glimde	glom	Overgeneralisation
-glimden	glommen	Overgeneralisation
-glomde	glom	Irregular form plus regular suffix
-glomden	glommen	Irregular form plus regular suffix
-geglimd	geglommen	Overgeneralisation+
-eglimd	geglommen	Overgeneralisation+Prefix ge without onset
-glimd	geglommen	Overgeneralisation+Lacking ge prefix
-geglimde	geglommene	Overgeneralisation+
-eglimde	geglommene	Overgeneralisation+Prefix ge without onset
-geglimt	geglommen	Overgeneralisation
-eglimt	geglommen	Overgeneralisation
-glimt	geglommen	Overgeneralisation
-geglimmen	geglommen	Wrong -en suffix
-eglimmen	geglommen	Wrong -en suffix
-glimmen	geglommen	Wrong -en suffix
-geglomt	geglommen	Overgeneralisation
-eglommen	geglommen	Prefix ge without onset
-glommen	geglommen	Lacking ge prefix
-graafde	groef	Overgeneralisation
-graafden	groeven	Overgeneralisation
-groefde	groef	Irregular form plus regular suffix
-groefden	groeven	Irregular form plus regular suffix
-gegraafd	gegraven	Overgeneralisation
-egraafd	gegraven	Overgeneralisation+Prefix ge without onset
-graafd	gegraven	Overgeneralisation+Lacking ge prefix
-gegraafde	gegravene	Overgeneralisation+
-egraafde	gegravene	Overgeneralisation+Prefix ge without onset
-gegraaft	gegraven	Overgeneralisation
-egraaft	gegraven	Overgeneralisation
-graaft	gegraven	Overgeneralisation
-gegrafen	gegraven	Wrong -en suffix
-egrafen	gegraven	Wrong -en suffix
-grafen	gegraven	Wrong -en suffix
-egraven	gegraven	Prefix ge without onset
-graven	gegraven	Lacking ge prefix
-grijpte	greep	Overgeneralisation
-grijpten	grepen	Overgeneralisation
-greepte	greep	Irregular form plus regular suffix
-greepten	grepen	Irregular form plus regular suffix
-gegrijpt	gegrepen	Overgeneralisation
-egrijpt	gegrepen	Overgeneralisation
-grijpt	gegrepen	Overgeneralisation
-gegrijpte	gegrepene	Overgeneralisation+
-egrijpte	gegrepene	Overgeneralisation+Prefix ge without onset
-gegrijpen	gegrepen	Wrong -en suffix
-egrijpen	gegrepen	Wrong -en suffix
-grijpen	gegrepen	Wrong -en suffix
-gegreept	gegrepen	Overgeneralisation
-egrepen	gegrepen	Prefix ge without onset
-grepen	gegrepen	Lacking ge prefix
-hangde	hing	Overgeneralisation
-hangden	hingen	Overgeneralisation
-hingde	hing	Irregular form plus regular suffix
-hingden	hingen	Irregular form plus regular suffix
-gehangd	gehangen	Overgeneralisation
-ehangd	gehangen	Overgeneralisation+Prefix ge without onset
-hangd	gehangen	Overgeneralisation+Lacking ge prefix
-gehangde	gehangene	Overgeneralisation+
-ehangde	gehangene	Overgeneralisation+Prefix ge without onset
-gehangt	gehangen	Overgeneralisation
-ehangt	gehangen	Overgeneralisation
-hangt	gehangen	Overgeneralisation
-ehangen	gehangen	Prefix ge without onset
-hangen	gehangen	Lacking ge prefix
-hebde	had	Overgeneralisation
-hebden	hadden	Overgeneralisation
-hadde	had	Irregular form plus regular suffix
-gehebd	gehad	Overgeneralisation+
-ehebd	gehad	Overgeneralisation+Prefix ge without onset
-hebd	gehad	Overgeneralisation+Lacking ge prefix
-gehebde	gehade	Overgeneralisation+
-ehebde	gehade	Overgeneralisation+Prefix ge without onset
-gehebt	gehad	Overgeneralisation
-ehebt	gehad	Overgeneralisation
-hebt	gehad	Overgeneralisation
-gehebben	gehad	Wrong -en suffix
-ehebben	gehad	Wrong -en suffix
-hebben	gehad	Wrong -en suffix
-ehad	gehad	Prefix ge without onset
-had	gehad	Lacking ge prefix
-hefte	hief	Overgeneralisation
-heften	hieven	Overgeneralisation
-hiefte	hief	Irregular form plus regular suffix
-hieften	hieven	Irregular form plus regular suffix
-geheft	geheven	Overgeneralisation
-eheft	geheven	Overgeneralisation
-heft	geheven	Overgeneralisation
-gehefte	gehevene	Overgeneralisation+
-ehefte	gehevene	Overgeneralisation+Prefix ge without onset
-geheffen	geheven	Wrong -en suffix
-eheffen	geheven	Wrong -en suffix
-heffen	geheven	Wrong -en suffix
-geheefd	geheven	Overgeneralisation
-geheeft	geheven	Overgeneralisation
-eheven	geheven	Prefix ge without onset
-heven	geheven	Lacking ge prefix
-helpte	hielp	Overgeneralisation
-helpten	hielpen	Overgeneralisation
-hielpte	hielp	Irregular form plus regular suffix
-hielpten	hielpen	Irregular form plus regular suffix
-gehelpt	geholpen	Overgeneralisation
-ehelpt	geholpen	Overgeneralisation
-helpt	geholpen	Overgeneralisation
-gehelpte	geholpene	Overgeneralisation+
-ehelpte	geholpene	Overgeneralisation+Prefix ge without onset
-gehelpen	geholpen	Wrong -en suffix
-ehelpen	geholpen	Wrong -en suffix
-helpen	geholpen	Wrong -en suffix
-geholpt	geholpen	Overgeneralisation
-eholpen	geholpen	Prefix ge without onset
-holpen	geholpen	Lacking ge prefix
-geheet	geheten	Overgeneralisation
-eheet	geheten	Overgeneralisation
-heet	geheten	Overgeneralisation
-gehete	gehetene	Overgeneralisation+
-ehete	gehetene	Overgeneralisation+Prefix ge without onset
-eheten	geheten	Prefix ge without onset
-heten	geheten	Lacking ge prefix
-hijste	hees	Overgeneralisation
-hijsten	hesen	Overgeneralisation
-heeste	hees	Irregular form plus regular suffix
-heesten	hesen	Irregular form plus regular suffix
-gehijst	gehesen	Overgeneralisation
-ehijst	gehesen	Overgeneralisation
-hijst	gehesen	Overgeneralisation
-gehijste	gehesene	Overgeneralisation+
-ehijste	gehesene	Overgeneralisation+Prefix ge without onset
-gehijsen	gehesen	Wrong -en suffix
-ehijsen	gehesen	Wrong -en suffix
-hijsen	gehesen	Wrong -en suffix
-geheest	gehesen	Overgeneralisation
-ehesen	gehesen	Prefix ge without onset
-hesen	gehesen	Lacking ge prefix
-gehoefd	gehoeven	Overgeneralisation
-ehoefd	gehoeven	Overgeneralisation+Prefix ge without onset
-hoefd	gehoeven	Overgeneralisation+Lacking ge prefix
-gehoefde	gehoevene	Overgeneralisation+
-ehoefde	gehoevene	Overgeneralisation+Prefix ge without onset
-gehoeft	gehoeven	Overgeneralisation
-ehoeft	gehoeven	Overgeneralisation
-hoeft	gehoeven	Overgeneralisation
-gehoefen	gehoeven	Wrong -en suffix
-ehoefen	gehoeven	Wrong -en suffix
-hoefen	gehoeven	Wrong -en suffix
-ehoeven	gehoeven	Prefix ge without onset
-hoeven	gehoeven	Lacking ge prefix
-houdde	hield	Overgeneralisation
-houdden	hielden	Overgeneralisation
-hieldde	hield	Irregular form plus regular suffix
-hieldden	hielden	Irregular form plus regular suffix
-gehoud	gehouden	Overgeneralisation
-ehoud	gehouden	Overgeneralisation
-houd	gehouden	Overgeneralisation
-gehoude	gehoudene	Overgeneralisation+
-ehoude	gehoudene	Overgeneralisation+Prefix ge without onset
-ehouden	gehouden	Prefix ge without onset
-houden	gehouden	Lacking ge prefix
-houwde	hieuw	Overgeneralisation
-houwden	hieuwen	Overgeneralisation
-hieuwde	hieuw	Irregular form plus regular suffix
-hieuwden	hieuwen	Irregular form plus regular suffix
-gehouwd	gehouwen	Overgeneralisation
-ehouwd	gehouwen	Overgeneralisation+Prefix ge without onset
-houwd	gehouwen	Overgeneralisation+Lacking ge prefix
-gehouwde	gehouwene	Overgeneralisation+
-ehouwde	gehouwene	Overgeneralisation+Prefix ge without onset
-gehouwt	gehouwen	Overgeneralisation
-ehouwt	gehouwen	Overgeneralisation
-houwt	gehouwen	Overgeneralisation
-ehouwen	gehouwen	Prefix ge without onset
-houwen	gehouwen	Lacking ge prefix
-ejaagd	gejaagd	Prefix ge without onset
-jaagd	gejaagd	Lacking ge prefix
-ejaagde	gejaagde	Overgeneralisation+Prefix ge without onset
-gejaagt	gejaagd	Overgeneralisation
-ejaagt	gejaagd	Overgeneralisation
-jaagt	gejaagd	Overgeneralisation
-gejagen	gejaagd	Wrong -en suffix
-ejagen	gejaagd	Wrong -en suffix
-jagen	gejaagd	Wrong -en suffix
-kiesde	koos	Overgeneralisation
-kiesden	kozen	Overgeneralisation
-koosde	koos	Irregular form plus regular suffix
-koosden	kozen	Irregular form plus regular suffix
-gekiesd	gekozen	Overgeneralisation+
-ekiesd	gekozen	Overgeneralisation+Prefix ge without onset
-kiesd	gekozen	Overgeneralisation+Lacking ge prefix
-gekiesde	gekozene	Overgeneralisation+
-ekiesde	gekozene	Overgeneralisation+Prefix ge without onset
-gekiest	gekozen	Overgeneralisation
-ekiest	gekozen	Overgeneralisation
-kiest	gekozen	Overgeneralisation
-gekiesen	gekozen	Wrong -en suffix
-ekiesen	gekozen	Wrong -en suffix
-kiesen	gekozen	Wrong -en suffix
-gekoost	gekozen	Overgeneralisation
-ekozen	gekozen	Prefix ge without onset
-kozen	gekozen	Lacking ge prefix
-kijkte	keek	Overgeneralisation
-kijkten	keken	Overgeneralisation
-keekte	keek	Irregular form plus regular suffix
-keekten	keken	Irregular form plus regular suffix
-gekijkt	gekeken	Overgeneralisation
-ekijkt	gekeken	Overgeneralisation
-kijkt	gekeken	Overgeneralisation
-gekijkte	gekekene	Overgeneralisation+
-ekijkte	gekekene	Overgeneralisation+Prefix ge without onset
-gekijken	gekeken	Wrong -en suffix
-ekijken	gekeken	Wrong -en suffix
-kijken	gekeken	Wrong -en suffix
-gekeekt	gekeken	Overgeneralisation
-ekeken	gekeken	Prefix ge without onset
-keken	gekeken	Lacking ge prefix
-klimde	klom	Overgeneralisation
-klimden	klommen	Overgeneralisation
-klomde	klom	Irregular form plus regular suffix
-klomden	klommen	Irregular form plus regular suffix
-geklimd	geklommen	Overgeneralisation+
-eklimd	geklommen	Overgeneralisation+Prefix ge without onset
-klimd	geklommen	Overgeneralisation+Lacking ge prefix
-geklimde	geklommene	Overgeneralisation+
-eklimde	geklommene	Overgeneralisation+Prefix ge without onset
-geklimt	geklommen	Overgeneralisation
-eklimt	geklommen	Overgeneralisation
-klimt	geklommen	Overgeneralisation
-geklimmen	geklommen	Wrong -en suffix
-eklimmen	geklommen	Wrong -en suffix
-klimmen	geklommen	Wrong -en suffix
-geklomt	geklommen	Overgeneralisation
-eklommen	geklommen	Prefix ge without onset
-klommen	geklommen	Lacking ge prefix
-klinkte	klonk	Overgeneralisation
-klinkten	klonken	Overgeneralisation
-klonkte	klonk	Irregular form plus regular suffix
-klonkten	klonken	Irregular form plus regular suffix
-geklinkt	geklonken	Overgeneralisation
-eklinkt	geklonken	Overgeneralisation
-klinkt	geklonken	Overgeneralisation
-geklinkte	geklonkene	Overgeneralisation+
-eklinkte	geklonkene	Overgeneralisation+Prefix ge without onset
-geklinken	geklonken	Wrong -en suffix
-eklinken	geklonken	Wrong -en suffix
-klinken	geklonken	Wrong -en suffix
-geklonkt	geklonken	Overgeneralisation
-eklonken	geklonken	Prefix ge without onset
-klonken	geklonken	Lacking ge prefix
-kluifde	kloof	Overgeneralisation
-kluifden	kloven	Overgeneralisation
-kloofde	kloof	Irregular form plus regular suffix
-kloofden	kloven	Irregular form plus regular suffix
-gekluifd	gekloven	Overgeneralisation+
-ekluifd	gekloven	Overgeneralisation+Prefix ge without onset
-kluifd	gekloven	Overgeneralisation+Lacking ge prefix
-gekluifde	geklovene	Overgeneralisation+
-ekluifde	geklovene	Overgeneralisation+Prefix ge without onset
-gekluift	gekloven	Overgeneralisation
-ekluift	gekloven	Overgeneralisation
-kluift	gekloven	Overgeneralisation
-gekluifen	gekloven	Wrong -en suffix
-ekluifen	gekloven	Wrong -en suffix
-kluifen	gekloven	Wrong -en suffix
-geklooft	gekloven	Overgeneralisation
-ekloven	gekloven	Prefix ge without onset
-kloven	gekloven	Lacking ge prefix
-knijpte	kneep	Overgeneralisation
-knijpten	knepen	Overgeneralisation
-kneepte	kneep	Irregular form plus regular suffix
-kneepten	knepen	Irregular form plus regular suffix
-geknijpt	geknepen	Overgeneralisation
-eknijpt	geknepen	Overgeneralisation
-knijpt	geknepen	Overgeneralisation
-geknijpte	geknepene	Overgeneralisation+
-eknijpte	geknepene	Overgeneralisation+Prefix ge without onset
-geknijpen	geknepen	Wrong -en suffix
-eknijpen	geknepen	Wrong -en suffix
-knijpen	geknepen	Wrong -en suffix
-gekneept	geknepen	Overgeneralisation
-eknepen	geknepen	Prefix ge without onset
-knepen	geknepen	Lacking ge prefix
-koopte	kocht	Overgeneralisation
-koopten	kochten	Overgeneralisation
-kochtte	kocht	Irregular form plus regular suffix
-kochtten	kochten	Irregular form plus regular suffix
-gekoopt	gekocht	Overgeneralisation
-ekoopt	gekocht	Overgeneralisation
-koopt	gekocht	Overgeneralisation
-gekoopte	gekochte	Overgeneralisation+
-ekoopte	gekochte	Overgeneralisation+Prefix ge without onset
-gekopen	gekocht	Wrong -en suffix
-ekopen	gekocht	Wrong -en suffix
-kopen	gekocht	Wrong -en suffix
-ekocht	gekocht	Prefix ge without onset
-kocht	gekocht	Lacking ge prefix
-krijgde	kreeg	Overgeneralisation
-krijgden	kregen	Overgeneralisation
-kreegde	kreeg	Irregular form plus regular suffix
-kreegden	kregen	Irregular form plus regular suffix
-gekrijgd	gekregen	Overgeneralisation+
-ekrijgd	gekregen	Overgeneralisation+Prefix ge without onset
-krijgd	gekregen	Overgeneralisation+Lacking ge prefix
-gekrijgde	gekregene	Overgeneralisation+
-ekrijgde	gekregene	Overgeneralisation+Prefix ge without onset
-gekrijgt	gekregen	Overgeneralisation
-ekrijgt	gekregen	Overgeneralisation
-krijgt	gekregen	Overgeneralisation
-gekrijgen	gekregen	Wrong -en suffix
-ekrijgen	gekregen	Wrong -en suffix
-krijgen	gekregen	Wrong -en suffix
-gekreegd	gekregen	Overgeneralisation
-gekreegt	gekregen	Overgeneralisation
-ekregen	gekregen	Prefix ge without onset
-kregen	gekregen	Lacking ge prefix
-krimpte	kromp	Overgeneralisation
-krimpten	krompen	Overgeneralisation
-krompte	kromp	Irregular form plus regular suffix
-krompten	krompen	Irregular form plus regular suffix
-gekrimpt	gekrompen	Overgeneralisation
-ekrimpt	gekrompen	Overgeneralisation
-krimpt	gekrompen	Overgeneralisation
-gekrimpte	gekrompene	Overgeneralisation+
-ekrimpte	gekrompene	Overgeneralisation+Prefix ge without onset
-gekrimpen	gekrompen	Wrong -en suffix
-ekrimpen	gekrompen	Wrong -en suffix
-krimpen	gekrompen	Wrong -en suffix
-gekrompt	gekrompen	Overgeneralisation
-ekrompen	gekrompen	Prefix ge without onset
-krompen	gekrompen	Lacking ge prefix
-kruipte	kroop	Overgeneralisation
-kruipten	kropen	Overgeneralisation
-kroopte	kroop	Irregular form plus regular suffix
-kroopten	kropen	Irregular form plus regular suffix
-gekruipt	gekropen	Overgeneralisation
-ekruipt	gekropen	Overgeneralisation
-kruipt	gekropen	Overgeneralisation
-gekruipte	gekropene	Overgeneralisation+
-ekruipte	gekropene	Overgeneralisation+Prefix ge without onset
-gekruipen	gekropen	Wrong -en suffix
-ekruipen	gekropen	Wrong -en suffix
-kruipen	gekropen	Wrong -en suffix
-gekroopt	gekropen	Overgeneralisation
-ekropen	gekropen	Prefix ge without onset
-kropen	gekropen	Lacking ge prefix
-kwijtte	kweet	Overgeneralisation
-kwijtten	kweten	Overgeneralisation
-kweette	kweet	Irregular form plus regular suffix
-kweetten	kweten	Irregular form plus regular suffix
-gekwijt	gekweten	Overgeneralisation
-ekwijt	gekweten	Overgeneralisation
-kwijt	gekweten	Overgeneralisation
-gekwijte	gekwetene	Overgeneralisation+
-ekwijte	gekwetene	Overgeneralisation+Prefix ge without onset
-gekwijten	gekweten	Wrong -en suffix
-ekwijten	gekweten	Wrong -en suffix
-kwijten	gekweten	Wrong -en suffix
-gekweet	gekweten	Overgeneralisation
-ekweten	gekweten	Prefix ge without onset
-kweten	gekweten	Lacking ge prefix
-lachde	lachte	Overgeneralisation
-lachden	lachten	Overgeneralisation
-gelachd	gelachen	Overgeneralisation
-elachd	gelachen	Overgeneralisation+Prefix ge without onset
-lachd	gelachen	Overgeneralisation+Lacking ge prefix
-gelachde	gelachene	Overgeneralisation+
-elachde	gelachene	Overgeneralisation+Prefix ge without onset
-gelacht	gelachen	Overgeneralisation
-elacht	gelachen	Overgeneralisation
-lacht	gelachen	Overgeneralisation
-elachen	gelachen	Prefix ge without onset
-lachen	gelachen	Lacking ge prefix
-gelaad	geladen	Overgeneralisation
-elaad	geladen	Overgeneralisation
-laad	geladen	Overgeneralisation
-gelade	geladene	Overgeneralisation+
-elade	geladene	Overgeneralisation+Prefix ge without onset
-eladen	geladen	Prefix ge without onset
-laden	geladen	Lacking ge prefix
-laatte	liet	Overgeneralisation
-laatten	lieten	Overgeneralisation
-liette	liet	Irregular form plus regular suffix
-lietten	lieten	Irregular form plus regular suffix
-gelaat	gelaten	Overgeneralisation
-elaat	gelaten	Overgeneralisation
-laat	gelaten	Overgeneralisation
-gelate	gelatene	Overgeneralisation+
-elate	gelatene	Overgeneralisation+Prefix ge without onset
-elaten	gelaten	Prefix ge without onset
-laten	gelaten	Lacking ge prefix
-leesde	las	Overgeneralisation
-leesden	lazen	Overgeneralisation
-lasde	las	Irregular form plus regular suffix
-lasden	lazen	Irregular form plus regular suffix
-geleesd	gelezen	Overgeneralisation
-eleesd	gelezen	Overgeneralisation+Prefix ge without onset
-leesd	gelezen	Overgeneralisation+Lacking ge prefix
-geleesde	gelezene	Overgeneralisation+
-eleesde	gelezene	Overgeneralisation+Prefix ge without onset
-geleest	gelezen	Overgeneralisation
-eleest	gelezen	Overgeneralisation
-leest	gelezen	Overgeneralisation
-gelesen	gelezen	Wrong -en suffix
-elesen	gelezen	Wrong -en suffix
-lesen	gelezen	Wrong -en suffix
-elezen	gelezen	Prefix ge without onset
-lezen	gelezen	Lacking ge prefix
-liegde	loog	Overgeneralisation
-liegden	logen	Overgeneralisation
-loogde	loog	Irregular form plus regular suffix
-loogden	logen	Irregular form plus regular suffix
-geliegd	gelogen	Overgeneralisation+
-eliegd	gelogen	Overgeneralisation+Prefix ge without onset
-liegd	gelogen	Overgeneralisation+Lacking ge prefix
-geliegde	gelogene	Overgeneralisation+
-eliegde	gelogene	Overgeneralisation+Prefix ge without onset
-geliegt	gelogen	Overgeneralisation
-eliegt	gelogen	Overgeneralisation
-liegt	gelogen	Overgeneralisation
-geliegen	gelogen	Wrong -en suffix
-eliegen	gelogen	Wrong -en suffix
-liegen	gelogen	Wrong -en suffix
-geloogt	gelogen	Overgeneralisation
-elogen	gelogen	Prefix ge without onset
-logen	gelogen	Lacking ge prefix
-ligde	lag	Overgeneralisation
-ligden	lagen	Overgeneralisation
-lagde	lag	Irregular form plus regular suffix
-lagden	lagen	Irregular form plus regular suffix
-geligd	gelegen	Overgeneralisation+
-eligd	gelegen	Overgeneralisation+Prefix ge without onset
-ligd	gelegen	Overgeneralisation+Lacking ge prefix
-geligde	gelegene	Overgeneralisation+
-eligde	gelegene	Overgeneralisation+Prefix ge without onset
-geligt	gelegen	Overgeneralisation
-eligt	gelegen	Overgeneralisation
-ligt	gelegen	Overgeneralisation
-geliggen	gelegen	Wrong -en suffix
-eliggen	gelegen	Wrong -en suffix
-liggen	gelegen	Wrong -en suffix
-geleegd	gelegen	Overgeneralisation
-geleegt	gelegen	Overgeneralisation
-elegen	gelegen	Prefix ge without onset
-legen	gelegen	Lacking ge prefix
-lijdde	leed	Overgeneralisation
-lijdden	leden	Overgeneralisation
-leedde	leed	Irregular form plus regular suffix
-leedden	leden	Irregular form plus regular suffix
-gelijd	geleden	Overgeneralisation
-elijd	geleden	Overgeneralisation
-lijd	geleden	Overgeneralisation
-gelijde	geledene	Overgeneralisation+
-elijde	geledene	Overgeneralisation+Prefix ge without onset
-gelijden	geleden	Wrong -en suffix
-elijden	geleden	Wrong -en suffix
-lijden	geleden	Wrong -en suffix
-geleed	geleden	Overgeneralisation
-eleden	geleden	Prefix ge without onset
-leden	geleden	Lacking ge prefix
-lijkte	leek	Overgeneralisation
-lijkten	leken	Overgeneralisation
-leekte	leek	Irregular form plus regular suffix
-leekten	leken	Irregular form plus regular suffix
-gelijkt	geleken	Overgeneralisation
-elijkt	geleken	Overgeneralisation
-lijkt	geleken	Overgeneralisation
-gelijkte	gelekene	Overgeneralisation+
-elijkte	gelekene	Overgeneralisation+Prefix ge without onset
-gelijken	geleken	Wrong -en suffix
-elijken	geleken	Wrong -en suffix
-lijken	geleken	Wrong -en suffix
-geleekt	geleken	Overgeneralisation
-eleken	geleken	Prefix ge without onset
-leken	geleken	Lacking ge prefix
-loopte	liep	Overgeneralisation
-loopten	liepen	Overgeneralisation
-liepte	liep	Irregular form plus regular suffix
-liepten	liepen	Irregular form plus regular suffix
-geloopt	gelopen	Overgeneralisation
-eloopt	gelopen	Overgeneralisation
-loopt	gelopen	Overgeneralisation
-geloopte	gelopene	Overgeneralisation+
-eloopte	gelopene	Overgeneralisation+Prefix ge without onset
-elopen	gelopen	Prefix ge without onset
-lopen	gelopen	Lacking ge prefix
-gemaald	gemalen	Overgeneralisation
-emaald	gemalen	Overgeneralisation+Prefix ge without onset
-maald	gemalen	Overgeneralisation+Lacking ge prefix
-gemaalde	gemalene	Overgeneralisation+
-emaalde	gemalene	Overgeneralisation+Prefix ge without onset
-gemaalt	gemalen	Overgeneralisation
-emaalt	gemalen	Overgeneralisation
-maalt	gemalen	Overgeneralisation
-emalen	gemalen	Prefix ge without onset
-malen	gemalen	Lacking ge prefix
-emelkt	gemelkt	Prefix ge without onset
-melkt	gemelkt	Lacking ge prefix
-emelkte	gemelkte	Overgeneralisation+Prefix ge without onset
-gemelken	gemelkt	Wrong -en suffix
-emelken	gemelkt	Wrong -en suffix
-melken	gemelkt	Wrong -en suffix
-meette	mat	Overgeneralisation
-meetten	maten	Overgeneralisation
-matte	mat	Irregular form plus regular suffix
-matten	maten	Irregular form plus regular suffix
-gemeet	gemeten	Overgeneralisation
-emeet	gemeten	Overgeneralisation
-meet	gemeten	Overgeneralisation
-gemete	gemetene	Overgeneralisation+
-emete	gemetene	Overgeneralisation+Prefix ge without onset
-emeten	gemeten	Prefix ge without onset
-meten	gemeten	Lacking ge prefix
-mijdde	meed	Overgeneralisation
-mijdden	meden	Overgeneralisation
-meedde	meed	Irregular form plus regular suffix
-meedden	meden	Irregular form plus regular suffix
-gemijd	gemeden	Overgeneralisation
-emijd	gemeden	Overgeneralisation
-mijd	gemeden	Overgeneralisation
-gemijde	gemedene	Overgeneralisation+
-emijde	gemedene	Overgeneralisation+Prefix ge without onset
-gemijden	gemeden	Wrong -en suffix
-emijden	gemeden	Wrong -en suffix
-mijden	gemeden	Wrong -en suffix
-gemeed	gemeden	Overgeneralisation
-emeden	gemeden	Prefix ge without onset
-meden	gemeden	Lacking ge prefix
-moette	moest	Overgeneralisation
-moetten	moesten	Overgeneralisation
-moestte	moest	Irregular form plus regular suffix
-moestten	moesten	Irregular form plus regular suffix
-gemoet	gemoeten	Overgeneralisation
-emoet	gemoeten	Overgeneralisation
-moet	gemoeten	Overgeneralisation
-gemoete	gemoetene	Overgeneralisation+
-emoete	gemoetene	Overgeneralisation+Prefix ge without onset
-emoeten	gemoeten	Prefix ge without onset
-moeten	gemoeten	Lacking ge prefix
-neemde	nam	Overgeneralisation
-neemden	namen	Overgeneralisation
-namde	nam	Irregular form plus regular suffix
-namden	namen	Irregular form plus regular suffix
-geneemd	genomen	Overgeneralisation+
-eneemd	genomen	Overgeneralisation+Prefix ge without onset
-neemd	genomen	Overgeneralisation+Lacking ge prefix
-geneemde	genomene	Overgeneralisation+
-eneemde	genomene	Overgeneralisation+Prefix ge without onset
-geneemt	genomen	Overgeneralisation
-eneemt	genomen	Overgeneralisation
-neemt	genomen	Overgeneralisation
-genemen	genomen	Wrong -en suffix
-enemen	genomen	Wrong -en suffix
-nemen	genomen	Wrong -en suffix
-genoomt	genomen	Overgeneralisation
-enomen	genomen	Prefix ge without onset
-nomen	genomen	Lacking ge prefix
-nijgde	neeg	Overgeneralisation
-nijgden	negen	Overgeneralisation
-neegde	neeg	Irregular form plus regular suffix
-neegden	negen	Irregular form plus regular suffix
-genijgd	genegen	Overgeneralisation+
-enijgd	genegen	Overgeneralisation+Prefix ge without onset
-nijgd	genegen	Overgeneralisation+Lacking ge prefix
-genijgde	genegene	Overgeneralisation+
-enijgde	genegene	Overgeneralisation+Prefix ge without onset
-genijgt	genegen	Overgeneralisation
-enijgt	genegen	Overgeneralisation
-nijgt	genegen	Overgeneralisation
-genijgen	genegen	Wrong -en suffix
-enijgen	genegen	Wrong -en suffix
-nijgen	genegen	Wrong -en suffix
-geneegd	genegen	Overgeneralisation
-geneegt	genegen	Overgeneralisation
-enegen	genegen	Prefix ge without onset
-negen	genegen	Lacking ge prefix
-ontginde	ontgonnene	Overgeneralisation
-ontginden	ontgonnen	Overgeneralisation
-ontgonde	ontgon	Irregular form plus regular suffix
-ontgonden	ontgonnen	Irregular form plus regular suffix
-ontgind	ontgonnen	Overgeneralisation
-ontgint	ontgonnen	Overgeneralisation
-ontginnen	ontgonnen	Wrong -en suffix
-ontgont	ontgonnen	Overgeneralisation
-ontluikte	ontlokene	Overgeneralisation
-ontluikten	ontloken	Overgeneralisation
-ontlookte	ontlook	Irregular form plus regular suffix
-ontlookten	ontloken	Irregular form plus regular suffix
-ontluikt	ontloken	Overgeneralisation
-ontluiken	ontloken	Wrong -en suffix
-ontlookt	ontloken	Overgeneralisation
-pluisde	ploos	Overgeneralisation
-pluisden	plozen	Overgeneralisation
-ploosde	ploos	Irregular form plus regular suffix
-ploosden	plozen	Irregular form plus regular suffix
-gepluisd	geplozen	Overgeneralisation+
-epluisd	geplozen	Overgeneralisation+Prefix ge without onset
-pluisd	geplozen	Overgeneralisation+Lacking ge prefix
-gepluisde	geplozene	Overgeneralisation+
-epluisde	geplozene	Overgeneralisation+Prefix ge without onset
-gepluist	geplozen	Overgeneralisation
-epluist	geplozen	Overgeneralisation
-pluist	geplozen	Overgeneralisation
-gepluisen	geplozen	Wrong -en suffix
-epluisen	geplozen	Wrong -en suffix
-pluisen	geplozen	Wrong -en suffix
-geploost	geplozen	Overgeneralisation
-eplozen	geplozen	Prefix ge without onset
-plozen	geplozen	Lacking ge prefix
-prijsde	prees	Overgeneralisation
-prijsden	prezen	Overgeneralisation
-preesde	prees	Irregular form plus regular suffix
-preesden	prezen	Irregular form plus regular suffix
-geprijsd	geprezen	Overgeneralisation+
-eprijsd	geprezen	Overgeneralisation+Prefix ge without onset
-prijsd	geprezen	Overgeneralisation+Lacking ge prefix
-geprijsde	geprezene	Overgeneralisation+
-eprijsde	geprezene	Overgeneralisation+Prefix ge without onset
-geprijst	geprezen	Overgeneralisation
-eprijst	geprezen	Overgeneralisation
-prijst	geprezen	Overgeneralisation
-geprijsen	geprezen	Wrong -en suffix
-eprijsen	geprezen	Wrong -en suffix
-prijsen	geprezen	Wrong -en suffix
-gepreesd	geprezen	Overgeneralisation
-gepreest	geprezen	Overgeneralisation
-eprezen	geprezen	Prefix ge without onset
-prezen	geprezen	Lacking ge prefix
-geraad	geraden	Overgeneralisation
-eraad	geraden	Overgeneralisation
-raad	geraden	Overgeneralisation
-gerade	geradene	Overgeneralisation+
-erade	geradene	Overgeneralisation+Prefix ge without onset
-eraden	geraden	Prefix ge without onset
-raden	geraden	Lacking ge prefix
-verraad	verraden	Overgeneralisation
-verrade	verradene	Overgeneralisation
-rijdde	reed	Overgeneralisation
-rijdden	reden	Overgeneralisation
-reedde	reed	Irregular form plus regular suffix
-reedden	reden	Irregular form plus regular suffix
-gerijd	gereden	Overgeneralisation
-erijd	gereden	Overgeneralisation
-rijd	gereden	Overgeneralisation
-gerijde	geredene	Overgeneralisation+
-erijde	geredene	Overgeneralisation+Prefix ge without onset
-gerijden	gereden	Wrong -en suffix
-erijden	gereden	Wrong -en suffix
-rijden	gereden	Wrong -en suffix
-gereed	gereden	Overgeneralisation
-ereden	gereden	Prefix ge without onset
-reden	gereden	Lacking ge prefix
-rijgde	reeg	Overgeneralisation
-rijgden	regen	Overgeneralisation
-reegde	reeg	Irregular form plus regular suffix
-reegden	regen	Irregular form plus regular suffix
-gerijgd	geregen	Overgeneralisation+
-erijgd	geregen	Overgeneralisation+Prefix ge without onset
-rijgd	geregen	Overgeneralisation+Lacking ge prefix
-gerijgde	geregene	Overgeneralisation+
-erijgde	geregene	Overgeneralisation+Prefix ge without onset
-gerijgt	geregen	Overgeneralisation
-erijgt	geregen	Overgeneralisation
-rijgt	geregen	Overgeneralisation
-gerijgen	geregen	Wrong -en suffix
-erijgen	geregen	Wrong -en suffix
-rijgen	geregen	Wrong -en suffix
-gereegd	geregen	Overgeneralisation
-gereegt	geregen	Overgeneralisation
-eregen	geregen	Prefix ge without onset
-regen	geregen	Lacking ge prefix
-rijtte	reet	Overgeneralisation
-rijtten	reten	Overgeneralisation
-reette	reet	Irregular form plus regular suffix
-reetten	reten	Irregular form plus regular suffix
-gerijt	gereten	Overgeneralisation
-erijt	gereten	Overgeneralisation
-rijt	gereten	Overgeneralisation
-gerijte	geretene	Overgeneralisation+
-erijte	geretene	Overgeneralisation+Prefix ge without onset
-gerijten	gereten	Wrong -en suffix
-erijten	gereten	Wrong -en suffix
-rijten	gereten	Wrong -en suffix
-gereet	gereten	Overgeneralisation
-ereten	gereten	Prefix ge without onset
-reten	gereten	Lacking ge prefix
-rijsde	rees	Overgeneralisation
-rijsden	rezen	Overgeneralisation
-reesde	rees	Irregular form plus regular suffix
-reesden	rezen	Irregular form plus regular suffix
-gerijsd	Gerezen	Overgeneralisation+
-erijsd	Gerezen	Overgeneralisation+Prefix ge without onset
-rijsd	Gerezen	Overgeneralisation+Lacking ge prefix
-gerijsde	Gerezene	Overgeneralisation+
-erijsde	Gerezene	Overgeneralisation+Prefix ge without onset
-gerijst	Gerezen	Overgeneralisation
-erijst	Gerezen	Overgeneralisation
-rijst	Gerezen	Overgeneralisation
-gerijsen	Gerezen	Wrong -en suffix
-erijsen	Gerezen	Wrong -en suffix
-rijsen	Gerezen	Wrong -en suffix
-geGereesd	Gerezen	Overgeneralisation
-geGereest	Gerezen	Overgeneralisation
-roepte	riep	Overgeneralisation
-roepten	riepen	Overgeneralisation
-riepte	riep	Irregular form plus regular suffix
-riepten	riepen	Irregular form plus regular suffix
-geroept	geroepen	Overgeneralisation
-eroept	geroepen	Overgeneralisation
-roept	geroepen	Overgeneralisation
-geroepte	geroepene	Overgeneralisation+
-eroepte	geroepene	Overgeneralisation+Prefix ge without onset
-eroepen	geroepen	Prefix ge without onset
-roepen	geroepen	Lacking ge prefix
-ruikte	rook	Overgeneralisation
-ruikten	roken	Overgeneralisation
-rookte	rook	Irregular form plus regular suffix
-rookten	roken	Irregular form plus regular suffix
-geruikt	geroken	Overgeneralisation
-eruikt	geroken	Overgeneralisation
-ruikt	geroken	Overgeneralisation
-geruikte	gerokene	Overgeneralisation+
-eruikte	gerokene	Overgeneralisation+Prefix ge without onset
-geruiken	geroken	Wrong -en suffix
-eruiken	geroken	Wrong -en suffix
-ruiken	geroken	Wrong -en suffix
-gerookt	geroken	Overgeneralisation
-eroken	geroken	Prefix ge without onset
-roken	geroken	Lacking ge prefix
-gescheid	gescheiden	Overgeneralisation
-escheid	gescheiden	Overgeneralisation
-scheid	gescheiden	Overgeneralisation
-gescheide	gescheidene	Overgeneralisation+
-escheide	gescheidene	Overgeneralisation+Prefix ge without onset
-escheiden	gescheiden	Prefix ge without onset
-scheiden	gescheiden	Lacking ge prefix
-scheldde	schold	Overgeneralisation
-scheldden	scholden	Overgeneralisation
-scholdde	schold	Irregular form plus regular suffix
-scholdden	scholden	Irregular form plus regular suffix
-gescheld	gescholden	Overgeneralisation
-escheld	gescholden	Overgeneralisation
-scheld	gescholden	Overgeneralisation
-geschelde	gescholdene	Overgeneralisation+
-eschelde	gescholdene	Overgeneralisation+Prefix ge without onset
-geschelden	gescholden	Wrong -en suffix
-eschelden	gescholden	Wrong -en suffix
-schelden	gescholden	Wrong -en suffix
-geschold	gescholden	Overgeneralisation
-escholden	gescholden	Prefix ge without onset
-scholden	gescholden	Lacking ge prefix
-schendde	schond	Overgeneralisation
-schendden	schonden	Overgeneralisation
-schondde	schond	Irregular form plus regular suffix
-schondden	schonden	Irregular form plus regular suffix
-geschend	geschonden	Overgeneralisation
-eschend	geschonden	Overgeneralisation
-schend	geschonden	Overgeneralisation
-geschende	geschondene	Overgeneralisation+
-eschende	geschondene	Overgeneralisation+Prefix ge without onset
-geschenden	geschonden	Wrong -en suffix
-eschenden	geschonden	Wrong -en suffix
-schenden	geschonden	Wrong -en suffix
-geschond	geschonden	Overgeneralisation
-eschonden	geschonden	Prefix ge without onset
-schonden	geschonden	Lacking ge prefix
-schenkte	schonk	Overgeneralisation
-schenkten	schonken	Overgeneralisation
-schonkte	schonk	Irregular form plus regular suffix
-schonkten	schonken	Irregular form plus regular suffix
-geschenkt	geschonken	Overgeneralisation
-eschenkt	geschonken	Overgeneralisation
-schenkt	geschonken	Overgeneralisation
-geschenkte	geschonkene	Overgeneralisation+
-eschenkte	geschonkene	Overgeneralisation+Prefix ge without onset
-geschenken	geschonken	Wrong -en suffix
-eschenken	geschonken	Wrong -en suffix
-schenken	geschonken	Wrong -en suffix
-geschonkt	geschonken	Overgeneralisation
-eschonken	geschonken	Prefix ge without onset
-schonken	geschonken	Lacking ge prefix
-schepte	shiep	Overgeneralisation
-schepten	schiepen	Overgeneralisation
-shiepte	shiep	Irregular form plus regular suffix
-shiepten	schiepen	Irregular form plus regular suffix
-geschept	geschapen	Overgeneralisation
-eschept	geschapen	Overgeneralisation
-schept	geschapen	Overgeneralisation
-geschepte	geschapene	Overgeneralisation+
-eschepte	geschapene	Overgeneralisation+Prefix ge without onset
-gescheppen	geschapen	Wrong -en suffix
-escheppen	geschapen	Wrong -en suffix
-scheppen	geschapen	Wrong -en suffix
-geschaapt	geschapen	Overgeneralisation
-eschapen	geschapen	Prefix ge without onset
-schapen	geschapen	Lacking ge prefix
-gescheerd	geschoren	Overgeneralisation+
-escheerd	geschoren	Overgeneralisation+Prefix ge without onset
-scheerd	geschoren	Overgeneralisation+Lacking ge prefix
-gescheerde	geschorene	Overgeneralisation+
-escheerde	geschorene	Overgeneralisation+Prefix ge without onset
-gescheert	geschoren	Overgeneralisation
-escheert	geschoren	Overgeneralisation
-scheert	geschoren	Overgeneralisation
-gescheren	geschoren	Wrong -en suffix
-escheren	geschoren	Wrong -en suffix
-scheren	geschoren	Wrong -en suffix
-geschoort	geschoren	Overgeneralisation
-eschoren	geschoren	Prefix ge without onset
-schoren	geschoren	Lacking ge prefix
-schiette	schoot	Overgeneralisation
-schietten	schoten	Overgeneralisation
-schootte	schoot	Irregular form plus regular suffix
-schootten	schoten	Irregular form plus regular suffix
-geschiet	geschoten	Overgeneralisation
-eschiet	geschoten	Overgeneralisation
-schiet	geschoten	Overgeneralisation
-geschiete	geschotene	Overgeneralisation+
-eschiete	geschotene	Overgeneralisation+Prefix ge without onset
-geschieten	geschoten	Wrong -en suffix
-eschieten	geschoten	Wrong -en suffix
-schieten	geschoten	Wrong -en suffix
-geschoot	geschoten	Overgeneralisation
-eschoten	geschoten	Prefix ge without onset
-schoten	geschoten	Lacking ge prefix
-schijnde	scheen	Overgeneralisation
-schijnden	schenen	Overgeneralisation
-scheende	scheen	Irregular form plus regular suffix
-scheenden	schenen	Irregular form plus regular suffix
-geschijnd	geschenen	Overgeneralisation+
-eschijnd	geschenen	Overgeneralisation+Prefix ge without onset
-schijnd	geschenen	Overgeneralisation+Lacking ge prefix
-geschijnde	geschenene	Overgeneralisation+
-eschijnde	geschenene	Overgeneralisation+Prefix ge without onset
-geschijnt	geschenen	Overgeneralisation
-eschijnt	geschenen	Overgeneralisation
-schijnt	geschenen	Overgeneralisation
-geschijnen	geschenen	Wrong -en suffix
-eschijnen	geschenen	Wrong -en suffix
-schijnen	geschenen	Wrong -en suffix
-gescheend	geschenen	Overgeneralisation
-gescheent	geschenen	Overgeneralisation
-eschenen	geschenen	Prefix ge without onset
-schenen	geschenen	Lacking ge prefix
-schijtte	scheet	Overgeneralisation
-schijtten	scheten	Overgeneralisation
-scheette	scheet	Irregular form plus regular suffix
-scheetten	scheten	Irregular form plus regular suffix
-geschijt	gescheten	Overgeneralisation
-eschijt	gescheten	Overgeneralisation
-schijt	gescheten	Overgeneralisation
-geschijte	geschetene	Overgeneralisation+
-eschijte	geschetene	Overgeneralisation+Prefix ge without onset
-geschijten	gescheten	Wrong -en suffix
-eschijten	gescheten	Wrong -en suffix
-schijten	gescheten	Wrong -en suffix
-gescheet	gescheten	Overgeneralisation
-escheten	gescheten	Prefix ge without onset
-scheten	gescheten	Lacking ge prefix
-schrijfde	schreef	Overgeneralisation
-schrijfden	schreven	Overgeneralisation
-schreefde	schreef	Irregular form plus regular suffix
-schreefden	schreven	Irregular form plus regular suffix
-geschrijfd	geschreven	Overgeneralisation+
-eschrijfd	geschreven	Overgeneralisation+Prefix ge without onset
-schrijfd	geschreven	Overgeneralisation+Lacking ge prefix
-geschrijfde	geschrevene	Overgeneralisation+
-eschrijfde	geschrevene	Overgeneralisation+Prefix ge without onset
-geschrijft	geschreven	Overgeneralisation
-eschrijft	geschreven	Overgeneralisation
-schrijft	geschreven	Overgeneralisation
-geschrijfen	geschreven	Wrong -en suffix
-eschrijfen	geschreven	Wrong -en suffix
-schrijfen	geschreven	Wrong -en suffix
-geschreefd	geschreven	Overgeneralisation
-geschreeft	geschreven	Overgeneralisation
-eschreven	geschreven	Prefix ge without onset
-schreven	geschreven	Lacking ge prefix
-schrikte	schrok	Overgeneralisation
-schrikten	schrokken	Overgeneralisation
-schrokte	schrok	Irregular form plus regular suffix
-schrokten	schrokken	Irregular form plus regular suffix
-geschrikt	geschrokken	Overgeneralisation
-eschrikt	geschrokken	Overgeneralisation
-schrikt	geschrokken	Overgeneralisation
-geschrikte	geschrokkene	Overgeneralisation+
-eschrikte	geschrokkene	Overgeneralisation+Prefix ge without onset
-geschrikken	geschrokken	Wrong -en suffix
-eschrikken	geschrokken	Wrong -en suffix
-schrikken	geschrokken	Wrong -en suffix
-geschrokt	geschrokken	Overgeneralisation
-eschrokken	geschrokken	Prefix ge without onset
-schrokken	geschrokken	Lacking ge prefix
-eschuild	geschuild	Prefix ge without onset
-schuild	geschuild	Lacking ge prefix
-eschuilde	geschuilde	Overgeneralisation+Prefix ge without onset
-geschuilt	geschuild	Overgeneralisation
-eschuilt	geschuild	Overgeneralisation
-schuilt	geschuild	Overgeneralisation
-geschuilen	geschuild	Wrong -en suffix
-eschuilen	geschuild	Wrong -en suffix
-schuilen	geschuild	Wrong -en suffix
-schuifde	schoof	Overgeneralisation
-schuifden	schoven	Overgeneralisation
-schoofde	schoof	Irregular form plus regular suffix
-schoofden	schoven	Irregular form plus regular suffix
-geschuifd	geschoven	Overgeneralisation+
-eschuifd	geschoven	Overgeneralisation+Prefix ge without onset
-schuifd	geschoven	Overgeneralisation+Lacking ge prefix
-geschuifde	geschovene	Overgeneralisation+
-eschuifde	geschovene	Overgeneralisation+Prefix ge without onset
-geschuift	geschoven	Overgeneralisation
-eschuift	geschoven	Overgeneralisation
-schuift	geschoven	Overgeneralisation
-geschuifen	geschoven	Wrong -en suffix
-eschuifen	geschoven	Wrong -en suffix
-schuifen	geschoven	Wrong -en suffix
-geschooft	geschoven	Overgeneralisation
-eschoven	geschoven	Prefix ge without onset
-schoven	geschoven	Lacking ge prefix
-slade	sloeg	Overgeneralisation
-sladen	sloegen	Overgeneralisation
-sloegde	sloeg	Irregular form plus regular suffix
-sloegden	sloegen	Irregular form plus regular suffix
-geslaad	geslagen	Overgeneralisation+
-eslaad	geslagen	Overgeneralisation+Prefix ge without onset
-slaad	geslagen	Overgeneralisation+Lacking ge prefix
-geslade	geslagene	Overgeneralisation+
-eslade	geslagene	Overgeneralisation+Prefix ge without onset
-geslaat	geslagen	Overgeneralisation
-eslaat	geslagen	Overgeneralisation
-slaat	geslagen	Overgeneralisation
-geslaan	geslagen	Wrong -en suffix
-eslaan	geslagen	Wrong -en suffix
-slaan	geslagen	Wrong -en suffix
-geslaagd	geslagen	Overgeneralisation
-geslaagt	geslagen	Overgeneralisation
-eslagen	geslagen	Prefix ge without onset
-slagen	geslagen	Lacking ge prefix
-slaapte	sliep	Overgeneralisation
-slaapten	sliepen	Overgeneralisation
-sliepte	sliep	Irregular form plus regular suffix
-sliepten	sliepen	Irregular form plus regular suffix
-geslaapt	geslapen	Overgeneralisation
-eslaapt	geslapen	Overgeneralisation
-slaapt	geslapen	Overgeneralisation
-geslaapte	geslapene	Overgeneralisation+
-eslaapte	geslapene	Overgeneralisation+Prefix ge without onset
-eslapen	geslapen	Prefix ge without onset
-slapen	geslapen	Lacking ge prefix
-slijpte	sleep	Overgeneralisation
-slijpten	slepen	Overgeneralisation
-sleepte	sleep	Irregular form plus regular suffix
-sleepten	slepen	Irregular form plus regular suffix
-geslijpt	geslepen	Overgeneralisation
-eslijpt	geslepen	Overgeneralisation
-slijpt	geslepen	Overgeneralisation
-geslijpte	geslepene	Overgeneralisation+
-eslijpte	geslepene	Overgeneralisation+Prefix ge without onset
-geslijpen	geslepen	Wrong -en suffix
-eslijpen	geslepen	Wrong -en suffix
-slijpen	geslepen	Wrong -en suffix
-gesleept	geslepen	Overgeneralisation
-eslepen	geslepen	Prefix ge without onset
-slepen	geslepen	Lacking ge prefix
-slijtte	sleet	Overgeneralisation
-slijtten	sleten	Overgeneralisation
-sleette	sleet	Irregular form plus regular suffix
-sleetten	sleten	Irregular form plus regular suffix
-geslijt	gesleten	Overgeneralisation
-eslijt	gesleten	Overgeneralisation
-slijt	gesleten	Overgeneralisation
-geslijte	gesletene	Overgeneralisation+
-eslijte	gesletene	Overgeneralisation+Prefix ge without onset
-geslijten	gesleten	Wrong -en suffix
-eslijten	gesleten	Wrong -en suffix
-slijten	gesleten	Wrong -en suffix
-gesleet	gesleten	Overgeneralisation
-esleten	gesleten	Prefix ge without onset
-sleten	gesleten	Lacking ge prefix
-slinkte	slonk	Overgeneralisation
-slinkten	slonken	Overgeneralisation
-slonkte	slonk	Irregular form plus regular suffix
-slonkten	slonken	Irregular form plus regular suffix
-geslinkt	Geslonken	Overgeneralisation
-eslinkt	Geslonken	Overgeneralisation
-slinkt	Geslonken	Overgeneralisation
-geslinkte	Geslonkene	Overgeneralisation+
-eslinkte	Geslonkene	Overgeneralisation+Prefix ge without onset
-geslinken	Geslonken	Wrong -en suffix
-eslinken	Geslonken	Wrong -en suffix
-slinken	Geslonken	Wrong -en suffix
-geGeslonkt	Geslonken	Overgeneralisation
-sluipte	sloop	Overgeneralisation
-sluipten	slopen	Overgeneralisation
-sloopte	sloop	Irregular form plus regular suffix
-sloopten	slopen	Irregular form plus regular suffix
-gesluipt	geslopen	Overgeneralisation
-esluipt	geslopen	Overgeneralisation
-sluipt	geslopen	Overgeneralisation
-gesluipte	geslopene	Overgeneralisation+
-esluipte	geslopene	Overgeneralisation+Prefix ge without onset
-gesluipen	geslopen	Wrong -en suffix
-esluipen	geslopen	Wrong -en suffix
-sluipen	geslopen	Wrong -en suffix
-gesloopt	geslopen	Overgeneralisation
-eslopen	geslopen	Prefix ge without onset
-slopen	geslopen	Lacking ge prefix
-sluitte	sloot	Overgeneralisation
-sluitten	sloten	Overgeneralisation
-slootte	sloot	Irregular form plus regular suffix
-slootten	sloten	Irregular form plus regular suffix
-gesluit	gesloten	Overgeneralisation
-esluit	gesloten	Overgeneralisation
-sluit	gesloten	Overgeneralisation
-gesluite	geslotene	Overgeneralisation+
-esluite	geslotene	Overgeneralisation+Prefix ge without onset
-gesluiten	gesloten	Wrong -en suffix
-esluiten	gesloten	Wrong -en suffix
-sluiten	gesloten	Wrong -en suffix
-gesloot	gesloten	Overgeneralisation
-esloten	gesloten	Prefix ge without onset
-sloten	gesloten	Lacking ge prefix
-smeltte	smolt	Overgeneralisation
-smeltten	smolten	Overgeneralisation
-smoltte	smolt	Irregular form plus regular suffix
-smoltten	smolten	Irregular form plus regular suffix
-gesmelt	gesmolten	Overgeneralisation
-esmelt	gesmolten	Overgeneralisation
-smelt	gesmolten	Overgeneralisation
-gesmelte	gesmoltene	Overgeneralisation+
-esmelte	gesmoltene	Overgeneralisation+Prefix ge without onset
-gesmelten	gesmolten	Wrong -en suffix
-esmelten	gesmolten	Wrong -en suffix
-smelten	gesmolten	Wrong -en suffix
-gesmolt	gesmolten	Overgeneralisation
-esmolten	gesmolten	Prefix ge without onset
-smolten	gesmolten	Lacking ge prefix
-smijtte	smeet	Overgeneralisation
-smijtten	smeten	Overgeneralisation
-smeette	smeet	Irregular form plus regular suffix
-smeetten	smeten	Irregular form plus regular suffix
-gesmijt	gesmeten	Overgeneralisation
-esmijt	gesmeten	Overgeneralisation
-smijt	gesmeten	Overgeneralisation
-gesmijte	gesmetene	Overgeneralisation+
-esmijte	gesmetene	Overgeneralisation+Prefix ge without onset
-gesmijten	gesmeten	Wrong -en suffix
-esmijten	gesmeten	Wrong -en suffix
-smijten	gesmeten	Wrong -en suffix
-gesmeet	gesmeten	Overgeneralisation
-esmeten	gesmeten	Prefix ge without onset
-smeten	gesmeten	Lacking ge prefix
-snijdde	sneed	Overgeneralisation
-snijdden	sneden	Overgeneralisation
-sneedde	sneed	Irregular form plus regular suffix
-sneedden	sneden	Irregular form plus regular suffix
-gesnijd	gesneden	Overgeneralisation
-esnijd	gesneden	Overgeneralisation
-snijd	gesneden	Overgeneralisation
-gesnijde	gesnedene	Overgeneralisation+
-esnijde	gesnedene	Overgeneralisation+Prefix ge without onset
-gesnijden	gesneden	Wrong -en suffix
-esnijden	gesneden	Wrong -en suffix
-snijden	gesneden	Wrong -en suffix
-gesneed	gesneden	Overgeneralisation
-esneden	gesneden	Prefix ge without onset
-sneden	gesneden	Lacking ge prefix
-snuitte	snoot	Overgeneralisation
-snuitten	snoten	Overgeneralisation
-snootte	snoot	Irregular form plus regular suffix
-snootten	snoten	Irregular form plus regular suffix
-gesnuit	gesnoten	Overgeneralisation
-esnuit	gesnoten	Overgeneralisation
-snuit	gesnoten	Overgeneralisation
-gesnuite	gesnotene	Overgeneralisation+
-esnuite	gesnotene	Overgeneralisation+Prefix ge without onset
-gesnuiten	gesnoten	Wrong -en suffix
-esnuiten	gesnoten	Wrong -en suffix
-snuiten	gesnoten	Wrong -en suffix
-gesnoot	gesnoten	Overgeneralisation
-esnoten	gesnoten	Prefix ge without onset
-snoten	gesnoten	Lacking ge prefix
-snuifde	snoof	Overgeneralisation
-snuifden	snoven	Overgeneralisation
-snoofde	snoof	Irregular form plus regular suffix
-snoofden	snoven	Irregular form plus regular suffix
-gesnuifd	gesnoven	Overgeneralisation+
-esnuifd	gesnoven	Overgeneralisation+Prefix ge without onset
-snuifd	gesnoven	Overgeneralisation+Lacking ge prefix
-gesnuifde	gesnovene	Overgeneralisation+
-esnuifde	gesnovene	Overgeneralisation+Prefix ge without onset
-gesnuift	gesnoven	Overgeneralisation
-esnuift	gesnoven	Overgeneralisation
-snuift	gesnoven	Overgeneralisation
-gesnuifen	gesnoven	Wrong -en suffix
-esnuifen	gesnoven	Wrong -en suffix
-snuifen	gesnoven	Wrong -en suffix
-gesnooft	gesnoven	Overgeneralisation
-esnoven	gesnoven	Prefix ge without onset
-snoven	gesnoven	Lacking ge prefix
-gespand	gespannen	Overgeneralisation
-espand	gespannen	Overgeneralisation+Prefix ge without onset
-spand	gespannen	Overgeneralisation+Lacking ge prefix
-gespande	gespannene	Overgeneralisation+
-espande	gespannene	Overgeneralisation+Prefix ge without onset
-gespant	gespannen	Overgeneralisation
-espant	gespannen	Overgeneralisation
-spant	gespannen	Overgeneralisation
-espannen	gespannen	Prefix ge without onset
-spannen	gespannen	Lacking ge prefix
-spijtte	speet	Overgeneralisation
-spijtten	speten	Overgeneralisation
-speette	speet	Irregular form plus regular suffix
-speetten	speten	Irregular form plus regular suffix
-gespijt	gespeten	Overgeneralisation
-espijt	gespeten	Overgeneralisation
-spijt	gespeten	Overgeneralisation
-gespijte	gespetene	Overgeneralisation+
-espijte	gespetene	Overgeneralisation+Prefix ge without onset
-gespijten	gespeten	Wrong -en suffix
-espijten	gespeten	Wrong -en suffix
-spijten	gespeten	Wrong -en suffix
-gespeet	gespeten	Overgeneralisation
-espeten	gespeten	Prefix ge without onset
-speten	gespeten	Lacking ge prefix
-spinde	spon	Overgeneralisation
-spinden	sponnen	Overgeneralisation
-sponde	spon	Irregular form plus regular suffix
-sponden	sponnen	Irregular form plus regular suffix
-gespind	gesponnen	Overgeneralisation+
-espind	gesponnen	Overgeneralisation+Prefix ge without onset
-spind	gesponnen	Overgeneralisation+Lacking ge prefix
-gespinde	gesponnene	Overgeneralisation+
-espinde	gesponnene	Overgeneralisation+Prefix ge without onset
-gespint	gesponnen	Overgeneralisation
-espint	gesponnen	Overgeneralisation
-spint	gesponnen	Overgeneralisation
-gespinnen	gesponnen	Wrong -en suffix
-espinnen	gesponnen	Wrong -en suffix
-spinnen	gesponnen	Wrong -en suffix
-gespont	gesponnen	Overgeneralisation
-esponnen	gesponnen	Prefix ge without onset
-sponnen	gesponnen	Lacking ge prefix
-splijtte	spleet	Overgeneralisation
-splijtten	spleten	Overgeneralisation
-spleette	spleet	Irregular form plus regular suffix
-spleetten	spleten	Irregular form plus regular suffix
-gesplijt	gespleten	Overgeneralisation
-esplijt	gespleten	Overgeneralisation
-splijt	gespleten	Overgeneralisation
-gesplijte	gespletene	Overgeneralisation+
-esplijte	gespletene	Overgeneralisation+Prefix ge without onset
-gesplijten	gespleten	Wrong -en suffix
-esplijten	gespleten	Wrong -en suffix
-splijten	gespleten	Wrong -en suffix
-gespleet	gespleten	Overgeneralisation
-espleten	gespleten	Prefix ge without onset
-spleten	gespleten	Lacking ge prefix
-spreekte	sprak	Overgeneralisation
-spreekten	spraken	Overgeneralisation
-sprakte	sprak	Irregular form plus regular suffix
-sprakten	spraken	Irregular form plus regular suffix
-gespreekt	gesproken	Overgeneralisation
-espreekt	gesproken	Overgeneralisation
-spreekt	gesproken	Overgeneralisation
-gespreekte	gesprokene	Overgeneralisation+
-espreekte	gesprokene	Overgeneralisation+Prefix ge without onset
-gespreken	gesproken	Wrong -en suffix
-espreken	gesproken	Wrong -en suffix
-spreken	gesproken	Wrong -en suffix
-gesprookt	gesproken	Overgeneralisation
-esproken	gesproken	Prefix ge without onset
-sproken	gesproken	Lacking ge prefix
-springde	sprong	Overgeneralisation
-springden	sprongen	Overgeneralisation
-sprongde	sprong	Irregular form plus regular suffix
-sprongden	sprongen	Irregular form plus regular suffix
-gespringd	gesprongen	Overgeneralisation+
-espringd	gesprongen	Overgeneralisation+Prefix ge without onset
-springd	gesprongen	Overgeneralisation+Lacking ge prefix
-gespringde	gesprongene	Overgeneralisation+
-espringde	gesprongene	Overgeneralisation+Prefix ge without onset
-gespringt	gesprongen	Overgeneralisation
-espringt	gesprongen	Overgeneralisation
-springt	gesprongen	Overgeneralisation
-gespringen	gesprongen	Wrong -en suffix
-espringen	gesprongen	Wrong -en suffix
-springen	gesprongen	Wrong -en suffix
-gesprongd	gesprongen	Overgeneralisation
-gesprongt	gesprongen	Overgeneralisation
-esprongen	gesprongen	Prefix ge without onset
-sprongen	gesprongen	Lacking ge prefix
-spruitte	sproot	Overgeneralisation
-spruitten	sproten	Overgeneralisation
-sprootte	sproot	Irregular form plus regular suffix
-sprootten	sproten	Irregular form plus regular suffix
-gespruit	gesproten	Overgeneralisation
-espruit	gesproten	Overgeneralisation
-spruit	gesproten	Overgeneralisation
-gespruite	gesprotene	Overgeneralisation+
-espruite	gesprotene	Overgeneralisation+Prefix ge without onset
-gespruiten	gesproten	Wrong -en suffix
-espruiten	gesproten	Wrong -en suffix
-spruiten	gesproten	Wrong -en suffix
-gesproot	gesproten	Overgeneralisation
-esproten	gesproten	Prefix ge without onset
-sproten	gesproten	Lacking ge prefix
-spuitte	spoot	Overgeneralisation
-spuitten	spoten	Overgeneralisation
-spootte	spoot	Irregular form plus regular suffix
-spootten	spoten	Irregular form plus regular suffix
-gespuit	gespoten	Overgeneralisation
-espuit	gespoten	Overgeneralisation
-spuit	gespoten	Overgeneralisation
-gespuite	gespotene	Overgeneralisation+
-espuite	gespotene	Overgeneralisation+Prefix ge without onset
-gespuiten	gespoten	Wrong -en suffix
-espuiten	gespoten	Wrong -en suffix
-spuiten	gespoten	Wrong -en suffix
-gespoot	gespoten	Overgeneralisation
-espoten	gespoten	Prefix ge without onset
-spoten	gespoten	Lacking ge prefix
-state	stond	Overgeneralisation
-staten	stonden	Overgeneralisation
-stondte	stond	Irregular form plus regular suffix
-stondten	stonden	Irregular form plus regular suffix
-gestat	gestaan	Overgeneralisation+
-estat	gestaan	Overgeneralisation+Prefix ge without onset
-stat	gestaan	Overgeneralisation+Lacking ge prefix
-gestatte	gestaane	Overgeneralisation+
-estatte	gestaane	Overgeneralisation+Prefix ge without onset
-gestaat	gestaan	Overgeneralisation
-estaat	gestaan	Overgeneralisation
-staat	gestaan	Overgeneralisation
-estaan	gestaan	Prefix ge without onset
-staan	gestaan	Lacking ge prefix
-steekte	stak	Overgeneralisation
-steekten	staken	Overgeneralisation
-stakte	stak	Irregular form plus regular suffix
-stakten	staken	Irregular form plus regular suffix
-gesteekt	gestoken	Overgeneralisation
-esteekt	gestoken	Overgeneralisation
-steekt	gestoken	Overgeneralisation
-gesteekte	gestokene	Overgeneralisation+
-esteekte	gestokene	Overgeneralisation+Prefix ge without onset
-gesteken	gestoken	Wrong -en suffix
-esteken	gestoken	Wrong -en suffix
-steken	gestoken	Wrong -en suffix
-gestookt	gestoken	Overgeneralisation
-estoken	gestoken	Prefix ge without onset
-stoken	gestoken	Lacking ge prefix
-steelde	stal	Overgeneralisation
-steelden	stalen	Overgeneralisation
-stalde	stal	Irregular form plus regular suffix
-stalden	stalen	Irregular form plus regular suffix
-gesteeld	gestolen	Overgeneralisation+
-esteeld	gestolen	Overgeneralisation+Prefix ge without onset
-steeld	gestolen	Overgeneralisation+Lacking ge prefix
-gesteelde	gestolene	Overgeneralisation+
-esteelde	gestolene	Overgeneralisation+Prefix ge without onset
-gesteelt	gestolen	Overgeneralisation
-esteelt	gestolen	Overgeneralisation
-steelt	gestolen	Overgeneralisation
-gestelen	gestolen	Wrong -en suffix
-estelen	gestolen	Wrong -en suffix
-stelen	gestolen	Wrong -en suffix
-gestoolt	gestolen	Overgeneralisation
-estolen	gestolen	Prefix ge without onset
-stolen	gestolen	Lacking ge prefix
-sterfde	stierf	Overgeneralisation
-sterfden	stierven	Overgeneralisation
-stierfde	stierf	Irregular form plus regular suffix
-stierfden	stierven	Irregular form plus regular suffix
-gesterfd	gestorven	Overgeneralisation+
-esterfd	gestorven	Overgeneralisation+Prefix ge without onset
-sterfd	gestorven	Overgeneralisation+Lacking ge prefix
-gesterfde	gestorvene	Overgeneralisation+
-esterfde	gestorvene	Overgeneralisation+Prefix ge without onset
-gesterft	gestorven	Overgeneralisation
-esterft	gestorven	Overgeneralisation
-sterft	gestorven	Overgeneralisation
-gesterfen	gestorven	Wrong -en suffix
-esterfen	gestorven	Wrong -en suffix
-sterfen	gestorven	Wrong -en suffix
-gestorfd	gestorven	Overgeneralisation
-gestorft	gestorven	Overgeneralisation
-estorven	gestorven	Prefix ge without onset
-storven	gestorven	Lacking ge prefix
-stijgde	steeg	Overgeneralisation
-stijgden	stegen	Overgeneralisation
-steegde	steeg	Irregular form plus regular suffix
-steegden	stegen	Irregular form plus regular suffix
-gestijgd	gestegen	Overgeneralisation+
-estijgd	gestegen	Overgeneralisation+Prefix ge without onset
-stijgd	gestegen	Overgeneralisation+Lacking ge prefix
-gestijgde	gestegene	Overgeneralisation+
-estijgde	gestegene	Overgeneralisation+Prefix ge without onset
-gestijgt	gestegen	Overgeneralisation
-estijgt	gestegen	Overgeneralisation
-stijgt	gestegen	Overgeneralisation
-gestijgen	gestegen	Wrong -en suffix
-estijgen	gestegen	Wrong -en suffix
-stijgen	gestegen	Wrong -en suffix
-gesteegd	gestegen	Overgeneralisation
-gesteegt	gestegen	Overgeneralisation
-estegen	gestegen	Prefix ge without onset
-stegen	gestegen	Lacking ge prefix
-stijfde	steef	Overgeneralisation
-stijfden	steven	Overgeneralisation
-steefde	steef	Irregular form plus regular suffix
-steefden	steven	Irregular form plus regular suffix
-gestijfd	gesteven	Overgeneralisation+
-estijfd	gesteven	Overgeneralisation+Prefix ge without onset
-stijfd	gesteven	Overgeneralisation+Lacking ge prefix
-gestijfde	gestevene	Overgeneralisation+
-estijfde	gestevene	Overgeneralisation+Prefix ge without onset
-gestijft	gesteven	Overgeneralisation
-estijft	gesteven	Overgeneralisation
-stijft	gesteven	Overgeneralisation
-gestijfen	gesteven	Wrong -en suffix
-estijfen	gesteven	Wrong -en suffix
-stijfen	gesteven	Wrong -en suffix
-gesteefd	gesteven	Overgeneralisation
-gesteeft	gesteven	Overgeneralisation
-esteven	gesteven	Prefix ge without onset
-steven	gesteven	Lacking ge prefix
-stinkte	stonk	Overgeneralisation
-stinkten	stonken	Overgeneralisation
-stonkte	stonk	Irregular form plus regular suffix
-stonkten	stonken	Irregular form plus regular suffix
-gestinkt	gestonken	Overgeneralisation
-estinkt	gestonken	Overgeneralisation
-stinkt	gestonken	Overgeneralisation
-gestinkte	gestonkene	Overgeneralisation+
-estinkte	gestonkene	Overgeneralisation+Prefix ge without onset
-gestinken	gestonken	Wrong -en suffix
-estinken	gestonken	Wrong -en suffix
-stinken	gestonken	Wrong -en suffix
-gestonkt	gestonken	Overgeneralisation
-estonken	gestonken	Prefix ge without onset
-stonken	gestonken	Lacking ge prefix
-gestoot	gestoten	Overgeneralisation
-estoot	gestoten	Overgeneralisation
-stoot	gestoten	Overgeneralisation
-gestote	gestotene	Overgeneralisation+
-estote	gestotene	Overgeneralisation+Prefix ge without onset
-estoten	gestoten	Prefix ge without onset
-stoten	gestoten	Lacking ge prefix
-strijdde	streed	Overgeneralisation
-strijdden	streden	Overgeneralisation
-streedde	streed	Irregular form plus regular suffix
-streedden	streden	Irregular form plus regular suffix
-gestrijd	gestreden	Overgeneralisation
-estrijd	gestreden	Overgeneralisation
-strijd	gestreden	Overgeneralisation
-gestrijde	gestredene	Overgeneralisation+
-estrijde	gestredene	Overgeneralisation+Prefix ge without onset
-gestrijden	gestreden	Wrong -en suffix
-estrijden	gestreden	Wrong -en suffix
-strijden	gestreden	Wrong -en suffix
-gestreed	gestreden	Overgeneralisation
-estreden	gestreden	Prefix ge without onset
-streden	gestreden	Lacking ge prefix
-strijkte	streek	Overgeneralisation
-strijkten	streken	Overgeneralisation
-streekte	streek	Irregular form plus regular suffix
-streekten	streken	Irregular form plus regular suffix
-gestrijkt	gestreken	Overgeneralisation
-estrijkt	gestreken	Overgeneralisation
-strijkt	gestreken	Overgeneralisation
-gestrijkte	gestrekene	Overgeneralisation+
-estrijkte	gestrekene	Overgeneralisation+Prefix ge without onset
-gestrijken	gestreken	Wrong -en suffix
-estrijken	gestreken	Wrong -en suffix
-strijken	gestreken	Wrong -en suffix
-gestreekt	gestreken	Overgeneralisation
-estreken	gestreken	Prefix ge without onset
-streken	gestreken	Lacking ge prefix
-stuifde	stoof	Overgeneralisation
-stuifden	stoven	Overgeneralisation
-stoofde	stoof	Irregular form plus regular suffix
-stoofden	stoven	Irregular form plus regular suffix
-gestuifd	gestoventoven	Overgeneralisation+
-estuifd	gestoventoven	Overgeneralisation+Prefix ge without onset
-stuifd	gestoventoven	Overgeneralisation+Lacking ge prefix
-gestuifde	gestoventovene	Overgeneralisation+
-estuifde	gestoventovene	Overgeneralisation+Prefix ge without onset
-gestuift	gestoventoven	Overgeneralisation
-estuift	gestoventoven	Overgeneralisation
-stuift	gestoventoven	Overgeneralisation
-gestuifen	gestoventoven	Wrong -en suffix
-estuifen	gestoventoven	Wrong -en suffix
-stuifen	gestoventoven	Wrong -en suffix
-gestoventooft	gestoventoven	Overgeneralisation
-estoventoven	gestoventoven	Prefix ge without onset
-stoventoven	gestoventoven	Lacking ge prefix
-treedde	trad	Overgeneralisation
-treedden	traden	Overgeneralisation
-tradde	trad	Irregular form plus regular suffix
-tradden	traden	Irregular form plus regular suffix
-getreed	getreden	Overgeneralisation
-etreed	getreden	Overgeneralisation
-treed	getreden	Overgeneralisation
-getrede	getredene	Overgeneralisation+
-etrede	getredene	Overgeneralisation+Prefix ge without onset
-etreden	getreden	Prefix ge without onset
-treden	getreden	Lacking ge prefix
-trefte	trof	Overgeneralisation
-treften	troffen	Overgeneralisation
-trofte	trof	Irregular form plus regular suffix
-troften	troffen	Irregular form plus regular suffix
-getreft	getroffen	Overgeneralisation
-etreft	getroffen	Overgeneralisation
-treft	getroffen	Overgeneralisation
-getrefte	getroffene	Overgeneralisation+
-etrefte	getroffene	Overgeneralisation+Prefix ge without onset
-getreffen	getroffen	Wrong -en suffix
-etreffen	getroffen	Wrong -en suffix
-treffen	getroffen	Wrong -en suffix
-getroft	getroffen	Overgeneralisation
-etroffen	getroffen	Prefix ge without onset
-troffen	getroffen	Lacking ge prefix
-trekte	trok	Overgeneralisation
-trekten	trokken	Overgeneralisation
-trokte	trok	Irregular form plus regular suffix
-trokten	trokken	Irregular form plus regular suffix
-getrekt	getrokken	Overgeneralisation
-etrekt	getrokken	Overgeneralisation
-trekt	getrokken	Overgeneralisation
-getrekte	getrokkene	Overgeneralisation+
-etrekte	getrokkene	Overgeneralisation+Prefix ge without onset
-getrekken	getrokken	Wrong -en suffix
-etrekken	getrokken	Wrong -en suffix
-trekken	getrokken	Wrong -en suffix
-getrokt	getrokken	Overgeneralisation
-etrokken	getrokken	Prefix ge without onset
-trokken	getrokken	Lacking ge prefix
-valde	viel	Overgeneralisation
-valden	vielen	Overgeneralisation
-vielde	viel	Irregular form plus regular suffix
-vielden	vielen	Irregular form plus regular suffix
-gevald	gevallen	Overgeneralisation
-evald	gevallen	Overgeneralisation+Prefix ge without onset
-vald	gevallen	Overgeneralisation+Lacking ge prefix
-gevalde	gevallene	Overgeneralisation+
-evalde	gevallene	Overgeneralisation+Prefix ge without onset
-gevalt	gevallen	Overgeneralisation
-evalt	gevallen	Overgeneralisation
-valt	gevallen	Overgeneralisation
-evallen	gevallen	Prefix ge without onset
-vallen	gevallen	Lacking ge prefix
-vangde	ving	Overgeneralisation
-vangden	vingen	Overgeneralisation
-vingde	ving	Irregular form plus regular suffix
-vingden	vingen	Irregular form plus regular suffix
-gevangd	gevangen	Overgeneralisation
-evangd	gevangen	Overgeneralisation+Prefix ge without onset
-vangd	gevangen	Overgeneralisation+Lacking ge prefix
-gevangde	gevangene	Overgeneralisation+
-evangde	gevangene	Overgeneralisation+Prefix ge without onset
-gevangt	gevangen	Overgeneralisation
-evangt	gevangen	Overgeneralisation
-vangt	gevangen	Overgeneralisation
-evangen	gevangen	Prefix ge without onset
-vangen	gevangen	Lacking ge prefix
-vaarde	voer	Overgeneralisation
-vaarden	voeren	Overgeneralisation
-voerde	voer	Irregular form plus regular suffix
-voerden	voeren	Irregular form plus regular suffix
-gevaard	gevaren	Overgeneralisation
-evaard	gevaren	Overgeneralisation+Prefix ge without onset
-vaard	gevaren	Overgeneralisation+Lacking ge prefix
-gevaarde	gevarene	Overgeneralisation+
-evaarde	gevarene	Overgeneralisation+Prefix ge without onset
-gevaart	gevaren	Overgeneralisation
-evaart	gevaren	Overgeneralisation
-vaart	gevaren	Overgeneralisation
-evaren	gevaren	Prefix ge without onset
-varen	gevaren	Lacking ge prefix
-vechtte	vocht	Overgeneralisation
-vechtten	vochten	Overgeneralisation
-vochtte	vocht	Irregular form plus regular suffix
-vochtten	vochten	Irregular form plus regular suffix
-gevecht	gevochten	Overgeneralisation
-evecht	gevochten	Overgeneralisation
-vecht	gevochten	Overgeneralisation
-gevechte	gevochtene	Overgeneralisation+
-evechte	gevochtene	Overgeneralisation+Prefix ge without onset
-gevechten	gevochten	Wrong -en suffix
-evechten	gevochten	Wrong -en suffix
-vechten	gevochten	Wrong -en suffix
-gevocht	gevochten	Overgeneralisation
-evochten	gevochten	Prefix ge without onset
-vochten	gevochten	Lacking ge prefix
-verdriette	verdroot	Overgeneralisation
-verdrietten	verdroten	Overgeneralisation
-verdrootte	verdroot	Irregular form plus regular suffix
-verdrootten	verdroten	Irregular form plus regular suffix
-verdriet	verdroten	Overgeneralisation
-verdriete	verdrotene	Overgeneralisation
-verdrieten	verdroten	Wrong -en suffix
-verdroot	verdroten	Overgeneralisation
-verdwijnde	verdwenene	Overgeneralisation
-verdwijnden	verdwenen	Overgeneralisation
-verdweende	verdween	Irregular form plus regular suffix
-verdweenden	verdwenen	Irregular form plus regular suffix
-verdwijnd	verdwenen	Overgeneralisation
-verdwijnt	verdwenen	Overgeneralisation
-verdwijnen	verdwenen	Wrong -en suffix
-verdweend	verdwenen	Overgeneralisation
-verdweent	verdwenen	Overgeneralisation
-vergeette	vergat	Overgeneralisation
-vergeetten	vergaten	Overgeneralisation
-vergatte	vergat	Irregular form plus regular suffix
-vergatten	vergaten	Irregular form plus regular suffix
-vergeet	vergeten	Overgeneralisation
-vergete	vergetene	Overgeneralisation
-verliesde	verlorene	Overgeneralisation
-verliesden	verloren	Overgeneralisation
-verloorde	verloor	Irregular form plus regular suffix
-verloorden	verloren	Irregular form plus regular suffix
-verliesd	verloren	Overgeneralisation
-verliest	verloren	Overgeneralisation
-verliesen	verloren	Wrong -en suffix
-verloort	verloren	Overgeneralisation
-vindde	vond	Overgeneralisation
-vindden	vonden	Overgeneralisation
-vondde	vond	Irregular form plus regular suffix
-vondden	vonden	Irregular form plus regular suffix
-gevind	gevonden	Overgeneralisation
-evind	gevonden	Overgeneralisation
-vind	gevonden	Overgeneralisation
-gevinde	gevondene	Overgeneralisation+
-evinde	gevondene	Overgeneralisation+Prefix ge without onset
-gevinden	gevonden	Wrong -en suffix
-evinden	gevonden	Wrong -en suffix
-vinden	gevonden	Wrong -en suffix
-gevond	gevonden	Overgeneralisation
-evonden	gevonden	Prefix ge without onset
-vonden	gevonden	Lacking ge prefix
-vlechtte	vlocht	Overgeneralisation
-vlechtten	vlochten	Overgeneralisation
-vlochtte	vlocht	Irregular form plus regular suffix
-vlochtten	vlochten	Irregular form plus regular suffix
-gevlecht	gevlochten	Overgeneralisation
-evlecht	gevlochten	Overgeneralisation
-vlecht	gevlochten	Overgeneralisation
-gevlechte	gevlochtene	Overgeneralisation+
-evlechte	gevlochtene	Overgeneralisation+Prefix ge without onset
-gevlechten	gevlochten	Wrong -en suffix
-evlechten	gevlochten	Wrong -en suffix
-vlechten	gevlochten	Wrong -en suffix
-gevlocht	gevlochten	Overgeneralisation
-evlochten	gevlochten	Prefix ge without onset
-vlochten	gevlochten	Lacking ge prefix
-vliegde	vloog	Overgeneralisation
-vliegden	vlogen	Overgeneralisation
-vloogde	vloog	Irregular form plus regular suffix
-vloogden	vlogen	Irregular form plus regular suffix
-gevliegd	gevlogen	Overgeneralisation+
-evliegd	gevlogen	Overgeneralisation+Prefix ge without onset
-vliegd	gevlogen	Overgeneralisation+Lacking ge prefix
-gevliegde	gevlogene	Overgeneralisation+
-evliegde	gevlogene	Overgeneralisation+Prefix ge without onset
-gevliegt	gevlogen	Overgeneralisation
-evliegt	gevlogen	Overgeneralisation
-vliegt	gevlogen	Overgeneralisation
-gevliegen	gevlogen	Wrong -en suffix
-evliegen	gevlogen	Wrong -en suffix
-vliegen	gevlogen	Wrong -en suffix
-gevloogt	gevlogen	Overgeneralisation
-evlogen	gevlogen	Prefix ge without onset
-vlogen	gevlogen	Lacking ge prefix
-gevouwd	gevouwen	Overgeneralisation
-evouwd	gevouwen	Overgeneralisation+Prefix ge without onset
-vouwd	gevouwen	Overgeneralisation+Lacking ge prefix
-gevouwde	gevouwene	Overgeneralisation+
-evouwde	gevouwene	Overgeneralisation+Prefix ge without onset
-gevouwt	gevouwen	Overgeneralisation
-evouwt	gevouwen	Overgeneralisation
-vouwt	gevouwen	Overgeneralisation
-evouwen	gevouwen	Prefix ge without onset
-vouwen	gevouwen	Lacking ge prefix
-vraagde	vroeg	Overgeneralisation
-vraagden	vroegen	Overgeneralisation
-vroegde	vroeg	Irregular form plus regular suffix
-vroegden	vroegen	Irregular form plus regular suffix
-evraagd	gevraagd	Prefix ge without onset
-vraagd	gevraagd	Lacking ge prefix
-evraagde	gevraagde	Overgeneralisation+Prefix ge without onset
-gevraagt	gevraagd	Overgeneralisation
-evraagt	gevraagd	Overgeneralisation
-vraagt	gevraagd	Overgeneralisation
-gevragen	gevraagd	Wrong -en suffix
-evragen	gevraagd	Wrong -en suffix
-vragen	gevraagd	Wrong -en suffix
-vreette	vrat	Overgeneralisation
-vreetten	vraten	Overgeneralisation
-vratte	vrat	Irregular form plus regular suffix
-vratten	vraten	Irregular form plus regular suffix
-gevreet	gevreten	Overgeneralisation
-evreet	gevreten	Overgeneralisation
-vreet	gevreten	Overgeneralisation
-gevrete	gevretene	Overgeneralisation+
-evrete	gevretene	Overgeneralisation+Prefix ge without onset
-evreten	gevreten	Prefix ge without onset
-vreten	gevreten	Lacking ge prefix
-vriesde	vroor	Overgeneralisation
-vriesden	vroren	Overgeneralisation
-vroorde	vroor	Irregular form plus regular suffix
-vroorden	vroren	Irregular form plus regular suffix
-gevriesd	gevroren	Overgeneralisation+
-evriesd	gevroren	Overgeneralisation+Prefix ge without onset
-vriesd	gevroren	Overgeneralisation+Lacking ge prefix
-gevriesde	gevrorene	Overgeneralisation+
-evriesde	gevrorene	Overgeneralisation+Prefix ge without onset
-gevriest	gevroren	Overgeneralisation
-evriest	gevroren	Overgeneralisation
-vriest	gevroren	Overgeneralisation
-gevriesen	gevroren	Wrong -en suffix
-evriesen	gevroren	Wrong -en suffix
-vriesen	gevroren	Wrong -en suffix
-gevroort	gevroren	Overgeneralisation
-evroren	gevroren	Prefix ge without onset
-vroren	gevroren	Lacking ge prefix
-vriijde	vrijde	Overgeneralisation
-vriijden	vrijden	Overgeneralisation
-gevriijd	gevrijd	Overgeneralisation+
-evriijd	gevrijd	Overgeneralisation+Prefix ge without onset
-vriijd	gevrijd	Overgeneralisation+Lacking ge prefix
-gevriijde	gevrijde	Overgeneralisation+
-evriijde	gevrijde	Overgeneralisation+Prefix ge without onset
-gevriijt	gevrijd	Overgeneralisation
-evriijt	gevrijd	Overgeneralisation
-vriijt	gevrijd	Overgeneralisation
-gevrijen	gevrijd	Wrong -en suffix
-evrijen	gevrijd	Wrong -en suffix
-vrijen	gevrijd	Wrong -en suffix
-evrijd	gevrijd	Prefix ge without onset
-vrijd	gevrijd	Lacking ge prefix
-gewast	gewassen	Overgeneralisation
-ewast	gewassen	Overgeneralisation
-wast	gewassen	Overgeneralisation
-gewaste	gewassene	Overgeneralisation+
-ewaste	gewassene	Overgeneralisation+Prefix ge without onset
-ewassen	gewassen	Prefix ge without onset
-wassen	gewassen	Lacking ge prefix
-weegde	woog	Overgeneralisation
-weegden	wogen	Overgeneralisation
-woogde	woog	Irregular form plus regular suffix
-woogden	wogen	Irregular form plus regular suffix
-geweegd	gewogen	Overgeneralisation+
-eweegd	gewogen	Overgeneralisation+Prefix ge without onset
-weegd	gewogen	Overgeneralisation+Lacking ge prefix
-geweegde	gewogene	Overgeneralisation+
-eweegde	gewogene	Overgeneralisation+Prefix ge without onset
-geweegt	gewogen	Overgeneralisation
-eweegt	gewogen	Overgeneralisation
-weegt	gewogen	Overgeneralisation
-gewegen	gewogen	Wrong -en suffix
-ewegen	gewogen	Wrong -en suffix
-wegen	gewogen	Wrong -en suffix
-gewoogt	gewogen	Overgeneralisation
-ewogen	gewogen	Prefix ge without onset
-wogen	gewogen	Lacking ge prefix
-werpte	wierp	Overgeneralisation
-werpten	wierpen	Overgeneralisation
-wierpte	wierp	Irregular form plus regular suffix
-wierpten	wierpen	Irregular form plus regular suffix
-gewerpt	geworpen	Overgeneralisation
-ewerpt	geworpen	Overgeneralisation
-werpt	geworpen	Overgeneralisation
-gewerpte	geworpene	Overgeneralisation+
-ewerpte	geworpene	Overgeneralisation+Prefix ge without onset
-gewerpen	geworpen	Wrong -en suffix
-ewerpen	geworpen	Wrong -en suffix
-werpen	geworpen	Wrong -en suffix
-geworpt	geworpen	Overgeneralisation
-eworpen	geworpen	Prefix ge without onset
-worpen	geworpen	Lacking ge prefix
-werfde	wierf	Overgeneralisation
-werfden	wierven	Overgeneralisation
-wierfde	wierf	Irregular form plus regular suffix
-wierfden	wierven	Irregular form plus regular suffix
-gewerfd	geworven	Overgeneralisation+
-ewerfd	geworven	Overgeneralisation+Prefix ge without onset
-werfd	geworven	Overgeneralisation+Lacking ge prefix
-gewerfde	geworvene	Overgeneralisation+
-ewerfde	geworvene	Overgeneralisation+Prefix ge without onset
-gewerft	geworven	Overgeneralisation
-ewerft	geworven	Overgeneralisation
-werft	geworven	Overgeneralisation
-gewerfen	geworven	Wrong -en suffix
-ewerfen	geworven	Wrong -en suffix
-werfen	geworven	Wrong -en suffix
-geworfd	geworven	Overgeneralisation
-geworft	geworven	Overgeneralisation
-eworven	geworven	Prefix ge without onset
-worven	geworven	Lacking ge prefix
-weette	weet	Irregular form plus regular suffix
-weetten	weten	Irregular form plus regular suffix
-wistte	wist	Irregular form plus regular suffix
-wistten	wisten	Irregular form plus regular suffix
-geweet	geweten	Overgeneralisation
-eweet	geweten	Overgeneralisation
-weet	geweten	Overgeneralisation
-gewete	gewetene	Overgeneralisation+
-ewete	gewetene	Overgeneralisation+Prefix ge without onset
-eweten	geweten	Prefix ge without onset
-weten	geweten	Lacking ge prefix
-geweefd	geweven	Overgeneralisation
-eweefd	geweven	Overgeneralisation+Prefix ge without onset
-weefd	geweven	Overgeneralisation+Lacking ge prefix
-geweefde	gewevene	Overgeneralisation+
-eweefde	gewevene	Overgeneralisation+Prefix ge without onset
-geweeft	geweven	Overgeneralisation
-eweeft	geweven	Overgeneralisation
-weeft	geweven	Overgeneralisation
-gewefen	geweven	Wrong -en suffix
-ewefen	geweven	Wrong -en suffix
-wefen	geweven	Wrong -en suffix
-eweven	geweven	Prefix ge without onset
-weven	geweven	Lacking ge prefix
-wijkte	week	Overgeneralisation
-wijkten	weken	Overgeneralisation
-weekte	week	Irregular form plus regular suffix
-weekten	weken	Irregular form plus regular suffix
-gewijkt	geweken	Overgeneralisation
-ewijkt	geweken	Overgeneralisation
-wijkt	geweken	Overgeneralisation
-gewijkte	gewekene	Overgeneralisation+
-ewijkte	gewekene	Overgeneralisation+Prefix ge without onset
-gewijken	geweken	Wrong -en suffix
-ewijken	geweken	Wrong -en suffix
-wijken	geweken	Wrong -en suffix
-geweekt	geweken	Overgeneralisation
-eweken	geweken	Prefix ge without onset
-weken	geweken	Lacking ge prefix
-wijtte	weet	Overgeneralisation
-wijtten	weten	Overgeneralisation
-gewijt	geweten	Overgeneralisation
-ewijt	geweten	Overgeneralisation
-wijt	geweten	Overgeneralisation
-gewijte	gewetene	Overgeneralisation+
-ewijte	gewetene	Overgeneralisation+Prefix ge without onset
-gewijten	geweten	Wrong -en suffix
-ewijten	geweten	Wrong -en suffix
-wijten	geweten	Wrong -en suffix
-wijsde	wees	Overgeneralisation
-wijsden	wezen	Overgeneralisation
-weesde	wees	Irregular form plus regular suffix
-weesden	wezen	Irregular form plus regular suffix
-gewijsd	gewezen	Overgeneralisation+
-ewijsd	gewezen	Overgeneralisation+Prefix ge without onset
-wijsd	gewezen	Overgeneralisation+Lacking ge prefix
-gewijsde	gewezene	Overgeneralisation+
-ewijsde	gewezene	Overgeneralisation+Prefix ge without onset
-gewijst	gewezen	Overgeneralisation
-ewijst	gewezen	Overgeneralisation
-wijst	gewezen	Overgeneralisation
-gewijsen	gewezen	Wrong -en suffix
-ewijsen	gewezen	Wrong -en suffix
-wijsen	gewezen	Wrong -en suffix
-geweesd	gewezen	Overgeneralisation
-geweest	gewezen	Overgeneralisation
-ewezen	gewezen	Prefix ge without onset
-wezen	gewezen	Lacking ge prefix
-windde	wond	Overgeneralisation
-windden	wonden	Overgeneralisation
-wondde	wond	Irregular form plus regular suffix
-wondden	wonden	Irregular form plus regular suffix
-gewind	gewonnen	Overgeneralisation+
-ewind	gewonnen	Overgeneralisation+Prefix ge without onset
-wind	gewonnen	Overgeneralisation+Lacking ge prefix
-gewinde	gewonnene	Overgeneralisation+
-ewinde	gewonnene	Overgeneralisation+Prefix ge without onset
-gewinden	gewonden	Wrong -en suffix
-ewinden	gewonden	Wrong -en suffix
-winden	wonnen	Overgeneralisation
-gewond	gewonden	Overgeneralisation
-ewonden	gewonden	Prefix ge without onset
-wonden	wonnen	Irregular form plus regular suffix
-winde	won	Overgeneralisation
-wonde	won	Irregular form plus regular suffix
-gewint	gewonnen	Overgeneralisation
-ewint	gewonnen	Overgeneralisation
-wint	gewonnen	Overgeneralisation
-gewinnen	gewonnen	Wrong -en suffix
-ewinnen	gewonnen	Wrong -en suffix
-winnen	gewonnen	Wrong -en suffix
-gewont	gewonnen	Overgeneralisation
-ewonnen	gewonnen	Prefix ge without onset
-wonnen	gewonnen	Lacking ge prefix
-wordde	werd	Overgeneralisation
-wordden	werden	Overgeneralisation
-werdde	werd	Irregular form plus regular suffix
-werdden	werden	Irregular form plus regular suffix
-geword	geworden	Overgeneralisation
-eword	geworden	Overgeneralisation
-word	geworden	Overgeneralisation
-geworde	gewordene	Overgeneralisation+
-eworde	gewordene	Overgeneralisation+Prefix ge without onset
-eworden	geworden	Prefix ge without onset
-worden	geworden	Lacking ge prefix
-wrijfde	wreef	Overgeneralisation
-wrijfden	wreven	Overgeneralisation
-wreefde	wreef	Irregular form plus regular suffix
-wreefden	wreven	Irregular form plus regular suffix
-gewrijfd	gewreven	Overgeneralisation+
-ewrijfd	gewreven	Overgeneralisation+Prefix ge without onset
-wrijfd	gewreven	Overgeneralisation+Lacking ge prefix
-gewrijfde	gewrevene	Overgeneralisation+
-ewrijfde	gewrevene	Overgeneralisation+Prefix ge without onset
-gewrijft	gewreven	Overgeneralisation
-ewrijft	gewreven	Overgeneralisation
-wrijft	gewreven	Overgeneralisation
-gewrijfen	gewreven	Wrong -en suffix
-ewrijfen	gewreven	Wrong -en suffix
-wrijfen	gewreven	Wrong -en suffix
-gewreefd	gewreven	Overgeneralisation
-gewreeft	gewreven	Overgeneralisation
-ewreven	gewreven	Prefix ge without onset
-wreven	gewreven	Lacking ge prefix
-wringde	wrong	Overgeneralisation
-wringden	wrongen	Overgeneralisation
-wrongde	wrong	Irregular form plus regular suffix
-wrongden	wrongen	Irregular form plus regular suffix
-gewringd	gewrongen	Overgeneralisation+
-ewringd	gewrongen	Overgeneralisation+Prefix ge without onset
-wringd	gewrongen	Overgeneralisation+Lacking ge prefix
-gewringde	gewrongene	Overgeneralisation+
-ewringde	gewrongene	Overgeneralisation+Prefix ge without onset
-gewringt	gewrongen	Overgeneralisation
-ewringt	gewrongen	Overgeneralisation
-wringt	gewrongen	Overgeneralisation
-gewringen	gewrongen	Wrong -en suffix
-ewringen	gewrongen	Wrong -en suffix
-wringen	gewrongen	Wrong -en suffix
-gewrongd	gewrongen	Overgeneralisation
-gewrongt	gewrongen	Overgeneralisation
-ewrongen	gewrongen	Prefix ge without onset
-wrongen	gewrongen	Lacking ge prefix
-zegde	zei	Overgeneralisation
-zegden	zeiden	Overgeneralisation
-zeide	zei	Irregular form plus regular suffix
-ezegd	gezegd	Prefix ge without onset
-zegd	gezegd	Lacking ge prefix
-ezegde	gezegde	Overgeneralisation+Prefix ge without onset
-gezegt	gezegd	Overgeneralisation
-ezegt	gezegd	Overgeneralisation
-zegt	gezegd	Overgeneralisation
-gezeggen	gezegd	Wrong -en suffix
-ezeggen	gezegd	Wrong -en suffix
-zeggen	gezegd	Wrong -en suffix
-zendde	zond	Overgeneralisation
-zendden	zonden	Overgeneralisation
-zondde	zond	Irregular form plus regular suffix
-zondden	zonden	Irregular form plus regular suffix
-gezend	gezonden	Overgeneralisation
-ezend	gezonden	Overgeneralisation
-zend	gezonden	Overgeneralisation
-gezende	gezondene	Overgeneralisation+
-ezende	gezondene	Overgeneralisation+Prefix ge without onset
-gezenden	gezonden	Wrong -en suffix
-ezenden	gezonden	Wrong -en suffix
-zenden	gezonden	Wrong -en suffix
-gezond	gezonden	Overgeneralisation
-ezonden	gezonden	Prefix ge without onset
-zonden	zonnen	Irregular form plus regular suffix
-zijgde	zeeg	Overgeneralisation
-zijgden	zegen	Overgeneralisation
-zeegde	zeeg	Irregular form plus regular suffix
-zeegden	zegen	Irregular form plus regular suffix
-gezijgd	gezegen	Overgeneralisation+
-ezijgd	gezegen	Overgeneralisation+Prefix ge without onset
-zijgd	gezegen	Overgeneralisation+Lacking ge prefix
-gezijgde	gezegene	Overgeneralisation+
-ezijgde	gezegene	Overgeneralisation+Prefix ge without onset
-gezijgt	gezegen	Overgeneralisation
-ezijgt	gezegen	Overgeneralisation
-zijgt	gezegen	Overgeneralisation
-gezijgen	gezegen	Wrong -en suffix
-ezijgen	gezegen	Wrong -en suffix
-zijgen	gezegen	Wrong -en suffix
-gezeegd	gezegen	Overgeneralisation
-gezeegt	gezegen	Overgeneralisation
-ezegen	gezegen	Prefix ge without onset
-zegen	gezegen	Lacking ge prefix
-zijde	was	Overgeneralisation
-zijden	waren	Overgeneralisation
-wasde	was	Irregular form plus regular suffix
-wasden	waren	Irregular form plus regular suffix
-gezijd	geweest	Overgeneralisation+
-ezijd	geweest	Overgeneralisation+Prefix ge without onset
-zijd	geweest	Overgeneralisation+Lacking ge prefix
-gezijde	geweeste	Overgeneralisation+
-ezijde	geweeste	Overgeneralisation+Prefix ge without onset
-gezijt	geweest	Overgeneralisation
-ezijt	geweest	Overgeneralisation
-zijt	geweest	Overgeneralisation
-gezijjen	geweest	Wrong -en suffix
-ezijjen	geweest	Wrong -en suffix
-zijjen	geweest	Wrong -en suffix
-eweest	geweest	Prefix ge without onset
-weest	geweest	Lacking ge prefix
-zingde	zong	Overgeneralisation
-zingden	zongen	Overgeneralisation
-zongde	zong	Irregular form plus regular suffix
-zongden	zongen	Irregular form plus regular suffix
-gezingd	gezongen	Overgeneralisation+
-ezingd	gezongen	Overgeneralisation+Prefix ge without onset
-zingd	gezongen	Overgeneralisation+Lacking ge prefix
-gezingde	gezongene	Overgeneralisation+
-ezingde	gezongene	Overgeneralisation+Prefix ge without onset
-gezingt	gezongen	Overgeneralisation
-ezingt	gezongen	Overgeneralisation
-zingt	gezongen	Overgeneralisation
-gezingen	gezongen	Wrong -en suffix
-ezingen	gezongen	Wrong -en suffix
-zingen	gezongen	Wrong -en suffix
-gezongd	gezongen	Overgeneralisation
-gezongt	gezongen	Overgeneralisation
-ezongen	gezongen	Prefix ge without onset
-zongen	gezongen	Lacking ge prefix
-zinkte	zonk	Overgeneralisation
-zinkten	zonken	Overgeneralisation
-zonkte	zonk	Irregular form plus regular suffix
-zonkten	zonken	Irregular form plus regular suffix
-gezinkt	gezonken	Overgeneralisation
-ezinkt	gezonken	Overgeneralisation
-zinkt	gezonken	Overgeneralisation
-gezinkte	gezonkene	Overgeneralisation+
-ezinkte	gezonkene	Overgeneralisation+Prefix ge without onset
-gezinken	gezonken	Wrong -en suffix
-ezinken	gezonken	Wrong -en suffix
-zinken	gezonken	Wrong -en suffix
-gezonkt	gezonken	Overgeneralisation
-ezonken	gezonken	Prefix ge without onset
-zonken	gezonken	Lacking ge prefix
-zinde	zon	Overgeneralisation
-zinden	zonnen	Overgeneralisation
-zonde	zon	Irregular form plus regular suffix
-gezind	gezonnen	Overgeneralisation+
-ezind	gezonnen	Overgeneralisation+Prefix ge without onset
-zind	gezonnen	Overgeneralisation+Lacking ge prefix
-gezinde	gezonnene	Overgeneralisation+
-ezinde	gezonnene	Overgeneralisation+Prefix ge without onset
-gezint	gezonnen	Overgeneralisation
-ezint	gezonnen	Overgeneralisation
-zint	gezonnen	Overgeneralisation
-gezinnen	gezonnen	Wrong -en suffix
-ezinnen	gezonnen	Wrong -en suffix
-zinnen	gezonnen	Wrong -en suffix
-gezont	gezonnen	Overgeneralisation
-ezonnen	gezonnen	Prefix ge without onset
-zonnen	gezonnen	Lacking ge prefix
-zitte	zat	Overgeneralisation
-zitten	gezeten	Wrong -en suffix
-zatte	zat	Irregular form plus regular suffix
-zatten	zaten	Irregular form plus regular suffix
-gezit	gezeten	Overgeneralisation
-ezit	gezeten	Overgeneralisation
-zit	gezeten	Overgeneralisation
-gezitte	gezetene	Overgeneralisation+
-ezitte	gezetene	Overgeneralisation+Prefix ge without onset
-gezitten	gezeten	Wrong -en suffix
-ezitten	gezeten	Wrong -en suffix
-gezeet	gezeten	Overgeneralisation
-ezeten	gezeten	Prefix ge without onset
-zeten	gezeten	Lacking ge prefix
-zoekte	zocht	Overgeneralisation
-zoekten	zochten	Overgeneralisation
-zochtte	zocht	Irregular form plus regular suffix
-zochtten	zochten	Irregular form plus regular suffix
-gezoekt	gezocht	Overgeneralisation
-ezoekt	gezocht	Overgeneralisation
-zoekt	gezocht	Overgeneralisation
-gezoekte	gezochte	Overgeneralisation+
-ezoekte	gezochte	Overgeneralisation+Prefix ge without onset
-gezoeken	gezocht	Wrong -en suffix
-ezoeken	gezocht	Wrong -en suffix
-zoeken	gezocht	Wrong -en suffix
-ezocht	gezocht	Prefix ge without onset
-zocht	gezocht	Lacking ge prefix
-zuigde	zoog	Overgeneralisation
-zuigden	zogen	Overgeneralisation
-zoogde	zoog	Irregular form plus regular suffix
-zoogden	zogen	Irregular form plus regular suffix
-gezuigd	gezogen	Overgeneralisation+
-ezuigd	gezogen	Overgeneralisation+Prefix ge without onset
-zuigd	gezogen	Overgeneralisation+Lacking ge prefix
-gezuigde	gezogene	Overgeneralisation+
-ezuigde	gezogene	Overgeneralisation+Prefix ge without onset
-gezuigt	gezogen	Overgeneralisation
-ezuigt	gezogen	Overgeneralisation
-zuigt	gezogen	Overgeneralisation
-gezuigen	gezogen	Wrong -en suffix
-ezuigen	gezogen	Wrong -en suffix
-zuigen	gezogen	Wrong -en suffix
-gezoogt	gezogen	Overgeneralisation
-ezogen	gezogen	Prefix ge without onset
-zogen	gezogen	Lacking ge prefix
-zuipte	zoop	Overgeneralisation
-zuipten	zopen	Overgeneralisation
-zoopte	zoop	Irregular form plus regular suffix
-zoopten	zopen	Irregular form plus regular suffix
-gezuipt	gezopen	Overgeneralisation
-ezuipt	gezopen	Overgeneralisation
-zuipt	gezopen	Overgeneralisation
-gezuipte	gezopene	Overgeneralisation+
-ezuipte	gezopene	Overgeneralisation+Prefix ge without onset
-gezuipen	gezopen	Wrong -en suffix
-ezuipen	gezopen	Wrong -en suffix
-zuipen	gezopen	Wrong -en suffix
-gezoopt	gezopen	Overgeneralisation
-ezopen	gezopen	Prefix ge without onset
-zopen	gezopen	Lacking ge prefix
-zwelgde	zwolg	Overgeneralisation
-zwelgden	zwolgen	Overgeneralisation
-zwolgde	zwolg	Irregular form plus regular suffix
-zwolgden	zwolgen	Irregular form plus regular suffix
-gezwelgd	gezwolgen	Overgeneralisation+
-ezwelgd	gezwolgen	Overgeneralisation+Prefix ge without onset
-zwelgd	gezwolgen	Overgeneralisation+Lacking ge prefix
-gezwelgde	gezwolgene	Overgeneralisation+
-ezwelgde	gezwolgene	Overgeneralisation+Prefix ge without onset
-gezwelgt	gezwolgen	Overgeneralisation
-ezwelgt	gezwolgen	Overgeneralisation
-zwelgt	gezwolgen	Overgeneralisation
-gezwelgen	gezwolgen	Wrong -en suffix
-ezwelgen	gezwolgen	Wrong -en suffix
-zwelgen	gezwolgen	Wrong -en suffix
-gezwolgd	gezwolgen	Overgeneralisation
-gezwolgt	gezwolgen	Overgeneralisation
-ezwolgen	gezwolgen	Prefix ge without onset
-zwolgen	gezwolgen	Lacking ge prefix
-zwelde	zwol	Overgeneralisation
-zwelden	zwollen	Overgeneralisation
-zwolde	zwol	Irregular form plus regular suffix
-zwolden	zwollen	Irregular form plus regular suffix
-gezweld	gezwollen	Overgeneralisation+
-ezweld	gezwollen	Overgeneralisation+Prefix ge without onset
-zweld	gezwollen	Overgeneralisation+Lacking ge prefix
-gezwelde	gezwollene	Overgeneralisation+
-ezwelde	gezwollene	Overgeneralisation+Prefix ge without onset
-gezwelt	gezwollen	Overgeneralisation
-ezwelt	gezwollen	Overgeneralisation
-zwelt	gezwollen	Overgeneralisation
-gezwellen	gezwollen	Wrong -en suffix
-ezwellen	gezwollen	Wrong -en suffix
-zwellen	gezwollen	Wrong -en suffix
-gezwolt	gezwollen	Overgeneralisation
-ezwollen	gezwollen	Prefix ge without onset
-zwollen	gezwollen	Lacking ge prefix
-zwemde	zwom	Overgeneralisation
-zwemden	zwommen	Overgeneralisation
-zwomde	zwom	Irregular form plus regular suffix
-zwomden	zwommen	Irregular form plus regular suffix
-gezwemd	gezwommen	Overgeneralisation+
-ezwemd	gezwommen	Overgeneralisation+Prefix ge without onset
-zwemd	gezwommen	Overgeneralisation+Lacking ge prefix
-gezwemde	gezwommene	Overgeneralisation+
-ezwemde	gezwommene	Overgeneralisation+Prefix ge without onset
-gezwemt	gezwommen	Overgeneralisation
-ezwemt	gezwommen	Overgeneralisation
-zwemt	gezwommen	Overgeneralisation
-gezwemmen	gezwommen	Wrong -en suffix
-ezwemmen	gezwommen	Wrong -en suffix
-zwemmen	gezwommen	Wrong -en suffix
-gezwomt	gezwommen	Overgeneralisation
-ezwommen	gezwommen	Prefix ge without onset
-zwommen	gezwommen	Lacking ge prefix
-zweerde	zwoer	Overgeneralisation
-zweerden	zwoeren	Overgeneralisation
-zwoerde	zwoer	Irregular form plus regular suffix
-zwoerden	zwoeren	Irregular form plus regular suffix
-gezweerd	gezworen	Overgeneralisation+
-ezweerd	gezworen	Overgeneralisation+Prefix ge without onset
-zweerd	gezworen	Overgeneralisation+Lacking ge prefix
-gezweerde	gezworene	Overgeneralisation+
-ezweerde	gezworene	Overgeneralisation+Prefix ge without onset
-gezweert	gezworen	Overgeneralisation
-ezweert	gezworen	Overgeneralisation
-zweert	gezworen	Overgeneralisation
-gezweren	gezworen	Wrong -en suffix
-ezweren	gezworen	Wrong -en suffix
-zweren	gezworen	Wrong -en suffix
-gezwoort	gezworen	Overgeneralisation
-ezworen	gezworen	Prefix ge without onset
-zworen	gezworen	Lacking ge prefix
-zwerfde	zwierf	Overgeneralisation
-zwerfden	zwierven	Overgeneralisation
-zwierfde	zwierf	Irregular form plus regular suffix
-zwierfden	zwierven	Irregular form plus regular suffix
-gezwerfd	gezworven	Overgeneralisation+
-ezwerfd	gezworven	Overgeneralisation+Prefix ge without onset
-zwerfd	gezworven	Overgeneralisation+Lacking ge prefix
-gezwerfde	gezworvene	Overgeneralisation+
-ezwerfde	gezworvene	Overgeneralisation+Prefix ge without onset
-gezwerft	gezworven	Overgeneralisation
-ezwerft	gezworven	Overgeneralisation
-zwerft	gezworven	Overgeneralisation
-gezwerfen	gezworven	Wrong -en suffix
-ezwerfen	gezworven	Wrong -en suffix
-zwerfen	gezworven	Wrong -en suffix
-gezworfd	gezworven	Overgeneralisation
-gezworft	gezworven	Overgeneralisation
-ezworven	gezworven	Prefix ge without onset
-zworven	gezworven	Lacking ge prefix
-zwijgde	zweeg	Overgeneralisation
-zwijgden	zwegen	Overgeneralisation
-zweegde	zweeg	Irregular form plus regular suffix
-zweegden	zwegen	Irregular form plus regular suffix
-gezwijgd	gezwegen	Overgeneralisation+
-ezwijgd	gezwegen	Overgeneralisation+Prefix ge without onset
-zwijgd	gezwegen	Overgeneralisation+Lacking ge prefix
-gezwijgde	gezwegene	Overgeneralisation+
-ezwijgde	gezwegene	Overgeneralisation+Prefix ge without onset
-gezwijgt	gezwegen	Overgeneralisation
-ezwijgt	gezwegen	Overgeneralisation
-zwijgt	gezwegen	Overgeneralisation
-gezwijgen	gezwegen	Wrong -en suffix
-ezwijgen	gezwegen	Wrong -en suffix
-zwijgen	gezwegen	Wrong -en suffix
-gezweegd	gezwegen	Overgeneralisation
-gezweegt	gezwegen	Overgeneralisation
-ezwegen	gezwegen	Prefix ge without onset
-zwegen	gezwegen	Lacking ge prefix
+gebakt	gebakken	Overgeneralisation
+ebakt	gebakken	Overgeneralisation
+bakt	gebakken	Overgeneralisation
+gebakte	gebakkene	Overgeneralisation+
+ebakte	gebakkene	Overgeneralisation+Prefix ge without onset
+ebakken	gebakken	Prefix ge without onset
+bakken	gebakken	Lacking ge prefix
+geband	gebannen	Overgeneralisation
+eband	gebannen	Overgeneralisation+Prefix ge without onset
+band	gebannen	Overgeneralisation+Lacking ge prefix
+gebande	gebannene	Overgeneralisation+
+ebande	gebannene	Overgeneralisation+Prefix ge without onset
+gebant	gebannen	Overgeneralisation
+ebant	gebannen	Overgeneralisation
+bant	gebannen	Overgeneralisation
+ebannen	gebannen	Prefix ge without onset
+bannen	gebannen	Lacking ge prefix
+gebarst	gebarsten	Overgeneralisation
+ebarst	gebarsten	Overgeneralisation
+barst	gebarsten	Overgeneralisation
+gebarste	gebarstene	Overgeneralisation+
+ebarste	gebarstene	Overgeneralisation+Prefix ge without onset
+ebarsten	gebarsten	Prefix ge without onset
+barsten	gebarsten	Lacking ge prefix
+bederfde	bedorvene	Overgeneralisation
+bederfden	bedierven	Overgeneralisation
+bedierfde	bedierf	Irregular form plus regular suffix
+bedierfden	bedierven	Irregular form plus regular suffix
+bederfd	bedorven	Overgeneralisation
+bederft	bedorven	Overgeneralisation
+bederfen	bedorven	Wrong -en suffix
+bedorfd	bedorven	Overgeneralisation
+bedorft	bedorven	Overgeneralisation
+bedriegde	bedrogene	Overgeneralisation
+bedriegden	bedrogen	Overgeneralisation
+bedroogde	bedroog	Irregular form plus regular suffix
+bedroogden	bedrogen	Irregular form plus regular suffix
+bedriegd	bedrogen	Overgeneralisation
+bedriegt	bedrogen	Overgeneralisation
+bedriegen	bedrogen	Wrong -en suffix
+bedroogt	bedrogen	Overgeneralisation
+beginde	begonnene	Overgeneralisation
+beginden	begonnen	Overgeneralisation
+begonde	begon	Irregular form plus regular suffix
+begonden	begonnen	Irregular form plus regular suffix
+begind	begonnen	Overgeneralisation
+begint	begonnen	Overgeneralisation
+beginnen	begonnen	Wrong -en suffix
+begont	begonnen	Overgeneralisation
+behangde	behangene	Overgeneralisation
+behangden	behingen	Overgeneralisation
+behingde	behing	Irregular form plus regular suffix
+behingden	behingen	Irregular form plus regular suffix
+behangd	behangen	Overgeneralisation
+behangt	behangen	Overgeneralisation
+bergde	borg	Overgeneralisation
+bergden	borgen	Overgeneralisation
+borgde	borg	Irregular form plus regular suffix
+borgden	borgen	Irregular form plus regular suffix
+gebergd	geborgen	Overgeneralisation+
+ebergd	geborgen	Overgeneralisation+Prefix ge without onset
+bergd	geborgen	Overgeneralisation+Lacking ge prefix
+gebergde	geborgene	Overgeneralisation+
+ebergde	geborgene	Overgeneralisation+Prefix ge without onset
+gebergt	geborgen	Overgeneralisation
+ebergt	geborgen	Overgeneralisation
+bergt	geborgen	Overgeneralisation
+gebergen	geborgen	Wrong -en suffix
+ebergen	geborgen	Wrong -en suffix
+bergen	geborgen	Wrong -en suffix
+geborgd	geborgen	Overgeneralisation
+geborgt	geborgen	Overgeneralisation
+eborgen	geborgen	Prefix ge without onset
+borgen	geborgen	Lacking ge prefix
+beveelde	bevolene	Overgeneralisation
+beveelden	bevalen	Overgeneralisation
+bevalde	beval	Irregular form plus regular suffix
+bevalden	bevalen	Irregular form plus regular suffix
+beveeld	bevolen	Overgeneralisation
+beveelt	bevolen	Overgeneralisation
+bevelen	bevolen	Wrong -en suffix
+bevoolt	bevolen	Overgeneralisation
+bezwijkte	bezwekene	Overgeneralisation
+bezwijkten	bezweken	Overgeneralisation
+bezweekte	bezweek	Irregular form plus regular suffix
+bezweekten	bezweken	Irregular form plus regular suffix
+bezwijkt	bezweken	Overgeneralisation
+bezwijken	bezweken	Wrong -en suffix
+bezweekt	bezweken	Overgeneralisation
+bidde	bad	Overgeneralisation
+bidden	gebeden	Wrong -en suffix
+badde	bad	Irregular form plus regular suffix
+badden	baden	Irregular form plus regular suffix
+gebid	gebeden	Overgeneralisation
+ebid	gebeden	Overgeneralisation
+bid	gebeden	Overgeneralisation
+gebidde	gebedene	Overgeneralisation+
+ebidde	gebedene	Overgeneralisation+Prefix ge without onset
+gebidden	gebeden	Wrong -en suffix
+ebidden	gebeden	Wrong -en suffix
+gebeed	gebeden	Overgeneralisation
+ebeden	gebeden	Prefix ge without onset
+beden	gebeden	Lacking ge prefix
+biedde	bood	Overgeneralisation
+biedden	boden	Overgeneralisation
+boodde	bood	Irregular form plus regular suffix
+boodden	boden	Irregular form plus regular suffix
+gebied	geboden	Overgeneralisation
+ebied	geboden	Overgeneralisation
+bied	geboden	Overgeneralisation
+gebiede	gebodene	Overgeneralisation+
+ebiede	gebodene	Overgeneralisation+Prefix ge without onset
+gebieden	geboden	Wrong -en suffix
+ebieden	geboden	Wrong -en suffix
+bieden	geboden	Wrong -en suffix
+geboodt	geboden	Overgeneralisation
+gebood	geboden	Overgeneralisation
+eboden	geboden	Prefix ge without onset
+boden	geboden	Lacking ge prefix
+bijtte	beet	Overgeneralisation
+bijtten	beten	Overgeneralisation
+beette	beet	Irregular form plus regular suffix
+beetten	beten	Irregular form plus regular suffix
+gebijt	gebeten	Overgeneralisation
+ebijt	gebeten	Overgeneralisation
+bijt	gebeten	Overgeneralisation
+gebijte	gebetene	Overgeneralisation+
+ebijte	gebetene	Overgeneralisation+Prefix ge without onset
+gebijten	gebeten	Wrong -en suffix
+ebijten	gebeten	Wrong -en suffix
+bijten	gebeten	Wrong -en suffix
+gebeet	gebeten	Overgeneralisation
+ebeten	gebeten	Prefix ge without onset
+beten	gebeten	Lacking ge prefix
+bindde	bond	Overgeneralisation
+bindden	bonden	Overgeneralisation
+bondde	bond	Irregular form plus regular suffix
+bondden	bonden	Irregular form plus regular suffix
+gebind	gebonden	Overgeneralisation
+ebind	gebonden	Overgeneralisation
+bind	gebonden	Overgeneralisation
+gebinde	gebondene	Overgeneralisation+
+ebinde	gebondene	Overgeneralisation+Prefix ge without onset
+gebinden	gebonden	Wrong -en suffix
+ebinden	gebonden	Wrong -en suffix
+binden	gebonden	Wrong -en suffix
+gebond	gebonden	Overgeneralisation
+ebonden	gebonden	Prefix ge without onset
+bonden	gebonden	Lacking ge prefix
+blaasde	blies	Overgeneralisation
+blaasden	bliezen	Overgeneralisation
+bliesde	blies	Irregular form plus regular suffix
+bliesden	bliezen	Irregular form plus regular suffix
+geblaasd	geblazen	Overgeneralisation
+eblaasd	geblazen	Overgeneralisation+Prefix ge without onset
+blaasd	geblazen	Overgeneralisation+Lacking ge prefix
+geblaasde	geblazene	Overgeneralisation+
+eblaasde	geblazene	Overgeneralisation+Prefix ge without onset
+geblaast	geblazen	Overgeneralisation
+eblaast	geblazen	Overgeneralisation
+blaast	geblazen	Overgeneralisation
+geblasen	geblazen	Wrong -en suffix
+eblasen	geblazen	Wrong -en suffix
+blasen	geblazen	Wrong -en suffix
+eblazen	geblazen	Prefix ge without onset
+blazen	geblazen	Lacking ge prefix
+blijkte	bleek	Overgeneralisation
+blijkten	bleken	Overgeneralisation
+bleekte	bleek	Irregular form plus regular suffix
+bleekten	bleken	Irregular form plus regular suffix
+geblijkt	gebleken	Overgeneralisation
+eblijkt	gebleken	Overgeneralisation
+blijkt	gebleken	Overgeneralisation
+geblijkte	geblekene	Overgeneralisation+
+eblijkte	geblekene	Overgeneralisation+Prefix ge without onset
+geblijken	gebleken	Wrong -en suffix
+eblijken	gebleken	Wrong -en suffix
+blijken	gebleken	Wrong -en suffix
+gebleekt	gebleken	Overgeneralisation
+ebleken	gebleken	Prefix ge without onset
+bleken	gebleken	Lacking ge prefix
+blijfde	bleef	Overgeneralisation
+blijfden	bleven	Overgeneralisation
+bleefde	bleef	Irregular form plus regular suffix
+bleefden	bleven	Irregular form plus regular suffix
+geblijfd	gebleven	Overgeneralisation+
+eblijfd	gebleven	Overgeneralisation+Prefix ge without onset
+blijfd	gebleven	Overgeneralisation+Lacking ge prefix
+geblijfde	geblevene	Overgeneralisation+
+eblijfde	geblevene	Overgeneralisation+Prefix ge without onset
+geblijft	gebleven	Overgeneralisation
+eblijft	gebleven	Overgeneralisation
+blijft	gebleven	Overgeneralisation
+geblijfen	gebleven	Wrong -en suffix
+eblijfen	gebleven	Wrong -en suffix
+blijfen	gebleven	Wrong -en suffix
+gebleefd	gebleven	Overgeneralisation
+gebleeft	gebleven	Overgeneralisation
+ebleven	gebleven	Prefix ge without onset
+bleven	gebleven	Lacking ge prefix
+blinkte	blonk	Overgeneralisation
+blinkten	blonken	Overgeneralisation
+blonkte	blonk	Irregular form plus regular suffix
+blonkten	blonken	Irregular form plus regular suffix
+geblinkt	geblonken	Overgeneralisation
+eblinkt	geblonken	Overgeneralisation
+blinkt	geblonken	Overgeneralisation
+geblinkte	geblonkene	Overgeneralisation+
+eblinkte	geblonkene	Overgeneralisation+Prefix ge without onset
+geblinken	geblonken	Wrong -en suffix
+eblinken	geblonken	Wrong -en suffix
+blinken	geblonken	Wrong -en suffix
+geblonkt	geblonken	Overgeneralisation
+eblonken	geblonken	Prefix ge without onset
+blonken	geblonken	Lacking ge prefix
+gebraad	gebraden	Overgeneralisation
+ebraad	gebraden	Overgeneralisation
+braad	gebraden	Overgeneralisation
+gebrade	gebradene	Overgeneralisation+
+ebrade	gebradene	Overgeneralisation+Prefix ge without onset
+ebraden	gebraden	Prefix ge without onset
+braden	gebraden	Lacking ge prefix
+breekte	brak	Overgeneralisation
+breekten	braken	Overgeneralisation
+brakte	brak	Irregular form plus regular suffix
+brakten	braken	Irregular form plus regular suffix
+gebreekt	gebroken	Overgeneralisation
+ebreekt	gebroken	Overgeneralisation
+breekt	gebroken	Overgeneralisation
+gebreekte	gebrokene	Overgeneralisation+
+ebreekte	gebrokene	Overgeneralisation+Prefix ge without onset
+gebreken	gebroken	Wrong -en suffix
+ebreken	gebroken	Wrong -en suffix
+breken	gebroken	Wrong -en suffix
+gebrookt	gebroken	Overgeneralisation
+ebroken	gebroken	Prefix ge without onset
+broken	gebroken	Lacking ge prefix
+brengde	bracht	Overgeneralisation
+brengden	brachten	Overgeneralisation
+brachtde	bracht	Irregular form plus regular suffix
+brachtden	brachten	Irregular form plus regular suffix
+gebrengd	gebracht	Overgeneralisation+
+ebrengd	gebracht	Overgeneralisation+Prefix ge without onset
+brengd	gebracht	Overgeneralisation+Lacking ge prefix
+gebrengde	gebrachte	Overgeneralisation+
+ebrengde	gebrachte	Overgeneralisation+Prefix ge without onset
+gebrengt	gebracht	Overgeneralisation
+ebrengt	gebracht	Overgeneralisation
+brengt	gebracht	Overgeneralisation
+gebrengen	gebracht	Wrong -en suffix
+ebrengen	gebracht	Wrong -en suffix
+brengen	gebracht	Wrong -en suffix
+ebracht	gebracht	Prefix ge without onset
+bracht	gebracht	Lacking ge prefix
+gebrouwd	gebrouwen	Overgeneralisation
+ebrouwd	gebrouwen	Overgeneralisation+Prefix ge without onset
+brouwd	gebrouwen	Overgeneralisation+Lacking ge prefix
+gebrouwde	gebrouwene	Overgeneralisation+
+ebrouwde	gebrouwene	Overgeneralisation+Prefix ge without onset
+gebrouwt	gebrouwen	Overgeneralisation
+ebrouwt	gebrouwen	Overgeneralisation
+brouwt	gebrouwen	Overgeneralisation
+ebrouwen	gebrouwen	Prefix ge without onset
+brouwen	gebrouwen	Lacking ge prefix
+buigde	boog	Overgeneralisation
+buigden	bogen	Overgeneralisation
+boogde	boog	Irregular form plus regular suffix
+boogden	bogen	Irregular form plus regular suffix
+gebuigd	gebogen	Overgeneralisation+
+ebuigd	gebogen	Overgeneralisation+Prefix ge without onset
+buigd	gebogen	Overgeneralisation+Lacking ge prefix
+gebuigde	gebogene	Overgeneralisation+
+ebuigde	gebogene	Overgeneralisation+Prefix ge without onset
+gebuigt	gebogen	Overgeneralisation
+ebuigt	gebogen	Overgeneralisation
+buigt	gebogen	Overgeneralisation
+gebuigen	gebogen	Wrong -en suffix
+ebuigen	gebogen	Wrong -en suffix
+buigen	gebogen	Wrong -en suffix
+geboogt	gebogen	Overgeneralisation
+ebogen	gebogen	Prefix ge without onset
+bogen	gebogen	Lacking ge prefix
+denkte	dacht	Overgeneralisation
+denkten	dachten	Overgeneralisation
+dachtte	dacht	Irregular form plus regular suffix
+dachtten	dachten	Irregular form plus regular suffix
+gedenkt	gedacht	Overgeneralisation
+edenkt	gedacht	Overgeneralisation
+denkt	gedacht	Overgeneralisation
+gedenkte	gedachte	Overgeneralisation+
+edenkte	gedachte	Overgeneralisation+Prefix ge without onset
+gedenken	gedacht	Wrong -en suffix
+edenken	gedacht	Wrong -en suffix
+denken	gedacht	Wrong -en suffix
+edacht	gedacht	Prefix ge without onset
+dacht	gedacht	Lacking ge prefix
+dingde	dong	Overgeneralisation
+dingden	dongen	Overgeneralisation
+dongde	dong	Irregular form plus regular suffix
+dongden	dongen	Irregular form plus regular suffix
+gedingd	gedongen	Overgeneralisation+
+edingd	gedongen	Overgeneralisation+Prefix ge without onset
+dingd	gedongen	Overgeneralisation+Lacking ge prefix
+gedingde	gedongene	Overgeneralisation+
+edingde	gedongene	Overgeneralisation+Prefix ge without onset
+gedingt	gedongen	Overgeneralisation
+edingt	gedongen	Overgeneralisation
+dingt	gedongen	Overgeneralisation
+gedingen	gedongen	Wrong -en suffix
+edingen	gedongen	Wrong -en suffix
+dingen	gedongen	Wrong -en suffix
+gedongd	gedongen	Overgeneralisation
+gedongt	gedongen	Overgeneralisation
+edongen	gedongen	Prefix ge without onset
+dongen	gedongen	Lacking ge prefix
+doete	deed	Overgeneralisation
+doeten	deden	Overgeneralisation
+deedte	deed	Irregular form plus regular suffix
+deedten	deden	Irregular form plus regular suffix
+gedoet	gedaan	Overgeneralisation
+edoet	gedaan	Overgeneralisation
+doet	gedaan	Overgeneralisation
+gedoete	gedaane	Overgeneralisation+
+edoete	gedaane	Overgeneralisation+Prefix ge without onset
+gedoen	gedaan	Wrong -en suffix
+edoen	gedaan	Wrong -en suffix
+doen	gedaan	Wrong -en suffix
+edaan	gedaan	Prefix ge without onset
+daan	gedaan	Lacking ge prefix
+draagde	droeg	Overgeneralisation
+draagden	droegen	Overgeneralisation
+droegde	droeg	Irregular form plus regular suffix
+droegden	droegen	Irregular form plus regular suffix
+gedraagd	gedragen	Overgeneralisation
+edraagd	gedragen	Overgeneralisation+Prefix ge without onset
+draagd	gedragen	Overgeneralisation+Lacking ge prefix
+gedraagde	gedragene	Overgeneralisation+
+edraagde	gedragene	Overgeneralisation+Prefix ge without onset
+gedraagt	gedragen	Overgeneralisation
+edraagt	gedragen	Overgeneralisation
+draagt	gedragen	Overgeneralisation
+edragen	gedragen	Prefix ge without onset
+dragen	gedragen	Lacking ge prefix
+drijfde	dreef	Overgeneralisation
+drijfden	dreven	Overgeneralisation
+dreefde	dreef	Irregular form plus regular suffix
+dreefden	dreven	Irregular form plus regular suffix
+gedrijfd	gedreven	Overgeneralisation+
+edrijfd	gedreven	Overgeneralisation+Prefix ge without onset
+drijfd	gedreven	Overgeneralisation+Lacking ge prefix
+gedrijfde	gedrevene	Overgeneralisation+
+edrijfde	gedrevene	Overgeneralisation+Prefix ge without onset
+gedrijft	gedreven	Overgeneralisation
+edrijft	gedreven	Overgeneralisation
+drijft	gedreven	Overgeneralisation
+gedrijfen	gedreven	Wrong -en suffix
+edrijfen	gedreven	Wrong -en suffix
+drijfen	gedreven	Wrong -en suffix
+gedreefd	gedreven	Overgeneralisation
+gedreeft	gedreven	Overgeneralisation
+edreven	gedreven	Prefix ge without onset
+dreven	gedreven	Lacking ge prefix
+dringde	drong	Overgeneralisation
+dringden	drongen	Overgeneralisation
+drongde	drong	Irregular form plus regular suffix
+drongden	drongen	Irregular form plus regular suffix
+gedringd	gedrongen	Overgeneralisation+
+edringd	gedrongen	Overgeneralisation+Prefix ge without onset
+dringd	gedrongen	Overgeneralisation+Lacking ge prefix
+gedringde	gedrongene	Overgeneralisation+
+edringde	gedrongene	Overgeneralisation+Prefix ge without onset
+gedringt	gedrongen	Overgeneralisation
+edringt	gedrongen	Overgeneralisation
+dringt	gedrongen	Overgeneralisation
+gedringen	gedrongen	Wrong -en suffix
+edringen	gedrongen	Wrong -en suffix
+dringen	gedrongen	Wrong -en suffix
+gedrongd	gedrongen	Overgeneralisation
+gedrongt	gedrongen	Overgeneralisation
+edrongen	gedrongen	Prefix ge without onset
+drongen	gedrongen	Lacking ge prefix
+drinkte	dronk	Overgeneralisation
+drinkten	dronken	Overgeneralisation
+dronkte	dronk	Irregular form plus regular suffix
+dronkten	dronken	Irregular form plus regular suffix
+gedrinkt	gedronken	Overgeneralisation
+edrinkt	gedronken	Overgeneralisation
+drinkt	gedronken	Overgeneralisation
+gedrinkte	gedronkene	Overgeneralisation+
+edrinkte	gedronkene	Overgeneralisation+Prefix ge without onset
+gedrinken	gedronken	Wrong -en suffix
+edrinken	gedronken	Wrong -en suffix
+drinken	gedronken	Wrong -en suffix
+gedronkt	gedronken	Overgeneralisation
+edronken	gedronken	Prefix ge without onset
+dronken	gedronken	Lacking ge prefix
+druipte	droop	Overgeneralisation
+druipten	dropen	Overgeneralisation
+droopte	droop	Irregular form plus regular suffix
+droopten	dropen	Irregular form plus regular suffix
+gedruipt	gedropen	Overgeneralisation
+edruipt	gedropen	Overgeneralisation
+druipt	gedropen	Overgeneralisation
+gedruipte	gedropene	Overgeneralisation+
+edruipte	gedropene	Overgeneralisation+Prefix ge without onset
+gedruipen	gedropen	Wrong -en suffix
+edruipen	gedropen	Wrong -en suffix
+druipen	gedropen	Wrong -en suffix
+gedroopt	gedropen	Overgeneralisation
+edropen	gedropen	Prefix ge without onset
+dropen	gedropen	Lacking ge prefix
+duikte	dook	Overgeneralisation
+duikten	doken	Overgeneralisation
+dookte	dook	Irregular form plus regular suffix
+dookten	doken	Irregular form plus regular suffix
+geduikt	gedoken	Overgeneralisation
+eduikt	gedoken	Overgeneralisation
+duikt	gedoken	Overgeneralisation
+geduikte	gedokene	Overgeneralisation+
+eduikte	gedokene	Overgeneralisation+Prefix ge without onset
+geduiken	gedoken	Wrong -en suffix
+eduiken	gedoken	Wrong -en suffix
+duiken	gedoken	Wrong -en suffix
+gedookt	gedoken	Overgeneralisation
+edoken	gedoken	Prefix ge without onset
+doken	gedoken	Lacking ge prefix
+dwingde	dwong	Overgeneralisation
+dwingden	dwongen	Overgeneralisation
+dwongde	dwong	Irregular form plus regular suffix
+dwongden	dwongen	Irregular form plus regular suffix
+gedwingd	gedwongen	Overgeneralisation+
+edwingd	gedwongen	Overgeneralisation+Prefix ge without onset
+dwingd	gedwongen	Overgeneralisation+Lacking ge prefix
+gedwingde	gedwongene	Overgeneralisation+
+edwingde	gedwongene	Overgeneralisation+Prefix ge without onset
+gedwingt	gedwongen	Overgeneralisation
+edwingt	gedwongen	Overgeneralisation
+dwingt	gedwongen	Overgeneralisation
+gedwingen	gedwongen	Wrong -en suffix
+edwingen	gedwongen	Wrong -en suffix
+dwingen	gedwongen	Wrong -en suffix
+gedwongd	gedwongen	Overgeneralisation
+gedwongt	gedwongen	Overgeneralisation
+edwongen	gedwongen	Prefix ge without onset
+dwongen	gedwongen	Lacking ge prefix
+eette	at	Overgeneralisation
+eetten	aten	Overgeneralisation
+atte	at	Irregular form plus regular suffix
+atten	aten	Irregular form plus regular suffix
+geeet	gegeten	Overgeneralisation+
+eeet	gegeten	Overgeneralisation+Prefix ge without onset
+eet	gegeten	Overgeneralisation
+geete	gegetene	Overgeneralisation+
+eete	gegetene	Overgeneralisation+Prefix ge without onset
+geëet	gegeten	Overgeneralisation
+eëet	gegeten	Overgeneralisation
+geëten	gegeten	Wrong -en suffix
+eëten	gegeten	Wrong -en suffix
+eten	gegeten	Wrong -en suffix
+gegeet	gegeten	Overgeneralisation
+egeten	gegeten	Prefix ge without onset
+geten	gegeten	Lacking ge prefix
+fluitte	floot	Overgeneralisation
+fluitten	floten	Overgeneralisation
+flootte	floot	Irregular form plus regular suffix
+flootten	floten	Irregular form plus regular suffix
+gefluit	gefloten	Overgeneralisation
+efluit	gefloten	Overgeneralisation
+fluit	gefloten	Overgeneralisation
+gefluite	geflotene	Overgeneralisation+
+efluite	geflotene	Overgeneralisation+Prefix ge without onset
+gefluiten	gefloten	Wrong -en suffix
+efluiten	gefloten	Wrong -en suffix
+fluiten	gefloten	Wrong -en suffix
+gefloot	gefloten	Overgeneralisation
+efloten	gefloten	Prefix ge without onset
+floten	gefloten	Lacking ge prefix
+gade	ging	Overgeneralisation
+gaden	gingen	Overgeneralisation
+gingde	ging	Irregular form plus regular suffix
+gingden	gingen	Irregular form plus regular suffix
+gegaad	gegaan	Overgeneralisation+
+egaad	gegaan	Overgeneralisation+Prefix ge without onset
+gaad	gegaan	Overgeneralisation+Lacking ge prefix
+gegade	gegaane	Overgeneralisation+
+egade	gegaane	Overgeneralisation+Prefix ge without onset
+gegaat	gegaan	Overgeneralisation
+egaat	gegaan	Overgeneralisation
+gaat	gegaan	Overgeneralisation
+egaan	gegaan	Prefix ge without onset
+gaan	gegaan	Lacking ge prefix
+geldde	gold	Overgeneralisation
+geldden	golden	Overgeneralisation
+goldde	gold	Irregular form plus regular suffix
+goldden	golden	Irregular form plus regular suffix
+gegeld	gegolden	Overgeneralisation
+egeld	gegolden	Overgeneralisation
+geld	gegolden	Overgeneralisation
+gegelde	gegoldene	Overgeneralisation+
+egelde	gegoldene	Overgeneralisation+Prefix ge without onset
+gegelden	gegolden	Wrong -en suffix
+egelden	gegolden	Wrong -en suffix
+gelden	gegolden	Wrong -en suffix
+gegold	gegolden	Overgeneralisation
+egolden	gegolden	Prefix ge without onset
+golden	gegolden	Lacking ge prefix
+geneesde	genezene	Overgeneralisation
+geneesden	genazen	Overgeneralisation
+genasde	genas	Irregular form plus regular suffix
+genasden	genazen	Irregular form plus regular suffix
+geneesd	genezen	Overgeneralisation
+geneest	genezen	Overgeneralisation
+genesen	genezen	Wrong -en suffix
+enezen	genezen	Prefix ge without onset
+nezen	genezen	Lacking ge prefix
+geniette	genoot	Overgeneralisation
+genietten	genoten	Overgeneralisation
+genootte	genoot	Irregular form plus regular suffix
+genootten	genoten	Irregular form plus regular suffix
+geniet	genoten	Overgeneralisation
+geniete	genotene	Overgeneralisation
+genieten	genoten	Wrong -en suffix
+genoot	genoten	Overgeneralisation
+enoten	genoten	Prefix ge without onset
+noten	genoten	Lacking ge prefix
+geefde	gaf	Overgeneralisation
+geefden	gaven	Overgeneralisation
+gafde	gaf	Irregular form plus regular suffix
+gafden	gaven	Irregular form plus regular suffix
+gegeefd	gegeven	Overgeneralisation
+egeefd	gegeven	Overgeneralisation+Prefix ge without onset
+geefd	gegeven	Overgeneralisation+Lacking ge prefix
+gegeefde	gegevene	Overgeneralisation+
+egeefde	gegevene	Overgeneralisation+Prefix ge without onset
+gegeeft	gegeven	Overgeneralisation
+egeeft	gegeven	Overgeneralisation
+geeft	gegeven	Overgeneralisation
+gegefen	gegeven	Wrong -en suffix
+egefen	gegeven	Wrong -en suffix
+gefen	gegeven	Wrong -en suffix
+egeven	gegeven	Prefix ge without onset
+geven	gegeven	Lacking ge prefix
+giette	goot	Overgeneralisation
+gietten	goten	Overgeneralisation
+gootte	goot	Irregular form plus regular suffix
+gootten	goten	Irregular form plus regular suffix
+gegiet	gegoten	Overgeneralisation
+egiet	gegoten	Overgeneralisation
+giet	gegoten	Overgeneralisation
+gegiete	gegotene	Overgeneralisation+
+egiete	gegotene	Overgeneralisation+Prefix ge without onset
+gegieten	gegoten	Wrong -en suffix
+egieten	gegoten	Wrong -en suffix
+gieten	gegoten	Wrong -en suffix
+gegoot	gegoten	Overgeneralisation
+egoten	gegoten	Prefix ge without onset
+goten	gegoten	Lacking ge prefix
+glijdde	gleed	Overgeneralisation
+glijdden	gleden	Overgeneralisation
+gleedde	gleed	Irregular form plus regular suffix
+gleedden	gleden	Irregular form plus regular suffix
+geglijd	gegleden	Overgeneralisation
+eglijd	gegleden	Overgeneralisation
+glijd	gegleden	Overgeneralisation
+geglijde	gegledene	Overgeneralisation+
+eglijde	gegledene	Overgeneralisation+Prefix ge without onset
+geglijden	gegleden	Wrong -en suffix
+eglijden	gegleden	Wrong -en suffix
+glijden	gegleden	Wrong -en suffix
+gegleed	gegleden	Overgeneralisation
+egleden	gegleden	Prefix ge without onset
+gleden	gegleden	Lacking ge prefix
+glimde	glom	Overgeneralisation
+glimden	glommen	Overgeneralisation
+glomde	glom	Irregular form plus regular suffix
+glomden	glommen	Irregular form plus regular suffix
+geglimd	geglommen	Overgeneralisation+
+eglimd	geglommen	Overgeneralisation+Prefix ge without onset
+glimd	geglommen	Overgeneralisation+Lacking ge prefix
+geglimde	geglommene	Overgeneralisation+
+eglimde	geglommene	Overgeneralisation+Prefix ge without onset
+geglimt	geglommen	Overgeneralisation
+eglimt	geglommen	Overgeneralisation
+glimt	geglommen	Overgeneralisation
+geglimmen	geglommen	Wrong -en suffix
+eglimmen	geglommen	Wrong -en suffix
+glimmen	geglommen	Wrong -en suffix
+geglomt	geglommen	Overgeneralisation
+eglommen	geglommen	Prefix ge without onset
+glommen	geglommen	Lacking ge prefix
+graafde	groef	Overgeneralisation
+graafden	groeven	Overgeneralisation
+groefde	groef	Irregular form plus regular suffix
+groefden	groeven	Irregular form plus regular suffix
+gegraafd	gegraven	Overgeneralisation
+egraafd	gegraven	Overgeneralisation+Prefix ge without onset
+graafd	gegraven	Overgeneralisation+Lacking ge prefix
+gegraafde	gegravene	Overgeneralisation+
+egraafde	gegravene	Overgeneralisation+Prefix ge without onset
+gegraaft	gegraven	Overgeneralisation
+egraaft	gegraven	Overgeneralisation
+graaft	gegraven	Overgeneralisation
+gegrafen	gegraven	Wrong -en suffix
+egrafen	gegraven	Wrong -en suffix
+grafen	gegraven	Wrong -en suffix
+egraven	gegraven	Prefix ge without onset
+graven	gegraven	Lacking ge prefix
+grijpte	greep	Overgeneralisation
+grijpten	grepen	Overgeneralisation
+greepte	greep	Irregular form plus regular suffix
+greepten	grepen	Irregular form plus regular suffix
+gegrijpt	gegrepen	Overgeneralisation
+egrijpt	gegrepen	Overgeneralisation
+grijpt	gegrepen	Overgeneralisation
+gegrijpte	gegrepene	Overgeneralisation+
+egrijpte	gegrepene	Overgeneralisation+Prefix ge without onset
+gegrijpen	gegrepen	Wrong -en suffix
+egrijpen	gegrepen	Wrong -en suffix
+grijpen	gegrepen	Wrong -en suffix
+gegreept	gegrepen	Overgeneralisation
+egrepen	gegrepen	Prefix ge without onset
+grepen	gegrepen	Lacking ge prefix
+hangde	hing	Overgeneralisation
+hangden	hingen	Overgeneralisation
+hingde	hing	Irregular form plus regular suffix
+hingden	hingen	Irregular form plus regular suffix
+gehangd	gehangen	Overgeneralisation
+ehangd	gehangen	Overgeneralisation+Prefix ge without onset
+hangd	gehangen	Overgeneralisation+Lacking ge prefix
+gehangde	gehangene	Overgeneralisation+
+ehangde	gehangene	Overgeneralisation+Prefix ge without onset
+gehangt	gehangen	Overgeneralisation
+ehangt	gehangen	Overgeneralisation
+hangt	gehangen	Overgeneralisation
+ehangen	gehangen	Prefix ge without onset
+hangen	gehangen	Lacking ge prefix
+hebde	had	Overgeneralisation
+hebden	hadden	Overgeneralisation
+hadde	had	Irregular form plus regular suffix
+gehebd	gehad	Overgeneralisation+
+ehebd	gehad	Overgeneralisation+Prefix ge without onset
+hebd	gehad	Overgeneralisation+Lacking ge prefix
+gehebde	gehade	Overgeneralisation+
+ehebde	gehade	Overgeneralisation+Prefix ge without onset
+gehebt	gehad	Overgeneralisation
+ehebt	gehad	Overgeneralisation
+hebt	gehad	Overgeneralisation
+gehebben	gehad	Wrong -en suffix
+ehebben	gehad	Wrong -en suffix
+hebben	gehad	Wrong -en suffix
+ehad	gehad	Prefix ge without onset
+had	gehad	Lacking ge prefix
+hefte	hief	Overgeneralisation
+heften	hieven	Overgeneralisation
+hiefte	hief	Irregular form plus regular suffix
+hieften	hieven	Irregular form plus regular suffix
+geheft	geheven	Overgeneralisation
+eheft	geheven	Overgeneralisation
+heft	geheven	Overgeneralisation
+gehefte	gehevene	Overgeneralisation+
+ehefte	gehevene	Overgeneralisation+Prefix ge without onset
+geheffen	geheven	Wrong -en suffix
+eheffen	geheven	Wrong -en suffix
+heffen	geheven	Wrong -en suffix
+geheefd	geheven	Overgeneralisation
+geheeft	geheven	Overgeneralisation
+eheven	geheven	Prefix ge without onset
+heven	geheven	Lacking ge prefix
+helpte	hielp	Overgeneralisation
+helpten	hielpen	Overgeneralisation
+hielpte	hielp	Irregular form plus regular suffix
+hielpten	hielpen	Irregular form plus regular suffix
+gehelpt	geholpen	Overgeneralisation
+ehelpt	geholpen	Overgeneralisation
+helpt	geholpen	Overgeneralisation
+gehelpte	geholpene	Overgeneralisation+
+ehelpte	geholpene	Overgeneralisation+Prefix ge without onset
+gehelpen	geholpen	Wrong -en suffix
+ehelpen	geholpen	Wrong -en suffix
+helpen	geholpen	Wrong -en suffix
+geholpt	geholpen	Overgeneralisation
+eholpen	geholpen	Prefix ge without onset
+holpen	geholpen	Lacking ge prefix
+geheet	geheten	Overgeneralisation
+eheet	geheten	Overgeneralisation
+heet	geheten	Overgeneralisation
+gehete	gehetene	Overgeneralisation+
+ehete	gehetene	Overgeneralisation+Prefix ge without onset
+eheten	geheten	Prefix ge without onset
+heten	geheten	Lacking ge prefix
+hijste	hees	Overgeneralisation
+hijsten	hesen	Overgeneralisation
+heeste	hees	Irregular form plus regular suffix
+heesten	hesen	Irregular form plus regular suffix
+gehijst	gehesen	Overgeneralisation
+ehijst	gehesen	Overgeneralisation
+hijst	gehesen	Overgeneralisation
+gehijste	gehesene	Overgeneralisation+
+ehijste	gehesene	Overgeneralisation+Prefix ge without onset
+gehijsen	gehesen	Wrong -en suffix
+ehijsen	gehesen	Wrong -en suffix
+hijsen	gehesen	Wrong -en suffix
+geheest	gehesen	Overgeneralisation
+ehesen	gehesen	Prefix ge without onset
+hesen	gehesen	Lacking ge prefix
+gehoefd	gehoeven	Overgeneralisation
+ehoefd	gehoeven	Overgeneralisation+Prefix ge without onset
+hoefd	gehoeven	Overgeneralisation+Lacking ge prefix
+gehoefde	gehoevene	Overgeneralisation+
+ehoefde	gehoevene	Overgeneralisation+Prefix ge without onset
+gehoeft	gehoeven	Overgeneralisation
+ehoeft	gehoeven	Overgeneralisation
+hoeft	gehoeven	Overgeneralisation
+gehoefen	gehoeven	Wrong -en suffix
+ehoefen	gehoeven	Wrong -en suffix
+hoefen	gehoeven	Wrong -en suffix
+ehoeven	gehoeven	Prefix ge without onset
+hoeven	gehoeven	Lacking ge prefix
+houdde	hield	Overgeneralisation
+houdden	hielden	Overgeneralisation
+hieldde	hield	Irregular form plus regular suffix
+hieldden	hielden	Irregular form plus regular suffix
+gehoud	gehouden	Overgeneralisation
+ehoud	gehouden	Overgeneralisation
+houd	gehouden	Overgeneralisation
+gehoude	gehoudene	Overgeneralisation+
+ehoude	gehoudene	Overgeneralisation+Prefix ge without onset
+ehouden	gehouden	Prefix ge without onset
+houden	gehouden	Lacking ge prefix
+houwde	hieuw	Overgeneralisation
+houwden	hieuwen	Overgeneralisation
+hieuwde	hieuw	Irregular form plus regular suffix
+hieuwden	hieuwen	Irregular form plus regular suffix
+gehouwd	gehouwen	Overgeneralisation
+ehouwd	gehouwen	Overgeneralisation+Prefix ge without onset
+houwd	gehouwen	Overgeneralisation+Lacking ge prefix
+gehouwde	gehouwene	Overgeneralisation+
+ehouwde	gehouwene	Overgeneralisation+Prefix ge without onset
+gehouwt	gehouwen	Overgeneralisation
+ehouwt	gehouwen	Overgeneralisation
+houwt	gehouwen	Overgeneralisation
+ehouwen	gehouwen	Prefix ge without onset
+houwen	gehouwen	Lacking ge prefix
+ejaagd	gejaagd	Prefix ge without onset
+jaagd	gejaagd	Lacking ge prefix
+ejaagde	gejaagde	Overgeneralisation+Prefix ge without onset
+gejaagt	gejaagd	Overgeneralisation
+ejaagt	gejaagd	Overgeneralisation
+jaagt	gejaagd	Overgeneralisation
+gejagen	gejaagd	Wrong -en suffix
+ejagen	gejaagd	Wrong -en suffix
+jagen	gejaagd	Wrong -en suffix
+kiesde	koos	Overgeneralisation
+kiesden	kozen	Overgeneralisation
+koosde	koos	Irregular form plus regular suffix
+koosden	kozen	Irregular form plus regular suffix
+gekiesd	gekozen	Overgeneralisation+
+ekiesd	gekozen	Overgeneralisation+Prefix ge without onset
+kiesd	gekozen	Overgeneralisation+Lacking ge prefix
+gekiesde	gekozene	Overgeneralisation+
+ekiesde	gekozene	Overgeneralisation+Prefix ge without onset
+gekiest	gekozen	Overgeneralisation
+ekiest	gekozen	Overgeneralisation
+kiest	gekozen	Overgeneralisation
+gekiesen	gekozen	Wrong -en suffix
+ekiesen	gekozen	Wrong -en suffix
+kiesen	gekozen	Wrong -en suffix
+gekoost	gekozen	Overgeneralisation
+ekozen	gekozen	Prefix ge without onset
+kozen	gekozen	Lacking ge prefix
+kijkte	keek	Overgeneralisation
+kijkten	keken	Overgeneralisation
+keekte	keek	Irregular form plus regular suffix
+keekten	keken	Irregular form plus regular suffix
+gekijkt	gekeken	Overgeneralisation
+ekijkt	gekeken	Overgeneralisation
+kijkt	gekeken	Overgeneralisation
+gekijkte	gekekene	Overgeneralisation+
+ekijkte	gekekene	Overgeneralisation+Prefix ge without onset
+gekijken	gekeken	Wrong -en suffix
+ekijken	gekeken	Wrong -en suffix
+kijken	gekeken	Wrong -en suffix
+gekeekt	gekeken	Overgeneralisation
+ekeken	gekeken	Prefix ge without onset
+keken	gekeken	Lacking ge prefix
+klimde	klom	Overgeneralisation
+klimden	klommen	Overgeneralisation
+klomde	klom	Irregular form plus regular suffix
+klomden	klommen	Irregular form plus regular suffix
+geklimd	geklommen	Overgeneralisation+
+eklimd	geklommen	Overgeneralisation+Prefix ge without onset
+klimd	geklommen	Overgeneralisation+Lacking ge prefix
+geklimde	geklommene	Overgeneralisation+
+eklimde	geklommene	Overgeneralisation+Prefix ge without onset
+geklimt	geklommen	Overgeneralisation
+eklimt	geklommen	Overgeneralisation
+klimt	geklommen	Overgeneralisation
+geklimmen	geklommen	Wrong -en suffix
+eklimmen	geklommen	Wrong -en suffix
+klimmen	geklommen	Wrong -en suffix
+geklomt	geklommen	Overgeneralisation
+eklommen	geklommen	Prefix ge without onset
+klommen	geklommen	Lacking ge prefix
+klinkte	klonk	Overgeneralisation
+klinkten	klonken	Overgeneralisation
+klonkte	klonk	Irregular form plus regular suffix
+klonkten	klonken	Irregular form plus regular suffix
+geklinkt	geklonken	Overgeneralisation
+eklinkt	geklonken	Overgeneralisation
+klinkt	geklonken	Overgeneralisation
+geklinkte	geklonkene	Overgeneralisation+
+eklinkte	geklonkene	Overgeneralisation+Prefix ge without onset
+geklinken	geklonken	Wrong -en suffix
+eklinken	geklonken	Wrong -en suffix
+klinken	geklonken	Wrong -en suffix
+geklonkt	geklonken	Overgeneralisation
+eklonken	geklonken	Prefix ge without onset
+klonken	geklonken	Lacking ge prefix
+kluifde	kloof	Overgeneralisation
+kluifden	kloven	Overgeneralisation
+kloofde	kloof	Irregular form plus regular suffix
+kloofden	kloven	Irregular form plus regular suffix
+gekluifd	gekloven	Overgeneralisation+
+ekluifd	gekloven	Overgeneralisation+Prefix ge without onset
+kluifd	gekloven	Overgeneralisation+Lacking ge prefix
+gekluifde	geklovene	Overgeneralisation+
+ekluifde	geklovene	Overgeneralisation+Prefix ge without onset
+gekluift	gekloven	Overgeneralisation
+ekluift	gekloven	Overgeneralisation
+kluift	gekloven	Overgeneralisation
+gekluifen	gekloven	Wrong -en suffix
+ekluifen	gekloven	Wrong -en suffix
+kluifen	gekloven	Wrong -en suffix
+geklooft	gekloven	Overgeneralisation
+ekloven	gekloven	Prefix ge without onset
+kloven	gekloven	Lacking ge prefix
+knijpte	kneep	Overgeneralisation
+knijpten	knepen	Overgeneralisation
+kneepte	kneep	Irregular form plus regular suffix
+kneepten	knepen	Irregular form plus regular suffix
+geknijpt	geknepen	Overgeneralisation
+eknijpt	geknepen	Overgeneralisation
+knijpt	geknepen	Overgeneralisation
+geknijpte	geknepene	Overgeneralisation+
+eknijpte	geknepene	Overgeneralisation+Prefix ge without onset
+geknijpen	geknepen	Wrong -en suffix
+eknijpen	geknepen	Wrong -en suffix
+knijpen	geknepen	Wrong -en suffix
+gekneept	geknepen	Overgeneralisation
+eknepen	geknepen	Prefix ge without onset
+knepen	geknepen	Lacking ge prefix
+koopte	kocht	Overgeneralisation
+koopten	kochten	Overgeneralisation
+kochtte	kocht	Irregular form plus regular suffix
+kochtten	kochten	Irregular form plus regular suffix
+gekoopt	gekocht	Overgeneralisation
+ekoopt	gekocht	Overgeneralisation
+koopt	gekocht	Overgeneralisation
+gekoopte	gekochte	Overgeneralisation+
+ekoopte	gekochte	Overgeneralisation+Prefix ge without onset
+gekopen	gekocht	Wrong -en suffix
+ekopen	gekocht	Wrong -en suffix
+kopen	gekocht	Wrong -en suffix
+ekocht	gekocht	Prefix ge without onset
+kocht	gekocht	Lacking ge prefix
+krijgde	kreeg	Overgeneralisation
+krijgden	kregen	Overgeneralisation
+kreegde	kreeg	Irregular form plus regular suffix
+kreegden	kregen	Irregular form plus regular suffix
+gekrijgd	gekregen	Overgeneralisation+
+ekrijgd	gekregen	Overgeneralisation+Prefix ge without onset
+krijgd	gekregen	Overgeneralisation+Lacking ge prefix
+gekrijgde	gekregene	Overgeneralisation+
+ekrijgde	gekregene	Overgeneralisation+Prefix ge without onset
+gekrijgt	gekregen	Overgeneralisation
+ekrijgt	gekregen	Overgeneralisation
+krijgt	gekregen	Overgeneralisation
+gekrijgen	gekregen	Wrong -en suffix
+ekrijgen	gekregen	Wrong -en suffix
+krijgen	gekregen	Wrong -en suffix
+gekreegd	gekregen	Overgeneralisation
+gekreegt	gekregen	Overgeneralisation
+ekregen	gekregen	Prefix ge without onset
+kregen	gekregen	Lacking ge prefix
+krimpte	kromp	Overgeneralisation
+krimpten	krompen	Overgeneralisation
+krompte	kromp	Irregular form plus regular suffix
+krompten	krompen	Irregular form plus regular suffix
+gekrimpt	gekrompen	Overgeneralisation
+ekrimpt	gekrompen	Overgeneralisation
+krimpt	gekrompen	Overgeneralisation
+gekrimpte	gekrompene	Overgeneralisation+
+ekrimpte	gekrompene	Overgeneralisation+Prefix ge without onset
+gekrimpen	gekrompen	Wrong -en suffix
+ekrimpen	gekrompen	Wrong -en suffix
+krimpen	gekrompen	Wrong -en suffix
+gekrompt	gekrompen	Overgeneralisation
+ekrompen	gekrompen	Prefix ge without onset
+krompen	gekrompen	Lacking ge prefix
+kruipte	kroop	Overgeneralisation
+kruipten	kropen	Overgeneralisation
+kroopte	kroop	Irregular form plus regular suffix
+kroopten	kropen	Irregular form plus regular suffix
+gekruipt	gekropen	Overgeneralisation
+ekruipt	gekropen	Overgeneralisation
+kruipt	gekropen	Overgeneralisation
+gekruipte	gekropene	Overgeneralisation+
+ekruipte	gekropene	Overgeneralisation+Prefix ge without onset
+gekruipen	gekropen	Wrong -en suffix
+ekruipen	gekropen	Wrong -en suffix
+kruipen	gekropen	Wrong -en suffix
+gekroopt	gekropen	Overgeneralisation
+ekropen	gekropen	Prefix ge without onset
+kropen	gekropen	Lacking ge prefix
+kwijtte	kweet	Overgeneralisation
+kwijtten	kweten	Overgeneralisation
+kweette	kweet	Irregular form plus regular suffix
+kweetten	kweten	Irregular form plus regular suffix
+gekwijt	gekweten	Overgeneralisation
+ekwijt	gekweten	Overgeneralisation
+kwijt	gekweten	Overgeneralisation
+gekwijte	gekwetene	Overgeneralisation+
+ekwijte	gekwetene	Overgeneralisation+Prefix ge without onset
+gekwijten	gekweten	Wrong -en suffix
+ekwijten	gekweten	Wrong -en suffix
+kwijten	gekweten	Wrong -en suffix
+gekweet	gekweten	Overgeneralisation
+ekweten	gekweten	Prefix ge without onset
+kweten	gekweten	Lacking ge prefix
+lachde	lachte	Overgeneralisation
+lachden	lachten	Overgeneralisation
+gelachd	gelachen	Overgeneralisation
+elachd	gelachen	Overgeneralisation+Prefix ge without onset
+lachd	gelachen	Overgeneralisation+Lacking ge prefix
+gelachde	gelachene	Overgeneralisation+
+elachde	gelachene	Overgeneralisation+Prefix ge without onset
+gelacht	gelachen	Overgeneralisation
+elacht	gelachen	Overgeneralisation
+lacht	gelachen	Overgeneralisation
+elachen	gelachen	Prefix ge without onset
+lachen	gelachen	Lacking ge prefix
+gelaad	geladen	Overgeneralisation
+elaad	geladen	Overgeneralisation
+laad	geladen	Overgeneralisation
+gelade	geladene	Overgeneralisation+
+elade	geladene	Overgeneralisation+Prefix ge without onset
+eladen	geladen	Prefix ge without onset
+laden	geladen	Lacking ge prefix
+laatte	liet	Overgeneralisation
+laatten	lieten	Overgeneralisation
+liette	liet	Irregular form plus regular suffix
+lietten	lieten	Irregular form plus regular suffix
+gelaat	gelaten	Overgeneralisation
+elaat	gelaten	Overgeneralisation
+laat	gelaten	Overgeneralisation
+gelate	gelatene	Overgeneralisation+
+elate	gelatene	Overgeneralisation+Prefix ge without onset
+elaten	gelaten	Prefix ge without onset
+laten	gelaten	Lacking ge prefix
+leesde	las	Overgeneralisation
+leesden	lazen	Overgeneralisation
+lasde	las	Irregular form plus regular suffix
+lasden	lazen	Irregular form plus regular suffix
+geleesd	gelezen	Overgeneralisation
+eleesd	gelezen	Overgeneralisation+Prefix ge without onset
+leesd	gelezen	Overgeneralisation+Lacking ge prefix
+geleesde	gelezene	Overgeneralisation+
+eleesde	gelezene	Overgeneralisation+Prefix ge without onset
+geleest	gelezen	Overgeneralisation
+eleest	gelezen	Overgeneralisation
+leest	gelezen	Overgeneralisation
+gelesen	gelezen	Wrong -en suffix
+elesen	gelezen	Wrong -en suffix
+lesen	gelezen	Wrong -en suffix
+elezen	gelezen	Prefix ge without onset
+lezen	gelezen	Lacking ge prefix
+liegde	loog	Overgeneralisation
+liegden	logen	Overgeneralisation
+loogde	loog	Irregular form plus regular suffix
+loogden	logen	Irregular form plus regular suffix
+geliegd	gelogen	Overgeneralisation+
+eliegd	gelogen	Overgeneralisation+Prefix ge without onset
+liegd	gelogen	Overgeneralisation+Lacking ge prefix
+geliegde	gelogene	Overgeneralisation+
+eliegde	gelogene	Overgeneralisation+Prefix ge without onset
+geliegt	gelogen	Overgeneralisation
+eliegt	gelogen	Overgeneralisation
+liegt	gelogen	Overgeneralisation
+geliegen	gelogen	Wrong -en suffix
+eliegen	gelogen	Wrong -en suffix
+liegen	gelogen	Wrong -en suffix
+geloogt	gelogen	Overgeneralisation
+elogen	gelogen	Prefix ge without onset
+logen	gelogen	Lacking ge prefix
+ligde	lag	Overgeneralisation
+ligden	lagen	Overgeneralisation
+lagde	lag	Irregular form plus regular suffix
+lagden	lagen	Irregular form plus regular suffix
+geligd	gelegen	Overgeneralisation+
+eligd	gelegen	Overgeneralisation+Prefix ge without onset
+ligd	gelegen	Overgeneralisation+Lacking ge prefix
+geligde	gelegene	Overgeneralisation+
+eligde	gelegene	Overgeneralisation+Prefix ge without onset
+geligt	gelegen	Overgeneralisation
+eligt	gelegen	Overgeneralisation
+ligt	gelegen	Overgeneralisation
+geliggen	gelegen	Wrong -en suffix
+eliggen	gelegen	Wrong -en suffix
+liggen	gelegen	Wrong -en suffix
+geleegd	gelegen	Overgeneralisation
+geleegt	gelegen	Overgeneralisation
+elegen	gelegen	Prefix ge without onset
+legen	gelegen	Lacking ge prefix
+lijdde	leed	Overgeneralisation
+lijdden	leden	Overgeneralisation
+leedde	leed	Irregular form plus regular suffix
+leedden	leden	Irregular form plus regular suffix
+gelijd	geleden	Overgeneralisation
+elijd	geleden	Overgeneralisation
+lijd	geleden	Overgeneralisation
+gelijde	geledene	Overgeneralisation+
+elijde	geledene	Overgeneralisation+Prefix ge without onset
+gelijden	geleden	Wrong -en suffix
+elijden	geleden	Wrong -en suffix
+lijden	geleden	Wrong -en suffix
+geleed	geleden	Overgeneralisation
+eleden	geleden	Prefix ge without onset
+leden	geleden	Lacking ge prefix
+lijkte	leek	Overgeneralisation
+lijkten	leken	Overgeneralisation
+leekte	leek	Irregular form plus regular suffix
+leekten	leken	Irregular form plus regular suffix
+gelijkt	geleken	Overgeneralisation
+elijkt	geleken	Overgeneralisation
+lijkt	geleken	Overgeneralisation
+gelijkte	gelekene	Overgeneralisation+
+elijkte	gelekene	Overgeneralisation+Prefix ge without onset
+gelijken	geleken	Wrong -en suffix
+elijken	geleken	Wrong -en suffix
+lijken	geleken	Wrong -en suffix
+geleekt	geleken	Overgeneralisation
+eleken	geleken	Prefix ge without onset
+leken	geleken	Lacking ge prefix
+loopte	liep	Overgeneralisation
+loopten	liepen	Overgeneralisation
+liepte	liep	Irregular form plus regular suffix
+liepten	liepen	Irregular form plus regular suffix
+geloopt	gelopen	Overgeneralisation
+eloopt	gelopen	Overgeneralisation
+loopt	gelopen	Overgeneralisation
+geloopte	gelopene	Overgeneralisation+
+eloopte	gelopene	Overgeneralisation+Prefix ge without onset
+elopen	gelopen	Prefix ge without onset
+lopen	gelopen	Lacking ge prefix
+gemaald	gemalen	Overgeneralisation
+emaald	gemalen	Overgeneralisation+Prefix ge without onset
+maald	gemalen	Overgeneralisation+Lacking ge prefix
+gemaalde	gemalene	Overgeneralisation+
+emaalde	gemalene	Overgeneralisation+Prefix ge without onset
+gemaalt	gemalen	Overgeneralisation
+emaalt	gemalen	Overgeneralisation
+maalt	gemalen	Overgeneralisation
+emalen	gemalen	Prefix ge without onset
+malen	gemalen	Lacking ge prefix
+emelkt	gemelkt	Prefix ge without onset
+melkt	gemelkt	Lacking ge prefix
+emelkte	gemelkte	Overgeneralisation+Prefix ge without onset
+gemelken	gemelkt	Wrong -en suffix
+emelken	gemelkt	Wrong -en suffix
+melken	gemelkt	Wrong -en suffix
+meette	mat	Overgeneralisation
+meetten	maten	Overgeneralisation
+matte	mat	Irregular form plus regular suffix
+matten	maten	Irregular form plus regular suffix
+gemeet	gemeten	Overgeneralisation
+emeet	gemeten	Overgeneralisation
+meet	gemeten	Overgeneralisation
+gemete	gemetene	Overgeneralisation+
+emete	gemetene	Overgeneralisation+Prefix ge without onset
+emeten	gemeten	Prefix ge without onset
+meten	gemeten	Lacking ge prefix
+mijdde	meed	Overgeneralisation
+mijdden	meden	Overgeneralisation
+meedde	meed	Irregular form plus regular suffix
+meedden	meden	Irregular form plus regular suffix
+gemijd	gemeden	Overgeneralisation
+emijd	gemeden	Overgeneralisation
+mijd	gemeden	Overgeneralisation
+gemijde	gemedene	Overgeneralisation+
+emijde	gemedene	Overgeneralisation+Prefix ge without onset
+gemijden	gemeden	Wrong -en suffix
+emijden	gemeden	Wrong -en suffix
+mijden	gemeden	Wrong -en suffix
+gemeed	gemeden	Overgeneralisation
+emeden	gemeden	Prefix ge without onset
+meden	gemeden	Lacking ge prefix
+moette	moest	Overgeneralisation
+moetten	moesten	Overgeneralisation
+moestte	moest	Irregular form plus regular suffix
+moestten	moesten	Irregular form plus regular suffix
+gemoet	gemoeten	Overgeneralisation
+emoet	gemoeten	Overgeneralisation
+moet	gemoeten	Overgeneralisation
+gemoete	gemoetene	Overgeneralisation+
+emoete	gemoetene	Overgeneralisation+Prefix ge without onset
+emoeten	gemoeten	Prefix ge without onset
+moeten	gemoeten	Lacking ge prefix
+neemde	nam	Overgeneralisation
+neemden	namen	Overgeneralisation
+namde	nam	Irregular form plus regular suffix
+namden	namen	Irregular form plus regular suffix
+geneemd	genomen	Overgeneralisation+
+eneemd	genomen	Overgeneralisation+Prefix ge without onset
+neemd	genomen	Overgeneralisation+Lacking ge prefix
+geneemde	genomene	Overgeneralisation+
+eneemde	genomene	Overgeneralisation+Prefix ge without onset
+geneemt	genomen	Overgeneralisation
+eneemt	genomen	Overgeneralisation
+neemt	genomen	Overgeneralisation
+genemen	genomen	Wrong -en suffix
+enemen	genomen	Wrong -en suffix
+nemen	genomen	Wrong -en suffix
+genoomt	genomen	Overgeneralisation
+enomen	genomen	Prefix ge without onset
+nomen	genomen	Lacking ge prefix
+nijgde	neeg	Overgeneralisation
+nijgden	negen	Overgeneralisation
+neegde	neeg	Irregular form plus regular suffix
+neegden	negen	Irregular form plus regular suffix
+genijgd	genegen	Overgeneralisation+
+enijgd	genegen	Overgeneralisation+Prefix ge without onset
+nijgd	genegen	Overgeneralisation+Lacking ge prefix
+genijgde	genegene	Overgeneralisation+
+enijgde	genegene	Overgeneralisation+Prefix ge without onset
+genijgt	genegen	Overgeneralisation
+enijgt	genegen	Overgeneralisation
+nijgt	genegen	Overgeneralisation
+genijgen	genegen	Wrong -en suffix
+enijgen	genegen	Wrong -en suffix
+nijgen	genegen	Wrong -en suffix
+geneegd	genegen	Overgeneralisation
+geneegt	genegen	Overgeneralisation
+enegen	genegen	Prefix ge without onset
+negen	genegen	Lacking ge prefix
+ontginde	ontgonnene	Overgeneralisation
+ontginden	ontgonnen	Overgeneralisation
+ontgonde	ontgon	Irregular form plus regular suffix
+ontgonden	ontgonnen	Irregular form plus regular suffix
+ontgind	ontgonnen	Overgeneralisation
+ontgint	ontgonnen	Overgeneralisation
+ontginnen	ontgonnen	Wrong -en suffix
+ontgont	ontgonnen	Overgeneralisation
+ontluikte	ontlokene	Overgeneralisation
+ontluikten	ontloken	Overgeneralisation
+ontlookte	ontlook	Irregular form plus regular suffix
+ontlookten	ontloken	Irregular form plus regular suffix
+ontluikt	ontloken	Overgeneralisation
+ontluiken	ontloken	Wrong -en suffix
+ontlookt	ontloken	Overgeneralisation
+pluisde	ploos	Overgeneralisation
+pluisden	plozen	Overgeneralisation
+ploosde	ploos	Irregular form plus regular suffix
+ploosden	plozen	Irregular form plus regular suffix
+gepluisd	geplozen	Overgeneralisation+
+epluisd	geplozen	Overgeneralisation+Prefix ge without onset
+pluisd	geplozen	Overgeneralisation+Lacking ge prefix
+gepluisde	geplozene	Overgeneralisation+
+epluisde	geplozene	Overgeneralisation+Prefix ge without onset
+gepluist	geplozen	Overgeneralisation
+epluist	geplozen	Overgeneralisation
+pluist	geplozen	Overgeneralisation
+gepluisen	geplozen	Wrong -en suffix
+epluisen	geplozen	Wrong -en suffix
+pluisen	geplozen	Wrong -en suffix
+geploost	geplozen	Overgeneralisation
+eplozen	geplozen	Prefix ge without onset
+plozen	geplozen	Lacking ge prefix
+prijsde	prees	Overgeneralisation
+prijsden	prezen	Overgeneralisation
+preesde	prees	Irregular form plus regular suffix
+preesden	prezen	Irregular form plus regular suffix
+geprijsd	geprezen	Overgeneralisation+
+eprijsd	geprezen	Overgeneralisation+Prefix ge without onset
+prijsd	geprezen	Overgeneralisation+Lacking ge prefix
+geprijsde	geprezene	Overgeneralisation+
+eprijsde	geprezene	Overgeneralisation+Prefix ge without onset
+geprijst	geprezen	Overgeneralisation
+eprijst	geprezen	Overgeneralisation
+prijst	geprezen	Overgeneralisation
+geprijsen	geprezen	Wrong -en suffix
+eprijsen	geprezen	Wrong -en suffix
+prijsen	geprezen	Wrong -en suffix
+gepreesd	geprezen	Overgeneralisation
+gepreest	geprezen	Overgeneralisation
+eprezen	geprezen	Prefix ge without onset
+prezen	geprezen	Lacking ge prefix
+geraad	geraden	Overgeneralisation
+eraad	geraden	Overgeneralisation
+raad	geraden	Overgeneralisation
+gerade	geradene	Overgeneralisation+
+erade	geradene	Overgeneralisation+Prefix ge without onset
+eraden	geraden	Prefix ge without onset
+raden	geraden	Lacking ge prefix
+verraad	verraden	Overgeneralisation
+verrade	verradene	Overgeneralisation
+rijdde	reed	Overgeneralisation
+rijdden	reden	Overgeneralisation
+reedde	reed	Irregular form plus regular suffix
+reedden	reden	Irregular form plus regular suffix
+gerijd	gereden	Overgeneralisation
+erijd	gereden	Overgeneralisation
+rijd	gereden	Overgeneralisation
+gerijde	geredene	Overgeneralisation+
+erijde	geredene	Overgeneralisation+Prefix ge without onset
+gerijden	gereden	Wrong -en suffix
+erijden	gereden	Wrong -en suffix
+rijden	gereden	Wrong -en suffix
+gereed	gereden	Overgeneralisation
+ereden	gereden	Prefix ge without onset
+reden	gereden	Lacking ge prefix
+rijgde	reeg	Overgeneralisation
+rijgden	regen	Overgeneralisation
+reegde	reeg	Irregular form plus regular suffix
+reegden	regen	Irregular form plus regular suffix
+gerijgd	geregen	Overgeneralisation+
+erijgd	geregen	Overgeneralisation+Prefix ge without onset
+rijgd	geregen	Overgeneralisation+Lacking ge prefix
+gerijgde	geregene	Overgeneralisation+
+erijgde	geregene	Overgeneralisation+Prefix ge without onset
+gerijgt	geregen	Overgeneralisation
+erijgt	geregen	Overgeneralisation
+rijgt	geregen	Overgeneralisation
+gerijgen	geregen	Wrong -en suffix
+erijgen	geregen	Wrong -en suffix
+rijgen	geregen	Wrong -en suffix
+gereegd	geregen	Overgeneralisation
+gereegt	geregen	Overgeneralisation
+eregen	geregen	Prefix ge without onset
+regen	geregen	Lacking ge prefix
+rijtte	reet	Overgeneralisation
+rijtten	reten	Overgeneralisation
+reette	reet	Irregular form plus regular suffix
+reetten	reten	Irregular form plus regular suffix
+gerijt	gereten	Overgeneralisation
+erijt	gereten	Overgeneralisation
+rijt	gereten	Overgeneralisation
+gerijte	geretene	Overgeneralisation+
+erijte	geretene	Overgeneralisation+Prefix ge without onset
+gerijten	gereten	Wrong -en suffix
+erijten	gereten	Wrong -en suffix
+rijten	gereten	Wrong -en suffix
+gereet	gereten	Overgeneralisation
+ereten	gereten	Prefix ge without onset
+reten	gereten	Lacking ge prefix
+rijsde	rees	Overgeneralisation
+rijsden	rezen	Overgeneralisation
+reesde	rees	Irregular form plus regular suffix
+reesden	rezen	Irregular form plus regular suffix
+gerijsd	Gerezen	Overgeneralisation+
+erijsd	Gerezen	Overgeneralisation+Prefix ge without onset
+rijsd	Gerezen	Overgeneralisation+Lacking ge prefix
+gerijsde	Gerezene	Overgeneralisation+
+erijsde	Gerezene	Overgeneralisation+Prefix ge without onset
+gerijst	Gerezen	Overgeneralisation
+erijst	Gerezen	Overgeneralisation
+rijst	Gerezen	Overgeneralisation
+gerijsen	Gerezen	Wrong -en suffix
+erijsen	Gerezen	Wrong -en suffix
+rijsen	Gerezen	Wrong -en suffix
+geGereesd	Gerezen	Overgeneralisation
+geGereest	Gerezen	Overgeneralisation
+roepte	riep	Overgeneralisation
+roepten	riepen	Overgeneralisation
+riepte	riep	Irregular form plus regular suffix
+riepten	riepen	Irregular form plus regular suffix
+geroept	geroepen	Overgeneralisation
+eroept	geroepen	Overgeneralisation
+roept	geroepen	Overgeneralisation
+geroepte	geroepene	Overgeneralisation+
+eroepte	geroepene	Overgeneralisation+Prefix ge without onset
+eroepen	geroepen	Prefix ge without onset
+roepen	geroepen	Lacking ge prefix
+ruikte	rook	Overgeneralisation
+ruikten	roken	Overgeneralisation
+rookte	rook	Irregular form plus regular suffix
+rookten	roken	Irregular form plus regular suffix
+geruikt	geroken	Overgeneralisation
+eruikt	geroken	Overgeneralisation
+ruikt	geroken	Overgeneralisation
+geruikte	gerokene	Overgeneralisation+
+eruikte	gerokene	Overgeneralisation+Prefix ge without onset
+geruiken	geroken	Wrong -en suffix
+eruiken	geroken	Wrong -en suffix
+ruiken	geroken	Wrong -en suffix
+gerookt	geroken	Overgeneralisation
+eroken	geroken	Prefix ge without onset
+roken	geroken	Lacking ge prefix
+gescheid	gescheiden	Overgeneralisation
+escheid	gescheiden	Overgeneralisation
+scheid	gescheiden	Overgeneralisation
+gescheide	gescheidene	Overgeneralisation+
+escheide	gescheidene	Overgeneralisation+Prefix ge without onset
+escheiden	gescheiden	Prefix ge without onset
+scheiden	gescheiden	Lacking ge prefix
+scheldde	schold	Overgeneralisation
+scheldden	scholden	Overgeneralisation
+scholdde	schold	Irregular form plus regular suffix
+scholdden	scholden	Irregular form plus regular suffix
+gescheld	gescholden	Overgeneralisation
+escheld	gescholden	Overgeneralisation
+scheld	gescholden	Overgeneralisation
+geschelde	gescholdene	Overgeneralisation+
+eschelde	gescholdene	Overgeneralisation+Prefix ge without onset
+geschelden	gescholden	Wrong -en suffix
+eschelden	gescholden	Wrong -en suffix
+schelden	gescholden	Wrong -en suffix
+geschold	gescholden	Overgeneralisation
+escholden	gescholden	Prefix ge without onset
+scholden	gescholden	Lacking ge prefix
+schendde	schond	Overgeneralisation
+schendden	schonden	Overgeneralisation
+schondde	schond	Irregular form plus regular suffix
+schondden	schonden	Irregular form plus regular suffix
+geschend	geschonden	Overgeneralisation
+eschend	geschonden	Overgeneralisation
+schend	geschonden	Overgeneralisation
+geschende	geschondene	Overgeneralisation+
+eschende	geschondene	Overgeneralisation+Prefix ge without onset
+geschenden	geschonden	Wrong -en suffix
+eschenden	geschonden	Wrong -en suffix
+schenden	geschonden	Wrong -en suffix
+geschond	geschonden	Overgeneralisation
+eschonden	geschonden	Prefix ge without onset
+schonden	geschonden	Lacking ge prefix
+schenkte	schonk	Overgeneralisation
+schenkten	schonken	Overgeneralisation
+schonkte	schonk	Irregular form plus regular suffix
+schonkten	schonken	Irregular form plus regular suffix
+geschenkt	geschonken	Overgeneralisation
+eschenkt	geschonken	Overgeneralisation
+schenkt	geschonken	Overgeneralisation
+geschenkte	geschonkene	Overgeneralisation+
+eschenkte	geschonkene	Overgeneralisation+Prefix ge without onset
+geschenken	geschonken	Wrong -en suffix
+eschenken	geschonken	Wrong -en suffix
+schenken	geschonken	Wrong -en suffix
+geschonkt	geschonken	Overgeneralisation
+eschonken	geschonken	Prefix ge without onset
+schonken	geschonken	Lacking ge prefix
+schepte	shiep	Overgeneralisation
+schepten	schiepen	Overgeneralisation
+shiepte	shiep	Irregular form plus regular suffix
+shiepten	schiepen	Irregular form plus regular suffix
+geschept	geschapen	Overgeneralisation
+eschept	geschapen	Overgeneralisation
+schept	geschapen	Overgeneralisation
+geschepte	geschapene	Overgeneralisation+
+eschepte	geschapene	Overgeneralisation+Prefix ge without onset
+gescheppen	geschapen	Wrong -en suffix
+escheppen	geschapen	Wrong -en suffix
+scheppen	geschapen	Wrong -en suffix
+geschaapt	geschapen	Overgeneralisation
+eschapen	geschapen	Prefix ge without onset
+schapen	geschapen	Lacking ge prefix
+gescheerd	geschoren	Overgeneralisation+
+escheerd	geschoren	Overgeneralisation+Prefix ge without onset
+scheerd	geschoren	Overgeneralisation+Lacking ge prefix
+gescheerde	geschorene	Overgeneralisation+
+escheerde	geschorene	Overgeneralisation+Prefix ge without onset
+gescheert	geschoren	Overgeneralisation
+escheert	geschoren	Overgeneralisation
+scheert	geschoren	Overgeneralisation
+gescheren	geschoren	Wrong -en suffix
+escheren	geschoren	Wrong -en suffix
+scheren	geschoren	Wrong -en suffix
+geschoort	geschoren	Overgeneralisation
+eschoren	geschoren	Prefix ge without onset
+schoren	geschoren	Lacking ge prefix
+schiette	schoot	Overgeneralisation
+schietten	schoten	Overgeneralisation
+schootte	schoot	Irregular form plus regular suffix
+schootten	schoten	Irregular form plus regular suffix
+geschiet	geschoten	Overgeneralisation
+eschiet	geschoten	Overgeneralisation
+schiet	geschoten	Overgeneralisation
+geschiete	geschotene	Overgeneralisation+
+eschiete	geschotene	Overgeneralisation+Prefix ge without onset
+geschieten	geschoten	Wrong -en suffix
+eschieten	geschoten	Wrong -en suffix
+schieten	geschoten	Wrong -en suffix
+geschoot	geschoten	Overgeneralisation
+eschoten	geschoten	Prefix ge without onset
+schoten	geschoten	Lacking ge prefix
+schijnde	scheen	Overgeneralisation
+schijnden	schenen	Overgeneralisation
+scheende	scheen	Irregular form plus regular suffix
+scheenden	schenen	Irregular form plus regular suffix
+geschijnd	geschenen	Overgeneralisation+
+eschijnd	geschenen	Overgeneralisation+Prefix ge without onset
+schijnd	geschenen	Overgeneralisation+Lacking ge prefix
+geschijnde	geschenene	Overgeneralisation+
+eschijnde	geschenene	Overgeneralisation+Prefix ge without onset
+geschijnt	geschenen	Overgeneralisation
+eschijnt	geschenen	Overgeneralisation
+schijnt	geschenen	Overgeneralisation
+geschijnen	geschenen	Wrong -en suffix
+eschijnen	geschenen	Wrong -en suffix
+schijnen	geschenen	Wrong -en suffix
+gescheend	geschenen	Overgeneralisation
+gescheent	geschenen	Overgeneralisation
+eschenen	geschenen	Prefix ge without onset
+schenen	geschenen	Lacking ge prefix
+schijtte	scheet	Overgeneralisation
+schijtten	scheten	Overgeneralisation
+scheette	scheet	Irregular form plus regular suffix
+scheetten	scheten	Irregular form plus regular suffix
+geschijt	gescheten	Overgeneralisation
+eschijt	gescheten	Overgeneralisation
+schijt	gescheten	Overgeneralisation
+geschijte	geschetene	Overgeneralisation+
+eschijte	geschetene	Overgeneralisation+Prefix ge without onset
+geschijten	gescheten	Wrong -en suffix
+eschijten	gescheten	Wrong -en suffix
+schijten	gescheten	Wrong -en suffix
+gescheet	gescheten	Overgeneralisation
+escheten	gescheten	Prefix ge without onset
+scheten	gescheten	Lacking ge prefix
+schrijfde	schreef	Overgeneralisation
+schrijfden	schreven	Overgeneralisation
+schreefde	schreef	Irregular form plus regular suffix
+schreefden	schreven	Irregular form plus regular suffix
+geschrijfd	geschreven	Overgeneralisation+
+eschrijfd	geschreven	Overgeneralisation+Prefix ge without onset
+schrijfd	geschreven	Overgeneralisation+Lacking ge prefix
+geschrijfde	geschrevene	Overgeneralisation+
+eschrijfde	geschrevene	Overgeneralisation+Prefix ge without onset
+geschrijft	geschreven	Overgeneralisation
+eschrijft	geschreven	Overgeneralisation
+schrijft	geschreven	Overgeneralisation
+geschrijfen	geschreven	Wrong -en suffix
+eschrijfen	geschreven	Wrong -en suffix
+schrijfen	geschreven	Wrong -en suffix
+geschreefd	geschreven	Overgeneralisation
+geschreeft	geschreven	Overgeneralisation
+eschreven	geschreven	Prefix ge without onset
+schreven	geschreven	Lacking ge prefix
+schrikte	schrok	Overgeneralisation
+schrikten	schrokken	Overgeneralisation
+schrokte	schrok	Irregular form plus regular suffix
+schrokten	schrokken	Irregular form plus regular suffix
+geschrikt	geschrokken	Overgeneralisation
+eschrikt	geschrokken	Overgeneralisation
+schrikt	geschrokken	Overgeneralisation
+geschrikte	geschrokkene	Overgeneralisation+
+eschrikte	geschrokkene	Overgeneralisation+Prefix ge without onset
+geschrikken	geschrokken	Wrong -en suffix
+eschrikken	geschrokken	Wrong -en suffix
+schrikken	geschrokken	Wrong -en suffix
+geschrokt	geschrokken	Overgeneralisation
+eschrokken	geschrokken	Prefix ge without onset
+schrokken	geschrokken	Lacking ge prefix
+eschuild	geschuild	Prefix ge without onset
+schuild	geschuild	Lacking ge prefix
+eschuilde	geschuilde	Overgeneralisation+Prefix ge without onset
+geschuilt	geschuild	Overgeneralisation
+eschuilt	geschuild	Overgeneralisation
+schuilt	geschuild	Overgeneralisation
+geschuilen	geschuild	Wrong -en suffix
+eschuilen	geschuild	Wrong -en suffix
+schuilen	geschuild	Wrong -en suffix
+schuifde	schoof	Overgeneralisation
+schuifden	schoven	Overgeneralisation
+schoofde	schoof	Irregular form plus regular suffix
+schoofden	schoven	Irregular form plus regular suffix
+geschuifd	geschoven	Overgeneralisation+
+eschuifd	geschoven	Overgeneralisation+Prefix ge without onset
+schuifd	geschoven	Overgeneralisation+Lacking ge prefix
+geschuifde	geschovene	Overgeneralisation+
+eschuifde	geschovene	Overgeneralisation+Prefix ge without onset
+geschuift	geschoven	Overgeneralisation
+eschuift	geschoven	Overgeneralisation
+schuift	geschoven	Overgeneralisation
+geschuifen	geschoven	Wrong -en suffix
+eschuifen	geschoven	Wrong -en suffix
+schuifen	geschoven	Wrong -en suffix
+geschooft	geschoven	Overgeneralisation
+eschoven	geschoven	Prefix ge without onset
+schoven	geschoven	Lacking ge prefix
+slade	sloeg	Overgeneralisation
+sladen	sloegen	Overgeneralisation
+sloegde	sloeg	Irregular form plus regular suffix
+sloegden	sloegen	Irregular form plus regular suffix
+geslaad	geslagen	Overgeneralisation+
+eslaad	geslagen	Overgeneralisation+Prefix ge without onset
+slaad	geslagen	Overgeneralisation+Lacking ge prefix
+geslade	geslagene	Overgeneralisation+
+eslade	geslagene	Overgeneralisation+Prefix ge without onset
+geslaat	geslagen	Overgeneralisation
+eslaat	geslagen	Overgeneralisation
+slaat	geslagen	Overgeneralisation
+geslaan	geslagen	Wrong -en suffix
+eslaan	geslagen	Wrong -en suffix
+slaan	geslagen	Wrong -en suffix
+geslaagd	geslagen	Overgeneralisation
+geslaagt	geslagen	Overgeneralisation
+eslagen	geslagen	Prefix ge without onset
+slagen	geslagen	Lacking ge prefix
+slaapte	sliep	Overgeneralisation
+slaapten	sliepen	Overgeneralisation
+sliepte	sliep	Irregular form plus regular suffix
+sliepten	sliepen	Irregular form plus regular suffix
+geslaapt	geslapen	Overgeneralisation
+eslaapt	geslapen	Overgeneralisation
+slaapt	geslapen	Overgeneralisation
+geslaapte	geslapene	Overgeneralisation+
+eslaapte	geslapene	Overgeneralisation+Prefix ge without onset
+eslapen	geslapen	Prefix ge without onset
+slapen	geslapen	Lacking ge prefix
+slijpte	sleep	Overgeneralisation
+slijpten	slepen	Overgeneralisation
+sleepte	sleep	Irregular form plus regular suffix
+sleepten	slepen	Irregular form plus regular suffix
+geslijpt	geslepen	Overgeneralisation
+eslijpt	geslepen	Overgeneralisation
+slijpt	geslepen	Overgeneralisation
+geslijpte	geslepene	Overgeneralisation+
+eslijpte	geslepene	Overgeneralisation+Prefix ge without onset
+geslijpen	geslepen	Wrong -en suffix
+eslijpen	geslepen	Wrong -en suffix
+slijpen	geslepen	Wrong -en suffix
+gesleept	geslepen	Overgeneralisation
+eslepen	geslepen	Prefix ge without onset
+slepen	geslepen	Lacking ge prefix
+slijtte	sleet	Overgeneralisation
+slijtten	sleten	Overgeneralisation
+sleette	sleet	Irregular form plus regular suffix
+sleetten	sleten	Irregular form plus regular suffix
+geslijt	gesleten	Overgeneralisation
+eslijt	gesleten	Overgeneralisation
+slijt	gesleten	Overgeneralisation
+geslijte	gesletene	Overgeneralisation+
+eslijte	gesletene	Overgeneralisation+Prefix ge without onset
+geslijten	gesleten	Wrong -en suffix
+eslijten	gesleten	Wrong -en suffix
+slijten	gesleten	Wrong -en suffix
+gesleet	gesleten	Overgeneralisation
+esleten	gesleten	Prefix ge without onset
+sleten	gesleten	Lacking ge prefix
+slinkte	slonk	Overgeneralisation
+slinkten	slonken	Overgeneralisation
+slonkte	slonk	Irregular form plus regular suffix
+slonkten	slonken	Irregular form plus regular suffix
+geslinkt	Geslonken	Overgeneralisation
+eslinkt	Geslonken	Overgeneralisation
+slinkt	Geslonken	Overgeneralisation
+geslinkte	Geslonkene	Overgeneralisation+
+eslinkte	Geslonkene	Overgeneralisation+Prefix ge without onset
+geslinken	Geslonken	Wrong -en suffix
+eslinken	Geslonken	Wrong -en suffix
+slinken	Geslonken	Wrong -en suffix
+geGeslonkt	Geslonken	Overgeneralisation
+sluipte	sloop	Overgeneralisation
+sluipten	slopen	Overgeneralisation
+sloopte	sloop	Irregular form plus regular suffix
+sloopten	slopen	Irregular form plus regular suffix
+gesluipt	geslopen	Overgeneralisation
+esluipt	geslopen	Overgeneralisation
+sluipt	geslopen	Overgeneralisation
+gesluipte	geslopene	Overgeneralisation+
+esluipte	geslopene	Overgeneralisation+Prefix ge without onset
+gesluipen	geslopen	Wrong -en suffix
+esluipen	geslopen	Wrong -en suffix
+sluipen	geslopen	Wrong -en suffix
+gesloopt	geslopen	Overgeneralisation
+eslopen	geslopen	Prefix ge without onset
+slopen	geslopen	Lacking ge prefix
+sluitte	sloot	Overgeneralisation
+sluitten	sloten	Overgeneralisation
+slootte	sloot	Irregular form plus regular suffix
+slootten	sloten	Irregular form plus regular suffix
+gesluit	gesloten	Overgeneralisation
+esluit	gesloten	Overgeneralisation
+sluit	gesloten	Overgeneralisation
+gesluite	geslotene	Overgeneralisation+
+esluite	geslotene	Overgeneralisation+Prefix ge without onset
+gesluiten	gesloten	Wrong -en suffix
+esluiten	gesloten	Wrong -en suffix
+sluiten	gesloten	Wrong -en suffix
+gesloot	gesloten	Overgeneralisation
+esloten	gesloten	Prefix ge without onset
+sloten	gesloten	Lacking ge prefix
+smeltte	smolt	Overgeneralisation
+smeltten	smolten	Overgeneralisation
+smoltte	smolt	Irregular form plus regular suffix
+smoltten	smolten	Irregular form plus regular suffix
+gesmelt	gesmolten	Overgeneralisation
+esmelt	gesmolten	Overgeneralisation
+smelt	gesmolten	Overgeneralisation
+gesmelte	gesmoltene	Overgeneralisation+
+esmelte	gesmoltene	Overgeneralisation+Prefix ge without onset
+gesmelten	gesmolten	Wrong -en suffix
+esmelten	gesmolten	Wrong -en suffix
+smelten	gesmolten	Wrong -en suffix
+gesmolt	gesmolten	Overgeneralisation
+esmolten	gesmolten	Prefix ge without onset
+smolten	gesmolten	Lacking ge prefix
+smijtte	smeet	Overgeneralisation
+smijtten	smeten	Overgeneralisation
+smeette	smeet	Irregular form plus regular suffix
+smeetten	smeten	Irregular form plus regular suffix
+gesmijt	gesmeten	Overgeneralisation
+esmijt	gesmeten	Overgeneralisation
+smijt	gesmeten	Overgeneralisation
+gesmijte	gesmetene	Overgeneralisation+
+esmijte	gesmetene	Overgeneralisation+Prefix ge without onset
+gesmijten	gesmeten	Wrong -en suffix
+esmijten	gesmeten	Wrong -en suffix
+smijten	gesmeten	Wrong -en suffix
+gesmeet	gesmeten	Overgeneralisation
+esmeten	gesmeten	Prefix ge without onset
+smeten	gesmeten	Lacking ge prefix
+snijdde	sneed	Overgeneralisation
+snijdden	sneden	Overgeneralisation
+sneedde	sneed	Irregular form plus regular suffix
+sneedden	sneden	Irregular form plus regular suffix
+gesnijd	gesneden	Overgeneralisation
+esnijd	gesneden	Overgeneralisation
+snijd	gesneden	Overgeneralisation
+gesnijde	gesnedene	Overgeneralisation+
+esnijde	gesnedene	Overgeneralisation+Prefix ge without onset
+gesnijden	gesneden	Wrong -en suffix
+esnijden	gesneden	Wrong -en suffix
+snijden	gesneden	Wrong -en suffix
+gesneed	gesneden	Overgeneralisation
+esneden	gesneden	Prefix ge without onset
+sneden	gesneden	Lacking ge prefix
+snuitte	snoot	Overgeneralisation
+snuitten	snoten	Overgeneralisation
+snootte	snoot	Irregular form plus regular suffix
+snootten	snoten	Irregular form plus regular suffix
+gesnuit	gesnoten	Overgeneralisation
+esnuit	gesnoten	Overgeneralisation
+snuit	gesnoten	Overgeneralisation
+gesnuite	gesnotene	Overgeneralisation+
+esnuite	gesnotene	Overgeneralisation+Prefix ge without onset
+gesnuiten	gesnoten	Wrong -en suffix
+esnuiten	gesnoten	Wrong -en suffix
+snuiten	gesnoten	Wrong -en suffix
+gesnoot	gesnoten	Overgeneralisation
+esnoten	gesnoten	Prefix ge without onset
+snoten	gesnoten	Lacking ge prefix
+snuifde	snoof	Overgeneralisation
+snuifden	snoven	Overgeneralisation
+snoofde	snoof	Irregular form plus regular suffix
+snoofden	snoven	Irregular form plus regular suffix
+gesnuifd	gesnoven	Overgeneralisation+
+esnuifd	gesnoven	Overgeneralisation+Prefix ge without onset
+snuifd	gesnoven	Overgeneralisation+Lacking ge prefix
+gesnuifde	gesnovene	Overgeneralisation+
+esnuifde	gesnovene	Overgeneralisation+Prefix ge without onset
+gesnuift	gesnoven	Overgeneralisation
+esnuift	gesnoven	Overgeneralisation
+snuift	gesnoven	Overgeneralisation
+gesnuifen	gesnoven	Wrong -en suffix
+esnuifen	gesnoven	Wrong -en suffix
+snuifen	gesnoven	Wrong -en suffix
+gesnooft	gesnoven	Overgeneralisation
+esnoven	gesnoven	Prefix ge without onset
+snoven	gesnoven	Lacking ge prefix
+gespand	gespannen	Overgeneralisation
+espand	gespannen	Overgeneralisation+Prefix ge without onset
+spand	gespannen	Overgeneralisation+Lacking ge prefix
+gespande	gespannene	Overgeneralisation+
+espande	gespannene	Overgeneralisation+Prefix ge without onset
+gespant	gespannen	Overgeneralisation
+espant	gespannen	Overgeneralisation
+spant	gespannen	Overgeneralisation
+espannen	gespannen	Prefix ge without onset
+spannen	gespannen	Lacking ge prefix
+spijtte	speet	Overgeneralisation
+spijtten	speten	Overgeneralisation
+speette	speet	Irregular form plus regular suffix
+speetten	speten	Irregular form plus regular suffix
+gespijt	gespeten	Overgeneralisation
+espijt	gespeten	Overgeneralisation
+spijt	gespeten	Overgeneralisation
+gespijte	gespetene	Overgeneralisation+
+espijte	gespetene	Overgeneralisation+Prefix ge without onset
+gespijten	gespeten	Wrong -en suffix
+espijten	gespeten	Wrong -en suffix
+spijten	gespeten	Wrong -en suffix
+gespeet	gespeten	Overgeneralisation
+espeten	gespeten	Prefix ge without onset
+speten	gespeten	Lacking ge prefix
+spinde	spon	Overgeneralisation
+spinden	sponnen	Overgeneralisation
+sponde	spon	Irregular form plus regular suffix
+sponden	sponnen	Irregular form plus regular suffix
+gespind	gesponnen	Overgeneralisation+
+espind	gesponnen	Overgeneralisation+Prefix ge without onset
+spind	gesponnen	Overgeneralisation+Lacking ge prefix
+gespinde	gesponnene	Overgeneralisation+
+espinde	gesponnene	Overgeneralisation+Prefix ge without onset
+gespint	gesponnen	Overgeneralisation
+espint	gesponnen	Overgeneralisation
+spint	gesponnen	Overgeneralisation
+gespinnen	gesponnen	Wrong -en suffix
+espinnen	gesponnen	Wrong -en suffix
+spinnen	gesponnen	Wrong -en suffix
+gespont	gesponnen	Overgeneralisation
+esponnen	gesponnen	Prefix ge without onset
+sponnen	gesponnen	Lacking ge prefix
+splijtte	spleet	Overgeneralisation
+splijtten	spleten	Overgeneralisation
+spleette	spleet	Irregular form plus regular suffix
+spleetten	spleten	Irregular form plus regular suffix
+gesplijt	gespleten	Overgeneralisation
+esplijt	gespleten	Overgeneralisation
+splijt	gespleten	Overgeneralisation
+gesplijte	gespletene	Overgeneralisation+
+esplijte	gespletene	Overgeneralisation+Prefix ge without onset
+gesplijten	gespleten	Wrong -en suffix
+esplijten	gespleten	Wrong -en suffix
+splijten	gespleten	Wrong -en suffix
+gespleet	gespleten	Overgeneralisation
+espleten	gespleten	Prefix ge without onset
+spleten	gespleten	Lacking ge prefix
+spreekte	sprak	Overgeneralisation
+spreekten	spraken	Overgeneralisation
+sprakte	sprak	Irregular form plus regular suffix
+sprakten	spraken	Irregular form plus regular suffix
+gespreekt	gesproken	Overgeneralisation
+espreekt	gesproken	Overgeneralisation
+spreekt	gesproken	Overgeneralisation
+gespreekte	gesprokene	Overgeneralisation+
+espreekte	gesprokene	Overgeneralisation+Prefix ge without onset
+gespreken	gesproken	Wrong -en suffix
+espreken	gesproken	Wrong -en suffix
+spreken	gesproken	Wrong -en suffix
+gesprookt	gesproken	Overgeneralisation
+esproken	gesproken	Prefix ge without onset
+sproken	gesproken	Lacking ge prefix
+springde	sprong	Overgeneralisation
+springden	sprongen	Overgeneralisation
+sprongde	sprong	Irregular form plus regular suffix
+sprongden	sprongen	Irregular form plus regular suffix
+gespringd	gesprongen	Overgeneralisation+
+espringd	gesprongen	Overgeneralisation+Prefix ge without onset
+springd	gesprongen	Overgeneralisation+Lacking ge prefix
+gespringde	gesprongene	Overgeneralisation+
+espringde	gesprongene	Overgeneralisation+Prefix ge without onset
+gespringt	gesprongen	Overgeneralisation
+espringt	gesprongen	Overgeneralisation
+springt	gesprongen	Overgeneralisation
+gespringen	gesprongen	Wrong -en suffix
+espringen	gesprongen	Wrong -en suffix
+springen	gesprongen	Wrong -en suffix
+gesprongd	gesprongen	Overgeneralisation
+gesprongt	gesprongen	Overgeneralisation
+esprongen	gesprongen	Prefix ge without onset
+sprongen	gesprongen	Lacking ge prefix
+spruitte	sproot	Overgeneralisation
+spruitten	sproten	Overgeneralisation
+sprootte	sproot	Irregular form plus regular suffix
+sprootten	sproten	Irregular form plus regular suffix
+gespruit	gesproten	Overgeneralisation
+espruit	gesproten	Overgeneralisation
+spruit	gesproten	Overgeneralisation
+gespruite	gesprotene	Overgeneralisation+
+espruite	gesprotene	Overgeneralisation+Prefix ge without onset
+gespruiten	gesproten	Wrong -en suffix
+espruiten	gesproten	Wrong -en suffix
+spruiten	gesproten	Wrong -en suffix
+gesproot	gesproten	Overgeneralisation
+esproten	gesproten	Prefix ge without onset
+sproten	gesproten	Lacking ge prefix
+spuitte	spoot	Overgeneralisation
+spuitten	spoten	Overgeneralisation
+spootte	spoot	Irregular form plus regular suffix
+spootten	spoten	Irregular form plus regular suffix
+gespuit	gespoten	Overgeneralisation
+espuit	gespoten	Overgeneralisation
+spuit	gespoten	Overgeneralisation
+gespuite	gespotene	Overgeneralisation+
+espuite	gespotene	Overgeneralisation+Prefix ge without onset
+gespuiten	gespoten	Wrong -en suffix
+espuiten	gespoten	Wrong -en suffix
+spuiten	gespoten	Wrong -en suffix
+gespoot	gespoten	Overgeneralisation
+espoten	gespoten	Prefix ge without onset
+spoten	gespoten	Lacking ge prefix
+state	stond	Overgeneralisation
+staten	stonden	Overgeneralisation
+stondte	stond	Irregular form plus regular suffix
+stondten	stonden	Irregular form plus regular suffix
+gestat	gestaan	Overgeneralisation+
+estat	gestaan	Overgeneralisation+Prefix ge without onset
+stat	gestaan	Overgeneralisation+Lacking ge prefix
+gestatte	gestaane	Overgeneralisation+
+estatte	gestaane	Overgeneralisation+Prefix ge without onset
+gestaat	gestaan	Overgeneralisation
+estaat	gestaan	Overgeneralisation
+staat	gestaan	Overgeneralisation
+estaan	gestaan	Prefix ge without onset
+staan	gestaan	Lacking ge prefix
+steekte	stak	Overgeneralisation
+steekten	staken	Overgeneralisation
+stakte	stak	Irregular form plus regular suffix
+stakten	staken	Irregular form plus regular suffix
+gesteekt	gestoken	Overgeneralisation
+esteekt	gestoken	Overgeneralisation
+steekt	gestoken	Overgeneralisation
+gesteekte	gestokene	Overgeneralisation+
+esteekte	gestokene	Overgeneralisation+Prefix ge without onset
+gesteken	gestoken	Wrong -en suffix
+esteken	gestoken	Wrong -en suffix
+steken	gestoken	Wrong -en suffix
+gestookt	gestoken	Overgeneralisation
+estoken	gestoken	Prefix ge without onset
+stoken	gestoken	Lacking ge prefix
+steelde	stal	Overgeneralisation
+steelden	stalen	Overgeneralisation
+stalde	stal	Irregular form plus regular suffix
+stalden	stalen	Irregular form plus regular suffix
+gesteeld	gestolen	Overgeneralisation+
+esteeld	gestolen	Overgeneralisation+Prefix ge without onset
+steeld	gestolen	Overgeneralisation+Lacking ge prefix
+gesteelde	gestolene	Overgeneralisation+
+esteelde	gestolene	Overgeneralisation+Prefix ge without onset
+gesteelt	gestolen	Overgeneralisation
+esteelt	gestolen	Overgeneralisation
+steelt	gestolen	Overgeneralisation
+gestelen	gestolen	Wrong -en suffix
+estelen	gestolen	Wrong -en suffix
+stelen	gestolen	Wrong -en suffix
+gestoolt	gestolen	Overgeneralisation
+estolen	gestolen	Prefix ge without onset
+stolen	gestolen	Lacking ge prefix
+sterfde	stierf	Overgeneralisation
+sterfden	stierven	Overgeneralisation
+stierfde	stierf	Irregular form plus regular suffix
+stierfden	stierven	Irregular form plus regular suffix
+gesterfd	gestorven	Overgeneralisation+
+esterfd	gestorven	Overgeneralisation+Prefix ge without onset
+sterfd	gestorven	Overgeneralisation+Lacking ge prefix
+gesterfde	gestorvene	Overgeneralisation+
+esterfde	gestorvene	Overgeneralisation+Prefix ge without onset
+gesterft	gestorven	Overgeneralisation
+esterft	gestorven	Overgeneralisation
+sterft	gestorven	Overgeneralisation
+gesterfen	gestorven	Wrong -en suffix
+esterfen	gestorven	Wrong -en suffix
+sterfen	gestorven	Wrong -en suffix
+gestorfd	gestorven	Overgeneralisation
+gestorft	gestorven	Overgeneralisation
+estorven	gestorven	Prefix ge without onset
+storven	gestorven	Lacking ge prefix
+stijgde	steeg	Overgeneralisation
+stijgden	stegen	Overgeneralisation
+steegde	steeg	Irregular form plus regular suffix
+steegden	stegen	Irregular form plus regular suffix
+gestijgd	gestegen	Overgeneralisation+
+estijgd	gestegen	Overgeneralisation+Prefix ge without onset
+stijgd	gestegen	Overgeneralisation+Lacking ge prefix
+gestijgde	gestegene	Overgeneralisation+
+estijgde	gestegene	Overgeneralisation+Prefix ge without onset
+gestijgt	gestegen	Overgeneralisation
+estijgt	gestegen	Overgeneralisation
+stijgt	gestegen	Overgeneralisation
+gestijgen	gestegen	Wrong -en suffix
+estijgen	gestegen	Wrong -en suffix
+stijgen	gestegen	Wrong -en suffix
+gesteegd	gestegen	Overgeneralisation
+gesteegt	gestegen	Overgeneralisation
+estegen	gestegen	Prefix ge without onset
+stegen	gestegen	Lacking ge prefix
+stijfde	steef	Overgeneralisation
+stijfden	steven	Overgeneralisation
+steefde	steef	Irregular form plus regular suffix
+steefden	steven	Irregular form plus regular suffix
+gestijfd	gesteven	Overgeneralisation+
+estijfd	gesteven	Overgeneralisation+Prefix ge without onset
+stijfd	gesteven	Overgeneralisation+Lacking ge prefix
+gestijfde	gestevene	Overgeneralisation+
+estijfde	gestevene	Overgeneralisation+Prefix ge without onset
+gestijft	gesteven	Overgeneralisation
+estijft	gesteven	Overgeneralisation
+stijft	gesteven	Overgeneralisation
+gestijfen	gesteven	Wrong -en suffix
+estijfen	gesteven	Wrong -en suffix
+stijfen	gesteven	Wrong -en suffix
+gesteefd	gesteven	Overgeneralisation
+gesteeft	gesteven	Overgeneralisation
+esteven	gesteven	Prefix ge without onset
+steven	gesteven	Lacking ge prefix
+stinkte	stonk	Overgeneralisation
+stinkten	stonken	Overgeneralisation
+stonkte	stonk	Irregular form plus regular suffix
+stonkten	stonken	Irregular form plus regular suffix
+gestinkt	gestonken	Overgeneralisation
+estinkt	gestonken	Overgeneralisation
+stinkt	gestonken	Overgeneralisation
+gestinkte	gestonkene	Overgeneralisation+
+estinkte	gestonkene	Overgeneralisation+Prefix ge without onset
+gestinken	gestonken	Wrong -en suffix
+estinken	gestonken	Wrong -en suffix
+stinken	gestonken	Wrong -en suffix
+gestonkt	gestonken	Overgeneralisation
+estonken	gestonken	Prefix ge without onset
+stonken	gestonken	Lacking ge prefix
+gestoot	gestoten	Overgeneralisation
+estoot	gestoten	Overgeneralisation
+stoot	gestoten	Overgeneralisation
+gestote	gestotene	Overgeneralisation+
+estote	gestotene	Overgeneralisation+Prefix ge without onset
+estoten	gestoten	Prefix ge without onset
+stoten	gestoten	Lacking ge prefix
+strijdde	streed	Overgeneralisation
+strijdden	streden	Overgeneralisation
+streedde	streed	Irregular form plus regular suffix
+streedden	streden	Irregular form plus regular suffix
+gestrijd	gestreden	Overgeneralisation
+estrijd	gestreden	Overgeneralisation
+strijd	gestreden	Overgeneralisation
+gestrijde	gestredene	Overgeneralisation+
+estrijde	gestredene	Overgeneralisation+Prefix ge without onset
+gestrijden	gestreden	Wrong -en suffix
+estrijden	gestreden	Wrong -en suffix
+strijden	gestreden	Wrong -en suffix
+gestreed	gestreden	Overgeneralisation
+estreden	gestreden	Prefix ge without onset
+streden	gestreden	Lacking ge prefix
+strijkte	streek	Overgeneralisation
+strijkten	streken	Overgeneralisation
+streekte	streek	Irregular form plus regular suffix
+streekten	streken	Irregular form plus regular suffix
+gestrijkt	gestreken	Overgeneralisation
+estrijkt	gestreken	Overgeneralisation
+strijkt	gestreken	Overgeneralisation
+gestrijkte	gestrekene	Overgeneralisation+
+estrijkte	gestrekene	Overgeneralisation+Prefix ge without onset
+gestrijken	gestreken	Wrong -en suffix
+estrijken	gestreken	Wrong -en suffix
+strijken	gestreken	Wrong -en suffix
+gestreekt	gestreken	Overgeneralisation
+estreken	gestreken	Prefix ge without onset
+streken	gestreken	Lacking ge prefix
+stuifde	stoof	Overgeneralisation
+stuifden	stoven	Overgeneralisation
+stoofde	stoof	Irregular form plus regular suffix
+stoofden	stoven	Irregular form plus regular suffix
+gestuifd	gestoventoven	Overgeneralisation+
+estuifd	gestoventoven	Overgeneralisation+Prefix ge without onset
+stuifd	gestoventoven	Overgeneralisation+Lacking ge prefix
+gestuifde	gestoventovene	Overgeneralisation+
+estuifde	gestoventovene	Overgeneralisation+Prefix ge without onset
+gestuift	gestoventoven	Overgeneralisation
+estuift	gestoventoven	Overgeneralisation
+stuift	gestoventoven	Overgeneralisation
+gestuifen	gestoventoven	Wrong -en suffix
+estuifen	gestoventoven	Wrong -en suffix
+stuifen	gestoventoven	Wrong -en suffix
+gestoventooft	gestoventoven	Overgeneralisation
+estoventoven	gestoventoven	Prefix ge without onset
+stoventoven	gestoventoven	Lacking ge prefix
+treedde	trad	Overgeneralisation
+treedden	traden	Overgeneralisation
+tradde	trad	Irregular form plus regular suffix
+tradden	traden	Irregular form plus regular suffix
+getreed	getreden	Overgeneralisation
+etreed	getreden	Overgeneralisation
+treed	getreden	Overgeneralisation
+getrede	getredene	Overgeneralisation+
+etrede	getredene	Overgeneralisation+Prefix ge without onset
+etreden	getreden	Prefix ge without onset
+treden	getreden	Lacking ge prefix
+trefte	trof	Overgeneralisation
+treften	troffen	Overgeneralisation
+trofte	trof	Irregular form plus regular suffix
+troften	troffen	Irregular form plus regular suffix
+getreft	getroffen	Overgeneralisation
+etreft	getroffen	Overgeneralisation
+treft	getroffen	Overgeneralisation
+getrefte	getroffene	Overgeneralisation+
+etrefte	getroffene	Overgeneralisation+Prefix ge without onset
+getreffen	getroffen	Wrong -en suffix
+etreffen	getroffen	Wrong -en suffix
+treffen	getroffen	Wrong -en suffix
+getroft	getroffen	Overgeneralisation
+etroffen	getroffen	Prefix ge without onset
+troffen	getroffen	Lacking ge prefix
+trekte	trok	Overgeneralisation
+trekten	trokken	Overgeneralisation
+trokte	trok	Irregular form plus regular suffix
+trokten	trokken	Irregular form plus regular suffix
+getrekt	getrokken	Overgeneralisation
+etrekt	getrokken	Overgeneralisation
+trekt	getrokken	Overgeneralisation
+getrekte	getrokkene	Overgeneralisation+
+etrekte	getrokkene	Overgeneralisation+Prefix ge without onset
+getrekken	getrokken	Wrong -en suffix
+etrekken	getrokken	Wrong -en suffix
+trekken	getrokken	Wrong -en suffix
+getrokt	getrokken	Overgeneralisation
+etrokken	getrokken	Prefix ge without onset
+trokken	getrokken	Lacking ge prefix
+valde	viel	Overgeneralisation
+valden	vielen	Overgeneralisation
+vielde	viel	Irregular form plus regular suffix
+vielden	vielen	Irregular form plus regular suffix
+gevald	gevallen	Overgeneralisation
+evald	gevallen	Overgeneralisation+Prefix ge without onset
+vald	gevallen	Overgeneralisation+Lacking ge prefix
+gevalde	gevallene	Overgeneralisation+
+evalde	gevallene	Overgeneralisation+Prefix ge without onset
+gevalt	gevallen	Overgeneralisation
+evalt	gevallen	Overgeneralisation
+valt	gevallen	Overgeneralisation
+evallen	gevallen	Prefix ge without onset
+vallen	gevallen	Lacking ge prefix
+vangde	ving	Overgeneralisation
+vangden	vingen	Overgeneralisation
+vingde	ving	Irregular form plus regular suffix
+vingden	vingen	Irregular form plus regular suffix
+gevangd	gevangen	Overgeneralisation
+evangd	gevangen	Overgeneralisation+Prefix ge without onset
+vangd	gevangen	Overgeneralisation+Lacking ge prefix
+gevangde	gevangene	Overgeneralisation+
+evangde	gevangene	Overgeneralisation+Prefix ge without onset
+gevangt	gevangen	Overgeneralisation
+evangt	gevangen	Overgeneralisation
+vangt	gevangen	Overgeneralisation
+evangen	gevangen	Prefix ge without onset
+vangen	gevangen	Lacking ge prefix
+vaarde	voer	Overgeneralisation
+vaarden	voeren	Overgeneralisation
+voerde	voer	Irregular form plus regular suffix
+voerden	voeren	Irregular form plus regular suffix
+gevaard	gevaren	Overgeneralisation
+evaard	gevaren	Overgeneralisation+Prefix ge without onset
+vaard	gevaren	Overgeneralisation+Lacking ge prefix
+gevaarde	gevarene	Overgeneralisation+
+evaarde	gevarene	Overgeneralisation+Prefix ge without onset
+gevaart	gevaren	Overgeneralisation
+evaart	gevaren	Overgeneralisation
+vaart	gevaren	Overgeneralisation
+evaren	gevaren	Prefix ge without onset
+varen	gevaren	Lacking ge prefix
+vechtte	vocht	Overgeneralisation
+vechtten	vochten	Overgeneralisation
+vochtte	vocht	Irregular form plus regular suffix
+vochtten	vochten	Irregular form plus regular suffix
+gevecht	gevochten	Overgeneralisation
+evecht	gevochten	Overgeneralisation
+vecht	gevochten	Overgeneralisation
+gevechte	gevochtene	Overgeneralisation+
+evechte	gevochtene	Overgeneralisation+Prefix ge without onset
+gevechten	gevochten	Wrong -en suffix
+evechten	gevochten	Wrong -en suffix
+vechten	gevochten	Wrong -en suffix
+gevocht	gevochten	Overgeneralisation
+evochten	gevochten	Prefix ge without onset
+vochten	gevochten	Lacking ge prefix
+verdriette	verdroot	Overgeneralisation
+verdrietten	verdroten	Overgeneralisation
+verdrootte	verdroot	Irregular form plus regular suffix
+verdrootten	verdroten	Irregular form plus regular suffix
+verdriet	verdroten	Overgeneralisation
+verdriete	verdrotene	Overgeneralisation
+verdrieten	verdroten	Wrong -en suffix
+verdroot	verdroten	Overgeneralisation
+verdwijnde	verdwenene	Overgeneralisation
+verdwijnden	verdwenen	Overgeneralisation
+verdweende	verdween	Irregular form plus regular suffix
+verdweenden	verdwenen	Irregular form plus regular suffix
+verdwijnd	verdwenen	Overgeneralisation
+verdwijnt	verdwenen	Overgeneralisation
+verdwijnen	verdwenen	Wrong -en suffix
+verdweend	verdwenen	Overgeneralisation
+verdweent	verdwenen	Overgeneralisation
+vergeette	vergat	Overgeneralisation
+vergeetten	vergaten	Overgeneralisation
+vergatte	vergat	Irregular form plus regular suffix
+vergatten	vergaten	Irregular form plus regular suffix
+vergeet	vergeten	Overgeneralisation
+vergete	vergetene	Overgeneralisation
+verliesde	verlorene	Overgeneralisation
+verliesden	verloren	Overgeneralisation
+verloorde	verloor	Irregular form plus regular suffix
+verloorden	verloren	Irregular form plus regular suffix
+verliesd	verloren	Overgeneralisation
+verliest	verloren	Overgeneralisation
+verliesen	verloren	Wrong -en suffix
+verloort	verloren	Overgeneralisation
+vindde	vond	Overgeneralisation
+vindden	vonden	Overgeneralisation
+vondde	vond	Irregular form plus regular suffix
+vondden	vonden	Irregular form plus regular suffix
+gevind	gevonden	Overgeneralisation
+evind	gevonden	Overgeneralisation
+vind	gevonden	Overgeneralisation
+gevinde	gevondene	Overgeneralisation+
+evinde	gevondene	Overgeneralisation+Prefix ge without onset
+gevinden	gevonden	Wrong -en suffix
+evinden	gevonden	Wrong -en suffix
+vinden	gevonden	Wrong -en suffix
+gevond	gevonden	Overgeneralisation
+evonden	gevonden	Prefix ge without onset
+vonden	gevonden	Lacking ge prefix
+vlechtte	vlocht	Overgeneralisation
+vlechtten	vlochten	Overgeneralisation
+vlochtte	vlocht	Irregular form plus regular suffix
+vlochtten	vlochten	Irregular form plus regular suffix
+gevlecht	gevlochten	Overgeneralisation
+evlecht	gevlochten	Overgeneralisation
+vlecht	gevlochten	Overgeneralisation
+gevlechte	gevlochtene	Overgeneralisation+
+evlechte	gevlochtene	Overgeneralisation+Prefix ge without onset
+gevlechten	gevlochten	Wrong -en suffix
+evlechten	gevlochten	Wrong -en suffix
+vlechten	gevlochten	Wrong -en suffix
+gevlocht	gevlochten	Overgeneralisation
+evlochten	gevlochten	Prefix ge without onset
+vlochten	gevlochten	Lacking ge prefix
+vliegde	vloog	Overgeneralisation
+vliegden	vlogen	Overgeneralisation
+vloogde	vloog	Irregular form plus regular suffix
+vloogden	vlogen	Irregular form plus regular suffix
+gevliegd	gevlogen	Overgeneralisation+
+evliegd	gevlogen	Overgeneralisation+Prefix ge without onset
+vliegd	gevlogen	Overgeneralisation+Lacking ge prefix
+gevliegde	gevlogene	Overgeneralisation+
+evliegde	gevlogene	Overgeneralisation+Prefix ge without onset
+gevliegt	gevlogen	Overgeneralisation
+evliegt	gevlogen	Overgeneralisation
+vliegt	gevlogen	Overgeneralisation
+gevliegen	gevlogen	Wrong -en suffix
+evliegen	gevlogen	Wrong -en suffix
+vliegen	gevlogen	Wrong -en suffix
+gevloogt	gevlogen	Overgeneralisation
+evlogen	gevlogen	Prefix ge without onset
+vlogen	gevlogen	Lacking ge prefix
+gevouwd	gevouwen	Overgeneralisation
+evouwd	gevouwen	Overgeneralisation+Prefix ge without onset
+vouwd	gevouwen	Overgeneralisation+Lacking ge prefix
+gevouwde	gevouwene	Overgeneralisation+
+evouwde	gevouwene	Overgeneralisation+Prefix ge without onset
+gevouwt	gevouwen	Overgeneralisation
+evouwt	gevouwen	Overgeneralisation
+vouwt	gevouwen	Overgeneralisation
+evouwen	gevouwen	Prefix ge without onset
+vouwen	gevouwen	Lacking ge prefix
+vraagde	vroeg	Overgeneralisation
+vraagden	vroegen	Overgeneralisation
+vroegde	vroeg	Irregular form plus regular suffix
+vroegden	vroegen	Irregular form plus regular suffix
+evraagd	gevraagd	Prefix ge without onset
+vraagd	gevraagd	Lacking ge prefix
+evraagde	gevraagde	Overgeneralisation+Prefix ge without onset
+gevraagt	gevraagd	Overgeneralisation
+evraagt	gevraagd	Overgeneralisation
+vraagt	gevraagd	Overgeneralisation
+gevragen	gevraagd	Wrong -en suffix
+evragen	gevraagd	Wrong -en suffix
+vragen	gevraagd	Wrong -en suffix
+vreette	vrat	Overgeneralisation
+vreetten	vraten	Overgeneralisation
+vratte	vrat	Irregular form plus regular suffix
+vratten	vraten	Irregular form plus regular suffix
+gevreet	gevreten	Overgeneralisation
+evreet	gevreten	Overgeneralisation
+vreet	gevreten	Overgeneralisation
+gevrete	gevretene	Overgeneralisation+
+evrete	gevretene	Overgeneralisation+Prefix ge without onset
+evreten	gevreten	Prefix ge without onset
+vreten	gevreten	Lacking ge prefix
+vriesde	vroor	Overgeneralisation
+vriesden	vroren	Overgeneralisation
+vroorde	vroor	Irregular form plus regular suffix
+vroorden	vroren	Irregular form plus regular suffix
+gevriesd	gevroren	Overgeneralisation+
+evriesd	gevroren	Overgeneralisation+Prefix ge without onset
+vriesd	gevroren	Overgeneralisation+Lacking ge prefix
+gevriesde	gevrorene	Overgeneralisation+
+evriesde	gevrorene	Overgeneralisation+Prefix ge without onset
+gevriest	gevroren	Overgeneralisation
+evriest	gevroren	Overgeneralisation
+vriest	gevroren	Overgeneralisation
+gevriesen	gevroren	Wrong -en suffix
+evriesen	gevroren	Wrong -en suffix
+vriesen	gevroren	Wrong -en suffix
+gevroort	gevroren	Overgeneralisation
+evroren	gevroren	Prefix ge without onset
+vroren	gevroren	Lacking ge prefix
+vriijde	vrijde	Overgeneralisation
+vriijden	vrijden	Overgeneralisation
+gevriijd	gevrijd	Overgeneralisation+
+evriijd	gevrijd	Overgeneralisation+Prefix ge without onset
+vriijd	gevrijd	Overgeneralisation+Lacking ge prefix
+gevriijde	gevrijde	Overgeneralisation+
+evriijde	gevrijde	Overgeneralisation+Prefix ge without onset
+gevriijt	gevrijd	Overgeneralisation
+evriijt	gevrijd	Overgeneralisation
+vriijt	gevrijd	Overgeneralisation
+gevrijen	gevrijd	Wrong -en suffix
+evrijen	gevrijd	Wrong -en suffix
+vrijen	gevrijd	Wrong -en suffix
+evrijd	gevrijd	Prefix ge without onset
+vrijd	gevrijd	Lacking ge prefix
+gewast	gewassen	Overgeneralisation
+ewast	gewassen	Overgeneralisation
+wast	gewassen	Overgeneralisation
+gewaste	gewassene	Overgeneralisation+
+ewaste	gewassene	Overgeneralisation+Prefix ge without onset
+ewassen	gewassen	Prefix ge without onset
+wassen	gewassen	Lacking ge prefix
+weegde	woog	Overgeneralisation
+weegden	wogen	Overgeneralisation
+woogde	woog	Irregular form plus regular suffix
+woogden	wogen	Irregular form plus regular suffix
+geweegd	gewogen	Overgeneralisation+
+eweegd	gewogen	Overgeneralisation+Prefix ge without onset
+weegd	gewogen	Overgeneralisation+Lacking ge prefix
+geweegde	gewogene	Overgeneralisation+
+eweegde	gewogene	Overgeneralisation+Prefix ge without onset
+geweegt	gewogen	Overgeneralisation
+eweegt	gewogen	Overgeneralisation
+weegt	gewogen	Overgeneralisation
+gewegen	gewogen	Wrong -en suffix
+ewegen	gewogen	Wrong -en suffix
+wegen	gewogen	Wrong -en suffix
+gewoogt	gewogen	Overgeneralisation
+ewogen	gewogen	Prefix ge without onset
+wogen	gewogen	Lacking ge prefix
+werpte	wierp	Overgeneralisation
+werpten	wierpen	Overgeneralisation
+wierpte	wierp	Irregular form plus regular suffix
+wierpten	wierpen	Irregular form plus regular suffix
+gewerpt	geworpen	Overgeneralisation
+ewerpt	geworpen	Overgeneralisation
+werpt	geworpen	Overgeneralisation
+gewerpte	geworpene	Overgeneralisation+
+ewerpte	geworpene	Overgeneralisation+Prefix ge without onset
+gewerpen	geworpen	Wrong -en suffix
+ewerpen	geworpen	Wrong -en suffix
+werpen	geworpen	Wrong -en suffix
+geworpt	geworpen	Overgeneralisation
+eworpen	geworpen	Prefix ge without onset
+worpen	geworpen	Lacking ge prefix
+werfde	wierf	Overgeneralisation
+werfden	wierven	Overgeneralisation
+wierfde	wierf	Irregular form plus regular suffix
+wierfden	wierven	Irregular form plus regular suffix
+gewerfd	geworven	Overgeneralisation+
+ewerfd	geworven	Overgeneralisation+Prefix ge without onset
+werfd	geworven	Overgeneralisation+Lacking ge prefix
+gewerfde	geworvene	Overgeneralisation+
+ewerfde	geworvene	Overgeneralisation+Prefix ge without onset
+gewerft	geworven	Overgeneralisation
+ewerft	geworven	Overgeneralisation
+werft	geworven	Overgeneralisation
+gewerfen	geworven	Wrong -en suffix
+ewerfen	geworven	Wrong -en suffix
+werfen	geworven	Wrong -en suffix
+geworfd	geworven	Overgeneralisation
+geworft	geworven	Overgeneralisation
+eworven	geworven	Prefix ge without onset
+worven	geworven	Lacking ge prefix
+weette	weet	Irregular form plus regular suffix
+weetten	weten	Irregular form plus regular suffix
+wistte	wist	Irregular form plus regular suffix
+wistten	wisten	Irregular form plus regular suffix
+geweet	geweten	Overgeneralisation
+eweet	geweten	Overgeneralisation
+weet	geweten	Overgeneralisation
+gewete	gewetene	Overgeneralisation+
+ewete	gewetene	Overgeneralisation+Prefix ge without onset
+eweten	geweten	Prefix ge without onset
+weten	geweten	Lacking ge prefix
+geweefd	geweven	Overgeneralisation
+eweefd	geweven	Overgeneralisation+Prefix ge without onset
+weefd	geweven	Overgeneralisation+Lacking ge prefix
+geweefde	gewevene	Overgeneralisation+
+eweefde	gewevene	Overgeneralisation+Prefix ge without onset
+geweeft	geweven	Overgeneralisation
+eweeft	geweven	Overgeneralisation
+weeft	geweven	Overgeneralisation
+gewefen	geweven	Wrong -en suffix
+ewefen	geweven	Wrong -en suffix
+wefen	geweven	Wrong -en suffix
+eweven	geweven	Prefix ge without onset
+weven	geweven	Lacking ge prefix
+wijkte	week	Overgeneralisation
+wijkten	weken	Overgeneralisation
+weekte	week	Irregular form plus regular suffix
+weekten	weken	Irregular form plus regular suffix
+gewijkt	geweken	Overgeneralisation
+ewijkt	geweken	Overgeneralisation
+wijkt	geweken	Overgeneralisation
+gewijkte	gewekene	Overgeneralisation+
+ewijkte	gewekene	Overgeneralisation+Prefix ge without onset
+gewijken	geweken	Wrong -en suffix
+ewijken	geweken	Wrong -en suffix
+wijken	geweken	Wrong -en suffix
+geweekt	geweken	Overgeneralisation
+eweken	geweken	Prefix ge without onset
+weken	geweken	Lacking ge prefix
+wijtte	weet	Overgeneralisation
+wijtten	weten	Overgeneralisation
+gewijt	geweten	Overgeneralisation
+ewijt	geweten	Overgeneralisation
+wijt	geweten	Overgeneralisation
+gewijte	gewetene	Overgeneralisation+
+ewijte	gewetene	Overgeneralisation+Prefix ge without onset
+gewijten	geweten	Wrong -en suffix
+ewijten	geweten	Wrong -en suffix
+wijten	geweten	Wrong -en suffix
+wijsde	wees	Overgeneralisation
+wijsden	wezen	Overgeneralisation
+weesde	wees	Irregular form plus regular suffix
+weesden	wezen	Irregular form plus regular suffix
+gewijsd	gewezen	Overgeneralisation+
+ewijsd	gewezen	Overgeneralisation+Prefix ge without onset
+wijsd	gewezen	Overgeneralisation+Lacking ge prefix
+gewijsde	gewezene	Overgeneralisation+
+ewijsde	gewezene	Overgeneralisation+Prefix ge without onset
+gewijst	gewezen	Overgeneralisation
+ewijst	gewezen	Overgeneralisation
+wijst	gewezen	Overgeneralisation
+gewijsen	gewezen	Wrong -en suffix
+ewijsen	gewezen	Wrong -en suffix
+wijsen	gewezen	Wrong -en suffix
+geweesd	gewezen	Overgeneralisation
+geweest	gewezen	Overgeneralisation
+ewezen	gewezen	Prefix ge without onset
+wezen	gewezen	Lacking ge prefix
+windde	wond	Overgeneralisation
+windden	wonden	Overgeneralisation
+wondde	wond	Irregular form plus regular suffix
+wondden	wonden	Irregular form plus regular suffix
+gewind	gewonnen	Overgeneralisation+
+ewind	gewonnen	Overgeneralisation+Prefix ge without onset
+wind	gewonnen	Overgeneralisation+Lacking ge prefix
+gewinde	gewonnene	Overgeneralisation+
+ewinde	gewonnene	Overgeneralisation+Prefix ge without onset
+gewinden	gewonden	Wrong -en suffix
+ewinden	gewonden	Wrong -en suffix
+winden	wonnen	Overgeneralisation
+gewond	gewonden	Overgeneralisation
+ewonden	gewonden	Prefix ge without onset
+wonden	wonnen	Irregular form plus regular suffix
+winde	won	Overgeneralisation
+wonde	won	Irregular form plus regular suffix
+gewint	gewonnen	Overgeneralisation
+ewint	gewonnen	Overgeneralisation
+wint	gewonnen	Overgeneralisation
+gewinnen	gewonnen	Wrong -en suffix
+ewinnen	gewonnen	Wrong -en suffix
+winnen	gewonnen	Wrong -en suffix
+gewont	gewonnen	Overgeneralisation
+ewonnen	gewonnen	Prefix ge without onset
+wonnen	gewonnen	Lacking ge prefix
+wordde	werd	Overgeneralisation
+wordden	werden	Overgeneralisation
+werdde	werd	Irregular form plus regular suffix
+werdden	werden	Irregular form plus regular suffix
+geword	geworden	Overgeneralisation
+eword	geworden	Overgeneralisation
+word	geworden	Overgeneralisation
+geworde	gewordene	Overgeneralisation+
+eworde	gewordene	Overgeneralisation+Prefix ge without onset
+eworden	geworden	Prefix ge without onset
+worden	geworden	Lacking ge prefix
+wrijfde	wreef	Overgeneralisation
+wrijfden	wreven	Overgeneralisation
+wreefde	wreef	Irregular form plus regular suffix
+wreefden	wreven	Irregular form plus regular suffix
+gewrijfd	gewreven	Overgeneralisation+
+ewrijfd	gewreven	Overgeneralisation+Prefix ge without onset
+wrijfd	gewreven	Overgeneralisation+Lacking ge prefix
+gewrijfde	gewrevene	Overgeneralisation+
+ewrijfde	gewrevene	Overgeneralisation+Prefix ge without onset
+gewrijft	gewreven	Overgeneralisation
+ewrijft	gewreven	Overgeneralisation
+wrijft	gewreven	Overgeneralisation
+gewrijfen	gewreven	Wrong -en suffix
+ewrijfen	gewreven	Wrong -en suffix
+wrijfen	gewreven	Wrong -en suffix
+gewreefd	gewreven	Overgeneralisation
+gewreeft	gewreven	Overgeneralisation
+ewreven	gewreven	Prefix ge without onset
+wreven	gewreven	Lacking ge prefix
+wringde	wrong	Overgeneralisation
+wringden	wrongen	Overgeneralisation
+wrongde	wrong	Irregular form plus regular suffix
+wrongden	wrongen	Irregular form plus regular suffix
+gewringd	gewrongen	Overgeneralisation+
+ewringd	gewrongen	Overgeneralisation+Prefix ge without onset
+wringd	gewrongen	Overgeneralisation+Lacking ge prefix
+gewringde	gewrongene	Overgeneralisation+
+ewringde	gewrongene	Overgeneralisation+Prefix ge without onset
+gewringt	gewrongen	Overgeneralisation
+ewringt	gewrongen	Overgeneralisation
+wringt	gewrongen	Overgeneralisation
+gewringen	gewrongen	Wrong -en suffix
+ewringen	gewrongen	Wrong -en suffix
+wringen	gewrongen	Wrong -en suffix
+gewrongd	gewrongen	Overgeneralisation
+gewrongt	gewrongen	Overgeneralisation
+ewrongen	gewrongen	Prefix ge without onset
+wrongen	gewrongen	Lacking ge prefix
+zegde	zei	Overgeneralisation
+zegden	zeiden	Overgeneralisation
+zeide	zei	Irregular form plus regular suffix
+ezegd	gezegd	Prefix ge without onset
+zegd	gezegd	Lacking ge prefix
+ezegde	gezegde	Overgeneralisation+Prefix ge without onset
+gezegt	gezegd	Overgeneralisation
+ezegt	gezegd	Overgeneralisation
+zegt	gezegd	Overgeneralisation
+gezeggen	gezegd	Wrong -en suffix
+ezeggen	gezegd	Wrong -en suffix
+zeggen	gezegd	Wrong -en suffix
+zendde	zond	Overgeneralisation
+zendden	zonden	Overgeneralisation
+zondde	zond	Irregular form plus regular suffix
+zondden	zonden	Irregular form plus regular suffix
+gezend	gezonden	Overgeneralisation
+ezend	gezonden	Overgeneralisation
+zend	gezonden	Overgeneralisation
+gezende	gezondene	Overgeneralisation+
+ezende	gezondene	Overgeneralisation+Prefix ge without onset
+gezenden	gezonden	Wrong -en suffix
+ezenden	gezonden	Wrong -en suffix
+zenden	gezonden	Wrong -en suffix
+gezond	gezonden	Overgeneralisation
+ezonden	gezonden	Prefix ge without onset
+zonden	zonnen	Irregular form plus regular suffix
+zijgde	zeeg	Overgeneralisation
+zijgden	zegen	Overgeneralisation
+zeegde	zeeg	Irregular form plus regular suffix
+zeegden	zegen	Irregular form plus regular suffix
+gezijgd	gezegen	Overgeneralisation+
+ezijgd	gezegen	Overgeneralisation+Prefix ge without onset
+zijgd	gezegen	Overgeneralisation+Lacking ge prefix
+gezijgde	gezegene	Overgeneralisation+
+ezijgde	gezegene	Overgeneralisation+Prefix ge without onset
+gezijgt	gezegen	Overgeneralisation
+ezijgt	gezegen	Overgeneralisation
+zijgt	gezegen	Overgeneralisation
+gezijgen	gezegen	Wrong -en suffix
+ezijgen	gezegen	Wrong -en suffix
+zijgen	gezegen	Wrong -en suffix
+gezeegd	gezegen	Overgeneralisation
+gezeegt	gezegen	Overgeneralisation
+ezegen	gezegen	Prefix ge without onset
+zegen	gezegen	Lacking ge prefix
+zijde	was	Overgeneralisation
+zijden	waren	Overgeneralisation
+wasde	was	Irregular form plus regular suffix
+wasden	waren	Irregular form plus regular suffix
+gezijd	geweest	Overgeneralisation+
+ezijd	geweest	Overgeneralisation+Prefix ge without onset
+zijd	geweest	Overgeneralisation+Lacking ge prefix
+gezijde	geweeste	Overgeneralisation+
+ezijde	geweeste	Overgeneralisation+Prefix ge without onset
+gezijt	geweest	Overgeneralisation
+ezijt	geweest	Overgeneralisation
+zijt	geweest	Overgeneralisation
+gezijjen	geweest	Wrong -en suffix
+ezijjen	geweest	Wrong -en suffix
+zijjen	geweest	Wrong -en suffix
+eweest	geweest	Prefix ge without onset
+weest	geweest	Lacking ge prefix
+zingde	zong	Overgeneralisation
+zingden	zongen	Overgeneralisation
+zongde	zong	Irregular form plus regular suffix
+zongden	zongen	Irregular form plus regular suffix
+gezingd	gezongen	Overgeneralisation+
+ezingd	gezongen	Overgeneralisation+Prefix ge without onset
+zingd	gezongen	Overgeneralisation+Lacking ge prefix
+gezingde	gezongene	Overgeneralisation+
+ezingde	gezongene	Overgeneralisation+Prefix ge without onset
+gezingt	gezongen	Overgeneralisation
+ezingt	gezongen	Overgeneralisation
+zingt	gezongen	Overgeneralisation
+gezingen	gezongen	Wrong -en suffix
+ezingen	gezongen	Wrong -en suffix
+zingen	gezongen	Wrong -en suffix
+gezongd	gezongen	Overgeneralisation
+gezongt	gezongen	Overgeneralisation
+ezongen	gezongen	Prefix ge without onset
+zongen	gezongen	Lacking ge prefix
+zinkte	zonk	Overgeneralisation
+zinkten	zonken	Overgeneralisation
+zonkte	zonk	Irregular form plus regular suffix
+zonkten	zonken	Irregular form plus regular suffix
+gezinkt	gezonken	Overgeneralisation
+ezinkt	gezonken	Overgeneralisation
+zinkt	gezonken	Overgeneralisation
+gezinkte	gezonkene	Overgeneralisation+
+ezinkte	gezonkene	Overgeneralisation+Prefix ge without onset
+gezinken	gezonken	Wrong -en suffix
+ezinken	gezonken	Wrong -en suffix
+zinken	gezonken	Wrong -en suffix
+gezonkt	gezonken	Overgeneralisation
+ezonken	gezonken	Prefix ge without onset
+zonken	gezonken	Lacking ge prefix
+zinde	zon	Overgeneralisation
+zinden	zonnen	Overgeneralisation
+zonde	zon	Irregular form plus regular suffix
+gezind	gezonnen	Overgeneralisation+
+ezind	gezonnen	Overgeneralisation+Prefix ge without onset
+zind	gezonnen	Overgeneralisation+Lacking ge prefix
+gezinde	gezonnene	Overgeneralisation+
+ezinde	gezonnene	Overgeneralisation+Prefix ge without onset
+gezint	gezonnen	Overgeneralisation
+ezint	gezonnen	Overgeneralisation
+zint	gezonnen	Overgeneralisation
+gezinnen	gezonnen	Wrong -en suffix
+ezinnen	gezonnen	Wrong -en suffix
+zinnen	gezonnen	Wrong -en suffix
+gezont	gezonnen	Overgeneralisation
+ezonnen	gezonnen	Prefix ge without onset
+zonnen	gezonnen	Lacking ge prefix
+zitte	zat	Overgeneralisation
+zitten	gezeten	Wrong -en suffix
+zatte	zat	Irregular form plus regular suffix
+zatten	zaten	Irregular form plus regular suffix
+gezit	gezeten	Overgeneralisation
+ezit	gezeten	Overgeneralisation
+zit	gezeten	Overgeneralisation
+gezitte	gezetene	Overgeneralisation+
+ezitte	gezetene	Overgeneralisation+Prefix ge without onset
+gezitten	gezeten	Wrong -en suffix
+ezitten	gezeten	Wrong -en suffix
+gezeet	gezeten	Overgeneralisation
+ezeten	gezeten	Prefix ge without onset
+zeten	gezeten	Lacking ge prefix
+zoekte	zocht	Overgeneralisation
+zoekten	zochten	Overgeneralisation
+zochtte	zocht	Irregular form plus regular suffix
+zochtten	zochten	Irregular form plus regular suffix
+gezoekt	gezocht	Overgeneralisation
+ezoekt	gezocht	Overgeneralisation
+zoekt	gezocht	Overgeneralisation
+gezoekte	gezochte	Overgeneralisation+
+ezoekte	gezochte	Overgeneralisation+Prefix ge without onset
+gezoeken	gezocht	Wrong -en suffix
+ezoeken	gezocht	Wrong -en suffix
+zoeken	gezocht	Wrong -en suffix
+ezocht	gezocht	Prefix ge without onset
+zocht	gezocht	Lacking ge prefix
+zuigde	zoog	Overgeneralisation
+zuigden	zogen	Overgeneralisation
+zoogde	zoog	Irregular form plus regular suffix
+zoogden	zogen	Irregular form plus regular suffix
+gezuigd	gezogen	Overgeneralisation+
+ezuigd	gezogen	Overgeneralisation+Prefix ge without onset
+zuigd	gezogen	Overgeneralisation+Lacking ge prefix
+gezuigde	gezogene	Overgeneralisation+
+ezuigde	gezogene	Overgeneralisation+Prefix ge without onset
+gezuigt	gezogen	Overgeneralisation
+ezuigt	gezogen	Overgeneralisation
+zuigt	gezogen	Overgeneralisation
+gezuigen	gezogen	Wrong -en suffix
+ezuigen	gezogen	Wrong -en suffix
+zuigen	gezogen	Wrong -en suffix
+gezoogt	gezogen	Overgeneralisation
+ezogen	gezogen	Prefix ge without onset
+zogen	gezogen	Lacking ge prefix
+zuipte	zoop	Overgeneralisation
+zuipten	zopen	Overgeneralisation
+zoopte	zoop	Irregular form plus regular suffix
+zoopten	zopen	Irregular form plus regular suffix
+gezuipt	gezopen	Overgeneralisation
+ezuipt	gezopen	Overgeneralisation
+zuipt	gezopen	Overgeneralisation
+gezuipte	gezopene	Overgeneralisation+
+ezuipte	gezopene	Overgeneralisation+Prefix ge without onset
+gezuipen	gezopen	Wrong -en suffix
+ezuipen	gezopen	Wrong -en suffix
+zuipen	gezopen	Wrong -en suffix
+gezoopt	gezopen	Overgeneralisation
+ezopen	gezopen	Prefix ge without onset
+zopen	gezopen	Lacking ge prefix
+zwelgde	zwolg	Overgeneralisation
+zwelgden	zwolgen	Overgeneralisation
+zwolgde	zwolg	Irregular form plus regular suffix
+zwolgden	zwolgen	Irregular form plus regular suffix
+gezwelgd	gezwolgen	Overgeneralisation+
+ezwelgd	gezwolgen	Overgeneralisation+Prefix ge without onset
+zwelgd	gezwolgen	Overgeneralisation+Lacking ge prefix
+gezwelgde	gezwolgene	Overgeneralisation+
+ezwelgde	gezwolgene	Overgeneralisation+Prefix ge without onset
+gezwelgt	gezwolgen	Overgeneralisation
+ezwelgt	gezwolgen	Overgeneralisation
+zwelgt	gezwolgen	Overgeneralisation
+gezwelgen	gezwolgen	Wrong -en suffix
+ezwelgen	gezwolgen	Wrong -en suffix
+zwelgen	gezwolgen	Wrong -en suffix
+gezwolgd	gezwolgen	Overgeneralisation
+gezwolgt	gezwolgen	Overgeneralisation
+ezwolgen	gezwolgen	Prefix ge without onset
+zwolgen	gezwolgen	Lacking ge prefix
+zwelde	zwol	Overgeneralisation
+zwelden	zwollen	Overgeneralisation
+zwolde	zwol	Irregular form plus regular suffix
+zwolden	zwollen	Irregular form plus regular suffix
+gezweld	gezwollen	Overgeneralisation+
+ezweld	gezwollen	Overgeneralisation+Prefix ge without onset
+zweld	gezwollen	Overgeneralisation+Lacking ge prefix
+gezwelde	gezwollene	Overgeneralisation+
+ezwelde	gezwollene	Overgeneralisation+Prefix ge without onset
+gezwelt	gezwollen	Overgeneralisation
+ezwelt	gezwollen	Overgeneralisation
+zwelt	gezwollen	Overgeneralisation
+gezwellen	gezwollen	Wrong -en suffix
+ezwellen	gezwollen	Wrong -en suffix
+zwellen	gezwollen	Wrong -en suffix
+gezwolt	gezwollen	Overgeneralisation
+ezwollen	gezwollen	Prefix ge without onset
+zwollen	gezwollen	Lacking ge prefix
+zwemde	zwom	Overgeneralisation
+zwemden	zwommen	Overgeneralisation
+zwomde	zwom	Irregular form plus regular suffix
+zwomden	zwommen	Irregular form plus regular suffix
+gezwemd	gezwommen	Overgeneralisation+
+ezwemd	gezwommen	Overgeneralisation+Prefix ge without onset
+zwemd	gezwommen	Overgeneralisation+Lacking ge prefix
+gezwemde	gezwommene	Overgeneralisation+
+ezwemde	gezwommene	Overgeneralisation+Prefix ge without onset
+gezwemt	gezwommen	Overgeneralisation
+ezwemt	gezwommen	Overgeneralisation
+zwemt	gezwommen	Overgeneralisation
+gezwemmen	gezwommen	Wrong -en suffix
+ezwemmen	gezwommen	Wrong -en suffix
+zwemmen	gezwommen	Wrong -en suffix
+gezwomt	gezwommen	Overgeneralisation
+ezwommen	gezwommen	Prefix ge without onset
+zwommen	gezwommen	Lacking ge prefix
+zweerde	zwoer	Overgeneralisation
+zweerden	zwoeren	Overgeneralisation
+zwoerde	zwoer	Irregular form plus regular suffix
+zwoerden	zwoeren	Irregular form plus regular suffix
+gezweerd	gezworen	Overgeneralisation+
+ezweerd	gezworen	Overgeneralisation+Prefix ge without onset
+zweerd	gezworen	Overgeneralisation+Lacking ge prefix
+gezweerde	gezworene	Overgeneralisation+
+ezweerde	gezworene	Overgeneralisation+Prefix ge without onset
+gezweert	gezworen	Overgeneralisation
+ezweert	gezworen	Overgeneralisation
+zweert	gezworen	Overgeneralisation
+gezweren	gezworen	Wrong -en suffix
+ezweren	gezworen	Wrong -en suffix
+zweren	gezworen	Wrong -en suffix
+gezwoort	gezworen	Overgeneralisation
+ezworen	gezworen	Prefix ge without onset
+zworen	gezworen	Lacking ge prefix
+zwerfde	zwierf	Overgeneralisation
+zwerfden	zwierven	Overgeneralisation
+zwierfde	zwierf	Irregular form plus regular suffix
+zwierfden	zwierven	Irregular form plus regular suffix
+gezwerfd	gezworven	Overgeneralisation+
+ezwerfd	gezworven	Overgeneralisation+Prefix ge without onset
+zwerfd	gezworven	Overgeneralisation+Lacking ge prefix
+gezwerfde	gezworvene	Overgeneralisation+
+ezwerfde	gezworvene	Overgeneralisation+Prefix ge without onset
+gezwerft	gezworven	Overgeneralisation
+ezwerft	gezworven	Overgeneralisation
+zwerft	gezworven	Overgeneralisation
+gezwerfen	gezworven	Wrong -en suffix
+ezwerfen	gezworven	Wrong -en suffix
+zwerfen	gezworven	Wrong -en suffix
+gezworfd	gezworven	Overgeneralisation
+gezworft	gezworven	Overgeneralisation
+ezworven	gezworven	Prefix ge without onset
+zworven	gezworven	Lacking ge prefix
+zwijgde	zweeg	Overgeneralisation
+zwijgden	zwegen	Overgeneralisation
+zweegde	zweeg	Irregular form plus regular suffix
+zweegden	zwegen	Irregular form plus regular suffix
+gezwijgd	gezwegen	Overgeneralisation+
+ezwijgd	gezwegen	Overgeneralisation+Prefix ge without onset
+zwijgd	gezwegen	Overgeneralisation+Lacking ge prefix
+gezwijgde	gezwegene	Overgeneralisation+
+ezwijgde	gezwegene	Overgeneralisation+Prefix ge without onset
+gezwijgt	gezwegen	Overgeneralisation
+ezwijgt	gezwegen	Overgeneralisation
+zwijgt	gezwegen	Overgeneralisation
+gezwijgen	gezwegen	Wrong -en suffix
+ezwijgen	gezwegen	Wrong -en suffix
+zwijgen	gezwegen	Wrong -en suffix
+gezweegd	gezwegen	Overgeneralisation
+gezweegt	gezwegen	Overgeneralisation
+ezwegen	gezwegen	Prefix ge without onset
+zwegen	gezwegen	Lacking ge prefix
```

### Comparing `sastadev-0.1.5/src/sastadev/data/macros/newimperatives.txt` & `sastadev-0.2.0/src/sastadev/data/macros/newimperatives.txt`

 * *Files 13% similar despite different names*

```diff
@@ -53,35 +53,39 @@
 imprelok = """(@rel="--" or @rel="nucl")"""
 
 basicimpmod = """(node[@rel="mod" and (@lemma="maar" or @lemma="eens")])"""
 
 impmodfound = """(%basicimpmod% or node[%nonfinvc% and %basicimpmod%])"""
 nonfincat = """(@cat="inf" or @cat="ppart")"""
 
+
 nonfinvc = """(@rel="vc" and %nonfincat%) """
 
 realcomplormodnode = """node[%realcomplormod%]"""
 realcomplormod = """(not(%particlesvp%) and (not(%indexnode%) or %includeindexnode%) and not(%nonfinvc%) and not(@rel="hd"))"""
 indexnode = """(@index and not (@cat or @pt or @pos))"""
+indexnodecount = """(count(node[%indexnode%]))"""
 includeindexnode = """(%indexnode% and  parent::node[@cat="ssub" and parent::node[@cat="rel" ]])"""
 suindexnode = """(%indexnode% and @rel="su") """
 nonfinindexnode = """(%indexnode% and parent::node[%nonfinvc%])"""
+nonsuindexnode = """(%indexnode% and @rel!="su") """
+nonsuindexnodecount = """(count(node[%nonsuindexnode%]))"""
 
 fillednode = """node[not(%indexnode%)]"""
 
 particlesvp = """(@rel="svp" and @pt="vz")"""
 
 realcomplormodnodecount = """count(%realcomplormodnode% | node[%nonfinvc%]/%realcomplormodnode%)"""
 
 wx = """(%basicimperative%
         and  %realcomplormodnodecount% <= 1)"""
 
 
 wxy = """(%basicimperative%
-        and  %realcomplormodnodecount% = 2)"""
+        and  %realcomplormodnodecount% = 2) and not(node[%Tarsp_kijkVU%])"""
 
 
 wxyz = """(%basicimperative%
         and  %realcomplormodnodecount% = 3)"""
 
 
 wxyz5 = """(%basicimperative%
@@ -108,17 +112,25 @@
 
 Tarsp_OndB = """(%Ond% and  node[%Tarsp_Basic_B%]  and count(node) = 2)"""	
 
 Tarsp_OndVC = """(%Ond% and  node[%Tarsp_Basic_VC%]  and count(node) = 2) """
 
 Tarsp_OndBVC = """(%Ond% and node[%Tarsp_Basic_B%]  and node[%Tarsp_Basic_VC%]  and count(node) = 3) """
 
-Tarsp_OndW = """(%declarative% and %Ond% and  (%Tarsp_W%  or node[%Tarsp_onlyWinVC%]) and %realcomplormodnodecount% = 1 )"""
+Tarsp_OndW = """(%declarative% and %Ond% and  
+                ((%Tarsp_W%  and node[%Tarsp_onlyWinVC%]) or 
+				 (%Tarsp_W% and not(node[@rel="vc"])) or 
+				 (not(node[%Tarsp_W%]) and node[%Tarsp_onlyWinVC%]) 
+				) and 
+                 (%realcomplormodnodecount% + %indexnodecount% = 1) and 
+                (@rel!="dp" or (count(descendant::node[%realwordnode%]) = count(ancestor::node[@cat="top"]/descendant::node[%realwordnode%]) ) )
+				
+				)"""
 
-Tarsp_onlyWinVC = """(@rel="vc" and node[@rel="hd" and @pt="ww" and %realcomplormodnodecount% = 0])"""
+Tarsp_onlyWinVC = """(@rel="vc" and node[@rel="hd" and @pt="ww"] and (%realcomplormodnodecount% + %nonsuindexnodecount% = 0) )"""
 
 
 Tarsp_OndWB = """(%declarative% and %Ond% and  %Tarsp_W% and %Tarsp_B_X%  and %realcomplormodnodecount% = 2 )"""
 
 Tarsp_BasicVCW = """(node[@pt="ww" and @rel="hd"] and node[%Tarsp_Basic_VC%] and count(%fillednode%)=2)"""
 
 Tarsp_VCW_X = """(%Tarsp_BasicVCW% or (node[%nonfinvc% and %Tarsp_BasicVCW%] and count(node)=1) )""" 
@@ -196,27 +208,85 @@
 				not(%Tarsp_OndVC%) and
 				%realcomplormodnodecount% = 2) """
 
 
 onlywordinutt = """(ancestor::node[@cat="top" and count(.//node[@pt])=1] )"""
 
 Tarsp_kijkVU_old = """(@pt="ww" and @lemma="kijken" and @wvorm="pv" and @pvagr="ev" and @pvtijd="tgw" and count(ancestor::node[@cat="top"]/descendant::node[@pt!="let"])<=2)"""
-Tarsp_kijkVU = """(@pt="ww" and @lemma="kijken" and @wvorm="pv" and @pvagr="ev" and @pvtijd="tgw" and not(../node[%Tarsp_pporvc%]))"""
+Tarsp_kijkVU_old2 = """(@pt="ww" and @lemma="kijken" and @wvorm="pv" and @pvagr="ev" and @pvtijd="tgw" and not(../node[%Tarsp_pporvc%]))"""
+Tarsp_kijkVU1 = """(@pt="ww" and @lemma="kijken" and (( @wvorm="pv" and @pvagr="ev" and @pvtijd="tgw") or @word = "kijke" or @word = "kij") and not(../node[@rel="vc" or @rel="su" or @cat="pp" or @lemma="maar" or @lemma="eens" or @lemma="dan" or @lemma="nou"])) """
+Tarsp_kijkVU2 = """(@lemma = "kijk" and (@pt="bw" or @pt="n")) """
+Tarsp_kijkVU3 = """(@pt="ww" and @lemma="kijken" and @wvorm="pv" and @pvagr="ev" and @pvtijd="tgw" and ../node[@rel="mod" and (@lemma="eens" or @lemma="hier")] and 
+                   (parent::node[count(node) = 2] or (parent::node[count(node) = 3] and ../node[@rel="obj1"]))  
+				   ) """
+Tarsp_kijkVU = """( %Tarsp_kijkVU1% or %Tarsp_kijkVU2% or %Tarsp_kijkVU3%)"""
 
 Tarsp_pporvc = """ (((@rel="pc" or @rel="mod" or @rel="ld") and @cat="pp")  or @rel="vc")"""
 
 Tarsp_coreW = """ ( @pt="ww" and (@wvorm="pv" or parent::node[@rel!="vc"] or %Tarsp_BarenonfinW%) and 
         not(%Tarsp_kijkVU%) and
         not((@lemma="zijn" or @lemma="worden") and 
             parent::node[node[@rel="vc"]]) )"""
 
 Tarsp_BarenonfinW = """parent::node[@rel="vc" and  parent::node[@cat="smain" and count(node)=1]]"""
 
-Tarsp_Hwwi = """(( @pt="ww" and @rel="hd" and @wvorm="pv" and
-                  %Tarsp_hww% and
-                  ((parent::node[node[@cat="inf"and @rel="vc"]]) or
-                   (parent::node[node[@pt="ww" and @rel="vc" and @wvorm="inf"]])
-                  )
-       ) or
-	   %robusthwwi%   )"""
+Tarsp_coreHwwi = """ ( @pt="ww" and @rel="hd" and @wvorm="pv" and
+                       %Tarsp_hww% and
+                       ((parent::node[node[@cat="inf"and @rel="vc" and node[@rel="hd" and @pt="ww"]]]) or
+                        (parent::node[node[@pt="ww" and @rel="vc" and @wvorm="inf"]])
+                       )
+                     )
+"""
+
+Tarsp_Hwwi = """( %Tarsp_coreHwwi% or
+	              %robusthwwi%  
+	            )"""
+				
+
+robusthwwi = """((not(%Tarsp_coreHwwi%) and @pt="ww" and %Tarsp_hww% and @wvorm="pv" and ancestor::node[@cat="top" and descendant::node[@pt="ww" and @wvorm="inf" ]]))
+				
+			 """
+
+oldrobusthwwi = """ (@cat="top" and 
+                  .//node[@pt="ww" and %Tarsp_hww% and @wvorm="pv" and (@rel="--" or @rel="dp")] and
+				  .//node[@pt="ww" and @wvorm="inf" and (@rel="--" or @rel="dp")]
+				  )
+				  
+"""
+				
 	   
-Tarsp_hehe = """ (@lemma="hè" and @end = ancestor::node[@cat="top"]/descendant::node[@lemma="hè"]/@begin)"""
+Tarsp_hehe = """ (@lemma="hè" and @end = ancestor::node[@cat="top"]/descendant::node[@lemma="hè"]/@begin)"""
+
+simplevcw = """
+( node[@rel="hd" and @pt="ww" and not(%Tarsp_kijkVU%)] and
+  node[%Tarsp_Basic_VC%] and
+  count(node) = 2
+)
+"""
+
+vcvcw = """
+(node[@rel="vc" and @cat="inf" and %simplevcw%] and
+ count(node) = 1
+)
+"""
+
+suvcw = """
+( node[@rel="su"] and
+  node[@rel="vc" and @cat="inf" and node[@rel="su"] and node[@rel="hd" and @pt="ww"] and count(node)=2]
+  and count(node) =2
+)
+"""
+
+Tarsp_vcw = """
+( (@rel="--" or @rel="nucl")  and (count(descendant::node[%realwordnode%]) = count(ancestor::node[@cat="top"]/descendant::node[%realwordnode%]) ) and
+ ( %simplevcw% or
+   %vcvcw%    
+ )
+)
+"""
+
+realwordnode = """ ((@pt="ww" or @pt="n" or @pt="adj" or @pt="bw" or @pt="vz" or @pt="vg") and not(%Tarsp_kijkVU%))
+"""
+
+horenaux = """(@lemma="horen" and 
+               @pt="ww" and 
+			   ../node[@rel="ld" or @rel="mod"] and not(../node[@rel="obj1" or @rel="vc"]))"""
```

### Comparing `sastadev-0.1.5/src/sastadev/data/macros/sastamacros1.txt` & `sastadev-0.2.0/src/sastadev/data/macros/sastamacros1.txt`

 * *Files 2% similar despite different names*

```diff
@@ -164,1159 +164,1284 @@
 00000a30: 0d0a 2020 406c 656d 6d61 203d 2022 626c  ..  @lemma = "bl
 00000a40: 696a 7665 6e22 206f 720d 0a20 2040 6c65  ijven" or..  @le
 00000a50: 6d6d 6120 3d20 2277 696c 6c65 6e22 206f  mma = "willen" o
 00000a60: 720d 0a20 2040 6c65 6d6d 6120 3d20 227a  r..  @lemma = "z
 00000a70: 756c 6c65 6e22 206f 7220 2020 0d0a 2020  ullen" or   ..  
 00000a80: 406c 656d 6d61 203d 2022 646f 656e 2220  @lemma = "doen" 
 00000a90: 6f72 0d0a 2020 406c 656d 6d61 203d 2022  or..  @lemma = "
-00000aa0: 6761 616e 2220 6f72 0d0a 2020 406c 656d  gaan" or..  @lem
-00000ab0: 6d61 203d 2022 686f 7265 6e22 206f 720d  ma = "horen" or.
-00000ac0: 0a20 2040 6c65 6d6d 6120 3d20 226b 6f6d  .  @lemma = "kom
-00000ad0: 656e 2220 6f72 0d0a 2020 406c 656d 6d61  en" or..  @lemma
-00000ae0: 203d 2022 6c61 7465 6e22 206f 720d 0a20   = "laten" or.. 
-00000af0: 2040 6c65 6d6d 6120 3d20 226c 6967 6765   @lemma = "ligge
-00000b00: 6e22 206f 720d 0a20 2040 6c65 6d6d 6120  n" or..  @lemma 
-00000b10: 3d20 226c 6f70 656e 2220 6f72 0d0a 2020  = "lopen" or..  
-00000b20: 406c 656d 6d61 203d 2022 6d6f 6765 6e22  @lemma = "mogen"
-00000b30: 206f 720d 0a20 2040 6c65 6d6d 6120 3d20   or..  @lemma = 
-00000b40: 2273 7461 616e 2220 6f72 0d0a 2020 406c  "staan" or..  @l
-00000b50: 656d 6d61 203d 2022 7a69 7474 656e 2229  emma = "zitten")
-00000b60: 0d0a 2022 2222 0d0a 200d 0a54 6172 7370  .. """.. ..Tarsp
-00000b70: 5f76 635f 7369 626c 696e 6720 3d20 2222  _vc_sibling = ""
-00000b80: 2270 6172 656e 743a 3a6e 6f64 655b 206e  "parent::node[ n
-00000b90: 6f64 655b 4072 656c 3d22 7663 2220 616e  ode[@rel="vc" an
-00000ba0: 6420 6e6f 6465 5b40 7265 6c3d 2268 6422  d node[@rel="hd"
-00000bb0: 5d5d 5d22 2222 0d0a 5461 7273 705f 7072  ]]]"""..Tarsp_pr
-00000bc0: 6564 635f 7369 626c 696e 6720 3d20 2222  edc_sibling = ""
-00000bd0: 2270 6172 656e 743a 3a6e 6f64 655b 206e  "parent::node[ n
-00000be0: 6f64 655b 4072 656c 3d22 7072 6564 6322  ode[@rel="predc"
-00000bf0: 5d5d 2222 220d 0a54 6172 7370 5f6f 626a  ]]"""..Tarsp_obj
-00000c00: 315f 7369 626c 696e 6720 3d20 2222 2270  1_sibling = """p
-00000c10: 6172 656e 743a 3a6e 6f64 655b 206e 6f64  arent::node[ nod
-00000c20: 655b 4072 656c 3d22 6f62 6a31 225d 5d22  e[@rel="obj1"]]"
-00000c30: 2222 0d0a 5461 7273 705f 6c64 5f73 6962  ""..Tarsp_ld_sib
-00000c40: 6c69 6e67 203d 2022 2222 7061 7265 6e74  ling = """parent
-00000c50: 3a3a 6e6f 6465 5b20 6e6f 6465 5b40 7265  ::node[ node[@re
-00000c60: 6c3d 226c 6422 5d5d 2222 220d 0a54 6172  l="ld"]]"""..Tar
-00000c70: 7370 5f6f 6e6c 796d 6f64 525f 7369 626c  sp_onlymodR_sibl
-00000c80: 696e 6720 3d20 2222 2228 7061 7265 6e74  ing = """(parent
-00000c90: 3a3a 6e6f 6465 5b6e 6f64 655b 4072 656c  ::node[node[@rel
-00000ca0: 3d22 6d6f 6422 2061 6e64 2025 5270 726f  ="mod" and %Rpro
-00000cb0: 6e6f 756e 255d 2061 6e64 206e 6f74 286e  noun%] and not(n
-00000cc0: 6f64 655b 4072 656c 3d22 7072 6564 6322  ode[@rel="predc"
-00000cd0: 5d29 5d29 2222 220d 0a0d 0a54 6172 7370  ])])"""....Tarsp
-00000ce0: 5f48 7777 5a20 3d20 2222 2228 4070 743d  _HwwZ = """(@pt=
-00000cf0: 2277 7722 2061 6e64 2040 7265 6c3d 2268  "ww" and @rel="h
-00000d00: 6422 2061 6e64 2040 7776 6f72 6d3d 2270  d" and @wvorm="p
-00000d10: 7622 2061 6e64 2040 7076 6167 7221 3d22  v" and @pvagr!="
-00000d20: 6d76 2220 616e 6420 4070 7674 696a 6421  mv" and @pvtijd!
-00000d30: 3d22 7665 726c 2220 616e 640d 0a20 2828  ="verl" and.. ((
-00000d40: 0d0a 2020 2025 5461 7273 705f 6877 7725  ..   %Tarsp_hww%
-00000d50: 206f 720d 0a20 2020 406c 656d 6d61 203d   or..   @lemma =
-00000d60: 2022 6865 6262 656e 2220 0d0a 2020 2029   "hebben" ..   )
-00000d70: 2061 6e64 200d 0a20 2020 6e6f 7428 2554   and ..   not(%T
-00000d80: 6172 7370 5f76 635f 7369 626c 696e 6725  arsp_vc_sibling%
-00000d90: 2929 206f 720d 0a20 2020 2840 6c65 6d6d  )) or..   (@lemm
-00000da0: 613d 227a 696a 6e22 2061 6e64 206e 6f74  a="zijn" and not
-00000db0: 2825 5461 7273 705f 7663 5f73 6962 6c69  (%Tarsp_vc_sibli
-00000dc0: 6e67 2529 2061 6e64 2025 5461 7273 705f  ng%) and %Tarsp_
-00000dd0: 6c64 5f73 6962 6c69 6e67 2520 290d 0a0d  ld_sibling% )...
-00000de0: 0a20 290d 0a22 2222 0d0a 0d0a 7664 6877  . ).."""....vdhw
-00000df0: 7773 203d 2022 2222 2840 6c65 6d6d 613d  ws = """(@lemma=
-00000e00: 2268 6562 6265 6e22 206f 7220 406c 656d  "hebben" or @lem
-00000e10: 6d61 3d22 7a69 6a6e 2220 6f72 2040 6c65  ma="zijn" or @le
-00000e20: 6d6d 613d 2277 6f72 6465 6e22 290d 0a22  mma="worden").."
-00000e30: 2222 0d0a 0d0a 5461 7273 705f 4b6f 7020  ""....Tarsp_Kop 
-00000e40: 3d20 2222 220d 0a20 2820 2020 4070 743d  = """.. (   @pt=
-00000e50: 2277 7722 2061 6e64 2040 7265 6c3d 2268  "ww" and @rel="h
-00000e60: 6422 2061 6e64 206e 6f74 2825 5461 7273  d" and not(%Tars
-00000e70: 705f 6877 7725 2920 616e 640d 0a0d 0a20  p_hww%) and.... 
-00000e80: 2020 2028 2825 5461 7273 705f 7072 6564     ((%Tarsp_pred
-00000e90: 635f 7369 626c 696e 6725 2061 6e64 206e  c_sibling% and n
-00000ea0: 6f74 2825 5461 7273 705f 6f62 6a31 5f73  ot(%Tarsp_obj1_s
-00000eb0: 6962 6c69 6e67 2529 2920 6f72 0d0a 0d0a  ibling%)) or....
-00000ec0: 2020 2020 2028 406c 656d 6d61 3d22 7a69       (@lemma="zi
-00000ed0: 6a6e 2220 616e 6420 6e6f 7428 2554 6172  jn" and not(%Tar
-00000ee0: 7370 5f76 635f 7369 626c 696e 6725 2920  sp_vc_sibling%) 
-00000ef0: 616e 6420 6e6f 7428 2554 6172 7370 5f6c  and not(%Tarsp_l
-00000f00: 645f 7369 626c 696e 6725 2920 616e 6420  d_sibling%) and 
-00000f10: 6e6f 7428 2554 6172 7370 5f6f 6e6c 796d  not(%Tarsp_onlym
-00000f20: 6f64 525f 7369 626c 696e 6725 2929 0d0a  odR_sibling%))..
-00000f30: 2020 2020 290d 0a20 290d 0a22 2222 0d0a      ).. ).."""..
-00000f40: 0d0a 726f 6275 7374 6877 7769 203d 2022  ..robusthwwi = "
-00000f50: 2222 2028 4063 6174 3d22 746f 7022 2061  "" (@cat="top" a
-00000f60: 6e64 200d 0a20 2020 2020 2020 2020 2020  nd ..           
-00000f70: 2020 2020 2020 202e 2f2f 6e6f 6465 5b40         .//node[@
-00000f80: 7074 3d22 7777 2220 616e 6420 2554 6172  pt="ww" and %Tar
-00000f90: 7370 5f68 7777 2520 616e 6420 4077 766f  sp_hww% and @wvo
-00000fa0: 726d 3d22 7076 2220 616e 6420 2840 7265  rm="pv" and (@re
-00000fb0: 6c3d 222d 2d22 206f 7220 4072 656c 3d22  l="--" or @rel="
-00000fc0: 6470 2229 5d20 616e 640d 0a09 0909 0920  dp")] and...... 
-00000fd0: 202e 2f2f 6e6f 6465 5b40 7074 3d22 7777   .//node[@pt="ww
-00000fe0: 2220 616e 6420 4077 766f 726d 3d22 696e  " and @wvorm="in
-00000ff0: 6622 2061 6e64 2028 4072 656c 3d22 2d2d  f" and (@rel="--
-00001000: 2220 6f72 2040 7265 6c3d 2264 7022 295d  " or @rel="dp")]
-00001010: 0d0a 0909 0909 2020 290d 0a09 0909 0920  ......  )...... 
-00001020: 200d 0a22 2222 0d0a 0d0a 726f 6275 7374   .."""....robust
-00001030: 6877 7776 6420 3d20 2222 2220 2840 6361  hwwvd = """ (@ca
-00001040: 743d 2274 6f70 2220 616e 6420 0d0a 2020  t="top" and ..  
-00001050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001060: 2e2f 2f6e 6f64 655b 4070 743d 2277 7722  .//node[@pt="ww"
-00001070: 2061 6e64 2025 7664 6877 7773 2520 616e   and %vdhwws% an
-00001080: 6420 4077 766f 726d 3d22 7076 2220 616e  d @wvorm="pv" an
-00001090: 6420 2840 7265 6c3d 222d 2d22 206f 7220  d (@rel="--" or 
-000010a0: 4072 656c 3d22 6470 2229 5d20 616e 640d  @rel="dp")] and.
-000010b0: 0a09 0909 0920 202e 2f2f 6e6f 6465 5b40  .....  .//node[@
-000010c0: 7074 3d22 7777 2220 616e 6420 4077 766f  pt="ww" and @wvo
-000010d0: 726d 3d22 7664 2220 616e 6420 2840 7265  rm="vd" and (@re
-000010e0: 6c3d 222d 2d22 206f 7220 4072 656c 3d22  l="--" or @rel="
-000010f0: 6470 2229 5d0d 0a09 0909 0920 2029 0d0a  dp")]......  )..
-00001100: 0909 0909 2020 0d0a 2222 220d 0a0d 0a0d  ....  ..""".....
-00001110: 0a72 6f62 7573 7469 6e76 6572 7369 6f6e  .robustinversion
-00001120: 203d 2022 2222 2840 6361 743d 2274 6f70   = """(@cat="top
-00001130: 2220 616e 6420 0d0a 2020 2020 2020 202e  " and ..       .
-00001140: 2f2f 6e6f 6465 5b40 7074 3d22 7777 2220  //node[@pt="ww" 
-00001150: 2061 6e64 2040 7776 6f72 6d3d 2270 7622   and @wvorm="pv"
-00001160: 2061 6e64 2020 4072 656c 213d 2268 6422   and  @rel!="hd"
-00001170: 2061 6e64 2028 6e6f 7428 4073 7479 7065   and (not(@stype
-00001180: 2920 6f72 2040 7374 7970 6521 3d22 696d  ) or @stype!="im
-00001190: 7061 7261 7469 7665 2229 5d20 616e 6420  parative")] and 
-000011a0: 0d0a 2020 2020 2020 202e 2f2f 6e6f 6465  ..       .//node
-000011b0: 5b40 7074 3d22 766e 7722 2061 6e64 2040  [@pt="vnw" and @
-000011c0: 6e61 616d 7661 6c3d 226e 6f6d 696e 2220  naamval="nomin" 
-000011d0: 616e 6420 4072 656c 213d 2273 7522 2061  and @rel!="su" a
-000011e0: 6e64 0d0a 2020 2020 2020 2020 2020 2020  nd..            
-000011f0: 2020 2040 656e 643e 2e2e 2f2f 6e6f 6465     @end>..//node
-00001200: 5b40 7074 3d22 7777 2220 616e 6420 4077  [@pt="ww" and @w
-00001210: 766f 726d 3d22 7076 225d 2f40 656e 645d  vorm="pv"]/@end]
-00001220: 290d 0a09 0909 2020 2022 2222 0d0a 0d0a  ).....   """....
-00001230: 6c6f 6376 6572 6220 3d20 2222 2228 406c  locverb = """(@l
-00001240: 656d 6d61 3d22 7374 6161 6e22 206f 7220  emma="staan" or 
-00001250: 406c 656d 6d61 3d22 7a69 7474 656e 2220  @lemma="zitten" 
-00001260: 6f72 2040 6c65 6d6d 613d 2272 696a 6465  or @lemma="rijde
-00001270: 6e22 206f 7220 406c 656d 6d61 3d22 7661  n" or @lemma="va
-00001280: 6c6c 656e 2220 6f72 2040 6c65 6d6d 613d  llen" or @lemma=
-00001290: 2264 6f65 6e22 206f 7220 406c 656d 6d61  "doen" or @lemma
-000012a0: 3d22 6761 616e 2220 6f72 2040 6c65 6d6d  ="gaan" or @lemm
-000012b0: 613d 226b 6f6d 656e 2220 6f72 2040 6c65  a="komen" or @le
-000012c0: 6d6d 613d 227a 696a 6e22 2020 6f72 2025  mma="zijn"  or %
-000012d0: 6c6f 636d 6f64 616c 7665 7262 2520 290d  locmodalverb% ).
-000012e0: 0a22 2222 0d0a 0d0a 6c6f 636d 6f64 616c  ."""....locmodal
-000012f0: 7665 7262 203d 2022 2222 2028 406c 656d  verb = """ (@lem
-00001300: 6d61 3d22 6b75 6e6e 656e 2220 6f72 2040  ma="kunnen" or @
-00001310: 6c65 6d6d 613d 226d 6f65 7465 6e22 206f  lemma="moeten" o
-00001320: 7220 406c 656d 6d61 3d22 686f 6576 656e  r @lemma="hoeven
-00001330: 2220 6f72 2040 6c65 6d6d 613d 2277 696c  " or @lemma="wil
-00001340: 6c65 6e22 206f 7220 406c 656d 6d61 3d22  len" or @lemma="
-00001350: 6d6f 6765 6e22 2922 2222 0d0a 0d0a 0d0a  mogen")"""......
-00001360: 6164 6a6f 7261 6476 203d 2022 2222 2840  adjoradv = """(@
-00001370: 7074 3d22 6277 2220 6f72 2040 7074 3d22  pt="bw" or @pt="
-00001380: 6164 6a22 206f 7220 2840 7074 3d22 766e  adj" or (@pt="vn
-00001390: 7722 2061 6e64 2028 4070 6f73 3d22 6164  w" and (@pos="ad
-000013a0: 6a22 206f 7220 4070 6f73 3d22 6164 7622  j" or @pos="adv"
-000013b0: 2929 2922 2222 0d0a 0d0a 6164 6a61 6476  )))"""....adjadv
-000013c0: 203d 2022 2222 0d0a 2840 7074 3d27 6164   = """..(@pt='ad
-000013d0: 6a27 2061 6e64 2028 406c 656d 6d61 3d27  j' and (@lemma='
-000013e0: 7765 6c27 2929 0d0a 2222 220d 0a0d 0a0d  wel'))..""".....
-000013f0: 0a72 6561 6c6e 6f64 6520 3d20 2222 2228  .realnode = """(
-00001400: 286e 6f74 2840 7074 2920 6f72 2028 4070  (not(@pt) or (@p
-00001410: 7421 3d22 6c65 7422 2061 6e64 2040 7074  t!="let" and @pt
-00001420: 213d 2274 7377 2229 2920 616e 6420 286e  !="tsw")) and (n
-00001430: 6f74 2840 706f 7374 6167 2920 6f72 2040  ot(@postag) or @
-00001440: 706f 7374 6167 213d 224e 4128 2922 2929  postag!="NA()"))
-00001450: 2222 220d 0a6e 6f74 6f6e 6c79 7265 616c  """..notonlyreal
-00001460: 6e6f 6465 203d 2022 2222 2870 6172 656e  node = """(paren
-00001470: 743a 3a6e 6f64 655b 636f 756e 7428 6e6f  t::node[count(no
-00001480: 6465 5b25 7265 616c 6e6f 6465 255d 293e  de[%realnode%])>
-00001490: 315d 2922 2222 0d0a 0d0a 5270 726f 6e6f  1])"""....Rprono
-000014a0: 756e 203d 2022 2222 2840 7074 3d27 766e  un = """(@pt='vn
-000014b0: 7727 2061 6e64 2028 406c 656d 6d61 3d27  w' and (@lemma='
-000014c0: 6572 2720 6f72 2040 6c65 6d6d 613d 2768  er' or @lemma='h
-000014d0: 6965 7227 206f 7220 406c 656d 6d61 3d27  ier' or @lemma='
-000014e0: 6461 6172 2720 6f72 2040 6c65 6d6d 613d  daar' or @lemma=
-000014f0: 2777 6161 7227 206f 7220 406c 656d 6d61  'waar' or @lemma
-00001500: 3d27 6572 6765 6e73 2720 6f72 2040 6c65  ='ergens' or @le
-00001510: 6d6d 613d 276e 6572 6765 6e73 2720 6f72  mma='nergens' or
-00001520: 2040 6c65 6d6d 613d 276f 7665 7261 6c27   @lemma='overal'
-00001530: 2929 0d0a 2222 220d 0a0d 0a70 7620 3d20  )).."""....pv = 
-00001540: 2222 2228 4070 743d 2277 7722 2061 6e64  """(@pt="ww" and
-00001550: 2040 7776 6f72 6d3d 2270 7622 2029 2222   @wvorm="pv" )""
-00001560: 220d 0a0d 0a62 786e 7031 203d 2022 2222  "....bxnp1 = """
-00001570: 2840 6361 743d 226e 7022 2061 6e64 2063  (@cat="np" and c
-00001580: 6f75 6e74 286e 6f64 6529 3d32 2061 6e64  ount(node)=2 and
-00001590: 206e 6f64 655b 4072 656c 3d22 6864 2220   node[@rel="hd" 
-000015a0: 616e 6420 4070 743d 2277 7722 5d20 616e  and @pt="ww"] an
-000015b0: 6420 6e6f 6465 5b40 7265 6c3d 226d 6f64  d node[@rel="mod
-000015c0: 2220 616e 6420 4070 745d 2922 2222 0d0a  " and @pt])"""..
-000015d0: 6278 6e70 3220 3d20 2222 2228 4063 6174  bxnp2 = """(@cat
-000015e0: 3d22 6e70 2220 616e 6420 636f 756e 7428  ="np" and count(
-000015f0: 6e6f 6465 293d 3220 616e 6420 6e6f 6465  node)=2 and node
-00001600: 5b40 7265 6c3d 2268 6422 5d20 616e 6420  [@rel="hd"] and 
-00001610: 6e6f 6465 5b40 7265 6c3d 226d 6f64 2220  node[@rel="mod" 
-00001620: 616e 6420 2573 696e 676c 6577 6f72 6462  and %singlewordb
-00001630: 7725 5d29 2222 220d 0a0d 0a54 6172 7370  w%])"""....Tarsp
-00001640: 5f42 6173 6963 5f56 4320 3d20 2222 2228  _Basic_VC = """(
-00001650: 2840 7265 6c3d 226f 626a 3122 206f 7220  (@rel="obj1" or 
-00001660: 4072 656c 3d22 7063 2220 206f 7220 4072  @rel="pc"  or @r
-00001670: 656c 3d22 7072 6564 6322 206f 7220 4072  el="predc" or @r
-00001680: 656c 3d22 6c64 2220 6f72 2040 7265 6c3d  el="ld" or @rel=
-00001690: 226f 626a 3222 206f 7220 2554 6172 7370  "obj2" or %Tarsp
-000016a0: 5f66 696e 7663 2520 6f72 2025 5461 7273  _finvc% or %Tars
-000016b0: 705f 7663 766e 7725 206f 7220 2840 7265  p_vcvnw% or (@re
-000016c0: 6c3d 2273 7670 2220 616e 6420 4070 7421  l="svp" and @pt!
-000016d0: 3d22 767a 2229 2920 616e 6420 6e6f 7428  ="vz")) and not(
-000016e0: 2554 6172 7370 5f42 6173 6963 5f42 2529  %Tarsp_Basic_B%)
-000016f0: 2029 2222 220d 0a0d 0a0d 0a54 6172 7370   )"""......Tarsp
-00001700: 5f42 6173 6963 5f42 203d 2022 2222 2840  _Basic_B = """(@
-00001710: 7265 6c3d 226d 6f64 2220 6f72 2040 7265  rel="mod" or @re
-00001720: 6c3d 226c 6422 206f 7220 4072 656c 3d22  l="ld" or @rel="
-00001730: 7072 6564 6d22 2020 6f72 2025 5461 7273  predm"  or %Tars
-00001740: 705f 425f 7072 6564 6325 2920 2222 220d  p_B_predc%) """.
-00001750: 0a0d 0a54 6172 7370 5f42 5f70 7265 6463  ...Tarsp_B_predc
-00001760: 203d 2022 2222 2840 7265 6c3d 7072 6564   = """(@rel=pred
-00001770: 6320 616e 6420 2840 7074 3d22 767a 2220  c and (@pt="vz" 
-00001780: 6f72 2040 7074 3d22 6277 2220 6f72 2040  or @pt="bw" or @
-00001790: 6361 743d 2270 7022 206f 7220 4063 6174  cat="pp" or @cat
-000017a0: 3d22 6164 7670 2220 6f72 2025 5270 726f  ="advp" or %Rpro
-000017b0: 6e6f 756e 2529 2922 2222 0d0a 0d0a 5461  noun%))"""....Ta
-000017c0: 7273 705f 4220 3d20 2222 2228 0d0a 2020  rsp_B = """(..  
-000017d0: 2020 2020 2028 2828 2840 7265 6c3d 226d       ((((@rel="m
-000017e0: 6f64 2220 6f72 2040 7265 6c3d 226c 6422  od" or @rel="ld"
-000017f0: 206f 7220 4072 656c 3d22 7072 6564 6d22   or @rel="predm"
-00001800: 2920 616e 640d 0a20 2020 2020 2020 2020  ) and..         
-00001810: 2028 6e6f 7428 4063 6174 2920 6f72 2040   (not(@cat) or @
-00001820: 6361 7421 3d22 636f 6e6a 2229 2061 6e64  cat!="conj") and
-00001830: 0d0a 0909 2020 286e 6f74 2840 7074 2920  ....  (not(@pt) 
-00001840: 6f72 2040 7074 213d 2274 7377 2229 0d0a  or @pt!="tsw")..
-00001850: 2020 2020 2020 2020 2029 6f72 200d 0a20           )or .. 
-00001860: 2020 2020 2020 2020 2825 7072 6564 6342          (%predcB
-00001870: 250d 0a20 2020 2020 2020 2020 290d 0a20  %..         ).. 
-00001880: 2020 2020 2020 2020 2920 616e 6420 0d0a          ) and ..
-00001890: 2020 2020 2020 2020 2028 2e2e 2f6e 6f64           (../nod
-000018a0: 655b 4070 743d 2277 7722 2061 6e64 2040  e[@pt="ww" and @
-000018b0: 7265 6c3d 2268 6422 5d29 0d0a 2020 2020  rel="hd"])..    
-000018c0: 2020 2020 2920 6f72 0d0a 2020 2020 2020      ) or..      
-000018d0: 2020 2828 4070 743d 2276 7a22 206f 7220    ((@pt="vz" or 
-000018e0: 4070 743d 2262 7722 206f 7220 2552 7072  @pt="bw" or %Rpr
-000018f0: 6f6e 6f75 6e25 2920 616e 6420 2840 7265  onoun%) and (@re
-00001900: 6c3d 2264 7022 206f 7220 4072 656c 3d22  l="dp" or @rel="
-00001910: 2d2d 2220 6f72 2040 7265 6c3d 226e 7563  --" or @rel="nuc
-00001920: 6c22 206f 7220 4072 656c 3d22 626f 6479  l" or @rel="body
-00001930: 2229 2061 6e64 2025 6e6f 746f 6e6c 7972  ") and %notonlyr
-00001940: 6561 6c6e 6f64 6525 2920 6f72 0d0a 2020  ealnode%) or..  
-00001950: 2020 2020 2020 2840 6361 743d 2270 7022        (@cat="pp"
-00001960: 2061 6e64 2028 4072 656c 3d22 2d2d 2220   and (@rel="--" 
-00001970: 6f72 2040 7265 6c3d 2264 7022 2920 616e  or @rel="dp") an
-00001980: 6420 256e 6f74 6f6e 6c79 7265 616c 6e6f  d %notonlyrealno
-00001990: 6465 2529 206f 720d 0a09 0928 4072 656c  de%) or....(@rel
-000019a0: 3d22 7063 2220 616e 6420 2e2e 2f6e 6f64  ="pc" and ../nod
-000019b0: 655b 4072 656c 3d22 6864 2220 616e 6420  e[@rel="hd" and 
-000019c0: 256c 6f63 7665 7262 255d 2920 6f72 0d0a  %locverb%]) or..
-000019d0: 2020 2020 2020 2020 2840 7265 6c3d 2263          (@rel="c
-000019e0: 6e6a 2220 616e 6420 7061 7265 6e74 3a3a  nj" and parent::
-000019f0: 6e6f 6465 5b40 7265 6c3d 226d 6f64 2220  node[@rel="mod" 
-00001a00: 6f72 2040 7265 6c3d 226c 6422 206f 7220  or @rel="ld" or 
-00001a10: 4072 656c 3d22 7072 6564 6d22 5d29 206f  @rel="predm"]) o
-00001a20: 720d 0a20 2020 2020 2020 2028 4072 656c  r..        (@rel
-00001a30: 3d22 6d6f 6422 2061 6e64 2040 7074 3d22  ="mod" and @pt="
-00001a40: 6277 2220 616e 6420 7061 7265 6e74 3a3a  bw" and parent::
-00001a50: 6e6f 6465 5b40 6361 743d 226e 7022 5d20  node[@cat="np"] 
-00001a60: 2920 6f72 0d0a 0909 2554 6172 7370 5f6e  ) or....%Tarsp_n
-00001a70: 6f6e 6d6f 6461 6476 6370 2520 6f72 0d0a  onmodadvcp% or..
-00001a80: 0909 2554 6172 7370 5f70 635f 7663 5f65  ..%Tarsp_pc_vc_e
-00001a90: 7863 6570 7469 6f6e 250d 0a09 0929 0d0a  xception%....)..
-00001aa0: 2020 2020 200d 0a22 2222 0d0a 0d0a 636f       .."""....co
-00001ab0: 6d70 6c65 6d65 6e74 203d 2022 2222 2828  mplement = """((
-00001ac0: 4072 656c 3d22 6f62 6a31 2220 6f72 2040  @rel="obj1" or @
-00001ad0: 7265 6c3d 226f 626a 3222 2920 6f72 200d  rel="obj2") or .
-00001ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001af0: 2020 2840 7265 6c3d 2270 7265 6463 2220    (@rel="predc" 
-00001b00: 616e 6420 6e6f 7428 2570 7265 6463 4225  and not(%predcB%
-00001b10: 2929 206f 720d 0a09 0920 2020 2020 2020  )) or....       
-00001b20: 2020 2840 7265 6c3d 2270 6f62 6a31 2220    (@rel="pobj1" 
-00001b30: 616e 6420 6e6f 7428 2570 6f62 6a31 4225  and not(%pobj1B%
-00001b40: 2920 2920 6f72 0d0a 0909 0909 2025 7665  ) ) or...... %ve
-00001b50: 7262 616c 636f 6d70 6c65 6d65 6e74 250d  rbalcomplement%.
-00001b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001b70: 2029 2222 220d 0a09 0909 090d 0a76 6572   )"""........ver
-00001b80: 6261 6c63 6f6d 706c 656d 656e 7420 3d20  balcomplement = 
-00001b90: 2222 2228 4072 656c 3d22 7663 2220 616e  """(@rel="vc" an
-00001ba0: 6420 2840 6361 743d 2263 7022 206f 7220  d (@cat="cp" or 
-00001bb0: 4063 6174 3d22 7768 7122 206f 7220 4063  @cat="whq" or @c
-00001bc0: 6174 3d22 7768 7375 6222 2929 2222 220d  at="whsub"))""".
-00001bd0: 0a09 0920 0d0a 7072 6564 6342 203d 2022  ... ..predcB = "
-00001be0: 2222 2840 7265 6c3d 2270 7265 6463 2220  ""(@rel="predc" 
-00001bf0: 616e 6420 0d0a 2020 2020 2020 2020 2020  and ..          
-00001c00: 2028 4070 743d 2261 646a 2220 6f72 2040   (@pt="adj" or @
-00001c10: 7074 3d22 6277 2220 6f72 2040 6361 743d  pt="bw" or @cat=
-00001c20: 2261 7022 206f 7220 4063 6174 3d22 6164  "ap" or @cat="ad
-00001c30: 7670 2229 2061 6e64 0d0a 2020 2020 2020  vp") and..      
-00001c40: 2020 2020 202e 2e2f 6e6f 6465 5b40 7265       ../node[@re
-00001c50: 6c3d 226f 626a 3122 5d0d 0a20 2020 2020  l="obj1"]..     
-00001c60: 2020 2020 2922 2222 0d0a 0909 200d 0a70      )""".... ..p
-00001c70: 6f62 6a31 4220 3d20 2222 2228 4072 656c  obj1B = """(@rel
-00001c80: 3d22 7063 2220 616e 6420 2e2e 2f6e 6f64  ="pc" and ../nod
-00001c90: 655b 4072 656c 3d22 6864 2220 616e 6420  e[@rel="hd" and 
-00001ca0: 256c 6f63 7665 7262 255d 2922 2222 0d0a  %locverb%])"""..
-00001cb0: 200d 0a0d 0a0d 0a73 696e 676c 6577 6f72   ......singlewor
-00001cc0: 6462 7720 3d20 2222 2220 2840 7074 3d22  dbw = """ (@pt="
-00001cd0: 6277 2220 6f72 2025 5270 726f 6e6f 756e  bw" or %Rpronoun
-00001ce0: 2520 6f72 2025 6164 6a61 6476 2529 0d0a  % or %adjadv%)..
-00001cf0: 2222 220d 0a0d 0a0d 0a64 6965 6461 7472  """......diedatr
-00001d00: 656c 203d 2022 2222 2840 7074 3d22 766e  el = """(@pt="vn
-00001d10: 7722 2061 6e64 2040 7677 7479 7065 3d22  w" and @vwtype="
-00001d20: 6265 7472 2220 616e 6420 4072 656c 3d22  betr" and @rel="
-00001d30: 7268 6422 2061 6e64 2028 406c 656d 6d61  rhd" and (@lemma
-00001d40: 3d22 6469 6522 206f 7220 406c 656d 6d61  ="die" or @lemma
-00001d50: 3d22 6461 7422 2929 2222 220d 0a0d 0a61  ="dat"))"""....a
-00001d60: 766e 7265 6c20 3d20 2222 2228 2564 6965  vnrel = """(%die
-00001d70: 6461 7472 656c 2520 616e 6420 7061 7265  datrel% and pare
-00001d80: 6e74 3a3a 6e6f 6465 5b40 6361 743d 2272  nt::node[@cat="r
-00001d90: 656c 2220 616e 6420 4072 656c 213d 226d  el" and @rel!="m
-00001da0: 6f64 225d 2922 2222 0d0a 0d0a 7632 7072  od"])"""....v2pr
-00001db0: 6f62 6c65 6d20 3d20 2222 222f 2f6e 6f64  oblem = """//nod
-00001dc0: 655b 4070 743d 2277 7722 2061 6e64 2040  e[@pt="ww" and @
-00001dd0: 7776 6f72 6d3d 2270 7622 2061 6e64 200d  wvorm="pv" and .
-00001de0: 0a20 2020 2020 2020 4062 6567 696e 2021  .       @begin !
-00001df0: 3d20 7061 7265 6e74 3a3a 6e6f 6465 5b40  = parent::node[@
-00001e00: 6361 743d 2273 7375 6222 5d2f 7061 7265  cat="ssub"]/pare
-00001e10: 6e74 3a3a 6e6f 6465 5b40 6361 743d 2272  nt::node[@cat="r
-00001e20: 656c 2220 616e 6420 4072 656c 213d 226d  el" and @rel!="m
-00001e30: 6f64 225d 2f6e 6f64 655b 2564 6965 6461  od"]/node[%dieda
-00001e40: 7472 656c 2520 5d2f 4065 6e64 0d0a 2020  trel% ]/@end..  
-00001e50: 2020 2020 5d22 2222 0d0a 0d0a 636f 7265      ]"""....core
-00001e60: 6176 6e20 3d20 2222 2228 4070 743d 2276  avn = """(@pt="v
-00001e70: 6e77 2220 2061 6e64 2040 7677 7479 7065  nw"  and @vwtype
-00001e80: 3d22 6161 6e77 2220 616e 6420 406c 656d  ="aanw" and @lem
-00001e90: 6d61 213d 2268 6965 7222 2061 6e64 2040  ma!="hier" and @
-00001ea0: 6c65 6d6d 6121 3d22 6461 6172 2220 616e  lemma!="daar" an
-00001eb0: 6420 406c 656d 6d61 213d 2265 7222 2061  d @lemma!="er" a
-00001ec0: 6e64 2040 7265 6c21 3d22 6465 7422 2061  nd @rel!="det" a
-00001ed0: 6e64 2028 6e6f 7428 4070 6f73 6974 6965  nd (not(@positie
-00001ee0: 2920 6f72 2040 706f 7369 7469 6521 3d22  ) or @positie!="
-00001ef0: 7072 656e 6f6d 2229 2029 2222 220d 0a0d  prenom") )"""...
-00001f00: 0a41 566e 203d 2022 2222 2825 636f 7265  .AVn = """(%core
-00001f10: 6176 6e25 206f 7220 2561 766e 7265 6c25  avn% or %avnrel%
-00001f20: 2922 2222 2220 0d0a 0d0a 636f 7265 7068  )"""" ....coreph
-00001f30: 7261 7365 203d 2022 2222 2840 6361 743d  rase = """(@cat=
-00001f40: 226e 7022 206f 7220 4063 6174 3d22 7070  "np" or @cat="pp
-00001f50: 2220 6f72 2040 6361 743d 2261 6476 7022  " or @cat="advp"
-00001f60: 206f 7220 4063 6174 3d22 6170 2229 2222   or @cat="ap")""
-00001f70: 220d 0a0d 0a63 6f72 6542 5820 3d20 2222  "....coreBX = ""
-00001f80: 2228 286e 6f64 655b 4063 6174 3d22 6475  "((node[@cat="du
-00001f90: 2220 616e 6420 6e6f 6465 5b25 7369 6e67  " and node[%sing
-00001fa0: 6c65 776f 7264 6277 2520 616e 6420 406c  lewordbw% and @l
-00001fb0: 656d 6d61 213d 226e 6965 7422 205d 2061  emma!="niet" ] a
-00001fc0: 6e64 206e 6f64 655b 2825 636f 7265 7068  nd node[(%coreph
-00001fd0: 7261 7365 2520 6f72 2028 4070 7420 616e  rase% or (@pt an
-00001fe0: 6420 6e6f 7428 2570 7625 2929 2920 616e  d not(%pv%))) an
-00001ff0: 6420 4062 6567 696e 213d 2e2e 2f6e 6f64  d @begin!=../nod
-00002000: 655b 2573 696e 676c 6577 6f72 6462 7725  e[%singlewordbw%
-00002010: 2061 6e64 2040 6c65 6d6d 6121 3d6e 6965   and @lemma!=nie
-00002020: 745d 2f40 6265 6769 6e20 5d5d 2920 2922  t]/@begin ]]) )"
-00002030: 2222 0d0a 0d0a 5461 7273 705f 626e 6f6e  ""....Tarsp_bnon
-00002040: 6669 6e20 3d20 2222 2228 2840 6361 743d  fin = """((@cat=
-00002050: 2269 6e66 2220 6f72 2040 6361 743d 2270  "inf" or @cat="p
-00002060: 7061 7274 2229 2061 6e64 2040 7265 6c3d  part") and @rel=
-00002070: 2276 6322 2061 6e64 2070 6172 656e 743a  "vc" and parent:
-00002080: 3a6e 6f64 655b 4063 6174 3d22 736d 6169  :node[@cat="smai
-00002090: 6e22 2061 6e64 2063 6f75 6e74 286e 6f64  n" and count(nod
-000020a0: 6529 3d31 5d20 616e 6420 6e6f 6465 5b25  e)=1] and node[%
-000020b0: 5461 7273 705f 4225 5d20 616e 6420 6e6f  Tarsp_B%] and no
-000020c0: 6465 5b40 7074 3d22 7777 2220 616e 6420  de[@pt="ww" and 
-000020d0: 4072 656c 3d22 6864 225d 2061 6e64 2063  @rel="hd"] and c
-000020e0: 6f75 6e74 286e 6f64 655b 2572 6561 6c63  ount(node[%realc
-000020f0: 6f6d 706c 6f72 6d6f 6425 5d29 3d31 2029  omplormod%])=1 )
-00002100: 2222 220d 0a0d 0a0d 0a41 5354 415f 7072  """......ASTA_pr
-00002110: 6564 203d 2020 2222 2228 4072 656c 3d22  ed =  """(@rel="
-00002120: 7072 6564 6322 206f 7220 4072 656c 3d22  predc" or @rel="
-00002130: 7072 6564 6d22 206f 7220 2840 7265 6c3d  predm" or (@rel=
-00002140: 2268 6422 2061 6e64 2070 6172 656e 743a  "hd" and parent:
-00002150: 3a6e 6f64 655b 4072 656c 3d22 7072 6564  :node[@rel="pred
-00002160: 6322 206f 7220 4072 656c 3d22 7072 6564  c" or @rel="pred
-00002170: 6d22 5d29 2922 2222 0d0a 0d0a 4153 5441  m"]))"""....ASTA
-00002180: 5f61 7474 7220 3d20 2022 2222 2828 4072  _attr =  """((@r
-00002190: 656c 3d22 6d6f 6422 2061 6e64 2070 6172  el="mod" and par
-000021a0: 656e 743a 3a6e 6f64 655b 6e6f 6465 5b40  ent::node[node[@
-000021b0: 7265 6c3d 2268 6422 2061 6e64 2028 4070  rel="hd" and (@p
-000021c0: 743d 226e 2220 6f72 2040 7074 3d22 766e  t="n" or @pt="vn
-000021d0: 7722 295d 5d20 2920 206f 720d 0a20 2020  w")]] )  or..   
-000021e0: 2020 2020 2840 7265 6c3d 2268 6422 2061      (@rel="hd" a
-000021f0: 6e64 2070 6172 656e 743a 3a6e 6f64 655b  nd parent::node[
-00002200: 4072 656c 3d22 6d6f 6422 2061 6e64 2070  @rel="mod" and p
-00002210: 6172 656e 743a 3a6e 6f64 655b 6e6f 6465  arent::node[node
-00002220: 5b40 7265 6c3d 2268 6422 2061 6e64 2028  [@rel="hd" and (
-00002230: 4070 743d 226e 2220 6f72 2040 7074 3d22  @pt="n" or @pt="
-00002240: 766e 7722 295d 5d5d 2929 2222 220d 0a0d  vnw")]]]))"""...
-00002250: 0a0d 0a41 5354 415f 6164 7665 7262 6961  ...ASTA_adverbia
-00002260: 6c20 3d20 2222 2220 200d 0a20 2020 2020  l = """  ..     
-00002270: 2028 2840 7265 6c3d 226d 6f64 2220 616e   ((@rel="mod" an
-00002280: 6420 7061 7265 6e74 3a3a 6e6f 6465 5b6e  d parent::node[n
-00002290: 6f64 655b 4072 656c 3d22 6864 2220 616e  ode[@rel="hd" an
-000022a0: 6420 6e6f 7428 4070 743d 226e 2220 6f72  d not(@pt="n" or
-000022b0: 2040 7074 3d22 766e 7722 295d 5d20 2920   @pt="vnw")]] ) 
-000022c0: 206f 720d 0a20 2020 2020 2020 2840 7265   or..       (@re
-000022d0: 6c3d 2268 6422 2061 6e64 2070 6172 656e  l="hd" and paren
-000022e0: 743a 3a6e 6f64 655b 4072 656c 3d22 6d6f  t::node[@rel="mo
-000022f0: 6422 2061 6e64 2070 6172 656e 743a 3a6e  d" and parent::n
-00002300: 6f64 655b 6e6f 6465 5b40 7265 6c3d 2268  ode[node[@rel="h
-00002310: 6422 2061 6e64 206e 6f74 2840 7074 3d22  d" and not(@pt="
-00002320: 6e22 206f 7220 4070 743d 2276 6e77 2229  n" or @pt="vnw")
-00002330: 5d5d 5d29 290d 0a20 2020 2020 2222 220d  ]]]))..     """.
-00002340: 0a0d 0a20 0d0a 4153 5441 5f6d 6f64 616c  ... ..ASTA_modal
-00002350: 7777 203d 2022 2222 2020 2840 6c65 6d6d  ww = """  (@lemm
-00002360: 613d 227a 756c 6c65 6e22 206f 7220 406c  a="zullen" or @l
-00002370: 656d 6d61 3d22 7769 6c6c 656e 2220 6f72  emma="willen" or
-00002380: 2040 6c65 6d6d 613d 226d 6f65 7465 6e22   @lemma="moeten"
-00002390: 206f 7220 406c 656d 6d61 3d22 6d6f 6765   or @lemma="moge
-000023a0: 6e22 206f 7220 406c 656d 6d61 3d22 6b75  n" or @lemma="ku
-000023b0: 6e6e 656e 2220 6f72 2040 6c65 6d6d 613d  nnen" or @lemma=
-000023c0: 2268 6f65 7665 6e22 2920 2222 220d 0a0d  "hoeven") """...
-000023d0: 0a41 5354 415f 6b6f 7077 7720 3d20 2222  .ASTA_kopww = ""
-000023e0: 2220 2820 2541 5354 415f 6261 7369 636b  " ( %ASTA_basick
-000023f0: 6f70 7777 2520 6f72 2025 4153 5441 5f67  opww% or %ASTA_g
-00002400: 6562 6f72 656e 5f6b 6f70 7777 2520 2922  eboren_kopww% )"
-00002410: 2222 0d0a 0d0a 4153 5441 5f62 6173 6963  ""....ASTA_basic
-00002420: 6b6f 7077 7720 3d20 2222 2220 2840 7074  kopww = """ (@pt
-00002430: 3d22 7777 2220 616e 6420 4072 656c 3d22  ="ww" and @rel="
-00002440: 6864 2220 616e 6420 406c 656d 6d61 213d  hd" and @lemma!=
-00002450: 2275 6974 5f7a 6965 6e22 2061 6e64 2040  "uit_zien" and @
-00002460: 6c65 6d6d 6121 3d22 6865 7465 6e22 2061  lemma!="heten" a
-00002470: 6e64 2040 6c65 6d6d 6121 3d22 6761 616e  nd @lemma!="gaan
-00002480: 2220 616e 6420 406c 656d 6d61 213d 227a  " and @lemma!="z
-00002490: 6974 7465 6e22 2061 6e64 2028 636f 6e74  itten" and (cont
-000024a0: 6169 6e73 2840 6672 616d 652c 2022 636f  ains(@frame, "co
-000024b0: 7075 6c61 2229 206f 7220 6e6f 7428 4073  pula") or not(@s
-000024c0: 7479 7065 3d22 746f 7069 635f 6472 6f70  type="topic_drop
-000024d0: 2229 2920 616e 6420 7061 7265 6e74 3a3a  ")) and parent::
-000024e0: 6e6f 6465 5b6e 6f64 655b 4072 656c 3d22  node[node[@rel="
-000024f0: 7072 6564 6322 5d20 616e 6420 6e6f 7428  predc"] and not(
-00002500: 6e6f 6465 5b40 7265 6c3d 226f 626a 3122  node[@rel="obj1"
-00002510: 5d29 205d 2029 2222 2220 0d0a 0d0a 4153  ]) ] )""" ....AS
-00002520: 5441 5f67 6562 6f72 656e 5f6b 6f70 7777  TA_geboren_kopww
-00002530: 203d 2022 2222 0d0a 0d0a 2840 7265 6c3d   = """....(@rel=
-00002540: 2268 6422 2061 6e64 2040 7074 3d22 7777  "hd" and @pt="ww
-00002550: 2220 616e 6420 2840 6c65 6d6d 613d 227a  " and (@lemma="z
-00002560: 696a 6e22 206f 7220 406c 656d 6d61 3d22  ijn" or @lemma="
-00002570: 776f 7264 656e 2229 2061 6e64 0d0a 2020  worden") and..  
-00002580: 2020 2020 2020 2028 2e2e 2f6e 6f64 655b         (../node[
-00002590: 4063 6174 3d22 7070 6172 7422 2061 6e64  @cat="ppart" and
-000025a0: 2040 7265 6c3d 2276 6322 2061 6e64 206e   @rel="vc" and n
-000025b0: 6f64 655b 2040 776f 7264 3d22 6765 626f  ode[ @word="gebo
-000025c0: 7265 6e22 2061 6e64 2040 7265 6c3d 2268  ren" and @rel="h
-000025d0: 6422 5d5d 206f 720d 0a09 0920 202e 2e2f  d"]] or....  ../
-000025e0: 6e6f 6465 5b40 7265 6c3d 2276 6322 2061  node[@rel="vc" a
-000025f0: 6e64 2040 776f 7264 3d22 6765 626f 7265  nd @word="gebore
-00002600: 6e22 5d0d 0a09 0920 290d 0a29 0d0a 0922  n"].... )..)..."
-00002610: 2222 0d0a 0d0a 4153 5441 5f77 616e 746d  ""....ASTA_wantm
-00002620: 6161 7262 696a 7a69 6e20 3d20 2222 220d  aarbijzin = """.
-00002630: 0a20 2020 2020 2020 2828 4077 6f72 643d  .       ((@word=
-00002640: 2277 616e 7422 206f 7220 4077 6f72 643d  "want" or @word=
-00002650: 226d 6161 7222 2920 616e 6420 4072 656c  "maar") and @rel
-00002660: 3d22 6372 6422 2061 6e64 2040 7074 3d22  ="crd" and @pt="
-00002670: 7667 2220 616e 640d 0a20 2020 2020 2020  vg" and..       
-00002680: 202e 2e2f 6e6f 6465 5b28 2840 6361 743d   ../node[((@cat=
-00002690: 2273 6d61 696e 2220 6f72 2040 6361 743d  "smain" or @cat=
-000026a0: 2273 7375 6222 206f 7220 2840 6361 743d  "ssub" or (@cat=
-000026b0: 2264 7522 2061 6e64 206e 6f64 655b 4063  "du" and node[@c
-000026c0: 6174 3d22 736d 6169 6e22 2061 6e64 2040  at="smain" and @
-000026d0: 7265 6c3d 226e 7563 6c22 5d29 2929 2061  rel="nucl"]))) a
-000026e0: 6e64 200d 0a09 2020 2020 4062 6567 696e  nd ...    @begin
-000026f0: 2020 3e3d 2e2e 2f6e 6f64 655b 2840 776f    >=../node[(@wo
-00002700: 7264 3d22 7761 6e74 2220 6f72 2040 776f  rd="want" or @wo
-00002710: 7264 3d22 6d61 6172 2229 5d2f 4065 6e64  rd="maar")]/@end
-00002720: 5d0d 0a09 2020 2029 0d0a 2222 220d 0a0d  ]...   ).."""...
-00002730: 0a41 5354 415f 7761 6e74 6d61 6172 6269  .ASTA_wantmaarbi
-00002740: 6a7a 696e 7a69 6e20 3d20 2222 220d 0a20  jzinzin = """.. 
-00002750: 2020 2020 2020 2820 2840 6361 743d 2273        ( (@cat="s
-00002760: 6d61 696e 2220 6f72 2040 6361 743d 2022  main" or @cat= "
-00002770: 7373 7562 2220 6f72 2028 4063 6174 3d22  ssub" or (@cat="
-00002780: 6475 2220 616e 6420 6e6f 6465 5b40 6361  du" and node[@ca
-00002790: 743d 2273 6d61 696e 2220 616e 6420 4072  t="smain" and @r
-000027a0: 656c 3d22 6e75 636c 225d 2929 2061 6e64  el="nucl"])) and
-000027b0: 0d0a 0920 2020 2020 2e2e 2f6e 6f64 655b  ...     ../node[
-000027c0: 2840 776f 7264 3d22 7761 6e74 2220 6f72  (@word="want" or
-000027d0: 2040 776f 7264 3d22 6d61 6172 2229 2061   @word="maar") a
-000027e0: 6e64 2040 7265 6c3d 2263 7264 2220 616e  nd @rel="crd" an
-000027f0: 6420 4070 743d 2276 6722 5d20 616e 6420  d @pt="vg"] and 
-00002800: 0d0a 0909 2040 6265 6769 6e20 203e 3d2e  .... @begin  >=.
-00002810: 2e2f 6e6f 6465 5b28 4077 6f72 643d 2277  ./node[(@word="w
-00002820: 616e 7422 206f 7220 4077 6f72 643d 226d  ant" or @word="m
-00002830: 6161 7222 295d 2f40 656e 640d 0a09 2020  aar")]/@end...  
-00002840: 2029 0d0a 2222 220d 0a0d 0a0d 0a41 5354   ).."""......AST
-00002850: 415f 6475 7362 696a 7a69 6e20 3d20 2222  A_dusbijzin = ""
-00002860: 220d 0a28 406c 656d 6d61 3d22 6475 7322  "..(@lemma="dus"
-00002870: 2061 6e64 2070 6172 656e 743a 3a6e 6f64   and parent::nod
-00002880: 655b 4063 6174 3d22 736d 6169 6e22 5d20  e[@cat="smain"] 
-00002890: 616e 6420 2040 6265 6769 6e3d 7061 7265  and  @begin=pare
-000028a0: 6e74 3a3a 6e6f 6465 2f40 6265 6769 6e20  nt::node/@begin 
-000028b0: 616e 6420 4070 743d 2262 7722 2061 6e64  and @pt="bw" and
-000028c0: 2040 7265 6c3d 226d 6f64 2229 0d0a 2222   @rel="mod")..""
-000028d0: 220d 0a0d 0a41 5354 415f 6475 7362 696a  "....ASTA_dusbij
-000028e0: 7a69 6e7a 696e 203d 2022 2222 0d0a 2840  zinzin = """..(@
-000028f0: 6361 743d 2273 6d61 696e 2220 616e 6420  cat="smain" and 
-00002900: 6e6f 6465 5b40 6c65 6d6d 613d 2264 7573  node[@lemma="dus
-00002910: 2220 2061 6e64 2020 4062 6567 696e 3d70  "  and  @begin=p
-00002920: 6172 656e 743a 3a6e 6f64 652f 4062 6567  arent::node/@beg
-00002930: 696e 2061 6e64 2040 7074 3d22 6277 2220  in and @pt="bw" 
-00002940: 616e 6420 4072 656c 3d22 6d6f 6422 5d29  and @rel="mod"])
-00002950: 0d0a 2222 220d 0a0d 0a0d 0a20 0d0a 4153  .."""...... ..AS
-00002960: 5441 5f64 6574 6164 6a73 203d 2022 2222  TA_detadjs = """
-00002970: 0d0a 2028 4070 743d 2276 6e77 2220 616e  .. (@pt="vnw" an
-00002980: 6420 2840 7265 6c3d 226d 6f64 2220 6f72  d (@rel="mod" or
-00002990: 2040 7265 6c3d 2264 6574 2229 2061 6e64   @rel="det") and
-000029a0: 2040 7677 7479 7065 3d22 6f6e 6265 7022   @vwtype="onbep"
-000029b0: 2061 6e64 2070 6172 656e 743a 3a6e 6f64   and parent::nod
-000029c0: 655b 4063 6174 3d22 6e70 225d 2061 6e64  e[@cat="np"] and
-000029d0: 0d0a 2840 6c65 6d6d 613d 2261 6c22 206f  ..(@lemma="al" o
-000029e0: 7220 406c 656d 6d61 3d22 6265 6964 6522  r @lemma="beide"
-000029f0: 206f 7220 406c 656d 6d61 3d22 656c 6b22   or @lemma="elk"
-00002a00: 206f 7220 406c 656d 6d61 3d22 656e 6967   or @lemma="enig
-00002a10: 2220 6f72 2040 6c65 6d6d 613d 2265 6e6b  " or @lemma="enk
-00002a20: 656c 2220 6f72 2040 6c65 6d6d 613d 2267  el" or @lemma="g
-00002a30: 6565 6e22 206f 7220 406c 656d 6d61 3d22  een" or @lemma="
-00002a40: 6965 6465 7222 206f 720d 0a20 406c 656d  ieder" or.. @lem
-00002a50: 6d61 3d22 6d65 6572 2220 6f72 2040 6c65  ma="meer" or @le
-00002a60: 6d6d 613d 226d 6565 7264 6572 6522 206f  mma="meerdere" o
-00002a70: 7220 406c 656d 6d61 3d22 6d65 6573 7422  r @lemma="meest"
-00002a80: 206f 7220 406c 656d 6d61 3d22 6d65 6e69   or @lemma="meni
-00002a90: 6722 206f 7220 406c 656d 6d61 3d22 6d69  g" or @lemma="mi
-00002aa0: 6e64 6572 2220 6f72 200d 0a20 406c 656d  nder" or .. @lem
-00002ab0: 6d61 3d22 6d69 6e73 7422 206f 7220 406c  ma="minst" or @l
-00002ac0: 656d 6d61 3d22 736f 6d6d 6967 6522 206f  emma="sommige" o
-00002ad0: 7220 406c 656d 6d61 3d22 7665 656c 2220  r @lemma="veel" 
-00002ae0: 6f72 2040 6c65 6d6d 613d 2277 6569 6e69  or @lemma="weini
-00002af0: 6722 2929 0d0a 0d0a 2222 220d 0a0d 0a54  g"))...."""....T
-00002b00: 6172 7370 5f6b 696a 6b65 656e 7320 3d20  arsp_kijkeens = 
-00002b10: 2222 220d 0a28 4063 6174 3d22 7376 3122  """..(@cat="sv1"
-00002b20: 2061 6e64 2040 7265 6c20 213d 2022 2d2d   and @rel != "--
-00002b30: 2220 616e 640d 0a20 2020 206e 6f64 655b  " and..    node[
-00002b40: 4070 743d 2277 7722 2061 6e64 2040 6c65  @pt="ww" and @le
-00002b50: 6d6d 613d 226b 696a 6b65 6e22 2061 6e64  mma="kijken" and
-00002b60: 2040 7265 6c3d 2268 6422 2020 616e 6420   @rel="hd"  and 
-00002b70: 4070 7661 6772 3d22 6576 2220 616e 6420  @pvagr="ev" and 
-00002b80: 4070 7674 696a 643d 2274 6777 2220 5d20  @pvtijd="tgw" ] 
-00002b90: 616e 640d 0a20 2020 206e 6f64 655b 406c  and..    node[@l
-00002ba0: 656d 6d61 3d22 6565 6e73 2220 616e 6420  emma="eens" and 
-00002bb0: 4072 656c 3d22 6d6f 6422 2061 6e64 2040  @rel="mod" and @
-00002bc0: 7074 3d22 6277 225d 2061 6e64 2063 6f75  pt="bw"] and cou
-00002bd0: 6e74 286e 6f64 6529 3d32 2920 0d0a 2222  nt(node)=2) ..""
-00002be0: 220d 0a0d 0a41 5354 415f 6e75 6d65 7261  "....ASTA_numera
-00002bf0: 6c20 3d20 2222 220d 0a28 406c 656d 6d61  l = """..(@lemma
-00002c00: 3d22 7477 6565 2220 6f72 2040 6c65 6d6d  ="twee" or @lemm
-00002c10: 613d 2264 7269 6522 206f 7220 406c 656d  a="drie" or @lem
-00002c20: 6d61 3d22 7669 6572 2220 6f72 2040 6c65  ma="vier" or @le
-00002c30: 6d6d 613d 2276 696a 6622 206f 7220 406c  mma="vijf" or @l
-00002c40: 656d 6d61 3d22 7a65 7322 206f 7220 406c  emma="zes" or @l
-00002c50: 656d 6d61 3d22 7a65 7665 6e22 206f 7220  emma="zeven" or 
-00002c60: 406c 656d 6d61 3d22 6163 6874 2220 6f72  @lemma="acht" or
-00002c70: 2040 6c65 6d6d 613d 226e 6567 656e 2220   @lemma="negen" 
-00002c80: 6f72 2040 6c65 6d6d 613d 2274 6965 6e22  or @lemma="tien"
-00002c90: 206f 7220 406c 656d 6d61 3d22 656c 6622   or @lemma="elf"
-00002ca0: 206f 7220 406c 656d 6d61 3d22 7477 6161   or @lemma="twaa
-00002cb0: 6c66 2220 6f72 2040 6c65 6d6d 613d 2264  lf" or @lemma="d
-00002cc0: 6572 7469 656e 2220 6f72 2040 6c65 6d6d  ertien" or @lemm
-00002cd0: 613d 2276 6565 7274 6965 6e22 206f 7220  a="veertien" or 
-00002ce0: 406c 656d 6d61 3d22 7669 6a66 7469 656e  @lemma="vijftien
-00002cf0: 2220 6f72 2040 6c65 6d6d 613d 227a 6573  " or @lemma="zes
-00002d00: 7469 656e 2220 6f72 2040 6c65 6d6d 613d  tien" or @lemma=
-00002d10: 227a 6576 656e 7469 656e 2220 6f72 2040  "zeventien" or @
-00002d20: 6c65 6d6d 613d 2261 6368 7474 6965 6e22  lemma="achttien"
-00002d30: 206f 7220 406c 656d 6d61 3d22 6e65 6765   or @lemma="nege
-00002d40: 6e74 6965 6e22 206f 7220 406c 656d 6d61  ntien" or @lemma
-00002d50: 3d22 7477 696e 7469 6722 206f 7220 406c  ="twintig" or @l
-00002d60: 656d 6d61 3d22 6565 6e74 6a65 2220 6f72  emma="eentje" or
-00002d70: 2020 406c 656d 6d61 3d22 7477 6565 746a    @lemma="tweetj
-00002d80: 6573 2220 6f72 2040 6c65 6d6d 613d 2264  es" or @lemma="d
-00002d90: 7269 6574 6a65 7322 206f 7220 406c 656d  rietjes" or @lem
-00002da0: 6d61 3d22 7669 6572 746a 6573 2220 6f72  ma="viertjes" or
-00002db0: 2040 6c65 6d6d 613d 2276 696a 666a 6573   @lemma="vijfjes
-00002dc0: 2220 6f72 2040 6c65 6d6d 613d 227a 6573  " or @lemma="zes
-00002dd0: 6a65 7322 2920 0d0a 2222 2220 0d0a 0d0a  jes") ..""" ....
-00002de0: 4153 5441 5f66 696c 6c65 645f 7061 7573  ASTA_filled_paus
-00002df0: 6520 3d20 2222 220d 0a28 406c 656d 6d61  e = """..(@lemma
-00002e00: 3d20 2275 6822 206f 7220 406c 656d 6d61  = "uh" or @lemma
-00002e10: 203d 2255 6822 206f 7220 406c 656d 6d61   ="Uh" or @lemma
-00002e20: 3d22 5568 6d22 206f 7220 406c 656d 6d61  ="Uhm" or @lemma
-00002e30: 3d20 2275 686d 2220 6f72 2020 406c 656d  = "uhm" or  @lem
-00002e40: 6d61 203d 2022 6575 6822 206f 7220 406c  ma = "euh" or @l
-00002e50: 656d 6d61 203d 2022 6568 2220 6f72 2040  emma = "eh" or @
-00002e60: 6c65 6d6d 6120 3d20 2267 6f68 2220 6f72  lemma = "goh" or
-00002e70: 2040 776f 7264 3d22 7878 7822 206f 7220   @word="xxx" or 
-00002e80: 4077 6f72 643d 2258 5858 2220 6f72 2040  @word="XXX" or @
-00002e90: 6c65 6d6d 613d 2267 6722 206f 7220 0d0a  lemma="gg" or ..
-00002ea0: 2020 406c 656d 6d61 3d22 6275 6822 206f    @lemma="buh" o
-00002eb0: 7220 406c 656d 6d61 3d22 7373 7322 206f  r @lemma="sss" o
-00002ec0: 7220 406c 656d 6d61 3d22 7066 2220 6f72  r @lemma="pf" or
-00002ed0: 2040 6c65 6d6d 613d 2774 6162 6c61 6127   @lemma='tablaa'
-00002ee0: 2029 0d0a 2222 220d 0a0d 0a41 5354 415f   ).."""....ASTA_
-00002ef0: 6765 626f 7265 6e20 3d20 2222 2220 2840  geboren = """ (@
-00002f00: 776f 7264 3d22 6765 626f 7265 6e22 2920  word="geboren") 
-00002f10: 2222 220d 0a0d 0a42 765a 6e20 3d20 2222  """....BvZn = ""
-00002f20: 2220 2863 6f75 6e74 286e 6f64 6529 3d32  " (count(node)=2
-00002f30: 2061 6e64 0d0a 2020 2020 2020 2020 2020   and..          
-00002f40: 2020 2820 2028 2568 6561 646e 2520 616e    (  (%headn% an
-00002f50: 6420 2825 636f 7265 6164 6a6d 6f64 2520  d (%coreadjmod% 
-00002f60: 6f72 2025 636f 7265 766e 776d 6f64 2520  or %corevnwmod% 
-00002f70: 6f72 2025 636f 7265 6277 6d6f 6425 2929  or %corebwmod%))
-00002f80: 200d 0a0d 0a09 0920 2020 2029 0d0a 0909   ......    )....
-00002f90: 2020 2029 090d 0a22 2222 0d0a 0d0a 7162     )..."""....qb
-00002fa0: 776c 656d 6d61 203d 2022 2222 2028 406c  wlemma = """ (@l
-00002fb0: 656d 6d61 3d22 6e6f 6722 2029 2022 2222  emma="nog" ) """
-00002fc0: 0d0a 0d0a 0d0a 6965 7473 6164 6a73 203d  ......ietsadjs =
-00002fd0: 2022 2222 286e 6f64 655b 4072 656c 3d22   """(node[@rel="
-00002fe0: 6864 2220 616e 6420 4070 743d 2276 6e77  hd" and @pt="vnw
-00002ff0: 225d 2061 6e64 206e 6f64 655b 4072 656c  "] and node[@rel
-00003000: 3d22 6d6f 6422 2061 6e64 2025 6164 6a73  ="mod" and %adjs
-00003010: 255d 290d 0a22 2222 0d0a 0d0a 6164 6a73  %]).."""....adjs
-00003020: 203d 2022 2222 2028 4070 743d 2261 646a   = """ (@pt="adj
-00003030: 2220 616e 6420 4062 7569 6769 6e67 3d22  " and @buiging="
-00003040: 6d65 742d 7322 2920 2222 220d 0a0d 0a61  met-s") """....a
-00003050: 7073 203d 2022 2222 2028 4063 6174 3d22  ps = """ (@cat="
-00003060: 6170 2220 616e 6420 6e6f 6465 5b40 7265  ap" and node[@re
-00003070: 6c3d 2268 6422 2061 6e64 2025 6164 6a73  l="hd" and %adjs
-00003080: 255d 2920 2222 220d 0a0d 0a68 6561 646e  %]) """....headn
-00003090: 203d 2022 2222 2028 206e 6f64 655b 4072   = """ ( node[@r
-000030a0: 656c 3d22 6864 2220 616e 6420 4070 743d  el="hd" and @pt=
-000030b0: 226e 225d 2029 2222 220d 0a0d 0a63 6f72  "n"] )"""....cor
-000030c0: 6561 646a 6d6f 6420 3d20 2222 2220 286e  eadjmod = """ (n
-000030d0: 6f64 655b 4072 656c 3d22 6d6f 6422 2061  ode[@rel="mod" a
-000030e0: 6e64 2028 2040 7074 3d22 6164 6a22 206f  nd ( @pt="adj" o
-000030f0: 7220 4070 743d 2274 7722 295d 2061 6e64  r @pt="tw")] and
-00003100: 206e 6f74 286e 6f64 655b 4072 656c 3d22   not(node[@rel="
-00003110: 6465 7422 5d29 2920 2222 220d 0a0d 0a63  det"])) """....c
-00003120: 6f72 6576 6e77 6d6f 6420 3d20 2222 2220  orevnwmod = """ 
-00003130: 286e 6f64 655b 4072 656c 3d22 6465 7422  (node[@rel="det"
-00003140: 2061 6e64 2028 4070 743d 2274 7722 206f   and (@pt="tw" o
-00003150: 7220 2840 7074 3d22 766e 7722 2061 6e64  r (@pt="vnw" and
-00003160: 2040 7677 7479 7065 3d22 6f6e 6265 7022   @vwtype="onbep"
-00003170: 2061 6e64 2040 6e61 616d 7661 6c21 3d22   and @naamval!="
-00003180: 6765 6e22 2061 6e64 2040 6c65 6d6d 6121  gen" and @lemma!
-00003190: 3d22 6765 656e 2229 295d 2029 2222 220d  ="geen"))] )""".
-000031a0: 0a0d 0a0d 0a63 6f72 6562 776d 6f64 203d  .....corebwmod =
-000031b0: 2022 2222 2028 6e6f 6465 5b40 7265 6c3d   """ (node[@rel=
-000031c0: 226d 6f64 2220 616e 6420 4070 743d 2262  "mod" and @pt="b
-000031d0: 7722 2061 6e64 2025 7162 776c 656d 6d61  w" and %qbwlemma
-000031e0: 255d 2920 2222 220d 0a0d 0a0d 0a73 7065  %]) """......spe
-000031f0: 635f 7072 6f70 6572 5f6e 616d 6520 3d20  c_proper_name = 
-00003200: 2222 2220 2840 7074 3d22 7370 6563 2220  """ (@pt="spec" 
-00003210: 616e 6420 0d0a 2020 2020 2020 2020 2020  and ..          
-00003220: 2020 2020 2020 2020 2020 2020 2020 2840                (@
-00003230: 706f 733d 226e 616d 6522 206f 7220 7374  pos="name" or st
-00003240: 6172 7473 2d77 6974 6828 4066 7261 6d65  arts-with(@frame
-00003250: 2c22 7072 6f70 6572 5f6e 616d 6522 2929  ,"proper_name"))
-00003260: 2061 6e64 0d0a 2020 2020 2020 2020 2020   and..          
-00003270: 2020 2020 2020 2020 2020 2020 2020 2863                (c
-00003280: 6f6e 7461 696e 7328 2241 4243 4445 4647  ontains("ABCDEFG
-00003290: 4849 4a4b 4c4d 4e4f 5051 5253 5455 5657  HIJKLMNOPQRSTUVW
-000032a0: 5859 5a22 2c20 7375 6273 7472 696e 6728  XYZ", substring(
-000032b0: 4077 6f72 642c 312c 3129 2929 0d0a 2020  @word,1,1)))..  
+00000aa0: 6761 616e 2220 6f72 0d0a 2020 2840 6c65  gaan" or..  (@le
+00000ab0: 6d6d 6120 3d20 2268 6f72 656e 2220 616e  mma = "horen" an
+00000ac0: 6420 2568 6f72 656e 6175 7825 2920 6f72  d %horenaux%) or
+00000ad0: 0d0a 2020 406c 656d 6d61 203d 2022 6b6f  ..  @lemma = "ko
+00000ae0: 6d65 6e22 206f 720d 0a20 2040 6c65 6d6d  men" or..  @lemm
+00000af0: 6120 3d20 226c 6174 656e 2220 6f72 0d0a  a = "laten" or..
+00000b00: 2020 406c 656d 6d61 203d 2022 6c69 6767    @lemma = "ligg
+00000b10: 656e 2220 6f72 0d0a 2020 406c 656d 6d61  en" or..  @lemma
+00000b20: 203d 2022 6c6f 7065 6e22 206f 720d 0a20   = "lopen" or.. 
+00000b30: 2040 6c65 6d6d 6120 3d20 226d 6f67 656e   @lemma = "mogen
+00000b40: 2220 6f72 0d0a 2020 406c 656d 6d61 203d  " or..  @lemma =
+00000b50: 2022 7374 6161 6e22 206f 720d 0a20 2040   "staan" or..  @
+00000b60: 6c65 6d6d 6120 3d20 227a 6974 7465 6e22  lemma = "zitten"
+00000b70: 290d 0a20 2222 220d 0a20 0d0a 5461 7273  ).. """.. ..Tars
+00000b80: 705f 7663 5f73 6962 6c69 6e67 203d 2022  p_vc_sibling = "
+00000b90: 2222 7061 7265 6e74 3a3a 6e6f 6465 5b20  ""parent::node[ 
+00000ba0: 6e6f 6465 5b40 7265 6c3d 2276 6322 2061  node[@rel="vc" a
+00000bb0: 6e64 206e 6f64 655b 4072 656c 3d22 6864  nd node[@rel="hd
+00000bc0: 225d 5d5d 2222 220d 0a54 6172 7370 5f70  "]]]"""..Tarsp_p
+00000bd0: 7265 6463 5f73 6962 6c69 6e67 203d 2022  redc_sibling = "
+00000be0: 2222 7061 7265 6e74 3a3a 6e6f 6465 5b20  ""parent::node[ 
+00000bf0: 6e6f 6465 5b40 7265 6c3d 2270 7265 6463  node[@rel="predc
+00000c00: 225d 5d22 2222 0d0a 5461 7273 705f 6f62  "]]"""..Tarsp_ob
+00000c10: 6a31 5f73 6962 6c69 6e67 203d 2022 2222  j1_sibling = """
+00000c20: 7061 7265 6e74 3a3a 6e6f 6465 5b20 6e6f  parent::node[ no
+00000c30: 6465 5b40 7265 6c3d 226f 626a 3122 5d5d  de[@rel="obj1"]]
+00000c40: 2222 220d 0a54 6172 7370 5f6c 645f 7369  """..Tarsp_ld_si
+00000c50: 626c 696e 6720 3d20 2222 2270 6172 656e  bling = """paren
+00000c60: 743a 3a6e 6f64 655b 206e 6f64 655b 4072  t::node[ node[@r
+00000c70: 656c 3d22 6c64 225d 5d22 2222 0d0a 5461  el="ld"]]"""..Ta
+00000c80: 7273 705f 6f6e 6c79 6d6f 6452 5f73 6962  rsp_onlymodR_sib
+00000c90: 6c69 6e67 203d 2022 2222 2870 6172 656e  ling = """(paren
+00000ca0: 743a 3a6e 6f64 655b 6e6f 6465 5b40 7265  t::node[node[@re
+00000cb0: 6c3d 226d 6f64 2220 616e 6420 2552 7072  l="mod" and %Rpr
+00000cc0: 6f6e 6f75 6e25 5d20 616e 6420 6e6f 7428  onoun%] and not(
+00000cd0: 6e6f 6465 5b40 7265 6c3d 2270 7265 6463  node[@rel="predc
+00000ce0: 225d 295d 2922 2222 0d0a 0d0a 6f6c 6454  "])])"""....oldT
+00000cf0: 6172 7370 5f48 7777 5a20 3d20 2222 2228  arsp_HwwZ = """(
+00000d00: 4070 743d 2277 7722 2061 6e64 2040 7265  @pt="ww" and @re
+00000d10: 6c3d 2268 6422 2061 6e64 2040 7776 6f72  l="hd" and @wvor
+00000d20: 6d3d 2270 7622 2061 6e64 2040 7076 6167  m="pv" and @pvag
+00000d30: 7221 3d22 6d76 2220 616e 6420 4070 7674  r!="mv" and @pvt
+00000d40: 696a 6421 3d22 7665 726c 2220 616e 640d  ijd!="verl" and.
+00000d50: 0a20 2828 0d0a 2020 2025 5461 7273 705f  . ((..   %Tarsp_
+00000d60: 6877 7725 206f 720d 0a20 2020 406c 656d  hww% or..   @lem
+00000d70: 6d61 203d 2022 6865 6262 656e 2220 0d0a  ma = "hebben" ..
+00000d80: 2020 2029 2061 6e64 200d 0a20 2020 6e6f     ) and ..   no
+00000d90: 7428 2554 6172 7370 5f76 635f 7369 626c  t(%Tarsp_vc_sibl
+00000da0: 696e 6725 2929 206f 720d 0a20 2020 2840  ing%)) or..   (@
+00000db0: 6c65 6d6d 613d 227a 696a 6e22 2061 6e64  lemma="zijn" and
+00000dc0: 206e 6f74 2825 5461 7273 705f 7663 5f73   not(%Tarsp_vc_s
+00000dd0: 6962 6c69 6e67 2529 2061 6e64 2025 5461  ibling%) and %Ta
+00000de0: 7273 705f 6c64 5f73 6962 6c69 6e67 2520  rsp_ld_sibling% 
+00000df0: 290d 0a0d 0a20 290d 0a22 2222 0d0a 0d0a  ).... ).."""....
+00000e00: 0d0a 5461 7273 705f 4877 775a 203d 2022  ..Tarsp_HwwZ = "
+00000e10: 2222 286e 6f74 2825 5461 7273 705f 4877  ""(not(%Tarsp_Hw
+00000e20: 7769 2529 2061 6e64 2028 4070 743d 2277  wi%) and (@pt="w
+00000e30: 7722 2061 6e64 2040 7265 6c3d 2268 6422  w" and @rel="hd"
+00000e40: 2061 6e64 2040 7776 6f72 6d3d 2270 7622   and @wvorm="pv"
+00000e50: 2061 6e64 2040 7076 6167 7221 3d22 6d76   and @pvagr!="mv
+00000e60: 2220 616e 6420 4070 7674 696a 6421 3d22  " and @pvtijd!="
+00000e70: 7665 726c 2220 616e 640d 0a20 2828 0d0a  verl" and.. ((..
+00000e80: 2020 2025 5461 7273 705f 6877 7725 206f     %Tarsp_hww% o
+00000e90: 720d 0a20 2020 406c 656d 6d61 203d 2022  r..   @lemma = "
+00000ea0: 6865 6262 656e 2220 0d0a 2020 2029 2061  hebben" ..   ) a
+00000eb0: 6e64 200d 0a20 2020 6e6f 7428 2554 6172  nd ..   not(%Tar
+00000ec0: 7370 5f76 635f 7369 626c 696e 6725 2929  sp_vc_sibling%))
+00000ed0: 206f 720d 0a20 2020 2840 6c65 6d6d 613d   or..   (@lemma=
+00000ee0: 227a 696a 6e22 2061 6e64 206e 6f74 2825  "zijn" and not(%
+00000ef0: 5461 7273 705f 7663 5f73 6962 6c69 6e67  Tarsp_vc_sibling
+00000f00: 2529 2061 6e64 2025 5461 7273 705f 6c64  %) and %Tarsp_ld
+00000f10: 5f73 6962 6c69 6e67 2520 290d 0a0d 0a20  _sibling% ).... 
+00000f20: 2929 0d0a 2222 220d 0a0d 0a0d 0a76 6468  )).."""......vdh
+00000f30: 7777 7320 3d20 2222 2228 406c 656d 6d61  wws = """(@lemma
+00000f40: 3d22 6865 6262 656e 2220 6f72 2040 6c65  ="hebben" or @le
+00000f50: 6d6d 613d 227a 696a 6e22 206f 7220 406c  mma="zijn" or @l
+00000f60: 656d 6d61 3d22 776f 7264 656e 2229 0d0a  emma="worden")..
+00000f70: 2222 220d 0a0d 0a54 6172 7370 5f4b 6f70  """....Tarsp_Kop
+00000f80: 203d 2022 2222 0d0a 2028 2020 2040 7074   = """.. (   @pt
+00000f90: 3d22 7777 2220 616e 6420 4072 656c 3d22  ="ww" and @rel="
+00000fa0: 6864 2220 616e 6420 6e6f 7428 2554 6172  hd" and not(%Tar
+00000fb0: 7370 5f68 7777 2529 2061 6e64 0d0a 0d0a  sp_hww%) and....
+00000fc0: 2020 2020 2828 2554 6172 7370 5f70 7265      ((%Tarsp_pre
+00000fd0: 6463 5f73 6962 6c69 6e67 2520 616e 6420  dc_sibling% and 
+00000fe0: 6e6f 7428 2554 6172 7370 5f6f 626a 315f  not(%Tarsp_obj1_
+00000ff0: 7369 626c 696e 6725 2929 206f 720d 0a0d  sibling%)) or...
+00001000: 0a20 2020 2020 2840 6c65 6d6d 613d 227a  .     (@lemma="z
+00001010: 696a 6e22 2061 6e64 206e 6f74 2825 5461  ijn" and not(%Ta
+00001020: 7273 705f 7663 5f73 6962 6c69 6e67 2529  rsp_vc_sibling%)
+00001030: 2061 6e64 206e 6f74 2825 5461 7273 705f   and not(%Tarsp_
+00001040: 6c64 5f73 6962 6c69 6e67 2529 2061 6e64  ld_sibling%) and
+00001050: 206e 6f74 2825 5461 7273 705f 6f6e 6c79   not(%Tarsp_only
+00001060: 6d6f 6452 5f73 6962 6c69 6e67 2529 290d  modR_sibling%)).
+00001070: 0a20 2020 2029 0d0a 2029 0d0a 2222 220d  .    ).. )..""".
+00001080: 0a0d 0a72 6f62 7573 7468 7777 7664 203d  ...robusthwwvd =
+00001090: 2022 2222 2028 4063 6174 3d22 746f 7022   """ (@cat="top"
+000010a0: 2061 6e64 200d 0a20 2020 2020 2020 2020   and ..         
+000010b0: 2020 2020 2020 2020 202e 2f2f 6e6f 6465           .//node
+000010c0: 5b40 7074 3d22 7777 2220 616e 6420 2576  [@pt="ww" and %v
+000010d0: 6468 7777 7325 2061 6e64 2040 7776 6f72  dhwws% and @wvor
+000010e0: 6d3d 2270 7622 2061 6e64 2028 4072 656c  m="pv" and (@rel
+000010f0: 3d22 2d2d 2220 6f72 2040 7265 6c3d 2264  ="--" or @rel="d
+00001100: 7022 295d 2061 6e64 0d0a 0909 0909 2020  p")] and......  
+00001110: 2e2f 2f6e 6f64 655b 4070 743d 2277 7722  .//node[@pt="ww"
+00001120: 2061 6e64 2040 7776 6f72 6d3d 2276 6422   and @wvorm="vd"
+00001130: 2061 6e64 2028 4072 656c 3d22 2d2d 2220   and (@rel="--" 
+00001140: 6f72 2040 7265 6c3d 2264 7022 295d 0d0a  or @rel="dp")]..
+00001150: 0909 0909 2020 290d 0a09 0909 0920 200d  ....  )......  .
+00001160: 0a22 2222 0d0a 0d0a 0d0a 726f 6275 7374  ."""......robust
+00001170: 696e 7665 7273 696f 6e20 3d20 2222 2228  inversion = """(
+00001180: 4063 6174 3d22 746f 7022 2061 6e64 200d  @cat="top" and .
+00001190: 0a20 2020 2020 2020 2e2f 2f6e 6f64 655b  .       .//node[
+000011a0: 4070 743d 2277 7722 2020 616e 6420 4077  @pt="ww"  and @w
+000011b0: 766f 726d 3d22 7076 2220 616e 6420 2040  vorm="pv" and  @
+000011c0: 7265 6c21 3d22 6864 2220 616e 6420 286e  rel!="hd" and (n
+000011d0: 6f74 2840 7374 7970 6529 206f 7220 4073  ot(@stype) or @s
+000011e0: 7479 7065 213d 2269 6d70 6172 6174 6976  type!="imparativ
+000011f0: 6522 295d 2061 6e64 200d 0a20 2020 2020  e")] and ..     
+00001200: 2020 2e2f 2f6e 6f64 655b 4070 743d 2276    .//node[@pt="v
+00001210: 6e77 2220 616e 6420 406e 6161 6d76 616c  nw" and @naamval
+00001220: 3d22 6e6f 6d69 6e22 2061 6e64 2040 7265  ="nomin" and @re
+00001230: 6c21 3d22 7375 2220 616e 640d 0a20 2020  l!="su" and..   
+00001240: 2020 2020 2020 2020 2020 2020 4065 6e64              @end
+00001250: 3e2e 2e2f 2f6e 6f64 655b 4070 743d 2277  >..//node[@pt="w
+00001260: 7722 2061 6e64 2040 7776 6f72 6d3d 2270  w" and @wvorm="p
+00001270: 7622 5d2f 4065 6e64 5d29 0d0a 0909 0920  v"]/@end])..... 
+00001280: 2020 2222 220d 0a0d 0a6c 6f63 7665 7262    """....locverb
+00001290: 203d 2022 2222 2840 6c65 6d6d 613d 2273   = """(@lemma="s
+000012a0: 7461 616e 2220 6f72 2040 6c65 6d6d 613d  taan" or @lemma=
+000012b0: 227a 6974 7465 6e22 206f 7220 406c 656d  "zitten" or @lem
+000012c0: 6d61 3d22 7269 6a64 656e 2220 6f72 2040  ma="rijden" or @
+000012d0: 6c65 6d6d 613d 2276 616c 6c65 6e22 206f  lemma="vallen" o
+000012e0: 7220 406c 656d 6d61 3d22 646f 656e 2220  r @lemma="doen" 
+000012f0: 6f72 2040 6c65 6d6d 613d 2267 6161 6e22  or @lemma="gaan"
+00001300: 206f 7220 406c 656d 6d61 3d22 6b6f 6d65   or @lemma="kome
+00001310: 6e22 206f 7220 406c 656d 6d61 3d22 7a69  n" or @lemma="zi
+00001320: 6a6e 2220 206f 7220 256c 6f63 6d6f 6461  jn"  or %locmoda
+00001330: 6c76 6572 6225 2029 0d0a 2222 220d 0a0d  lverb% ).."""...
+00001340: 0a6c 6f63 6d6f 6461 6c76 6572 6220 3d20  .locmodalverb = 
+00001350: 2222 2220 2840 6c65 6d6d 613d 226b 756e  """ (@lemma="kun
+00001360: 6e65 6e22 206f 7220 406c 656d 6d61 3d22  nen" or @lemma="
+00001370: 6d6f 6574 656e 2220 6f72 2040 6c65 6d6d  moeten" or @lemm
+00001380: 613d 2268 6f65 7665 6e22 206f 7220 406c  a="hoeven" or @l
+00001390: 656d 6d61 3d22 7769 6c6c 656e 2220 6f72  emma="willen" or
+000013a0: 2040 6c65 6d6d 613d 226d 6f67 656e 2229   @lemma="mogen")
+000013b0: 2222 220d 0a0d 0a0d 0a61 646a 6f72 6164  """......adjorad
+000013c0: 7620 3d20 2222 2228 4070 743d 2262 7722  v = """(@pt="bw"
+000013d0: 206f 7220 4070 743d 2261 646a 2220 6f72   or @pt="adj" or
+000013e0: 2028 4070 743d 2276 6e77 2220 616e 6420   (@pt="vnw" and 
+000013f0: 2840 706f 733d 2261 646a 2220 6f72 2040  (@pos="adj" or @
+00001400: 706f 733d 2261 6476 2229 2929 2222 220d  pos="adv")))""".
+00001410: 0a0d 0a61 646a 6164 7620 3d20 2222 220d  ...adjadv = """.
+00001420: 0a28 4070 743d 2761 646a 2720 616e 6420  .(@pt='adj' and 
+00001430: 2840 6c65 6d6d 613d 2777 656c 2729 290d  (@lemma='wel')).
+00001440: 0a22 2222 0d0a 0d0a 0d0a 7265 616c 6e6f  ."""......realno
+00001450: 6465 203d 2022 2222 2828 6e6f 7428 4070  de = """((not(@p
+00001460: 7429 206f 7220 2840 7074 213d 226c 6574  t) or (@pt!="let
+00001470: 2220 616e 6420 4070 7421 3d22 7473 7722  " and @pt!="tsw"
+00001480: 2929 2061 6e64 2028 6e6f 7428 4070 6f73  )) and (not(@pos
+00001490: 7461 6729 206f 7220 4070 6f73 7461 6721  tag) or @postag!
+000014a0: 3d22 4e41 2829 2229 2922 2222 0d0a 6e6f  ="NA()"))"""..no
+000014b0: 746f 6e6c 7972 6561 6c6e 6f64 6520 3d20  tonlyrealnode = 
+000014c0: 2222 2228 7061 7265 6e74 3a3a 6e6f 6465  """(parent::node
+000014d0: 5b63 6f75 6e74 286e 6f64 655b 2572 6561  [count(node[%rea
+000014e0: 6c6e 6f64 6525 5d29 3e31 5d29 2222 220d  lnode%])>1])""".
+000014f0: 0a0d 0a52 7072 6f6e 6f75 6e20 3d20 2222  ...Rpronoun = ""
+00001500: 2228 4070 743d 2776 6e77 2720 616e 6420  "(@pt='vnw' and 
+00001510: 2840 6c65 6d6d 613d 2765 7227 206f 7220  (@lemma='er' or 
+00001520: 406c 656d 6d61 3d27 6869 6572 2720 6f72  @lemma='hier' or
+00001530: 2040 6c65 6d6d 613d 2764 6161 7227 206f   @lemma='daar' o
+00001540: 7220 406c 656d 6d61 3d27 7761 6172 2720  r @lemma='waar' 
+00001550: 6f72 2040 6c65 6d6d 613d 2765 7267 656e  or @lemma='ergen
+00001560: 7327 206f 7220 406c 656d 6d61 3d27 6e65  s' or @lemma='ne
+00001570: 7267 656e 7327 206f 7220 406c 656d 6d61  rgens' or @lemma
+00001580: 3d27 6f76 6572 616c 2729 290d 0a22 2222  ='overal')).."""
+00001590: 0d0a 0d0a 7076 203d 2022 2222 2840 7074  ....pv = """(@pt
+000015a0: 3d22 7777 2220 616e 6420 4077 766f 726d  ="ww" and @wvorm
+000015b0: 3d22 7076 2220 2922 2222 0d0a 0d0a 6278  ="pv" )"""....bx
+000015c0: 6e70 3120 3d20 2222 2228 4063 6174 3d22  np1 = """(@cat="
+000015d0: 6e70 2220 616e 6420 636f 756e 7428 6e6f  np" and count(no
+000015e0: 6465 293d 3220 616e 6420 6e6f 6465 5b40  de)=2 and node[@
+000015f0: 7265 6c3d 2268 6422 2061 6e64 2040 7074  rel="hd" and @pt
+00001600: 3d22 7777 225d 2061 6e64 206e 6f64 655b  ="ww"] and node[
+00001610: 4072 656c 3d22 6d6f 6422 2061 6e64 2040  @rel="mod" and @
+00001620: 7074 5d29 2222 220d 0a62 786e 7032 203d  pt])"""..bxnp2 =
+00001630: 2022 2222 2840 6361 743d 226e 7022 2061   """(@cat="np" a
+00001640: 6e64 2063 6f75 6e74 286e 6f64 6529 3d32  nd count(node)=2
+00001650: 2061 6e64 206e 6f64 655b 4072 656c 3d22   and node[@rel="
+00001660: 6864 225d 2061 6e64 206e 6f64 655b 4072  hd"] and node[@r
+00001670: 656c 3d22 6d6f 6422 2061 6e64 2025 7369  el="mod" and %si
+00001680: 6e67 6c65 776f 7264 6277 255d 2922 2222  nglewordbw%])"""
+00001690: 0d0a 0d0a 5461 7273 705f 4261 7369 635f  ....Tarsp_Basic_
+000016a0: 5643 203d 2022 2222 2828 4072 656c 3d22  VC = """((@rel="
+000016b0: 6f62 6a31 2220 6f72 2040 7265 6c3d 2270  obj1" or @rel="p
+000016c0: 6322 2020 6f72 2040 7265 6c3d 2270 7265  c"  or @rel="pre
+000016d0: 6463 2220 6f72 2040 7265 6c3d 226c 6422  dc" or @rel="ld"
+000016e0: 206f 7220 4072 656c 3d22 6f62 6a32 2220   or @rel="obj2" 
+000016f0: 6f72 2025 5461 7273 705f 6669 6e76 6325  or %Tarsp_finvc%
+00001700: 206f 7220 2554 6172 7370 5f76 6376 6e77   or %Tarsp_vcvnw
+00001710: 2520 6f72 2028 4072 656c 3d22 7376 7022  % or (@rel="svp"
+00001720: 2061 6e64 2040 7074 213d 2276 7a22 2929   and @pt!="vz"))
+00001730: 2061 6e64 206e 6f74 2825 5461 7273 705f   and not(%Tarsp_
+00001740: 4261 7369 635f 4225 2920 2922 2222 0d0a  Basic_B%) )"""..
+00001750: 0d0a 0d0a 5461 7273 705f 4261 7369 635f  ....Tarsp_Basic_
+00001760: 4220 3d20 2222 2228 4072 656c 3d22 6d6f  B = """(@rel="mo
+00001770: 6422 206f 7220 4072 656c 3d22 6c64 2220  d" or @rel="ld" 
+00001780: 6f72 2040 7265 6c3d 2270 7265 646d 2220  or @rel="predm" 
+00001790: 206f 7220 2554 6172 7370 5f42 5f70 7265   or %Tarsp_B_pre
+000017a0: 6463 2529 2022 2222 0d0a 0d0a 5461 7273  dc%) """....Tars
+000017b0: 705f 425f 7072 6564 6320 3d20 2222 2228  p_B_predc = """(
+000017c0: 4072 656c 3d70 7265 6463 2061 6e64 2028  @rel=predc and (
+000017d0: 4070 743d 2276 7a22 206f 7220 4070 743d  @pt="vz" or @pt=
+000017e0: 2262 7722 206f 7220 4063 6174 3d22 7070  "bw" or @cat="pp
+000017f0: 2220 6f72 2040 6361 743d 2261 6476 7022  " or @cat="advp"
+00001800: 206f 7220 2552 7072 6f6e 6f75 6e25 2929   or %Rpronoun%))
+00001810: 2222 220d 0a0d 0a54 6172 7370 5f42 203d  """....Tarsp_B =
+00001820: 2022 2222 280d 0a20 2020 2020 2020 2828   """(..       ((
+00001830: 2828 4072 656c 3d22 6d6f 6422 206f 7220  ((@rel="mod" or 
+00001840: 4072 656c 3d22 6c64 2220 6f72 2040 7265  @rel="ld" or @re
+00001850: 6c3d 2270 7265 646d 2229 2061 6e64 0d0a  l="predm") and..
+00001860: 2020 2020 2020 2020 2020 286e 6f74 2840            (not(@
+00001870: 6361 7429 206f 7220 4063 6174 213d 2263  cat) or @cat!="c
+00001880: 6f6e 6a22 2920 616e 640d 0a09 0920 2028  onj") and....  (
+00001890: 6e6f 7428 4070 7429 206f 7220 4070 7421  not(@pt) or @pt!
+000018a0: 3d22 7473 7722 290d 0a20 2020 2020 2020  ="tsw")..       
+000018b0: 2020 296f 7220 0d0a 2020 2020 2020 2020    )or ..        
+000018c0: 2028 2570 7265 6463 4225 0d0a 2020 2020   (%predcB%..    
+000018d0: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+000018e0: 2029 2061 6e64 200d 0a20 2020 2020 2020   ) and ..       
+000018f0: 2020 282e 2e2f 6e6f 6465 5b40 7074 3d22    (../node[@pt="
+00001900: 7777 2220 616e 6420 4072 656c 3d22 6864  ww" and @rel="hd
+00001910: 225d 290d 0a20 2020 2020 2020 2029 206f  "])..        ) o
+00001920: 720d 0a20 2020 2020 2020 2028 2840 7074  r..        ((@pt
+00001930: 3d22 767a 2220 6f72 2040 7074 3d22 6277  ="vz" or @pt="bw
+00001940: 2220 6f72 2025 5270 726f 6e6f 756e 2529  " or %Rpronoun%)
+00001950: 2061 6e64 2028 4072 656c 3d22 6470 2220   and (@rel="dp" 
+00001960: 6f72 2040 7265 6c3d 222d 2d22 206f 7220  or @rel="--" or 
+00001970: 4072 656c 3d22 6e75 636c 2220 6f72 2040  @rel="nucl" or @
+00001980: 7265 6c3d 2262 6f64 7922 2920 616e 6420  rel="body") and 
+00001990: 256e 6f74 6f6e 6c79 7265 616c 6e6f 6465  %notonlyrealnode
+000019a0: 2529 206f 720d 0a20 2020 2020 2020 2028  %) or..        (
+000019b0: 4063 6174 3d22 7070 2220 616e 6420 2840  @cat="pp" and (@
+000019c0: 7265 6c3d 222d 2d22 206f 7220 4072 656c  rel="--" or @rel
+000019d0: 3d22 6470 2229 2061 6e64 2025 6e6f 746f  ="dp") and %noto
+000019e0: 6e6c 7972 6561 6c6e 6f64 6525 2920 6f72  nlyrealnode%) or
+000019f0: 0d0a 0909 2840 7265 6c3d 2270 6322 2061  ....(@rel="pc" a
+00001a00: 6e64 202e 2e2f 6e6f 6465 5b40 7265 6c3d  nd ../node[@rel=
+00001a10: 2268 6422 2061 6e64 2025 6c6f 6376 6572  "hd" and %locver
+00001a20: 6225 5d29 206f 720d 0a20 2020 2020 2020  b%]) or..       
+00001a30: 2028 4072 656c 3d22 636e 6a22 2061 6e64   (@rel="cnj" and
+00001a40: 2070 6172 656e 743a 3a6e 6f64 655b 4072   parent::node[@r
+00001a50: 656c 3d22 6d6f 6422 206f 7220 4072 656c  el="mod" or @rel
+00001a60: 3d22 6c64 2220 6f72 2040 7265 6c3d 2270  ="ld" or @rel="p
+00001a70: 7265 646d 225d 2920 6f72 0d0a 2020 2020  redm"]) or..    
+00001a80: 2020 2020 2840 7265 6c3d 226d 6f64 2220      (@rel="mod" 
+00001a90: 616e 6420 4070 743d 2262 7722 2061 6e64  and @pt="bw" and
+00001aa0: 2070 6172 656e 743a 3a6e 6f64 655b 4063   parent::node[@c
+00001ab0: 6174 3d22 6e70 225d 2029 206f 720d 0a09  at="np"] ) or...
+00001ac0: 0925 5461 7273 705f 6e6f 6e6d 6f64 6164  .%Tarsp_nonmodad
+00001ad0: 7663 7025 206f 720d 0a09 0925 5461 7273  vcp% or....%Tars
+00001ae0: 705f 7063 5f76 635f 6578 6365 7074 696f  p_pc_vc_exceptio
+00001af0: 6e25 0d0a 0909 290d 0a20 2020 2020 0d0a  n%....)..     ..
+00001b00: 2222 220d 0a0d 0a63 6f6d 706c 656d 656e  """....complemen
+00001b10: 7420 3d20 2222 2228 2840 7265 6c3d 226f  t = """((@rel="o
+00001b20: 626a 3122 206f 7220 4072 656c 3d22 6f62  bj1" or @rel="ob
+00001b30: 6a32 2229 206f 7220 0d0a 2020 2020 2020  j2") or ..      
+00001b40: 2020 2020 2020 2020 2020 2028 4072 656c             (@rel
+00001b50: 3d22 7072 6564 6322 2061 6e64 206e 6f74  ="predc" and not
+00001b60: 2825 7072 6564 6342 2529 2920 6f72 0d0a  (%predcB%)) or..
+00001b70: 0909 2020 2020 2020 2020 2028 4072 656c  ..         (@rel
+00001b80: 3d22 706f 626a 3122 2061 6e64 206e 6f74  ="pobj1" and not
+00001b90: 2825 706f 626a 3142 2529 2029 206f 720d  (%pobj1B%) ) or.
+00001ba0: 0a09 0909 0920 2576 6572 6261 6c63 6f6d  ..... %verbalcom
+00001bb0: 706c 656d 656e 7425 0d0a 2020 2020 2020  plement%..      
+00001bc0: 2020 2020 2020 2020 2020 2922 2222 0d0a            )"""..
+00001bd0: 0909 0909 0d0a 7665 7262 616c 636f 6d70  ......verbalcomp
+00001be0: 6c65 6d65 6e74 203d 2022 2222 2840 7265  lement = """(@re
+00001bf0: 6c3d 2276 6322 2061 6e64 2028 4063 6174  l="vc" and (@cat
+00001c00: 3d22 6370 2220 6f72 2040 6361 743d 2277  ="cp" or @cat="w
+00001c10: 6871 2220 6f72 2040 6361 743d 2277 6873  hq" or @cat="whs
+00001c20: 7562 2229 2922 2222 0d0a 0909 200d 0a70  ub"))""".... ..p
+00001c30: 7265 6463 4220 3d20 2222 2228 4072 656c  redcB = """(@rel
+00001c40: 3d22 7072 6564 6322 2061 6e64 200d 0a20  ="predc" and .. 
+00001c50: 2020 2020 2020 2020 2020 2840 7074 3d22            (@pt="
+00001c60: 6164 6a22 206f 7220 4070 743d 2262 7722  adj" or @pt="bw"
+00001c70: 206f 7220 4063 6174 3d22 6170 2220 6f72   or @cat="ap" or
+00001c80: 2040 6361 743d 2261 6476 7022 2920 616e   @cat="advp") an
+00001c90: 640d 0a20 2020 2020 2020 2020 2020 2e2e  d..           ..
+00001ca0: 2f6e 6f64 655b 4072 656c 3d22 6f62 6a31  /node[@rel="obj1
+00001cb0: 225d 0d0a 2020 2020 2020 2020 2029 2222  "]..         )""
+00001cc0: 220d 0a09 0920 0d0a 706f 626a 3142 203d  ".... ..pobj1B =
+00001cd0: 2022 2222 2840 7265 6c3d 2270 6322 2061   """(@rel="pc" a
+00001ce0: 6e64 202e 2e2f 6e6f 6465 5b40 7265 6c3d  nd ../node[@rel=
+00001cf0: 2268 6422 2061 6e64 2025 6c6f 6376 6572  "hd" and %locver
+00001d00: 6225 5d29 2222 220d 0a20 0d0a 0d0a 0d0a  b%])""".. ......
+00001d10: 7369 6e67 6c65 776f 7264 6277 203d 2022  singlewordbw = "
+00001d20: 2222 2028 4070 743d 2262 7722 206f 7220  "" (@pt="bw" or 
+00001d30: 2552 7072 6f6e 6f75 6e25 206f 7220 2561  %Rpronoun% or %a
+00001d40: 646a 6164 7625 290d 0a22 2222 0d0a 0d0a  djadv%).."""....
+00001d50: 0d0a 6469 6564 6174 7265 6c20 3d20 2222  ..diedatrel = ""
+00001d60: 2228 4070 743d 2276 6e77 2220 616e 6420  "(@pt="vnw" and 
+00001d70: 4076 7774 7970 653d 2262 6574 7222 2061  @vwtype="betr" a
+00001d80: 6e64 2040 7265 6c3d 2272 6864 2220 616e  nd @rel="rhd" an
+00001d90: 6420 2840 6c65 6d6d 613d 2264 6965 2220  d (@lemma="die" 
+00001da0: 6f72 2040 6c65 6d6d 613d 2264 6174 2229  or @lemma="dat")
+00001db0: 2922 2222 0d0a 0d0a 6176 6e72 656c 203d  )"""....avnrel =
+00001dc0: 2022 2222 2825 6469 6564 6174 7265 6c25   """(%diedatrel%
+00001dd0: 2061 6e64 2070 6172 656e 743a 3a6e 6f64   and parent::nod
+00001de0: 655b 4063 6174 3d22 7265 6c22 2061 6e64  e[@cat="rel" and
+00001df0: 2040 7265 6c21 3d22 6d6f 6422 5d29 2222   @rel!="mod"])""
+00001e00: 220d 0a0d 0a76 3270 726f 626c 656d 203d  "....v2problem =
+00001e10: 2022 2222 2f2f 6e6f 6465 5b40 7074 3d22   """//node[@pt="
+00001e20: 7777 2220 616e 6420 4077 766f 726d 3d22  ww" and @wvorm="
+00001e30: 7076 2220 616e 6420 0d0a 2020 2020 2020  pv" and ..      
+00001e40: 2040 6265 6769 6e20 213d 2070 6172 656e   @begin != paren
+00001e50: 743a 3a6e 6f64 655b 4063 6174 3d22 7373  t::node[@cat="ss
+00001e60: 7562 225d 2f70 6172 656e 743a 3a6e 6f64  ub"]/parent::nod
+00001e70: 655b 4063 6174 3d22 7265 6c22 2061 6e64  e[@cat="rel" and
+00001e80: 2040 7265 6c21 3d22 6d6f 6422 5d2f 6e6f   @rel!="mod"]/no
+00001e90: 6465 5b25 6469 6564 6174 7265 6c25 205d  de[%diedatrel% ]
+00001ea0: 2f40 656e 640d 0a20 2020 2020 205d 2222  /@end..      ]""
+00001eb0: 220d 0a0d 0a63 6f72 6561 766e 203d 2022  "....coreavn = "
+00001ec0: 2222 2840 7074 3d22 766e 7722 2020 616e  ""(@pt="vnw"  an
+00001ed0: 6420 4076 7774 7970 653d 2261 616e 7722  d @vwtype="aanw"
+00001ee0: 2061 6e64 2040 6c65 6d6d 6121 3d22 6869   and @lemma!="hi
+00001ef0: 6572 2220 616e 6420 406c 656d 6d61 213d  er" and @lemma!=
+00001f00: 2264 6161 7222 2061 6e64 2040 6c65 6d6d  "daar" and @lemm
+00001f10: 6121 3d22 6572 2220 616e 6420 4072 656c  a!="er" and @rel
+00001f20: 213d 2264 6574 2220 616e 6420 286e 6f74  !="det" and (not
+00001f30: 2840 706f 7369 7469 6529 206f 7220 4070  (@positie) or @p
+00001f40: 6f73 6974 6965 213d 2270 7265 6e6f 6d22  ositie!="prenom"
+00001f50: 2920 2922 2222 0d0a 0d0a 4156 6e20 3d20  ) )"""....AVn = 
+00001f60: 2222 2228 2563 6f72 6561 766e 2520 6f72  """(%coreavn% or
+00001f70: 2025 6176 6e72 656c 2529 2222 2222 200d   %avnrel%)"""" .
+00001f80: 0a0d 0a63 6f72 6570 6872 6173 6520 3d20  ...corephrase = 
+00001f90: 2222 2228 4063 6174 3d22 6e70 2220 6f72  """(@cat="np" or
+00001fa0: 2040 6361 743d 2270 7022 206f 7220 4063   @cat="pp" or @c
+00001fb0: 6174 3d22 6164 7670 2220 6f72 2040 6361  at="advp" or @ca
+00001fc0: 743d 2261 7022 2922 2222 0d0a 0d0a 636f  t="ap")"""....co
+00001fd0: 7265 4258 203d 2022 2222 2828 6e6f 6465  reBX = """((node
+00001fe0: 5b40 6361 743d 2264 7522 2061 6e64 206e  [@cat="du" and n
+00001ff0: 6f64 655b 2573 696e 676c 6577 6f72 6462  ode[%singlewordb
+00002000: 7725 2061 6e64 2040 6c65 6d6d 6121 3d22  w% and @lemma!="
+00002010: 6e69 6574 2220 5d20 616e 6420 6e6f 6465  niet" ] and node
+00002020: 5b28 2563 6f72 6570 6872 6173 6525 206f  [(%corephrase% o
+00002030: 7220 2840 7074 2061 6e64 206e 6f74 2825  r (@pt and not(%
+00002040: 7076 2529 2929 2061 6e64 2040 6265 6769  pv%))) and @begi
+00002050: 6e21 3d2e 2e2f 6e6f 6465 5b25 7369 6e67  n!=../node[%sing
+00002060: 6c65 776f 7264 6277 2520 616e 6420 406c  lewordbw% and @l
+00002070: 656d 6d61 213d 6e69 6574 5d2f 4062 6567  emma!=niet]/@beg
+00002080: 696e 205d 5d29 2029 2222 220d 0a0d 0a54  in ]]) )"""....T
+00002090: 6172 7370 5f62 6e6f 6e66 696e 203d 2022  arsp_bnonfin = "
+000020a0: 2222 2828 4063 6174 3d22 696e 6622 206f  ""((@cat="inf" o
+000020b0: 7220 4063 6174 3d22 7070 6172 7422 2920  r @cat="ppart") 
+000020c0: 616e 6420 4072 656c 3d22 7663 2220 616e  and @rel="vc" an
+000020d0: 6420 7061 7265 6e74 3a3a 6e6f 6465 5b40  d parent::node[@
+000020e0: 6361 743d 2273 6d61 696e 2220 616e 6420  cat="smain" and 
+000020f0: 636f 756e 7428 6e6f 6465 293d 315d 2061  count(node)=1] a
+00002100: 6e64 206e 6f64 655b 2554 6172 7370 5f42  nd node[%Tarsp_B
+00002110: 255d 2061 6e64 206e 6f64 655b 4070 743d  %] and node[@pt=
+00002120: 2277 7722 2061 6e64 2040 7265 6c3d 2268  "ww" and @rel="h
+00002130: 6422 5d20 616e 6420 636f 756e 7428 6e6f  d"] and count(no
+00002140: 6465 5b25 7265 616c 636f 6d70 6c6f 726d  de[%realcomplorm
+00002150: 6f64 255d 293d 3120 2922 2222 0d0a 0d0a  od%])=1 )"""....
+00002160: 0d0a 4153 5441 5f70 7265 6420 3d20 2022  ..ASTA_pred =  "
+00002170: 2222 2840 7265 6c3d 2270 7265 6463 2220  ""(@rel="predc" 
+00002180: 6f72 2040 7265 6c3d 2270 7265 646d 2220  or @rel="predm" 
+00002190: 6f72 2028 4072 656c 3d22 6864 2220 616e  or (@rel="hd" an
+000021a0: 6420 7061 7265 6e74 3a3a 6e6f 6465 5b40  d parent::node[@
+000021b0: 7265 6c3d 2270 7265 6463 2220 6f72 2040  rel="predc" or @
+000021c0: 7265 6c3d 2270 7265 646d 225d 2929 2222  rel="predm"]))""
+000021d0: 220d 0a0d 0a41 5354 415f 6174 7472 203d  "....ASTA_attr =
+000021e0: 2020 2222 2228 2840 7265 6c3d 226d 6f64    """((@rel="mod
+000021f0: 2220 616e 6420 7061 7265 6e74 3a3a 6e6f  " and parent::no
+00002200: 6465 5b6e 6f64 655b 4072 656c 3d22 6864  de[node[@rel="hd
+00002210: 2220 616e 6420 2840 7074 3d22 6e22 206f  " and (@pt="n" o
+00002220: 7220 4070 743d 2276 6e77 2229 5d5d 2029  r @pt="vnw")]] )
+00002230: 2020 6f72 0d0a 2020 2020 2020 2028 4072    or..       (@r
+00002240: 656c 3d22 6864 2220 616e 6420 7061 7265  el="hd" and pare
+00002250: 6e74 3a3a 6e6f 6465 5b40 7265 6c3d 226d  nt::node[@rel="m
+00002260: 6f64 2220 616e 6420 7061 7265 6e74 3a3a  od" and parent::
+00002270: 6e6f 6465 5b6e 6f64 655b 4072 656c 3d22  node[node[@rel="
+00002280: 6864 2220 616e 6420 2840 7074 3d22 6e22  hd" and (@pt="n"
+00002290: 206f 7220 4070 743d 2276 6e77 2229 5d5d   or @pt="vnw")]]
+000022a0: 5d29 2922 2222 0d0a 0d0a 0d0a 4153 5441  ]))"""......ASTA
+000022b0: 5f61 6476 6572 6269 616c 203d 2022 2222  _adverbial = """
+000022c0: 2020 0d0a 2020 2020 2020 2828 4072 656c    ..      ((@rel
+000022d0: 3d22 6d6f 6422 2061 6e64 2070 6172 656e  ="mod" and paren
+000022e0: 743a 3a6e 6f64 655b 6e6f 6465 5b40 7265  t::node[node[@re
+000022f0: 6c3d 2268 6422 2061 6e64 206e 6f74 2840  l="hd" and not(@
+00002300: 7074 3d22 6e22 206f 7220 4070 743d 2276  pt="n" or @pt="v
+00002310: 6e77 2229 5d5d 2029 2020 6f72 0d0a 2020  nw")]] )  or..  
+00002320: 2020 2020 2028 4072 656c 3d22 6864 2220       (@rel="hd" 
+00002330: 616e 6420 7061 7265 6e74 3a3a 6e6f 6465  and parent::node
+00002340: 5b40 7265 6c3d 226d 6f64 2220 616e 6420  [@rel="mod" and 
+00002350: 7061 7265 6e74 3a3a 6e6f 6465 5b6e 6f64  parent::node[nod
+00002360: 655b 4072 656c 3d22 6864 2220 616e 6420  e[@rel="hd" and 
+00002370: 6e6f 7428 4070 743d 226e 2220 6f72 2040  not(@pt="n" or @
+00002380: 7074 3d22 766e 7722 295d 5d5d 2929 0d0a  pt="vnw")]]]))..
+00002390: 2020 2020 2022 2222 0d0a 0d0a 200d 0a41       """.... ..A
+000023a0: 5354 415f 6d6f 6461 6c77 7720 3d20 2222  STA_modalww = ""
+000023b0: 2220 2028 406c 656d 6d61 3d22 7a75 6c6c  "  (@lemma="zull
+000023c0: 656e 2220 6f72 2040 6c65 6d6d 613d 2277  en" or @lemma="w
+000023d0: 696c 6c65 6e22 206f 7220 406c 656d 6d61  illen" or @lemma
+000023e0: 3d22 6d6f 6574 656e 2220 6f72 2040 6c65  ="moeten" or @le
+000023f0: 6d6d 613d 226d 6f67 656e 2220 6f72 2040  mma="mogen" or @
+00002400: 6c65 6d6d 613d 226b 756e 6e65 6e22 206f  lemma="kunnen" o
+00002410: 7220 406c 656d 6d61 3d22 686f 6576 656e  r @lemma="hoeven
+00002420: 2229 2022 2222 0d0a 0d0a 4153 5441 5f6b  ") """....ASTA_k
+00002430: 6f70 7777 203d 2022 2222 2028 2025 4153  opww = """ ( %AS
+00002440: 5441 5f62 6173 6963 6b6f 7077 7725 206f  TA_basickopww% o
+00002450: 7220 2541 5354 415f 6765 626f 7265 6e5f  r %ASTA_geboren_
+00002460: 6b6f 7077 7725 2029 2222 220d 0a0d 0a41  kopww% )"""....A
+00002470: 5354 415f 6261 7369 636b 6f70 7777 203d  STA_basickopww =
+00002480: 2022 2222 2028 4070 743d 2277 7722 2061   """ (@pt="ww" a
+00002490: 6e64 2040 7265 6c3d 2268 6422 2061 6e64  nd @rel="hd" and
+000024a0: 2040 6c65 6d6d 6121 3d22 7569 745f 7a69   @lemma!="uit_zi
+000024b0: 656e 2220 616e 6420 406c 656d 6d61 213d  en" and @lemma!=
+000024c0: 2268 6574 656e 2220 616e 6420 406c 656d  "heten" and @lem
+000024d0: 6d61 213d 2267 6161 6e22 2061 6e64 2040  ma!="gaan" and @
+000024e0: 6c65 6d6d 6121 3d22 7a69 7474 656e 2220  lemma!="zitten" 
+000024f0: 616e 6420 2863 6f6e 7461 696e 7328 4066  and (contains(@f
+00002500: 7261 6d65 2c20 2263 6f70 756c 6122 2920  rame, "copula") 
+00002510: 6f72 206e 6f74 2840 7374 7970 653d 2274  or not(@stype="t
+00002520: 6f70 6963 5f64 726f 7022 2929 2061 6e64  opic_drop")) and
+00002530: 2070 6172 656e 743a 3a6e 6f64 655b 6e6f   parent::node[no
+00002540: 6465 5b40 7265 6c3d 2270 7265 6463 225d  de[@rel="predc"]
+00002550: 2061 6e64 206e 6f74 286e 6f64 655b 4072   and not(node[@r
+00002560: 656c 3d22 6f62 6a31 225d 2920 5d20 2922  el="obj1"]) ] )"
+00002570: 2222 200d 0a0d 0a41 5354 415f 6765 626f  "" ....ASTA_gebo
+00002580: 7265 6e5f 6b6f 7077 7720 3d20 2222 220d  ren_kopww = """.
+00002590: 0a0d 0a28 4072 656c 3d22 6864 2220 616e  ...(@rel="hd" an
+000025a0: 6420 4070 743d 2277 7722 2061 6e64 2028  d @pt="ww" and (
+000025b0: 406c 656d 6d61 3d22 7a69 6a6e 2220 6f72  @lemma="zijn" or
+000025c0: 2040 6c65 6d6d 613d 2277 6f72 6465 6e22   @lemma="worden"
+000025d0: 2920 616e 640d 0a20 2020 2020 2020 2020  ) and..         
+000025e0: 282e 2e2f 6e6f 6465 5b40 6361 743d 2270  (../node[@cat="p
+000025f0: 7061 7274 2220 616e 6420 4072 656c 3d22  part" and @rel="
+00002600: 7663 2220 616e 6420 6e6f 6465 5b20 4077  vc" and node[ @w
+00002610: 6f72 643d 2267 6562 6f72 656e 2220 616e  ord="geboren" an
+00002620: 6420 4072 656c 3d22 6864 225d 5d20 6f72  d @rel="hd"]] or
+00002630: 0d0a 0909 2020 2e2e 2f6e 6f64 655b 4072  ....  ../node[@r
+00002640: 656c 3d22 7663 2220 616e 6420 4077 6f72  el="vc" and @wor
+00002650: 643d 2267 6562 6f72 656e 225d 0d0a 0909  d="geboren"]....
+00002660: 2029 0d0a 290d 0a09 2222 220d 0a0d 0a41   )..)..."""....A
+00002670: 5354 415f 7761 6e74 6d61 6172 6269 6a7a  STA_wantmaarbijz
+00002680: 696e 203d 2022 2222 0d0a 2020 2020 2020  in = """..      
+00002690: 2028 2840 776f 7264 3d22 7761 6e74 2220   ((@word="want" 
+000026a0: 6f72 2040 776f 7264 3d22 6d61 6172 2229  or @word="maar")
+000026b0: 2061 6e64 2040 7265 6c3d 2263 7264 2220   and @rel="crd" 
+000026c0: 616e 6420 4070 743d 2276 6722 2061 6e64  and @pt="vg" and
+000026d0: 0d0a 2020 2020 2020 2020 2e2e 2f6e 6f64  ..        ../nod
+000026e0: 655b 2828 4063 6174 3d22 736d 6169 6e22  e[((@cat="smain"
+000026f0: 206f 7220 4063 6174 3d22 7373 7562 2220   or @cat="ssub" 
+00002700: 6f72 2028 4063 6174 3d22 6475 2220 616e  or (@cat="du" an
+00002710: 6420 6e6f 6465 5b40 6361 743d 2273 6d61  d node[@cat="sma
+00002720: 696e 2220 616e 6420 4072 656c 3d22 6e75  in" and @rel="nu
+00002730: 636c 225d 2929 2920 616e 6420 0d0a 0920  cl"]))) and ... 
+00002740: 2020 2040 6265 6769 6e20 203e 3d2e 2e2f     @begin  >=../
+00002750: 6e6f 6465 5b28 4077 6f72 643d 2277 616e  node[(@word="wan
+00002760: 7422 206f 7220 4077 6f72 643d 226d 6161  t" or @word="maa
+00002770: 7222 295d 2f40 656e 645d 0d0a 0920 2020  r")]/@end]...   
+00002780: 290d 0a22 2222 0d0a 0d0a 4153 5441 5f77  ).."""....ASTA_w
+00002790: 616e 746d 6161 7262 696a 7a69 6e7a 696e  antmaarbijzinzin
+000027a0: 203d 2022 2222 0d0a 2020 2020 2020 2028   = """..       (
+000027b0: 2028 4063 6174 3d22 736d 6169 6e22 206f   (@cat="smain" o
+000027c0: 7220 4063 6174 3d20 2273 7375 6222 206f  r @cat= "ssub" o
+000027d0: 7220 2840 6361 743d 2264 7522 2061 6e64  r (@cat="du" and
+000027e0: 206e 6f64 655b 4063 6174 3d22 736d 6169   node[@cat="smai
+000027f0: 6e22 2061 6e64 2040 7265 6c3d 226e 7563  n" and @rel="nuc
+00002800: 6c22 5d29 2920 616e 640d 0a09 2020 2020  l"])) and...    
+00002810: 202e 2e2f 6e6f 6465 5b28 4077 6f72 643d   ../node[(@word=
+00002820: 2277 616e 7422 206f 7220 4077 6f72 643d  "want" or @word=
+00002830: 226d 6161 7222 2920 616e 6420 4072 656c  "maar") and @rel
+00002840: 3d22 6372 6422 2061 6e64 2040 7074 3d22  ="crd" and @pt="
+00002850: 7667 225d 2061 6e64 200d 0a09 0920 4062  vg"] and .... @b
+00002860: 6567 696e 2020 3e3d 2e2e 2f6e 6f64 655b  egin  >=../node[
+00002870: 2840 776f 7264 3d22 7761 6e74 2220 6f72  (@word="want" or
+00002880: 2040 776f 7264 3d22 6d61 6172 2229 5d2f   @word="maar")]/
+00002890: 4065 6e64 0d0a 0920 2020 290d 0a22 2222  @end...   ).."""
+000028a0: 0d0a 0d0a 0d0a 4153 5441 5f64 7573 6269  ......ASTA_dusbi
+000028b0: 6a7a 696e 203d 2022 2222 0d0a 2840 6c65  jzin = """..(@le
+000028c0: 6d6d 613d 2264 7573 2220 616e 6420 7061  mma="dus" and pa
+000028d0: 7265 6e74 3a3a 6e6f 6465 5b40 6361 743d  rent::node[@cat=
+000028e0: 2273 6d61 696e 225d 2061 6e64 2020 4062  "smain"] and  @b
+000028f0: 6567 696e 3d70 6172 656e 743a 3a6e 6f64  egin=parent::nod
+00002900: 652f 4062 6567 696e 2061 6e64 2040 7074  e/@begin and @pt
+00002910: 3d22 6277 2220 616e 6420 4072 656c 3d22  ="bw" and @rel="
+00002920: 6d6f 6422 290d 0a22 2222 0d0a 0d0a 4153  mod").."""....AS
+00002930: 5441 5f64 7573 6269 6a7a 696e 7a69 6e20  TA_dusbijzinzin 
+00002940: 3d20 2222 220d 0a28 4063 6174 3d22 736d  = """..(@cat="sm
+00002950: 6169 6e22 2061 6e64 206e 6f64 655b 406c  ain" and node[@l
+00002960: 656d 6d61 3d22 6475 7322 2020 616e 6420  emma="dus"  and 
+00002970: 2040 6265 6769 6e3d 7061 7265 6e74 3a3a   @begin=parent::
+00002980: 6e6f 6465 2f40 6265 6769 6e20 616e 6420  node/@begin and 
+00002990: 4070 743d 2262 7722 2061 6e64 2040 7265  @pt="bw" and @re
+000029a0: 6c3d 226d 6f64 225d 290d 0a22 2222 0d0a  l="mod"]).."""..
+000029b0: 0d0a 0d0a 200d 0a41 5354 415f 6465 7461  .... ..ASTA_deta
+000029c0: 646a 7320 3d20 2222 220d 0a20 2840 7074  djs = """.. (@pt
+000029d0: 3d22 766e 7722 2061 6e64 2028 4072 656c  ="vnw" and (@rel
+000029e0: 3d22 6d6f 6422 206f 7220 4072 656c 3d22  ="mod" or @rel="
+000029f0: 6465 7422 2920 616e 6420 4076 7774 7970  det") and @vwtyp
+00002a00: 653d 226f 6e62 6570 2220 616e 6420 7061  e="onbep" and pa
+00002a10: 7265 6e74 3a3a 6e6f 6465 5b40 6361 743d  rent::node[@cat=
+00002a20: 226e 7022 5d20 616e 640d 0a28 406c 656d  "np"] and..(@lem
+00002a30: 6d61 3d22 616c 2220 6f72 2040 6c65 6d6d  ma="al" or @lemm
+00002a40: 613d 2262 6569 6465 2220 6f72 2040 6c65  a="beide" or @le
+00002a50: 6d6d 613d 2265 6c6b 2220 6f72 2040 6c65  mma="elk" or @le
+00002a60: 6d6d 613d 2265 6e69 6722 206f 7220 406c  mma="enig" or @l
+00002a70: 656d 6d61 3d22 656e 6b65 6c22 206f 7220  emma="enkel" or 
+00002a80: 406c 656d 6d61 3d22 6765 656e 2220 6f72  @lemma="geen" or
+00002a90: 2040 6c65 6d6d 613d 2269 6564 6572 2220   @lemma="ieder" 
+00002aa0: 6f72 0d0a 2040 6c65 6d6d 613d 226d 6565  or.. @lemma="mee
+00002ab0: 7222 206f 7220 406c 656d 6d61 3d22 6d65  r" or @lemma="me
+00002ac0: 6572 6465 7265 2220 6f72 2040 6c65 6d6d  erdere" or @lemm
+00002ad0: 613d 226d 6565 7374 2220 6f72 2040 6c65  a="meest" or @le
+00002ae0: 6d6d 613d 226d 656e 6967 2220 6f72 2040  mma="menig" or @
+00002af0: 6c65 6d6d 613d 226d 696e 6465 7222 206f  lemma="minder" o
+00002b00: 7220 0d0a 2040 6c65 6d6d 613d 226d 696e  r .. @lemma="min
+00002b10: 7374 2220 6f72 2040 6c65 6d6d 613d 2273  st" or @lemma="s
+00002b20: 6f6d 6d69 6765 2220 6f72 2040 6c65 6d6d  ommige" or @lemm
+00002b30: 613d 2276 6565 6c22 206f 7220 406c 656d  a="veel" or @lem
+00002b40: 6d61 3d22 7765 696e 6967 2229 290d 0a0d  ma="weinig"))...
+00002b50: 0a22 2222 0d0a 0d0a 5461 7273 705f 6b69  ."""....Tarsp_ki
+00002b60: 6a6b 6565 6e73 203d 2022 2222 0d0a 2840  jkeens = """..(@
+00002b70: 6361 743d 2273 7631 2220 616e 6420 4072  cat="sv1" and @r
+00002b80: 656c 2021 3d20 222d 2d22 2061 6e64 0d0a  el != "--" and..
+00002b90: 2020 2020 6e6f 6465 5b40 7074 3d22 7777      node[@pt="ww
+00002ba0: 2220 616e 6420 406c 656d 6d61 3d22 6b69  " and @lemma="ki
+00002bb0: 6a6b 656e 2220 616e 6420 4072 656c 3d22  jken" and @rel="
+00002bc0: 6864 2220 2061 6e64 2040 7076 6167 723d  hd"  and @pvagr=
+00002bd0: 2265 7622 2061 6e64 2040 7076 7469 6a64  "ev" and @pvtijd
+00002be0: 3d22 7467 7722 205d 2061 6e64 0d0a 2020  ="tgw" ] and..  
+00002bf0: 2020 6e6f 6465 5b40 6c65 6d6d 613d 2265    node[@lemma="e
+00002c00: 656e 7322 2061 6e64 2040 7265 6c3d 226d  ens" and @rel="m
+00002c10: 6f64 2220 616e 6420 4070 743d 2262 7722  od" and @pt="bw"
+00002c20: 5d20 616e 6420 636f 756e 7428 6e6f 6465  ] and count(node
+00002c30: 293d 3229 200d 0a22 2222 0d0a 0d0a 4153  )=2) .."""....AS
+00002c40: 5441 5f6e 756d 6572 616c 203d 2022 2222  TA_numeral = """
+00002c50: 0d0a 2840 6c65 6d6d 613d 2274 7765 6522  ..(@lemma="twee"
+00002c60: 206f 7220 406c 656d 6d61 3d22 6472 6965   or @lemma="drie
+00002c70: 2220 6f72 2040 6c65 6d6d 613d 2276 6965  " or @lemma="vie
+00002c80: 7222 206f 7220 406c 656d 6d61 3d22 7669  r" or @lemma="vi
+00002c90: 6a66 2220 6f72 2040 6c65 6d6d 613d 227a  jf" or @lemma="z
+00002ca0: 6573 2220 6f72 2040 6c65 6d6d 613d 227a  es" or @lemma="z
+00002cb0: 6576 656e 2220 6f72 2040 6c65 6d6d 613d  even" or @lemma=
+00002cc0: 2261 6368 7422 206f 7220 406c 656d 6d61  "acht" or @lemma
+00002cd0: 3d22 6e65 6765 6e22 206f 7220 406c 656d  ="negen" or @lem
+00002ce0: 6d61 3d22 7469 656e 2220 6f72 2040 6c65  ma="tien" or @le
+00002cf0: 6d6d 613d 2265 6c66 2220 6f72 2040 6c65  mma="elf" or @le
+00002d00: 6d6d 613d 2274 7761 616c 6622 206f 7220  mma="twaalf" or 
+00002d10: 406c 656d 6d61 3d22 6465 7274 6965 6e22  @lemma="dertien"
+00002d20: 206f 7220 406c 656d 6d61 3d22 7665 6572   or @lemma="veer
+00002d30: 7469 656e 2220 6f72 2040 6c65 6d6d 613d  tien" or @lemma=
+00002d40: 2276 696a 6674 6965 6e22 206f 7220 406c  "vijftien" or @l
+00002d50: 656d 6d61 3d22 7a65 7374 6965 6e22 206f  emma="zestien" o
+00002d60: 7220 406c 656d 6d61 3d22 7a65 7665 6e74  r @lemma="zevent
+00002d70: 6965 6e22 206f 7220 406c 656d 6d61 3d22  ien" or @lemma="
+00002d80: 6163 6874 7469 656e 2220 6f72 2040 6c65  achttien" or @le
+00002d90: 6d6d 613d 226e 6567 656e 7469 656e 2220  mma="negentien" 
+00002da0: 6f72 2040 6c65 6d6d 613d 2274 7769 6e74  or @lemma="twint
+00002db0: 6967 2220 6f72 2040 6c65 6d6d 613d 2265  ig" or @lemma="e
+00002dc0: 656e 746a 6522 206f 7220 2040 6c65 6d6d  entje" or  @lemm
+00002dd0: 613d 2274 7765 6574 6a65 7322 206f 7220  a="tweetjes" or 
+00002de0: 406c 656d 6d61 3d22 6472 6965 746a 6573  @lemma="drietjes
+00002df0: 2220 6f72 2040 6c65 6d6d 613d 2276 6965  " or @lemma="vie
+00002e00: 7274 6a65 7322 206f 7220 406c 656d 6d61  rtjes" or @lemma
+00002e10: 3d22 7669 6a66 6a65 7322 206f 7220 406c  ="vijfjes" or @l
+00002e20: 656d 6d61 3d22 7a65 736a 6573 2229 200d  emma="zesjes") .
+00002e30: 0a22 2222 200d 0a0d 0a41 5354 415f 6669  .""" ....ASTA_fi
+00002e40: 6c6c 6564 5f70 6175 7365 203d 2022 2222  lled_pause = """
+00002e50: 0d0a 2840 6c65 6d6d 613d 2022 7568 2220  ..(@lemma= "uh" 
+00002e60: 6f72 2040 6c65 6d6d 6120 3d22 5568 2220  or @lemma ="Uh" 
+00002e70: 6f72 2040 6c65 6d6d 613d 2255 686d 2220  or @lemma="Uhm" 
+00002e80: 6f72 2040 6c65 6d6d 613d 2022 7568 6d22  or @lemma= "uhm"
+00002e90: 206f 7220 2040 6c65 6d6d 6120 3d20 2265   or  @lemma = "e
+00002ea0: 7568 2220 6f72 2040 6c65 6d6d 6120 3d20  uh" or @lemma = 
+00002eb0: 2265 6822 206f 7220 406c 656d 6d61 203d  "eh" or @lemma =
+00002ec0: 2022 676f 6822 206f 7220 4077 6f72 643d   "goh" or @word=
+00002ed0: 2278 7878 2220 6f72 2040 776f 7264 3d22  "xxx" or @word="
+00002ee0: 5858 5822 206f 7220 406c 656d 6d61 3d22  XXX" or @lemma="
+00002ef0: 6767 2220 6f72 200d 0a20 2040 6c65 6d6d  gg" or ..  @lemm
+00002f00: 613d 2262 7568 2220 6f72 2040 6c65 6d6d  a="buh" or @lemm
+00002f10: 613d 2273 7373 2220 6f72 2040 6c65 6d6d  a="sss" or @lemm
+00002f20: 613d 2270 6622 206f 7220 406c 656d 6d61  a="pf" or @lemma
+00002f30: 3d27 7461 626c 6161 2720 290d 0a22 2222  ='tablaa' ).."""
+00002f40: 0d0a 0d0a 4153 5441 5f67 6562 6f72 656e  ....ASTA_geboren
+00002f50: 203d 2022 2222 2028 4077 6f72 643d 2267   = """ (@word="g
+00002f60: 6562 6f72 656e 2229 2022 2222 0d0a 0d0a  eboren") """....
+00002f70: 4276 5a6e 203d 2022 2222 2028 636f 756e  BvZn = """ (coun
+00002f80: 7428 6e6f 6465 293d 3220 616e 640d 0a20  t(node)=2 and.. 
+00002f90: 2020 2020 2020 2020 2020 2028 2020 2825             (  (%
+00002fa0: 6865 6164 6e25 2061 6e64 2028 2563 6f72  headn% and (%cor
+00002fb0: 6561 646a 6d6f 6425 206f 7220 2563 6f72  eadjmod% or %cor
+00002fc0: 6576 6e77 6d6f 6425 206f 7220 2563 6f72  evnwmod% or %cor
+00002fd0: 6562 776d 6f64 2529 2920 0d0a 0d0a 0909  ebwmod%)) ......
+00002fe0: 2020 2020 290d 0a09 0920 2020 2909 0d0a      )....   )...
+00002ff0: 2222 220d 0a0d 0a71 6277 6c65 6d6d 6120  """....qbwlemma 
+00003000: 3d20 2222 2220 2840 6c65 6d6d 613d 226e  = """ (@lemma="n
+00003010: 6f67 2220 2920 2222 220d 0a0d 0a0d 0a69  og" ) """......i
+00003020: 6574 7361 646a 7320 3d20 2222 2228 6e6f  etsadjs = """(no
+00003030: 6465 5b40 7265 6c3d 2268 6422 2061 6e64  de[@rel="hd" and
+00003040: 2040 7074 3d22 766e 7722 5d20 616e 6420   @pt="vnw"] and 
+00003050: 6e6f 6465 5b40 7265 6c3d 226d 6f64 2220  node[@rel="mod" 
+00003060: 616e 6420 2561 646a 7325 5d29 0d0a 2222  and %adjs%])..""
+00003070: 220d 0a0d 0a61 646a 7320 3d20 2222 2220  "....adjs = """ 
+00003080: 2840 7074 3d22 6164 6a22 2061 6e64 2040  (@pt="adj" and @
+00003090: 6275 6967 696e 673d 226d 6574 2d73 2229  buiging="met-s")
+000030a0: 2022 2222 0d0a 0d0a 6170 7320 3d20 2222   """....aps = ""
+000030b0: 2220 2840 6361 743d 2261 7022 2061 6e64  " (@cat="ap" and
+000030c0: 206e 6f64 655b 4072 656c 3d22 6864 2220   node[@rel="hd" 
+000030d0: 616e 6420 2561 646a 7325 5d29 2022 2222  and %adjs%]) """
+000030e0: 0d0a 0d0a 6865 6164 6e20 3d20 2222 2220  ....headn = """ 
+000030f0: 2820 6e6f 6465 5b40 7265 6c3d 2268 6422  ( node[@rel="hd"
+00003100: 2061 6e64 2040 7074 3d22 6e22 5d20 2922   and @pt="n"] )"
+00003110: 2222 0d0a 0d0a 636f 7265 6164 6a6d 6f64  ""....coreadjmod
+00003120: 203d 2022 2222 2028 6e6f 6465 5b40 7265   = """ (node[@re
+00003130: 6c3d 226d 6f64 2220 616e 6420 2820 4070  l="mod" and ( @p
+00003140: 743d 2261 646a 2220 6f72 2040 7074 3d22  t="adj" or @pt="
+00003150: 7477 2229 5d20 616e 6420 6e6f 7428 6e6f  tw")] and not(no
+00003160: 6465 5b40 7265 6c3d 2264 6574 225d 2929  de[@rel="det"]))
+00003170: 2022 2222 0d0a 0d0a 636f 7265 766e 776d   """....corevnwm
+00003180: 6f64 203d 2022 2222 2028 6e6f 6465 5b40  od = """ (node[@
+00003190: 7265 6c3d 2264 6574 2220 616e 6420 2840  rel="det" and (@
+000031a0: 7074 3d22 7477 2220 6f72 2028 4070 743d  pt="tw" or (@pt=
+000031b0: 2276 6e77 2220 616e 6420 4076 7774 7970  "vnw" and @vwtyp
+000031c0: 653d 226f 6e62 6570 2220 616e 6420 406e  e="onbep" and @n
+000031d0: 6161 6d76 616c 213d 2267 656e 2220 616e  aamval!="gen" an
+000031e0: 6420 406c 656d 6d61 213d 2267 6565 6e22  d @lemma!="geen"
+000031f0: 2929 5d20 2922 2222 0d0a 0d0a 0d0a 636f  ))] )"""......co
+00003200: 7265 6277 6d6f 6420 3d20 2222 2220 286e  rebwmod = """ (n
+00003210: 6f64 655b 4072 656c 3d22 6d6f 6422 2061  ode[@rel="mod" a
+00003220: 6e64 2040 7074 3d22 6277 2220 616e 6420  nd @pt="bw" and 
+00003230: 2571 6277 6c65 6d6d 6125 5d29 2022 2222  %qbwlemma%]) """
+00003240: 0d0a 0d0a 0d0a 7370 6563 5f70 726f 7065  ......spec_prope
+00003250: 725f 6e61 6d65 203d 2022 2222 2028 4070  r_name = """ (@p
+00003260: 743d 2273 7065 6322 2061 6e64 200d 0a20  t="spec" and .. 
+00003270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003280: 2020 2020 2020 2028 4070 6f73 3d22 6e61         (@pos="na
+00003290: 6d65 2220 6f72 2073 7461 7274 732d 7769  me" or starts-wi
+000032a0: 7468 2840 6672 616d 652c 2270 726f 7065  th(@frame,"prope
+000032b0: 725f 6e61 6d65 2229 2920 616e 640d 0a20  r_name")) and.. 
 000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032d0: 2020 2020 2029 2022 2222 090d 0a0d 0a73       ) """.....s
-000032e0: 7065 635f 6e6f 756e 203d 2022 2222 2028  pec_noun = """ (
-000032f0: 4070 743d 2273 7065 6322 2061 6e64 2028  @pt="spec" and (
-00003300: 4070 6f73 3d22 6e61 6d65 2220 6f72 2073  @pos="name" or s
-00003310: 7461 7274 732d 7769 7468 2840 6672 616d  tarts-with(@fram
-00003320: 652c 2270 726f 7065 725f 6e61 6d65 2229  e,"proper_name")
-00003330: 2920 2922 2222 0909 0909 0920 2020 0d0a  ) )""".....   ..
-00003340: 200d 0a20 0d0a 2041 5354 415f 4c45 5820   .. .. ASTA_LEX 
-00003350: 3d20 2222 2220 280d 0a20 2020 2020 2020  = """ (..       
-00003360: 6e6f 7428 2541 5354 415f 6765 626f 7265  not(%ASTA_gebore
-00003370: 6e25 2920 616e 640d 0a09 2020 206e 6f74  n%) and...   not
-00003380: 2825 6173 7461 5f61 646a 2529 2061 6e64  (%asta_adj%) and
-00003390: 0d0a 2020 2020 2020 2040 7074 3d22 7777  ..       @pt="ww
-000033a0: 2220 616e 6420 0d0a 2020 2020 2020 206e  " and ..       n
-000033b0: 6f74 2825 4153 5441 5f6b 6f70 7777 2529  ot(%ASTA_kopww%)
-000033c0: 2020 2061 6e64 200d 0a09 2020 206e 6f74     and ...   not
-000033d0: 2825 4153 5441 5f6d 6f64 616c 7777 2529  (%ASTA_modalww%)
-000033e0: 2061 6e64 200d 0a09 2020 206e 6f74 2840   and ...   not(@
-000033f0: 6c65 6d6d 613d 227a 696a 6e22 2920 616e  lemma="zijn") an
-00003400: 6420 0d0a 0920 2020 6e6f 7428 636f 6e74  d ...   not(cont
-00003410: 6169 6e73 2840 6c65 6d6d 612c 2022 5f7a  ains(@lemma, "_z
-00003420: 696a 6e22 2929 2061 6e64 200d 0a09 2020  ijn")) and ...  
-00003430: 206e 6f74 2840 706f 7369 7469 653d 226e   not(@positie="n
-00003440: 6f6d 2229 2061 6e64 0d0a 0920 2020 286e  om") and...   (n
-00003450: 6f74 2840 6c65 6d6d 613d 2268 6562 6265  ot(@lemma="hebbe
-00003460: 6e22 2920 6f72 202e 2e2f 6e6f 6465 5b40  n") or ../node[@
-00003470: 7265 6c3d 226f 626a 3122 5d20 2920 616e  rel="obj1"] ) an
-00003480: 640d 0a20 2020 2020 2020 6e6f 7428 2020  d..       not(  
-00003490: 2820 406c 656d 6d61 3d22 6865 6262 656e  ( @lemma="hebben
-000034a0: 2220 6f72 2040 6c65 6d6d 613d 227a 696a  " or @lemma="zij
-000034b0: 6e22 206f 7220 406c 656d 6d61 3d22 776f  n" or @lemma="wo
-000034c0: 7264 656e 2220 2029 2061 6e64 2070 6172  rden"  ) and par
-000034d0: 656e 743a 3a6e 6f64 655b 6e6f 6465 5b40  ent::node[node[@
-000034e0: 7265 6c3d 2276 6322 5d5d 2029 0d0a 2020  rel="vc"]] )..  
-000034f0: 2020 2020 290d 0a20 0d0a 2022 2222 0d0a      ).. .. """..
-00003500: 200d 0a20 6173 7461 5f6e 756d 7672 696a   .. asta_numvrij
-00003510: 203d 2022 2222 2840 7074 3d22 7477 2220   = """(@pt="tw" 
-00003520: 616e 6420 4070 6f73 6974 6965 3d22 7672  and @positie="vr
-00003530: 696a 2220 616e 6420 4072 656c 213d 226d  ij" and @rel!="m
-00003540: 7770 2220 616e 6420 4072 656c 213d 2264  wp" and @rel!="d
-00003550: 6574 2220 616e 6420 4072 656c 213d 226d  et" and @rel!="m
-00003560: 6f64 2220 2922 2222 0d0a 200d 0a20 6173  od" )""".. .. as
-00003570: 7461 5f6e 6f75 6e20 3d20 2222 2220 2828  ta_noun = """ ((
-00003580: 4070 743d 226e 2220 616e 6420 6e6f 7428  @pt="n" and not(
-00003590: 2541 5354 415f 6669 6c6c 6564 5f70 6175  %ASTA_filled_pau
-000035a0: 7365 2529 2061 6e64 206e 6f74 2825 4153  se%) and not(%AS
-000035b0: 5441 5f6e 756d 6572 616c 2529 2920 6f72  TA_numeral%)) or
-000035c0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-000035d0: 2020 2020 2028 4070 743d 2277 7722 2061       (@pt="ww" a
-000035e0: 6e64 2040 706f 7369 7469 653d 226e 6f6d  nd @positie="nom
-000035f0: 2229 206f 7220 0d0a 0909 0909 2020 2825  ") or ......  (%
-00003600: 6d6f 6e74 686e 616d 6525 2920 6f72 200d  monthname%) or .
-00003610: 0a09 0909 0920 2040 706f 733d 226e 616d  .....  @pos="nam
-00003620: 6522 2029 0d0a 2022 2222 0d0a 0d0a 0d0a  e" ).. """......
-00003630: 6173 7461 5f61 646a 203d 2022 2222 0d0a  asta_adj = """..
-00003640: 2020 2020 2825 4153 5441 5f67 6562 6f72      (%ASTA_gebor
-00003650: 656e 2520 6f72 0d0a 2020 2020 2025 6174  en% or..     %at
-00003660: 7472 6962 7574 6976 655f 6164 6a25 206f  tributive_adj% o
-00003670: 720d 0a20 2020 2020 2561 7474 7269 6275  r..     %attribu
-00003680: 7469 7665 5f61 646a 696e 6164 6a70 2520  tive_adjinadjp% 
-00003690: 6f72 0d0a 2020 2020 2025 7261 6e67 7477  or..     %rangtw
-000036a0: 2520 6f72 0d0a 2020 2020 2025 7375 6273  % or..     %subs
-000036b0: 7461 6e74 6976 6973 6564 6164 6a25 206f  tantivisedadj% o
-000036c0: 720d 0a20 2020 2020 2573 7562 7374 616e  r..     %substan
-000036d0: 7469 7669 7365 6472 616e 6774 7725 206f  tivisedrangtw% o
-000036e0: 720d 0a09 2025 6174 7472 6962 7574 6976  r... %attributiv
-000036f0: 655f 7061 7374 7025 206f 720d 0a09 2025  e_pastp% or... %
-00003700: 6174 7472 6962 7574 6976 655f 7072 6573  attributive_pres
-00003710: 7025 206f 720d 0a09 2025 7369 6d70 6c65  p% or... %simple
-00003720: 7072 6564 6963 6174 6976 655f 6164 6a25  predicative_adj%
-00003730: 206f 720d 0a09 2025 7369 6d70 6c65 7072   or... %simplepr
-00003740: 6564 6963 6174 6976 655f 6164 6a69 6e61  edicative_adjina
-00003750: 646a 7025 206f 720d 0a09 2025 696e 6465  djp% or... %inde
-00003760: 6664 6574 2520 0d0a 0929 0d0a 2222 220d  fdet% ...)..""".
-00003770: 0a0d 0a61 646a 7061 7374 7061 7274 203d  ...adjpastpart =
-00003780: 2022 2222 2840 7074 3d22 7777 2220 616e   """(@pt="ww" an
-00003790: 6420 4077 766f 726d 3d22 7664 2220 616e  d @wvorm="vd" an
-000037a0: 6420 4070 6f73 3d22 6164 6a22 2061 6e64  d @pos="adj" and
-000037b0: 2040 7265 6c3d 2270 7265 6463 2220 2922   @rel="predc" )"
-000037c0: 2222 0d0a 0d0a 6174 7472 6962 7574 6976  ""....attributiv
-000037d0: 655f 6164 6a20 3d20 2222 2220 0d0a 2020  e_adj = """ ..  
-000037e0: 2020 2840 7074 3d22 6164 6a22 2061 6e64    (@pt="adj" and
-000037f0: 200d 0a20 2020 2020 2840 7265 6c3d 226d   ..     (@rel="m
-00003800: 6f64 2220 616e 6420 0d0a 2020 2020 2020  od" and ..      
-00003810: 7061 7265 6e74 3a3a 6e6f 6465 5b40 6361  parent::node[@ca
-00003820: 743d 226e 7022 5d20 616e 6420 0d0a 2020  t="np"] and ..  
-00003830: 2020 2020 2e2e 2f6e 6f64 655b 4072 656c      ../node[@rel
-00003840: 3d22 6864 2220 616e 6420 2840 7074 3d22  ="hd" and (@pt="
-00003850: 6e22 206f 7220 4070 743d 2276 6e77 2220  n" or @pt="vnw" 
-00003860: 6f72 2040 6361 743d 226d 7775 2229 5d20  or @cat="mwu")] 
-00003870: 616e 640d 0a09 2020 286e 6f74 2840 6265  and...  (not(@be
-00003880: 6769 6e20 3c20 2e2e 2f6e 6f64 655b 4072  gin < ../node[@r
-00003890: 656c 3d22 6465 7422 2061 6e64 2028 4070  el="det" and (@p
-000038a0: 743d 226c 6964 2220 6f72 2040 7074 3d22  t="lid" or @pt="
-000038b0: 766e 7722 295d 2f40 6265 6769 6e29 206f  vnw")]/@begin) o
-000038c0: 7220 406c 656d 6d61 3d27 6865 656c 2720  r @lemma='heel' 
-000038d0: 6f72 2040 6c65 6d6d 613d 2767 6568 6565  or @lemma='gehee
-000038e0: 6c27 290d 0a09 2029 0d0a 0929 0d0a 2222  l')... )...)..""
-000038f0: 220d 0a0d 0a61 7474 7269 6275 7469 7665  "....attributive
-00003900: 5f61 646a 696e 6164 6a70 203d 2022 2222  _adjinadjp = """
-00003910: 0d0a 2020 2028 4070 743d 2261 646a 2220  ..   (@pt="adj" 
-00003920: 616e 640d 0a20 2020 2028 4072 656c 3d22  and..    (@rel="
-00003930: 6864 2220 616e 640d 0a20 2020 2020 7061  hd" and..     pa
-00003940: 7265 6e74 3a3a 6e6f 6465 5b40 6361 743d  rent::node[@cat=
-00003950: 2261 7022 2061 6e64 2070 6172 656e 743a  "ap" and parent:
-00003960: 3a6e 6f64 655b 4063 6174 3d22 6e70 225d  :node[@cat="np"]
-00003970: 2061 6e64 200d 0a20 2020 2020 2e2e 2f6e   and ..     ../n
-00003980: 6f64 655b 4072 656c 3d22 6864 2220 616e  ode[@rel="hd" an
-00003990: 6420 2840 7074 3d22 6e22 206f 7220 4070  d (@pt="n" or @p
-000039a0: 743d 2276 6e77 2220 6f72 2040 6361 743d  t="vnw" or @cat=
-000039b0: 226d 7775 2229 5d5d 0d0a 0920 290d 0a09  "mwu")]]... )...
-000039c0: 290d 0a22 2222 0d0a 0d0a 7261 6e67 7477  ).."""....rangtw
-000039d0: 203d 2022 2222 0d0a 2020 2028 4070 743d   = """..   (@pt=
-000039e0: 2274 7722 2061 6e64 2040 6e75 6d74 7970  "tw" and @numtyp
-000039f0: 653d 2272 616e 6722 290d 0a22 2222 0d0a  e="rang").."""..
-00003a00: 0d0a 7375 6273 7461 6e74 6976 6973 6564  ..substantivised
-00003a10: 6164 6a20 3d20 2222 2220 0d0a 2020 2028  adj = """ ..   (
-00003a20: 4070 743d 2261 646a 2220 616e 6420 4072  @pt="adj" and @r
-00003a30: 656c 3d22 6864 2220 616e 6420 7061 7265  el="hd" and pare
-00003a40: 6e74 3a3a 6e6f 6465 5b40 6361 743d 226e  nt::node[@cat="n
-00003a50: 7022 5d29 0d0a 2222 220d 0a0d 0a73 7562  p"]).."""....sub
-00003a60: 7374 616e 7469 7669 7365 6472 616e 6774  stantivisedrangt
-00003a70: 7720 3d20 2222 220d 0a20 2020 2028 2572  w = """..    (%r
-00003a80: 616e 6774 7725 2061 6e64 2040 706f 7369  angtw% and @posi
-00003a90: 7469 6520 3d20 226e 6f6d 2220 290d 0a22  tie = "nom" ).."
-00003aa0: 2222 0d0a 0d0a 6174 7472 6962 7574 6976  ""....attributiv
-00003ab0: 655f 7061 7374 7020 3d20 2222 220d 0a20  e_pastp = """.. 
-00003ac0: 2020 2840 7074 3d22 7777 2220 616e 6420    (@pt="ww" and 
-00003ad0: 4077 766f 726d 3d22 7664 2220 616e 6420  @wvorm="vd" and 
-00003ae0: 4072 656c 3d22 6d6f 6422 2061 6e64 2070  @rel="mod" and p
-00003af0: 6172 656e 743a 3a6e 6f64 655b 4063 6174  arent::node[@cat
-00003b00: 3d22 6e70 225d 290d 0a22 2222 0d0a 0d0a  ="np"]).."""....
-00003b10: 6174 7472 6962 7574 6976 655f 7072 6573  attributive_pres
-00003b20: 7020 3d20 2222 220d 0a20 2020 2840 7074  p = """..   (@pt
-00003b30: 3d22 7777 2220 616e 6420 4077 766f 726d  ="ww" and @wvorm
-00003b40: 3d22 6f64 2220 616e 6420 4072 656c 3d22  ="od" and @rel="
-00003b50: 6d6f 6422 2061 6e64 2070 6172 656e 743a  mod" and parent:
-00003b60: 3a6e 6f64 655b 4063 6174 3d22 6e70 225d  :node[@cat="np"]
-00003b70: 290d 0a22 2222 0d0a 0d0a 7072 6564 6963  ).."""....predic
-00003b80: 6174 6976 6520 3d20 2222 2220 2840 7265  ative = """ (@re
-00003b90: 6c3d 2270 7265 6463 2220 6f72 2040 7265  l="predc" or @re
-00003ba0: 6c3d 2270 7265 646d 2220 2920 2222 220d  l="predm" ) """.
-00003bb0: 0a0d 0a73 696d 706c 6570 7265 6469 6361  ...simplepredica
-00003bc0: 7469 7665 203d 2022 2222 2028 2570 7265  tive = """ (%pre
-00003bd0: 6469 6361 7469 7665 2520 616e 6420 2e2e  dicative% and ..
-00003be0: 2f6e 6f64 655b 2541 5354 415f 6261 7369  /node[%ASTA_basi
-00003bf0: 636b 6f70 7777 255d 290d 0a22 2222 0d0a  ckopww%]).."""..
-00003c00: 0d0a 7369 6d70 6c65 7072 6564 6963 6174  ..simplepredicat
-00003c10: 6976 655f 6164 6a20 3d20 2222 220d 0a20  ive_adj = """.. 
-00003c20: 2020 2020 2840 7074 3d22 6164 6a22 2061      (@pt="adj" a
-00003c30: 6e64 2025 7369 6d70 6c65 7072 6564 6963  nd %simplepredic
-00003c40: 6174 6976 6525 290d 0a22 2222 0d0a 0920  ative%).."""... 
-00003c50: 0d0a 7369 6d70 6c65 7072 6564 6963 6174  ..simplepredicat
-00003c60: 6976 655f 6164 6a69 6e61 646a 7020 3d20  ive_adjinadjp = 
-00003c70: 2222 220d 0a20 2020 2020 2840 7074 3d22  """..     (@pt="
-00003c80: 6164 6a22 2061 6e64 2040 7265 6c3d 2268  adj" and @rel="h
-00003c90: 6422 2061 6e64 2070 6172 656e 743a 3a6e  d" and parent::n
-00003ca0: 6f64 655b 4063 6174 3d22 6170 2220 616e  ode[@cat="ap" an
+000032d0: 2020 2020 2020 2028 636f 6e74 6169 6e73         (contains
+000032e0: 2822 4142 4344 4546 4748 494a 4b4c 4d4e  ("ABCDEFGHIJKLMN
+000032f0: 4f50 5152 5354 5556 5758 595a 222c 2073  OPQRSTUVWXYZ", s
+00003300: 7562 7374 7269 6e67 2840 776f 7264 2c31  ubstring(@word,1
+00003310: 2c31 2929 290d 0a20 2020 2020 2020 2020  ,1)))..         
+00003320: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+00003330: 2222 2209 0d0a 0d0a 7370 6563 5f6e 6f75  """.....spec_nou
+00003340: 6e20 3d20 2222 2220 2840 7074 3d22 7370  n = """ (@pt="sp
+00003350: 6563 2220 616e 6420 2840 706f 733d 226e  ec" and (@pos="n
+00003360: 616d 6522 206f 7220 7374 6172 7473 2d77  ame" or starts-w
+00003370: 6974 6828 4066 7261 6d65 2c22 7072 6f70  ith(@frame,"prop
+00003380: 6572 5f6e 616d 6522 2929 2029 2222 2209  er_name")) )""".
+00003390: 0909 0909 2020 200d 0a20 0d0a 200d 0a20  ....   .. .. .. 
+000033a0: 4153 5441 5f4c 4558 203d 2022 2222 2028  ASTA_LEX = """ (
+000033b0: 0d0a 2020 2020 2020 206e 6f74 2825 4153  ..       not(%AS
+000033c0: 5441 5f67 6562 6f72 656e 2529 2061 6e64  TA_geboren%) and
+000033d0: 0d0a 0920 2020 6e6f 7428 2561 7374 615f  ...   not(%asta_
+000033e0: 6164 6a25 2920 616e 640d 0a20 2020 2020  adj%) and..     
+000033f0: 2020 4070 743d 2277 7722 2061 6e64 200d    @pt="ww" and .
+00003400: 0a20 2020 2020 2020 6e6f 7428 2541 5354  .       not(%AST
+00003410: 415f 6b6f 7077 7725 2920 2020 616e 6420  A_kopww%)   and 
+00003420: 0d0a 0920 2020 6e6f 7428 2541 5354 415f  ...   not(%ASTA_
+00003430: 6d6f 6461 6c77 7725 2920 616e 6420 0d0a  modalww%) and ..
+00003440: 0920 2020 6e6f 7428 406c 656d 6d61 3d22  .   not(@lemma="
+00003450: 7a69 6a6e 2229 2061 6e64 200d 0a09 2020  zijn") and ...  
+00003460: 206e 6f74 2863 6f6e 7461 696e 7328 406c   not(contains(@l
+00003470: 656d 6d61 2c20 225f 7a69 6a6e 2229 2920  emma, "_zijn")) 
+00003480: 616e 6420 0d0a 0920 2020 6e6f 7428 4070  and ...   not(@p
+00003490: 6f73 6974 6965 3d22 6e6f 6d22 2920 616e  ositie="nom") an
+000034a0: 640d 0a09 2020 2028 6e6f 7428 406c 656d  d...   (not(@lem
+000034b0: 6d61 3d22 6865 6262 656e 2229 206f 7220  ma="hebben") or 
+000034c0: 2e2e 2f6e 6f64 655b 4072 656c 3d22 6f62  ../node[@rel="ob
+000034d0: 6a31 225d 2029 2061 6e64 0d0a 2020 2020  j1"] ) and..    
+000034e0: 2020 206e 6f74 2820 2028 2040 6c65 6d6d     not(  ( @lemm
+000034f0: 613d 2268 6562 6265 6e22 206f 7220 406c  a="hebben" or @l
+00003500: 656d 6d61 3d22 7a69 6a6e 2220 6f72 2040  emma="zijn" or @
+00003510: 6c65 6d6d 613d 2277 6f72 6465 6e22 2020  lemma="worden"  
+00003520: 2920 616e 6420 7061 7265 6e74 3a3a 6e6f  ) and parent::no
+00003530: 6465 5b6e 6f64 655b 4072 656c 3d22 7663  de[node[@rel="vc
+00003540: 225d 5d20 290d 0a20 2020 2020 2029 0d0a  "]] )..      )..
+00003550: 200d 0a20 2222 220d 0a20 0d0a 2061 7374   .. """.. .. ast
+00003560: 615f 6e75 6d76 7269 6a20 3d20 2222 2228  a_numvrij = """(
+00003570: 4070 743d 2274 7722 2061 6e64 2040 706f  @pt="tw" and @po
+00003580: 7369 7469 653d 2276 7269 6a22 2061 6e64  sitie="vrij" and
+00003590: 2040 7265 6c21 3d22 6d77 7022 2061 6e64   @rel!="mwp" and
+000035a0: 2040 7265 6c21 3d22 6465 7422 2061 6e64   @rel!="det" and
+000035b0: 2040 7265 6c21 3d22 6d6f 6422 2029 2222   @rel!="mod" )""
+000035c0: 220d 0a20 0d0a 2061 7374 615f 6e6f 756e  ".. .. asta_noun
+000035d0: 203d 2022 2222 2028 2840 7074 3d22 6e22   = """ ((@pt="n"
+000035e0: 2061 6e64 206e 6f74 2825 4153 5441 5f66   and not(%ASTA_f
+000035f0: 696c 6c65 645f 7061 7573 6525 2920 616e  illed_pause%) an
+00003600: 6420 6e6f 7428 2541 5354 415f 6e75 6d65  d not(%ASTA_nume
+00003610: 7261 6c25 2929 206f 7220 0d0a 2020 2020  ral%)) or ..    
+00003620: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00003630: 406c 656d 6d61 3d22 3131 3222 2920 6f72  @lemma="112") or
+00003640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003650: 2020 2020 2840 7074 3d22 7777 2220 616e      (@pt="ww" an
+00003660: 6420 4070 6f73 6974 6965 3d22 6e6f 6d22  d @positie="nom"
+00003670: 2920 6f72 200d 0a09 0909 0920 2028 256d  ) or ......  (%m
+00003680: 6f6e 7468 6e61 6d65 2529 206f 7220 0d0a  onthname%) or ..
+00003690: 0909 0909 2020 4070 6f73 3d22 6e61 6d65  ....  @pos="name
+000036a0: 2220 290d 0a20 2222 220d 0a0d 0a0d 0a61  " ).. """......a
+000036b0: 7374 615f 6164 6a20 3d20 2222 220d 0a20  sta_adj = """.. 
+000036c0: 2020 2028 2541 5354 415f 6765 626f 7265     (%ASTA_gebore
+000036d0: 6e25 206f 720d 0a20 2020 2020 2561 7474  n% or..     %att
+000036e0: 7269 6275 7469 7665 5f61 646a 2520 6f72  ributive_adj% or
+000036f0: 0d0a 2020 2020 2025 6174 7472 6962 7574  ..     %attribut
+00003700: 6976 655f 6164 6a69 6e61 646a 7025 206f  ive_adjinadjp% o
+00003710: 720d 0a20 2020 2020 2572 616e 6774 7725  r..     %rangtw%
+00003720: 206f 720d 0a20 2020 2020 2573 7562 7374   or..     %subst
+00003730: 616e 7469 7669 7365 6461 646a 2520 6f72  antivisedadj% or
+00003740: 0d0a 2020 2020 2025 7375 6273 7461 6e74  ..     %substant
+00003750: 6976 6973 6564 7261 6e67 7477 2520 6f72  ivisedrangtw% or
+00003760: 0d0a 0920 2561 7474 7269 6275 7469 7665  ... %attributive
+00003770: 5f70 6173 7470 2520 6f72 0d0a 0920 2561  _pastp% or... %a
+00003780: 7474 7269 6275 7469 7665 5f70 7265 7370  ttributive_presp
+00003790: 2520 6f72 0d0a 0920 2573 696d 706c 6570  % or... %simplep
+000037a0: 7265 6469 6361 7469 7665 5f61 646a 2520  redicative_adj% 
+000037b0: 6f72 0d0a 0920 2573 696d 706c 6570 7265  or... %simplepre
+000037c0: 6469 6361 7469 7665 5f61 646a 696e 6164  dicative_adjinad
+000037d0: 6a70 2520 6f72 0d0a 0920 2569 6e64 6566  jp% or... %indef
+000037e0: 6465 7425 200d 0a09 290d 0a22 2222 0d0a  det% ...).."""..
+000037f0: 0d0a 6164 6a70 6173 7470 6172 7420 3d20  ..adjpastpart = 
+00003800: 2222 2228 4070 743d 2277 7722 2061 6e64  """(@pt="ww" and
+00003810: 2040 7776 6f72 6d3d 2276 6422 2061 6e64   @wvorm="vd" and
+00003820: 2040 706f 733d 2261 646a 2220 616e 6420   @pos="adj" and 
+00003830: 4072 656c 3d22 7072 6564 6322 2029 2222  @rel="predc" )""
+00003840: 220d 0a0d 0a61 7474 7269 6275 7469 7665  "....attributive
+00003850: 5f61 646a 203d 2022 2222 200d 0a20 2020  _adj = """ ..   
+00003860: 2028 4070 743d 2261 646a 2220 616e 6420   (@pt="adj" and 
+00003870: 0d0a 2020 2020 2028 4072 656c 3d22 6d6f  ..     (@rel="mo
+00003880: 6422 2061 6e64 200d 0a20 2020 2020 2070  d" and ..      p
+00003890: 6172 656e 743a 3a6e 6f64 655b 4063 6174  arent::node[@cat
+000038a0: 3d22 6e70 225d 2061 6e64 200d 0a20 2020  ="np"] and ..   
+000038b0: 2020 202e 2e2f 6e6f 6465 5b40 7265 6c3d     ../node[@rel=
+000038c0: 2268 6422 2061 6e64 2028 4070 743d 226e  "hd" and (@pt="n
+000038d0: 2220 6f72 2040 7074 3d22 766e 7722 206f  " or @pt="vnw" o
+000038e0: 7220 4063 6174 3d22 6d77 7522 295d 2061  r @cat="mwu")] a
+000038f0: 6e64 0d0a 0920 2028 6e6f 7428 4062 6567  nd...  (not(@beg
+00003900: 696e 203c 202e 2e2f 6e6f 6465 5b40 7265  in < ../node[@re
+00003910: 6c3d 2264 6574 2220 616e 6420 2840 7074  l="det" and (@pt
+00003920: 3d22 6c69 6422 206f 7220 4070 743d 2276  ="lid" or @pt="v
+00003930: 6e77 2229 5d2f 4062 6567 696e 2920 6f72  nw")]/@begin) or
+00003940: 2040 6c65 6d6d 613d 2768 6565 6c27 206f   @lemma='heel' o
+00003950: 7220 406c 656d 6d61 3d27 6765 6865 656c  r @lemma='geheel
+00003960: 2729 0d0a 0920 290d 0a09 290d 0a22 2222  ')... )...).."""
+00003970: 0d0a 0d0a 6174 7472 6962 7574 6976 655f  ....attributive_
+00003980: 6164 6a69 6e61 646a 7020 3d20 2222 220d  adjinadjp = """.
+00003990: 0a20 2020 2840 7074 3d22 6164 6a22 2061  .   (@pt="adj" a
+000039a0: 6e64 0d0a 2020 2020 2840 7265 6c3d 2268  nd..    (@rel="h
+000039b0: 6422 2061 6e64 0d0a 2020 2020 2070 6172  d" and..     par
+000039c0: 656e 743a 3a6e 6f64 655b 4063 6174 3d22  ent::node[@cat="
+000039d0: 6170 2220 616e 6420 7061 7265 6e74 3a3a  ap" and parent::
+000039e0: 6e6f 6465 5b40 6361 743d 226e 7022 5d20  node[@cat="np"] 
+000039f0: 616e 6420 0d0a 2020 2020 202e 2e2f 6e6f  and ..     ../no
+00003a00: 6465 5b40 7265 6c3d 2268 6422 2061 6e64  de[@rel="hd" and
+00003a10: 2028 4070 743d 226e 2220 6f72 2040 7074   (@pt="n" or @pt
+00003a20: 3d22 766e 7722 206f 7220 4063 6174 3d22  ="vnw" or @cat="
+00003a30: 6d77 7522 295d 5d0d 0a09 2029 0d0a 0929  mwu")]]... )...)
+00003a40: 0d0a 2222 220d 0a0d 0a72 616e 6774 7720  .."""....rangtw 
+00003a50: 3d20 2222 220d 0a20 2020 2840 7074 3d22  = """..   (@pt="
+00003a60: 7477 2220 616e 6420 406e 756d 7479 7065  tw" and @numtype
+00003a70: 3d22 7261 6e67 2229 0d0a 2222 220d 0a0d  ="rang").."""...
+00003a80: 0a73 7562 7374 616e 7469 7669 7365 6461  .substantiviseda
+00003a90: 646a 203d 2022 2222 200d 0a20 2020 2840  dj = """ ..   (@
+00003aa0: 7074 3d22 6164 6a22 2061 6e64 2040 7265  pt="adj" and @re
+00003ab0: 6c3d 2268 6422 2061 6e64 2070 6172 656e  l="hd" and paren
+00003ac0: 743a 3a6e 6f64 655b 4063 6174 3d22 6e70  t::node[@cat="np
+00003ad0: 225d 290d 0a22 2222 0d0a 0d0a 7375 6273  "]).."""....subs
+00003ae0: 7461 6e74 6976 6973 6564 7261 6e67 7477  tantivisedrangtw
+00003af0: 203d 2022 2222 0d0a 2020 2020 2825 7261   = """..    (%ra
+00003b00: 6e67 7477 2520 616e 6420 4070 6f73 6974  ngtw% and @posit
+00003b10: 6965 203d 2022 6e6f 6d22 2029 0d0a 2222  ie = "nom" )..""
+00003b20: 220d 0a0d 0a61 7474 7269 6275 7469 7665  "....attributive
+00003b30: 5f70 6173 7470 203d 2022 2222 0d0a 2020  _pastp = """..  
+00003b40: 2028 4070 743d 2277 7722 2061 6e64 2040   (@pt="ww" and @
+00003b50: 7776 6f72 6d3d 2276 6422 2061 6e64 2040  wvorm="vd" and @
+00003b60: 7265 6c3d 226d 6f64 2220 616e 6420 7061  rel="mod" and pa
+00003b70: 7265 6e74 3a3a 6e6f 6465 5b40 6361 743d  rent::node[@cat=
+00003b80: 226e 7022 5d29 0d0a 2222 220d 0a0d 0a61  "np"]).."""....a
+00003b90: 7474 7269 6275 7469 7665 5f70 7265 7370  ttributive_presp
+00003ba0: 203d 2022 2222 0d0a 2020 2028 4070 743d   = """..   (@pt=
+00003bb0: 2277 7722 2061 6e64 2040 7776 6f72 6d3d  "ww" and @wvorm=
+00003bc0: 226f 6422 2061 6e64 2040 7265 6c3d 226d  "od" and @rel="m
+00003bd0: 6f64 2220 616e 6420 7061 7265 6e74 3a3a  od" and parent::
+00003be0: 6e6f 6465 5b40 6361 743d 226e 7022 5d29  node[@cat="np"])
+00003bf0: 0d0a 2222 220d 0a0d 0a70 7265 6469 6361  .."""....predica
+00003c00: 7469 7665 203d 2022 2222 2028 4072 656c  tive = """ (@rel
+00003c10: 3d22 7072 6564 6322 206f 7220 4072 656c  ="predc" or @rel
+00003c20: 3d22 7072 6564 6d22 2029 2022 2222 0d0a  ="predm" ) """..
+00003c30: 0d0a 7369 6d70 6c65 7072 6564 6963 6174  ..simplepredicat
+00003c40: 6976 6520 3d20 2222 2220 2825 7072 6564  ive = """ (%pred
+00003c50: 6963 6174 6976 6525 2061 6e64 202e 2e2f  icative% and ../
+00003c60: 6e6f 6465 5b25 4153 5441 5f62 6173 6963  node[%ASTA_basic
+00003c70: 6b6f 7077 7725 5d29 0d0a 2222 220d 0a0d  kopww%]).."""...
+00003c80: 0a73 696d 706c 6570 7265 6469 6361 7469  .simplepredicati
+00003c90: 7665 5f61 646a 203d 2022 2222 0d0a 2020  ve_adj = """..  
+00003ca0: 2020 2028 4070 743d 2261 646a 2220 616e     (@pt="adj" an
 00003cb0: 6420 2573 696d 706c 6570 7265 6469 6361  d %simplepredica
-00003cc0: 7469 7665 255d 290d 0a22 2222 0d0a 0d0a  tive%]).."""....
-00003cd0: 696e 6465 6664 6574 203d 2022 2222 2028  indefdet = """ (
-00003ce0: 4072 656c 3d22 6465 7422 2061 6e64 2040  @rel="det" and @
-00003cf0: 7074 3d22 766e 7722 2061 6e64 2040 7677  pt="vnw" and @vw
-00003d00: 7479 7065 3d22 6f6e 6265 7022 290d 0a22  type="onbep").."
-00003d10: 2222 0d0a 0d0a 0d0a 4153 5441 5f43 4269  ""......ASTA_CBi
-00003d20: 6a7a 696e 203d 2022 2222 0d0a 2020 2020  jzin = """..    
-00003d30: 2020 2020 2028 2541 5354 415f 7761 6e74       (%ASTA_want
-00003d40: 6d61 6172 6269 6a7a 696e 2520 6f72 0d0a  maarbijzin% or..
-00003d50: 0909 2020 2541 5354 415f 6475 7362 696a  ..  %ASTA_dusbij
-00003d60: 7a69 6e25 290d 0a22 2222 0d0a 0d0a 4153  zin%).."""....AS
-00003d70: 5441 5f43 4269 6a7a 696e 7a69 6e20 3d20  TA_CBijzinzin = 
-00003d80: 2222 220d 0a28 2025 4153 5441 5f77 616e  """..( %ASTA_wan
-00003d90: 746d 6161 7262 696a 7a69 6e7a 696e 2520  tmaarbijzinzin% 
-00003da0: 6f72 0d0a 2020 2541 5354 415f 6475 7362  or..  %ASTA_dusb
-00003db0: 696a 7a69 6e7a 696e 250d 0a29 0d0a 2222  ijzinzin%..)..""
-00003dc0: 220d 0a0d 0a41 5354 415f 6f6c 6442 696a  "....ASTA_oldBij
-00003dd0: 7a69 6e20 3d20 2222 220d 0a20 2028 286e  zin = """..  ((n
-00003de0: 6f64 655b 4063 6174 3d22 7373 7562 225d  ode[@cat="ssub"]
-00003df0: 206f 7220 2840 6361 743d 2273 7631 2220   or (@cat="sv1" 
-00003e00: 616e 6420 4072 656c 3d22 6d6f 6422 2029  and @rel="mod" )
-00003e10: 2920 6f72 200d 0a20 2020 2020 2020 2020  ) or ..         
-00003e20: 2541 5354 415f 7761 6e74 6d61 6172 6269  %ASTA_wantmaarbi
-00003e30: 6a7a 696e 2520 6f72 0d0a 0909 2025 4153  jzin% or.... %AS
-00003e40: 5441 5f64 7573 6269 6a7a 696e 250d 0a20  TA_dusbijzin%.. 
-00003e50: 2029 0d0a 090d 0a22 2222 0d0a 0d0a 0d0a   )....."""......
-00003e60: 6f6c 6432 4153 5441 5f42 696a 7a69 6e20  old2ASTA_Bijzin 
-00003e70: 3d20 2222 220d 0a20 2820 2020 2020 2020  = """.. (       
-00003e80: 2861 6e63 6573 746f 723a 3a6e 6f64 655b  (ancestor::node[
-00003e90: 4063 6174 3d22 746f 7022 2061 6e64 200d  @cat="top" and .
-00003ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003eb0: 2020 2020 2020 2020 2020 636f 756e 7428            count(
-00003ec0: 2e2f 2f6e 6f64 655b 4063 6174 3d22 736d  .//node[@cat="sm
-00003ed0: 6169 6e22 206f 7220 4063 6174 3d22 7376  ain" or @cat="sv
-00003ee0: 3122 206f 7220 0d0a 0909 0909 0909 2020  1" or ........  
-00003ef0: 2020 2020 2020 2020 2020 2020 2840 6361              (@ca
-00003f00: 743d 2273 7375 6222 2061 6e64 2040 7265  t="ssub" and @re
-00003f10: 6c3d 2263 6e6a 2229 206f 7220 0d0a 0909  l="cnj") or ....
-00003f20: 0909 0909 0909 0920 2040 6361 743d 2277  .......  @cat="w
-00003f30: 6872 656c 2220 6f72 200d 0a09 0909 0909  hrel" or .......
-00003f40: 0909 0909 2020 4063 6174 3d22 7265 6c22  ....  @cat="rel"
-00003f50: 206f 7220 0d0a 0909 0909 0909 0909 0920   or ........... 
-00003f60: 2040 6361 743d 2277 6873 7562 2220 6f72   @cat="whsub" or
-00003f70: 200d 0a09 0909 0909 0909 0909 2020 4063   ...........  @c
-00003f80: 6174 3d22 6370 225d 2920 3e20 3120 5d29  at="cp"]) > 1 ])
-00003f90: 2061 6e64 200d 0a20 2020 2020 2020 2020   and ..         
-00003fa0: 2828 4063 6174 3d22 7373 7562 2220 616e  ((@cat="ssub" an
-00003fb0: 6420 4072 656c 3d22 636e 6a22 2920 6f72  d @rel="cnj") or
-00003fc0: 0d0a 2020 2020 2020 2020 2020 2840 6361  ..          (@ca
-00003fd0: 743d 2277 6872 656c 2220 6f72 2040 6361  t="whrel" or @ca
-00003fe0: 743d 2272 656c 2220 6f72 2040 6361 743d  t="rel" or @cat=
-00003ff0: 2277 6873 7562 2229 206f 720d 0a20 2020  "whsub") or..   
-00004000: 2020 2020 2020 2028 4063 6174 3d22 6370         (@cat="cp
-00004010: 2220 616e 6420 6e6f 6465 5b40 6361 743d  " and node[@cat=
-00004020: 2273 7375 6222 5d29 096f 7209 2020 0d0a  "ssub"]).or.  ..
-00004030: 0909 2020 2840 6361 743d 2273 7631 2220  ..  (@cat="sv1" 
-00004040: 616e 6420 2840 7265 6c3d 226d 6f64 2220  and (@rel="mod" 
-00004050: 6f72 2040 7265 6c3d 2263 6e6a 2229 2029  or @rel="cnj") )
-00004060: 206f 7220 0d0a 0909 2020 2840 6361 743d   or ....  (@cat=
-00004070: 2273 6d61 696e 2220 616e 6420 2840 7265  "smain" and (@re
-00004080: 6c3d 2263 6e6a 2220 6f72 2040 7265 6c3d  l="cnj" or @rel=
-00004090: 2262 6f64 7922 206f 7220 4072 656c 3d22  "body" or @rel="
-000040a0: 6e75 636c 2229 2061 6e64 206e 6f74 2825  nucl") and not(%
-000040b0: 4153 5441 5f43 4269 6a7a 696e 7a69 6e25  ASTA_CBijzinzin%
-000040c0: 2929 206f 720d 0a09 0920 2028 4063 6174  )) or....  (@cat
-000040d0: 3d22 6f74 6922 2920 6f72 0d0a 0909 2020  ="oti") or....  
-000040e0: 2025 4153 5441 5f43 4269 6a7a 696e 2520   %ASTA_CBijzin% 
-000040f0: 0d0a 0909 2020 290d 0a20 0d0a 2029 0d0a  ....  ).. .. )..
-00004100: 2222 220d 0a0d 0a41 5354 415f 4269 6a7a  """....ASTA_Bijz
-00004110: 696e 203d 2022 2222 0d0a 2028 2020 2020  in = """.. (    
-00004120: 2020 2020 0d0a 2020 2020 2020 2020 2028      ..         (
-00004130: 2840 6361 743d 2273 7375 6222 2061 6e64  (@cat="ssub" and
-00004140: 2040 7265 6c3d 2263 6e6a 2220 616e 6420   @rel="cnj" and 
-00004150: 6e6f 7428 2566 6972 7374 7373 7562 636f  not(%firstssubco
-00004160: 6e6a 756e 6374 2529 2061 6e64 206e 6f74  njunct%) and not
-00004170: 2825 4153 5441 5f43 4269 6a7a 696e 7a69  (%ASTA_CBijzinzi
-00004180: 6e25 2929 206f 720d 0a20 2020 2020 2020  n%)) or..       
-00004190: 2020 2028 4063 6174 3d22 7768 7265 6c22     (@cat="whrel"
-000041a0: 206f 7220 4063 6174 3d22 7265 6c22 206f   or @cat="rel" o
-000041b0: 7220 4063 6174 3d22 7768 7375 6222 2920  r @cat="whsub") 
-000041c0: 6f72 0d0a 0909 2020 2828 4063 6174 3d22  or....  ((@cat="
-000041d0: 736d 6169 6e22 206f 7220 4063 6174 3d22  smain" or @cat="
-000041e0: 7376 3122 2961 6e64 2040 7265 6c3d 222d  sv1")and @rel="-
-000041f0: 2d22 2920 6f72 0d0a 2020 2020 2020 2020  -") or..        
-00004200: 2020 2840 6361 743d 2263 7022 2061 6e64    (@cat="cp" and
-00004210: 206e 6f64 655b 4063 6174 3d22 7373 7562   node[@cat="ssub
-00004220: 2220 6f72 2040 6361 743d 2263 6f6e 6a22  " or @cat="conj"
-00004230: 5d29 096f 7209 2020 0d0a 0909 2020 2840  ]).or.  ....  (@
-00004240: 6361 743d 2273 7631 2220 616e 6420 2840  cat="sv1" and (@
-00004250: 7265 6c3d 226d 6f64 2220 6f72 2040 7265  rel="mod" or @re
-00004260: 6c3d 2263 6e6a 2229 2029 206f 7220 0d0a  l="cnj") ) or ..
-00004270: 0909 2020 2840 6361 743d 2273 6d61 696e  ..  (@cat="smain
-00004280: 2220 616e 6420 2840 7265 6c3d 2263 6e6a  " and (@rel="cnj
-00004290: 2220 6f72 2040 7265 6c3d 2262 6f64 7922  " or @rel="body"
-000042a0: 206f 7220 4072 656c 3d22 6e75 636c 2220   or @rel="nucl" 
-000042b0: 6f72 2040 7265 6c3d 2264 7022 2920 616e  or @rel="dp") an
-000042c0: 6420 6e6f 7428 2541 5354 415f 4342 696a  d not(%ASTA_CBij
-000042d0: 7a69 6e7a 696e 2529 2920 6f72 0d0a 0909  zinzin%)) or....
-000042e0: 2020 2840 6361 743d 226f 7469 2229 206f    (@cat="oti") o
-000042f0: 720d 0a09 0920 2020 2541 5354 415f 4342  r....   %ASTA_CB
-00004300: 696a 7a69 6e25 206f 720d 0a09 0920 2020  ijzin% or....   
-00004310: 2564 6972 6563 7465 7265 6465 5f76 6362  %directerede_vcb
-00004320: 696a 7a69 6e25 206f 720d 0a09 0920 2020  ijzin% or....   
-00004330: 2840 7074 3d22 7667 2220 616e 6420 4063  (@pt="vg" and @c
-00004340: 6f6e 6a74 7970 653d 226f 6e64 6572 2220  onjtype="onder" 
-00004350: 616e 6420 4072 656c 3d22 2d2d 2220 2029  and @rel="--"  )
-00004360: 206f 720d 0a09 0920 2020 2828 4070 743d   or....   ((@pt=
-00004370: 2262 7722 206f 7220 4070 743d 2276 6e77  "bw" or @pt="vnw
-00004380: 2229 2061 6e64 2040 7265 6c3d 2276 6322  ") and @rel="vc"
-00004390: 2061 6e64 2040 7768 3d22 7977 6822 290d   and @wh="ywh").
-000043a0: 0a09 0920 2029 0d0a 200d 0a20 290d 0a22  ...  ).. .. ).."
-000043b0: 2222 0d0a 0d0a 6669 7273 7473 7375 6263  ""....firstssubc
-000043c0: 6f6e 6a75 6e63 7420 3d20 2222 2228 2566  onjunct = """(%f
-000043d0: 6972 7374 7373 7562 636f 6e6a 756e 6374  irstssubconjunct
-000043e0: 6125 206f 7220 2566 6972 7374 7373 7562  a% or %firstssub
-000043f0: 636f 6e6a 756e 6374 6225 2922 2222 0d0a  conjunctb%)"""..
-00004400: 6669 7273 7473 7375 6263 6f6e 6a75 6e63  firstssubconjunc
-00004410: 7461 203d 2022 2222 2840 6361 743d 2273  ta = """(@cat="s
-00004420: 7375 6222 2061 6e64 2040 6265 6769 6e3d  sub" and @begin=
-00004430: 6e6f 6465 5b40 6361 7420 6f72 2040 7074  node[@cat or @pt
-00004440: 5d2f 4062 6567 696e 2061 6e64 2040 6265  ]/@begin and @be
-00004450: 6769 6e3d 7061 7265 6e74 3a3a 6e6f 6465  gin=parent::node
-00004460: 5b40 6361 743d 2263 6f6e 6a22 5d2f 7061  [@cat="conj"]/pa
-00004470: 7265 6e74 3a3a 6e6f 6465 5b40 6361 743d  rent::node[@cat=
-00004480: 2263 7022 5d2f 6e6f 6465 5b40 7074 3d22  "cp"]/node[@pt="
-00004490: 7667 225d 2f40 656e 6420 2922 2222 0d0a  vg"]/@end )"""..
-000044a0: 6669 7273 7473 7375 6263 6f6e 6a75 6e63  firstssubconjunc
-000044b0: 7462 203d 2022 2222 2840 6361 743d 2273  tb = """(@cat="s
-000044c0: 7375 6222 2061 6e64 2040 6265 6769 6e3d  sub" and @begin=
-000044d0: 6e6f 6465 5b40 6361 7420 6f72 2040 7074  node[@cat or @pt
-000044e0: 5d2f 4062 6567 696e 2061 6e64 2040 6265  ]/@begin and @be
-000044f0: 6769 6e3d 7061 7265 6e74 3a3a 6e6f 6465  gin=parent::node
-00004500: 5b40 6361 743d 2263 6f6e 6a22 5d2f 7061  [@cat="conj"]/pa
-00004510: 7265 6e74 3a3a 6e6f 6465 5b40 6361 743d  rent::node[@cat=
-00004520: 2272 656c 225d 2f6e 6f64 655b 4072 656c  "rel"]/node[@rel
-00004530: 3d22 7268 6422 5d2f 4065 6e64 2029 2222  ="rhd"]/@end )""
-00004540: 220d 0a0d 0a62 696a 7a69 6e63 6174 203d  "....bijzincat =
-00004550: 2022 2222 2820 4063 6174 3d22 736d 6169   """( @cat="smai
-00004560: 6e22 206f 7220 4063 6174 3d22 7376 3122  n" or @cat="sv1"
-00004570: 206f 7220 0d0a 0909 0909 0909 2020 2020   or ........    
-00004580: 2020 2020 2020 2020 2020 2840 6361 743d            (@cat=
-00004590: 2273 7375 6222 2061 6e64 2040 7265 6c3d  "ssub" and @rel=
-000045a0: 2263 6e6a 2229 206f 7220 0d0a 0909 0909  "cnj") or ......
-000045b0: 0909 0909 0920 2040 6361 743d 2277 6872  .....  @cat="whr
-000045c0: 656c 2220 6f72 200d 0a09 0909 0909 0909  el" or .........
-000045d0: 0909 2020 4063 6174 3d22 7265 6c22 206f  ..  @cat="rel" o
-000045e0: 7220 0d0a 0909 0909 0909 0909 0920 2040  r ...........  @
-000045f0: 6361 743d 2277 6873 7562 2220 6f72 200d  cat="whsub" or .
-00004600: 0a09 0909 0909 0909 0909 2020 4063 6174  ..........  @cat
-00004610: 3d22 6370 2229 2222 220d 0a0d 0a62 696a  ="cp")"""....bij
-00004620: 7a69 6e6e 6f64 6520 3d20 2222 2220 2861  zinnode = """ (a
-00004630: 6e63 6573 746f 723a 3a6e 6f64 655b 4063  ncestor::node[@c
-00004640: 6174 3d22 746f 7022 2061 6e64 200d 0a20  at="top" and .. 
-00004650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004660: 2020 2020 2020 2020 2e2f 2f6e 6f64 655b          .//node[
-00004670: 2562 696a 7a69 6e63 6174 255d 2020 5d29  %bijzincat%]  ])
-00004680: 2222 220d 0a09 0909 0909 0909 0909 2020  """...........  
-00004690: 0d0a 0909 0909 0909 0909 0920 200d 0a6e  ...........  ..n
-000046a0: 6f74 6669 7273 7462 696a 7a69 6e20 3d20  otfirstbijzin = 
-000046b0: 2222 2228 2562 696a 7a69 6e63 6174 2520  """(%bijzincat% 
-000046c0: 616e 6420 636f 756e 7428 2562 696a 7a69  and count(%bijzi
-000046d0: 6e6e 6f64 6525 2920 3e20 3120 2061 6e64  nnode%) > 1  and
-000046e0: 2040 6265 6769 6e5b 6e6f 7428 202e 203e   @begin[not( . >
-000046f0: 2025 6269 6a7a 696e 6e6f 6465 252f 4062   %bijzinnode%/@b
-00004700: 6567 696e 295d 5b31 5d29 2222 2220 0909  egin)][1])""" ..
-00004710: 090d 0a0d 0a0d 0a54 6172 7370 5f6e 6f6e  .......Tarsp_non
-00004720: 6d6f 6461 6476 6370 203d 2022 2222 2840  modadvcp = """(@
-00004730: 6361 743d 2263 7022 2061 6e64 2028 4072  cat="cp" and (@r
-00004740: 656c 3d22 6470 2220 6f72 2040 7265 6c3d  el="dp" or @rel=
-00004750: 222d 2d22 2920 616e 6420 6e6f 6465 5b40  "--") and node[@
-00004760: 7074 3d22 7667 2220 616e 6420 4063 6f6e  pt="vg" and @con
-00004770: 6a74 7970 653d 226f 6e64 6572 2220 616e  jtype="onder" an
-00004780: 6420 406c 656d 6d61 213d 2264 6174 2220  d @lemma!="dat" 
-00004790: 616e 6420 406c 656d 6d61 213d 226f 6622  and @lemma!="of"
-000047a0: 205d 2029 2222 220d 0a0d 0a0d 0a0d 0a64   ] )"""........d
-000047b0: 6972 6563 7465 7265 6465 5f76 6362 696a  irecterede_vcbij
-000047c0: 7a69 6e20 3d20 2222 2228 2025 636c 6175  zin = """( %clau
-000047d0: 7365 6361 7425 2061 6e64 206e 6f74 2840  secat% and not(@
-000047e0: 7265 6c3d 2263 6e6a 2229 2061 6e64 2028  rel="cnj") and (
-000047f0: 7072 6563 6564 696e 672d 7369 626c 696e  preceding-siblin
-00004800: 673a 3a6e 6f64 655b 256d 6574 6173 6d61  g::node[%metasma
-00004810: 696e 255d 206f 7220 666f 6c6c 6f77 696e  in%] or followin
-00004820: 672d 7369 626c 696e 673a 3a6e 6f64 655b  g-sibling::node[
-00004830: 256d 6574 6173 7631 255d 2929 2222 220d  %metasv1%]))""".
-00004840: 0a0d 0a0d 0a63 6c61 7573 6563 6174 203d  .....clausecat =
-00004850: 2022 2222 2840 6361 743d 2273 6d61 696e   """(@cat="smain
-00004860: 2220 6f72 2040 6361 743d 2277 6871 2220  " or @cat="whq" 
-00004870: 6f72 2025 6261 7265 7376 3125 2029 2222  or %baresv1% )""
-00004880: 220d 0a6d 6574 6176 6572 6220 3d20 2222  "..metaverb = ""
-00004890: 2228 406c 656d 6d61 3d22 7a65 6767 656e  "(@lemma="zeggen
-000048a0: 2220 6f72 2040 6c65 6d6d 613d 2264 656e  " or @lemma="den
-000048b0: 6b65 6e22 206f 7220 406c 656d 6d61 3d22  ken" or @lemma="
-000048c0: 7669 6e64 656e 2220 6f72 2040 6c65 6d6d  vinden" or @lemm
-000048d0: 613d 2276 7261 6765 6e22 206f 7220 406c  a="vragen" or @l
-000048e0: 656d 6d61 3d22 7363 6872 6565 7577 656e  emma="schreeuwen
-000048f0: 2220 6f72 2040 6c65 6d6d 613d 2266 6c75  " or @lemma="flu
-00004900: 6973 7465 7265 6e22 2029 2222 220d 0a6d  isteren" )"""..m
-00004910: 6574 6173 6d61 696e 203d 2022 2222 2840  etasmain = """(@
-00004920: 6361 743d 2273 6d61 696e 2220 616e 6420  cat="smain" and 
-00004930: 6e6f 7428 4072 656c 3d22 636e 6a22 2920  not(@rel="cnj") 
-00004940: 616e 6420 6e6f 6465 5b40 7265 6c3d 2268  and node[@rel="h
-00004950: 6422 2061 6e64 2025 6d65 7461 7665 7262  d" and %metaverb
-00004960: 255d 2920 2222 220d 0a6d 6574 6173 7631  %]) """..metasv1
-00004970: 203d 2022 2222 2840 6361 743d 2273 7631   = """(@cat="sv1
-00004980: 2220 616e 6420 6e6f 7428 4072 656c 3d22  " and not(@rel="
-00004990: 636e 6a22 2920 616e 6420 6e6f 6465 5b40  cnj") and node[@
-000049a0: 7265 6c3d 2268 6422 2061 6e64 2025 6d65  rel="hd" and %me
-000049b0: 7461 7665 7262 255d 2920 2222 220d 0a0d  taverb%]) """...
-000049c0: 0a62 6172 6573 7631 203d 2022 2222 2820  .baresv1 = """( 
-000049d0: 4063 6174 3d22 7376 3122 2061 6e64 206e  @cat="sv1" and n
-000049e0: 6f74 2870 6172 656e 743a 3a6e 6f64 655b  ot(parent::node[
-000049f0: 2840 6361 743d 2277 6871 2220 6f72 2040  (@cat="whq" or @
-00004a00: 6361 743d 2277 6872 656c 2229 5d29 2922  cat="whrel")]))"
-00004a10: 2222 0d0a 0d0a 0d0a 6465 6c70 765f 6e6f  ""......delpv_no
-00004a20: 6e66 696e 6361 7420 3d20 2222 2228 4063  nfincat = """(@c
-00004a30: 6174 3d22 7070 7265 7322 206f 7220 4063  at="ppres" or @c
-00004a40: 6174 3d22 7070 6172 7422 206f 7220 4063  at="ppart" or @c
-00004a50: 6174 3d22 7469 2220 6f72 2040 6361 743d  at="ti" or @cat=
-00004a60: 226f 7469 2220 6f72 2040 6361 743d 2261  "oti" or @cat="a
-00004a70: 6869 2220 6f72 2028 4063 6174 3d22 696e  hi" or (@cat="in
-00004a80: 6622 2061 6e64 2040 706f 7369 7469 6521  f" and @positie!
-00004a90: 3d22 6e6f 6d22 2920 2920 2222 220d 0a64  ="nom") ) """..d
-00004aa0: 656c 7076 5f63 6c61 7573 6563 6174 203d  elpv_clausecat =
-00004ab0: 2022 2222 2840 6361 743d 2273 6d61 696e   """(@cat="smain
-00004ac0: 2220 6f72 2040 6361 743d 2273 7375 6222  " or @cat="ssub"
-00004ad0: 206f 7220 4063 6174 3d22 7376 3122 206f   or @cat="sv1" o
-00004ae0: 7220 4063 6174 3d22 7070 7265 7322 206f  r @cat="ppres" o
-00004af0: 7220 4063 6174 3d22 7070 6172 7422 206f  r @cat="ppart" o
-00004b00: 7220 4063 6174 3d22 7469 2220 6f72 2040  r @cat="ti" or @
-00004b10: 6361 743d 226f 7469 2220 6f72 2040 6361  cat="oti" or @ca
-00004b20: 743d 2261 6869 2220 6f72 2040 6361 743d  t="ahi" or @cat=
-00004b30: 2269 6e66 2229 2222 220d 0a64 656c 7076  "inf")"""..delpv
-00004b40: 5f6e 6f6e 6669 6e77 7720 3d20 2222 2228  _nonfinww = """(
-00004b50: 4070 743d 2277 7722 2061 6e64 2028 4077  @pt="ww" and (@w
-00004b60: 766f 726d 3d22 7464 2220 6f72 2028 4077  vorm="td" or (@w
-00004b70: 766f 726d 3d22 696e 6622 2061 6e64 2040  vorm="inf" and @
-00004b80: 706f 7369 7469 6521 3d22 6e6f 6d22 2920  positie!="nom") 
-00004b90: 6f72 2040 7776 6f72 6d3d 2276 6422 2920  or @wvorm="vd") 
-00004ba0: 2922 2222 0d0a 0d0a 636f 7265 6465 6c70  )"""....coredelp
-00004bb0: 7620 3d20 2222 2228 2825 6465 6c70 765f  v = """((%delpv_
-00004bc0: 6e6f 6e66 696e 6361 7425 206f 7220 2564  nonfincat% or %d
-00004bd0: 656c 7076 5f6e 6f6e 6669 6e77 7725 2029  elpv_nonfinww% )
-00004be0: 2061 6e64 206e 6f74 2861 6e63 6573 746f   and not(ancesto
-00004bf0: 723a 3a6e 6f64 655b 2564 656c 7076 5f63  r::node[%delpv_c
-00004c00: 6c61 7573 6563 6174 255d 2920 2922 2222  lausecat%]) )"""
-00004c10: 0d0a 0d0a 726f 6275 7374 6465 6c70 7620  ....robustdelpv 
-00004c20: 3d20 2222 2228 6e6f 7428 4072 656c 3d22  = """(not(@rel="
-00004c30: 6470 2220 616e 6420 4062 6567 696e 203e  dp" and @begin >
-00004c40: 2061 6e63 6573 746f 723a 3a6e 6f64 655b   ancestor::node[
-00004c50: 4063 6174 3d22 746f 7022 5d2f 6465 7363  @cat="top"]/desc
-00004c60: 656e 6461 6e74 3a3a 6e6f 6465 5b40 7265  endant::node[@re
-00004c70: 6c3d 2264 7022 5d2f 6465 7363 656e 6461  l="dp"]/descenda
-00004c80: 6e74 3a3a 6e6f 6465 5b40 7074 3d22 7777  nt::node[@pt="ww
-00004c90: 2220 616e 6420 4077 766f 726d 3d22 7076  " and @wvorm="pv
-00004ca0: 225d 2f40 6265 6769 6e29 2922 2222 0d0a  "]/@begin))"""..
-00004cb0: 0d0a 6465 6c70 7620 3d20 2222 2228 2563  ..delpv = """(%c
-00004cc0: 6f72 6564 656c 7076 2520 616e 6420 2572  oredelpv% and %r
-00004cd0: 6f62 7573 7464 656c 7076 2529 2222 220d  obustdelpv%)""".
-00004ce0: 0a0d 0a56 6f62 696a 203d 2022 2222 2840  ...Vobij = """(@
-00004cf0: 7074 3d22 6277 2220 616e 6420 2863 6f6e  pt="bw" and (con
-00004d00: 7461 696e 7328 4066 7261 6d65 2c22 6572  tains(@frame,"er
-00004d10: 5f61 6476 6572 6222 2029 206f 7220 636f  _adverb" ) or co
-00004d20: 6e74 6169 6e73 2840 6672 616d 652c 2022  ntains(@frame, "
-00004d30: 746d 705f 6164 7665 7262 2229 206f 7220  tmp_adverb") or 
-00004d40: 636f 6e74 6169 6e73 2840 6672 616d 652c  contains(@frame,
-00004d50: 2022 7761 6172 5f61 6476 6572 6222 2920   "waar_adverb") 
-00004d60: 6f72 2040 6c65 6d6d 613d 2264 6161 726f  or @lemma="daaro
-00004d70: 6d22 2920 616e 6420 0d0a 406c 656d 6d61  m") and ..@lemma
-00004d80: 213d 2265 7222 2061 6e64 2040 6c65 6d6d  !="er" and @lemm
-00004d90: 6121 3d22 6461 6172 2220 616e 6420 406c  a!="daar" and @l
-00004da0: 656d 6d61 213d 2268 6965 7222 2061 6e64  emma!="hier" and
-00004db0: 2040 6c65 6d6d 6121 3d22 7761 6172 2220   @lemma!="waar" 
-00004dc0: 616e 6420 2873 7461 7274 732d 7769 7468  and (starts-with
-00004dd0: 2840 6c65 6d6d 612c 2027 6572 2729 206f  (@lemma, 'er') o
-00004de0: 7220 7374 6172 7473 2d77 6974 6828 406c  r starts-with(@l
-00004df0: 656d 6d61 2c20 2764 6161 7227 2920 6f72  emma, 'daar') or
-00004e00: 2073 7461 7274 732d 7769 7468 2840 6c65   starts-with(@le
-00004e10: 6d6d 612c 2027 6869 6572 2729 206f 7220  mma, 'hier') or 
-00004e20: 7374 6172 7473 2d77 6974 6828 406c 656d  starts-with(@lem
-00004e30: 6d61 2c20 2777 6161 7227 2929 2922 2222  ma, 'waar')))"""
-00004e40: 0d0a 0d0a 5461 7273 705f 567a 4e20 3d20  ....Tarsp_VzN = 
-00004e50: 2222 2228 2576 7a6e 3178 7061 7468 2520  """(%vzn1xpath% 
-00004e60: 6f72 2025 767a 6e32 7870 6174 6825 2029  or %vzn2xpath% )
-00004e70: 2022 2222 0d0a 0d0a 767a 6e31 7870 6174   """....vzn1xpat
-00004e80: 6820 3d20 2222 2228 4063 6174 3d22 7070  h = """(@cat="pp
-00004e90: 2220 616e 6420 286e 6f64 655b 4070 743d  " and (node[@pt=
-00004ea0: 2276 7a22 5d20 616e 6420 6e6f 6465 5b28  "vz"] and node[(
-00004eb0: 4070 743d 226e 2220 6f72 2040 7074 3d22  @pt="n" or @pt="
-00004ec0: 766e 7722 2920 616e 6420 6e6f 7420 2825  vnw") and not (%
-00004ed0: 5270 726f 6e6f 756e 2529 2061 6e64 2040  Rpronoun%) and @
-00004ee0: 7265 6c3d 226f 626a 3122 5d20 616e 6420  rel="obj1"] and 
-00004ef0: 6e6f 7428 6e6f 6465 5b40 7074 3d22 767a  not(node[@pt="vz
-00004f00: 2220 616e 6420 4076 7a74 7970 653d 2266  " and @vztype="f
-00004f10: 696e 225d 2929 2922 2222 0d0a 767a 6e32  in"])))"""..vzn2
-00004f20: 7870 6174 6820 3d20 2222 2228 6e6f 6465  xpath = """(node
-00004f30: 5b40 6c65 6d6d 613d 2269 6e22 2061 6e64  [@lemma="in" and
-00004f40: 2040 7265 6c3d 226d 7770 225d 2061 6e64   @rel="mwp"] and
-00004f50: 206e 6f64 655b 406c 656d 6d61 3d22 6465   node[@lemma="de
-00004f60: 7a65 2220 616e 6420 4072 656c 3d22 6d77  ze" and @rel="mw
-00004f70: 7022 5d29 2222 220d 0a76 7a6e 3378 7061  p"])"""..vzn3xpa
-00004f80: 7468 203d 2022 2222 2840 7074 3d22 767a  th = """(@pt="vz
-00004f90: 2220 616e 6420 2e2e 2f6e 6f64 655b 2840  " and ../node[(@
-00004fa0: 6c65 6d6d 613d 2264 6974 2220 6f72 2040  lemma="dit" or @
-00004fb0: 6c65 6d6d 613d 2264 6174 2229 2020 616e  lemma="dat")  an
-00004fc0: 6420 4062 6567 696e 3e3d 2e2e 2f6e 6f64  d @begin>=../nod
-00004fd0: 655b 4070 743d 2276 7a22 5d2f 4065 6e64  e[@pt="vz"]/@end
-00004fe0: 2061 6e64 2063 6f75 6e74 286e 6f64 6529   and count(node)
-00004ff0: 3c3d 335d 2029 2222 220d 0a0d 0a6e 6f52  <=3] )"""....noR
-00005000: 7072 6f6e 6f75 6e78 203d 2022 2222 6e6f  pronounx = """no
-00005010: 7428 616e 6365 7374 6f72 3a3a 6e6f 6465  t(ancestor::node
-00005020: 5b40 6361 743d 2274 6f70 225d 2f64 6573  [@cat="top"]/des
-00005030: 6365 6e64 616e 743a 3a6e 6f64 655b 2552  cendant::node[%R
-00005040: 7072 6f6e 6f75 6e78 255d 2922 2222 0d0a  pronounx%])"""..
-00005050: 0d0a 7472 616e 7369 7469 7665 767a 203d  ..transitivevz =
-00005060: 2022 2222 2820 406c 656d 6d61 3d27 6161   """( @lemma='aa
-00005070: 6e27 206f 7220 406c 656d 6d61 3d27 6269  n' or @lemma='bi
-00005080: 6a27 206f 7220 406c 656d 6d61 3d27 646f  j' or @lemma='do
-00005090: 6f72 2720 6f72 2040 6c65 6d6d 613d 2769  or' or @lemma='i
-000050a0: 6e27 206f 7220 406c 656d 6d61 3d27 6e61  n' or @lemma='na
-000050b0: 6172 2720 6f72 2040 6c65 6d6d 613d 276e  ar' or @lemma='n
-000050c0: 6161 7274 6f65 2720 206f 7220 0d0a 2020  aartoe'  or ..  
-000050d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050e0: 2020 406c 656d 6d61 3d27 6f70 2720 6f72    @lemma='op' or
-000050f0: 2020 406c 656d 6d61 3d27 6f76 6572 2720    @lemma='over' 
-00005100: 6f72 2020 2040 6c65 6d6d 613d 2774 6567  or   @lemma='teg
-00005110: 656e 2720 6f72 2040 6c65 6d6d 613d 2774  en' or @lemma='t
-00005120: 6f65 2720 6f72 2020 406c 656d 6d61 3d27  oe' or  @lemma='
-00005130: 7475 7373 656e 2720 6f72 2040 6c65 6d6d  tussen' or @lemm
-00005140: 613d 2775 6974 2720 6f72 0d0a 0909 0909  a='uit' or......
-00005150: 0940 6c65 6d6d 613d 2776 616e 2720 6f72  .@lemma='van' or
-00005160: 2020 406c 656d 6d61 3d27 766f 6f72 270d    @lemma='voor'.
-00005170: 0a09 0909 0909 2922 2222 0d0a 0d0a 5270  ......)"""....Rp
-00005180: 726f 6e6f 756e 7820 3d20 2222 2228 2552  ronounx = """(%R
-00005190: 7072 6f6e 6f75 6e25 206f 7220 406c 656d  pronoun% or @lem
-000051a0: 6d61 3d22 6461 6172 7a6f 2220 6f72 2040  ma="daarzo" or @
-000051b0: 6c65 6d6d 613d 2268 6965 727a 6f22 2920  lemma="hierzo") 
-000051c0: 2222 220d 0a0d 0a66 6f6c 6c6f 7765 6462  """....followedb
-000051d0: 7964 6574 203d 2022 2222 2840 656e 643d  ydet = """(@end=
-000051e0: 616e 6365 7374 6f72 3a3a 6e6f 6465 5b40  ancestor::node[@
-000051f0: 6361 743d 2274 6f70 225d 2f64 6573 6365  cat="top"]/desce
-00005200: 6e64 616e 743a 3a6e 6f64 655b 2564 6574  ndant::node[%det
-00005210: 255d 2f40 6265 6769 6e29 2222 220d 0a0d  %]/@begin)"""...
-00005220: 0a64 6574 203d 2022 2222 2840 7074 3d22  .det = """(@pt="
-00005230: 6c69 6422 206f 7220 406c 656d 6d61 3d22  lid" or @lemma="
-00005240: 6469 7422 206f 7220 406c 656d 6d61 3d22  dit" or @lemma="
-00005250: 6465 7a65 2220 6f72 2040 6c65 6d6d 613d  deze" or @lemma=
-00005260: 2264 6965 2220 6f72 2040 6c65 6d6d 613d  "die" or @lemma=
-00005270: 2264 6174 2220 6f72 2028 4070 743d 2276  "dat" or (@pt="v
-00005280: 6e77 2220 616e 6420 4076 7774 7970 653d  nw" and @vwtype=
-00005290: 2262 657a 2229 2029 2022 2222            "bez") ) """
+00003cc0: 7469 7665 2529 0d0a 2222 220d 0a09 200d  tive%).."""... .
+00003cd0: 0a73 696d 706c 6570 7265 6469 6361 7469  .simplepredicati
+00003ce0: 7665 5f61 646a 696e 6164 6a70 203d 2022  ve_adjinadjp = "
+00003cf0: 2222 0d0a 2020 2020 2028 4070 743d 2261  ""..     (@pt="a
+00003d00: 646a 2220 616e 6420 4072 656c 3d22 6864  dj" and @rel="hd
+00003d10: 2220 616e 6420 7061 7265 6e74 3a3a 6e6f  " and parent::no
+00003d20: 6465 5b40 6361 743d 2261 7022 2061 6e64  de[@cat="ap" and
+00003d30: 2025 7369 6d70 6c65 7072 6564 6963 6174   %simplepredicat
+00003d40: 6976 6525 5d29 0d0a 2222 220d 0a0d 0a69  ive%]).."""....i
+00003d50: 6e64 6566 6465 7420 3d20 2222 2220 2840  ndefdet = """ (@
+00003d60: 7265 6c3d 2264 6574 2220 616e 6420 4070  rel="det" and @p
+00003d70: 743d 2276 6e77 2220 616e 6420 4076 7774  t="vnw" and @vwt
+00003d80: 7970 653d 226f 6e62 6570 2229 0d0a 2222  ype="onbep")..""
+00003d90: 220d 0a0d 0a0d 0a41 5354 415f 4342 696a  "......ASTA_CBij
+00003da0: 7a69 6e20 3d20 2222 220d 0a20 2020 2020  zin = """..     
+00003db0: 2020 2020 2825 4153 5441 5f77 616e 746d      (%ASTA_wantm
+00003dc0: 6161 7262 696a 7a69 6e25 206f 720d 0a09  aarbijzin% or...
+00003dd0: 0920 2025 4153 5441 5f64 7573 6269 6a7a  .  %ASTA_dusbijz
+00003de0: 696e 2529 0d0a 2222 220d 0a0d 0a41 5354  in%).."""....AST
+00003df0: 415f 4342 696a 7a69 6e7a 696e 203d 2022  A_CBijzinzin = "
+00003e00: 2222 0d0a 2820 2541 5354 415f 7761 6e74  ""..( %ASTA_want
+00003e10: 6d61 6172 6269 6a7a 696e 7a69 6e25 206f  maarbijzinzin% o
+00003e20: 720d 0a20 2025 4153 5441 5f64 7573 6269  r..  %ASTA_dusbi
+00003e30: 6a7a 696e 7a69 6e25 0d0a 290d 0a22 2222  jzinzin%..).."""
+00003e40: 0d0a 0d0a 4153 5441 5f6f 6c64 4269 6a7a  ....ASTA_oldBijz
+00003e50: 696e 203d 2022 2222 0d0a 2020 2828 6e6f  in = """..  ((no
+00003e60: 6465 5b40 6361 743d 2273 7375 6222 5d20  de[@cat="ssub"] 
+00003e70: 6f72 2028 4063 6174 3d22 7376 3122 2061  or (@cat="sv1" a
+00003e80: 6e64 2040 7265 6c3d 226d 6f64 2220 2929  nd @rel="mod" ))
+00003e90: 206f 7220 0d0a 2020 2020 2020 2020 2025   or ..         %
+00003ea0: 4153 5441 5f77 616e 746d 6161 7262 696a  ASTA_wantmaarbij
+00003eb0: 7a69 6e25 206f 720d 0a09 0920 2541 5354  zin% or.... %AST
+00003ec0: 415f 6475 7362 696a 7a69 6e25 0d0a 2020  A_dusbijzin%..  
+00003ed0: 290d 0a09 0d0a 2222 220d 0a0d 0a0d 0a6f  )....."""......o
+00003ee0: 6c64 3241 5354 415f 4269 6a7a 696e 203d  ld2ASTA_Bijzin =
+00003ef0: 2022 2222 0d0a 2028 2020 2020 2020 2028   """.. (       (
+00003f00: 616e 6365 7374 6f72 3a3a 6e6f 6465 5b40  ancestor::node[@
+00003f10: 6361 743d 2274 6f70 2220 616e 6420 0d0a  cat="top" and ..
+00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f30: 2020 2020 2020 2020 2063 6f75 6e74 282e           count(.
+00003f40: 2f2f 6e6f 6465 5b40 6361 743d 2273 6d61  //node[@cat="sma
+00003f50: 696e 2220 6f72 2040 6361 743d 2273 7631  in" or @cat="sv1
+00003f60: 2220 6f72 200d 0a09 0909 0909 0920 2020  " or ........   
+00003f70: 2020 2020 2020 2020 2020 2028 4063 6174             (@cat
+00003f80: 3d22 7373 7562 2220 616e 6420 4072 656c  ="ssub" and @rel
+00003f90: 3d22 636e 6a22 2920 6f72 200d 0a09 0909  ="cnj") or .....
+00003fa0: 0909 0909 0909 2020 4063 6174 3d22 7768  ......  @cat="wh
+00003fb0: 7265 6c22 206f 7220 0d0a 0909 0909 0909  rel" or ........
+00003fc0: 0909 0920 2040 6361 743d 2272 656c 2220  ...  @cat="rel" 
+00003fd0: 6f72 200d 0a09 0909 0909 0909 0909 2020  or ...........  
+00003fe0: 4063 6174 3d22 7768 7375 6222 206f 7220  @cat="whsub" or 
+00003ff0: 0d0a 0909 0909 0909 0909 0920 2040 6361  ...........  @ca
+00004000: 743d 2263 7022 5d29 203e 2031 205d 2920  t="cp"]) > 1 ]) 
+00004010: 616e 6420 0d0a 2020 2020 2020 2020 2028  and ..         (
+00004020: 2840 6361 743d 2273 7375 6222 2061 6e64  (@cat="ssub" and
+00004030: 2040 7265 6c3d 2263 6e6a 2229 206f 720d   @rel="cnj") or.
+00004040: 0a20 2020 2020 2020 2020 2028 4063 6174  .          (@cat
+00004050: 3d22 7768 7265 6c22 206f 7220 4063 6174  ="whrel" or @cat
+00004060: 3d22 7265 6c22 206f 7220 4063 6174 3d22  ="rel" or @cat="
+00004070: 7768 7375 6222 2920 6f72 0d0a 2020 2020  whsub") or..    
+00004080: 2020 2020 2020 2840 6361 743d 2263 7022        (@cat="cp"
+00004090: 2061 6e64 206e 6f64 655b 4063 6174 3d22   and node[@cat="
+000040a0: 7373 7562 225d 2909 6f72 0920 200d 0a09  ssub"]).or.  ...
+000040b0: 0920 2028 4063 6174 3d22 7376 3122 2061  .  (@cat="sv1" a
+000040c0: 6e64 2028 4072 656c 3d22 6d6f 6422 206f  nd (@rel="mod" o
+000040d0: 7220 4072 656c 3d22 636e 6a22 2920 2920  r @rel="cnj") ) 
+000040e0: 6f72 200d 0a09 0920 2028 4063 6174 3d22  or ....  (@cat="
+000040f0: 736d 6169 6e22 2061 6e64 2028 4072 656c  smain" and (@rel
+00004100: 3d22 636e 6a22 206f 7220 4072 656c 3d22  ="cnj" or @rel="
+00004110: 626f 6479 2220 6f72 2040 7265 6c3d 226e  body" or @rel="n
+00004120: 7563 6c22 2920 616e 6420 6e6f 7428 2541  ucl") and not(%A
+00004130: 5354 415f 4342 696a 7a69 6e7a 696e 2529  STA_CBijzinzin%)
+00004140: 2920 6f72 0d0a 0909 2020 2840 6361 743d  ) or....  (@cat=
+00004150: 226f 7469 2229 206f 720d 0a09 0920 2020  "oti") or....   
+00004160: 2541 5354 415f 4342 696a 7a69 6e25 200d  %ASTA_CBijzin% .
+00004170: 0a09 0920 2029 0d0a 200d 0a20 290d 0a22  ...  ).. .. ).."
+00004180: 2222 0d0a 0d0a 4153 5441 5f42 696a 7a69  ""....ASTA_Bijzi
+00004190: 6e20 3d20 2222 220d 0a20 2820 2020 2020  n = """.. (     
+000041a0: 2020 200d 0a20 2020 2020 2020 2020 2828     ..         ((
+000041b0: 4063 6174 3d22 7373 7562 2220 616e 6420  @cat="ssub" and 
+000041c0: 4072 656c 3d22 636e 6a22 2061 6e64 206e  @rel="cnj" and n
+000041d0: 6f74 2825 6669 7273 7473 7375 6263 6f6e  ot(%firstssubcon
+000041e0: 6a75 6e63 7425 2920 616e 6420 6e6f 7428  junct%) and not(
+000041f0: 2541 5354 415f 4342 696a 7a69 6e7a 696e  %ASTA_CBijzinzin
+00004200: 2529 2920 6f72 0d0a 2020 2020 2020 2020  %)) or..        
+00004210: 2020 2840 6361 743d 2277 6872 656c 2220    (@cat="whrel" 
+00004220: 6f72 2040 6361 743d 2272 656c 2220 6f72  or @cat="rel" or
+00004230: 2040 6361 743d 2277 6873 7562 2229 206f   @cat="whsub") o
+00004240: 720d 0a09 0920 2028 2840 6361 743d 2273  r....  ((@cat="s
+00004250: 6d61 696e 2220 6f72 2040 6361 743d 2273  main" or @cat="s
+00004260: 7631 2229 616e 6420 4072 656c 3d22 2d2d  v1")and @rel="--
+00004270: 2229 206f 720d 0a20 2020 2020 2020 2020  ") or..         
+00004280: 2028 4063 6174 3d22 6370 2220 616e 6420   (@cat="cp" and 
+00004290: 6e6f 6465 5b40 6361 743d 2273 7375 6222  node[@cat="ssub"
+000042a0: 206f 7220 4063 6174 3d22 636f 6e6a 225d   or @cat="conj"]
+000042b0: 2909 6f72 0920 200d 0a09 0920 2028 4063  ).or.  ....  (@c
+000042c0: 6174 3d22 7376 3122 2061 6e64 2028 4072  at="sv1" and (@r
+000042d0: 656c 3d22 6d6f 6422 206f 7220 4072 656c  el="mod" or @rel
+000042e0: 3d22 636e 6a22 2920 2920 6f72 200d 0a09  ="cnj") ) or ...
+000042f0: 0920 2028 4063 6174 3d22 736d 6169 6e22  .  (@cat="smain"
+00004300: 2061 6e64 2028 4072 656c 3d22 636e 6a22   and (@rel="cnj"
+00004310: 206f 7220 4072 656c 3d22 626f 6479 2220   or @rel="body" 
+00004320: 6f72 2040 7265 6c3d 226e 7563 6c22 206f  or @rel="nucl" o
+00004330: 7220 4072 656c 3d22 6470 2229 2061 6e64  r @rel="dp") and
+00004340: 206e 6f74 2825 4153 5441 5f43 4269 6a7a   not(%ASTA_CBijz
+00004350: 696e 7a69 6e25 2929 206f 720d 0a09 0920  inzin%)) or.... 
+00004360: 2028 4063 6174 3d22 6f74 6922 2920 6f72   (@cat="oti") or
+00004370: 0d0a 0909 2020 2025 4153 5441 5f43 4269  ....   %ASTA_CBi
+00004380: 6a7a 696e 2520 6f72 0d0a 0909 2020 2025  jzin% or....   %
+00004390: 6469 7265 6374 6572 6564 655f 7663 6269  directerede_vcbi
+000043a0: 6a7a 696e 2520 6f72 0d0a 0909 2020 2028  jzin% or....   (
+000043b0: 4070 743d 2276 6722 2061 6e64 2040 636f  @pt="vg" and @co
+000043c0: 6e6a 7479 7065 3d22 6f6e 6465 7222 2061  njtype="onder" a
+000043d0: 6e64 2040 7265 6c3d 222d 2d22 2020 2920  nd @rel="--"  ) 
+000043e0: 6f72 0d0a 0909 2020 2028 2840 7074 3d22  or....   ((@pt="
+000043f0: 6277 2220 6f72 2040 7074 3d22 766e 7722  bw" or @pt="vnw"
+00004400: 2920 616e 6420 4072 656c 3d22 7663 2220  ) and @rel="vc" 
+00004410: 616e 6420 4077 683d 2279 7768 2229 0d0a  and @wh="ywh")..
+00004420: 0909 2020 290d 0a20 0d0a 2029 0d0a 2222  ..  ).. .. )..""
+00004430: 220d 0a0d 0a66 6972 7374 7373 7562 636f  "....firstssubco
+00004440: 6e6a 756e 6374 203d 2022 2222 2825 6669  njunct = """(%fi
+00004450: 7273 7473 7375 6263 6f6e 6a75 6e63 7461  rstssubconjuncta
+00004460: 2520 6f72 2025 6669 7273 7473 7375 6263  % or %firstssubc
+00004470: 6f6e 6a75 6e63 7462 2529 2222 220d 0a66  onjunctb%)"""..f
+00004480: 6972 7374 7373 7562 636f 6e6a 756e 6374  irstssubconjunct
+00004490: 6120 3d20 2222 2228 4063 6174 3d22 7373  a = """(@cat="ss
+000044a0: 7562 2220 616e 6420 4062 6567 696e 3d6e  ub" and @begin=n
+000044b0: 6f64 655b 4063 6174 206f 7220 4070 745d  ode[@cat or @pt]
+000044c0: 2f40 6265 6769 6e20 616e 6420 4062 6567  /@begin and @beg
+000044d0: 696e 3d70 6172 656e 743a 3a6e 6f64 655b  in=parent::node[
+000044e0: 4063 6174 3d22 636f 6e6a 225d 2f70 6172  @cat="conj"]/par
+000044f0: 656e 743a 3a6e 6f64 655b 4063 6174 3d22  ent::node[@cat="
+00004500: 6370 225d 2f6e 6f64 655b 4070 743d 2276  cp"]/node[@pt="v
+00004510: 6722 5d2f 4065 6e64 2029 2222 220d 0a66  g"]/@end )"""..f
+00004520: 6972 7374 7373 7562 636f 6e6a 756e 6374  irstssubconjunct
+00004530: 6220 3d20 2222 2228 4063 6174 3d22 7373  b = """(@cat="ss
+00004540: 7562 2220 616e 6420 4062 6567 696e 3d6e  ub" and @begin=n
+00004550: 6f64 655b 4063 6174 206f 7220 4070 745d  ode[@cat or @pt]
+00004560: 2f40 6265 6769 6e20 616e 6420 4062 6567  /@begin and @beg
+00004570: 696e 3d70 6172 656e 743a 3a6e 6f64 655b  in=parent::node[
+00004580: 4063 6174 3d22 636f 6e6a 225d 2f70 6172  @cat="conj"]/par
+00004590: 656e 743a 3a6e 6f64 655b 4063 6174 3d22  ent::node[@cat="
+000045a0: 7265 6c22 5d2f 6e6f 6465 5b40 7265 6c3d  rel"]/node[@rel=
+000045b0: 2272 6864 225d 2f40 656e 6420 2922 2222  "rhd"]/@end )"""
+000045c0: 0d0a 0d0a 6269 6a7a 696e 6361 7420 3d20  ....bijzincat = 
+000045d0: 2222 2228 2040 6361 743d 2273 6d61 696e  """( @cat="smain
+000045e0: 2220 6f72 2040 6361 743d 2273 7631 2220  " or @cat="sv1" 
+000045f0: 6f72 200d 0a09 0909 0909 0920 2020 2020  or ........     
+00004600: 2020 2020 2020 2020 2028 4063 6174 3d22           (@cat="
+00004610: 7373 7562 2220 616e 6420 4072 656c 3d22  ssub" and @rel="
+00004620: 636e 6a22 2920 6f72 200d 0a09 0909 0909  cnj") or .......
+00004630: 0909 0909 2020 4063 6174 3d22 7768 7265  ....  @cat="whre
+00004640: 6c22 206f 7220 0d0a 0909 0909 0909 0909  l" or ..........
+00004650: 0920 2040 6361 743d 2272 656c 2220 6f72  .  @cat="rel" or
+00004660: 200d 0a09 0909 0909 0909 0909 2020 4063   ...........  @c
+00004670: 6174 3d22 7768 7375 6222 206f 7220 0d0a  at="whsub" or ..
+00004680: 0909 0909 0909 0909 0920 2040 6361 743d  .........  @cat=
+00004690: 2263 7022 2922 2222 0d0a 0d0a 6269 6a7a  "cp")"""....bijz
+000046a0: 696e 6e6f 6465 203d 2022 2222 2028 616e  innode = """ (an
+000046b0: 6365 7374 6f72 3a3a 6e6f 6465 5b40 6361  cestor::node[@ca
+000046c0: 743d 2274 6f70 2220 616e 6420 0d0a 2020  t="top" and ..  
+000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046e0: 2020 2020 2020 202e 2f2f 6e6f 6465 5b25         .//node[%
+000046f0: 6269 6a7a 696e 6361 7425 5d20 205d 2922  bijzincat%]  ])"
+00004700: 2222 0d0a 0909 0909 0909 0909 0920 200d  ""...........  .
+00004710: 0a09 0909 0909 0909 0909 2020 0d0a 6e6f  ..........  ..no
+00004720: 7466 6972 7374 6269 6a7a 696e 203d 2022  tfirstbijzin = "
+00004730: 2222 2825 6269 6a7a 696e 6361 7425 2061  ""(%bijzincat% a
+00004740: 6e64 2063 6f75 6e74 2825 6269 6a7a 696e  nd count(%bijzin
+00004750: 6e6f 6465 2529 203e 2031 2020 616e 6420  node%) > 1  and 
+00004760: 4062 6567 696e 5b6e 6f74 2820 2e20 3e20  @begin[not( . > 
+00004770: 2562 696a 7a69 6e6e 6f64 6525 2f40 6265  %bijzinnode%/@be
+00004780: 6769 6e29 5d5b 315d 2922 2222 2009 0909  gin)][1])""" ...
+00004790: 0d0a 0d0a 0d0a 5461 7273 705f 6e6f 6e6d  ......Tarsp_nonm
+000047a0: 6f64 6164 7663 7020 3d20 2222 2228 4063  odadvcp = """(@c
+000047b0: 6174 3d22 6370 2220 616e 6420 2840 7265  at="cp" and (@re
+000047c0: 6c3d 2264 7022 206f 7220 4072 656c 3d22  l="dp" or @rel="
+000047d0: 2d2d 2229 2061 6e64 206e 6f64 655b 4070  --") and node[@p
+000047e0: 743d 2276 6722 2061 6e64 2040 636f 6e6a  t="vg" and @conj
+000047f0: 7479 7065 3d22 6f6e 6465 7222 2061 6e64  type="onder" and
+00004800: 2040 6c65 6d6d 6121 3d22 6461 7422 2061   @lemma!="dat" a
+00004810: 6e64 2040 6c65 6d6d 6121 3d22 6f66 2220  nd @lemma!="of" 
+00004820: 5d20 2922 2222 0d0a 0d0a 0d0a 0d0a 6469  ] )"""........di
+00004830: 7265 6374 6572 6564 655f 7663 6269 6a7a  recterede_vcbijz
+00004840: 696e 203d 2022 2222 2820 2563 6c61 7573  in = """( %claus
+00004850: 6563 6174 2520 616e 6420 6e6f 7428 4072  ecat% and not(@r
+00004860: 656c 3d22 636e 6a22 2920 616e 6420 2870  el="cnj") and (p
+00004870: 7265 6365 6469 6e67 2d73 6962 6c69 6e67  receding-sibling
+00004880: 3a3a 6e6f 6465 5b25 6d65 7461 736d 6169  ::node[%metasmai
+00004890: 6e25 5d20 6f72 2066 6f6c 6c6f 7769 6e67  n%] or following
+000048a0: 2d73 6962 6c69 6e67 3a3a 6e6f 6465 5b25  -sibling::node[%
+000048b0: 6d65 7461 7376 3125 5d29 2922 2222 0d0a  metasv1%]))"""..
+000048c0: 0d0a 0d0a 636c 6175 7365 6361 7420 3d20  ....clausecat = 
+000048d0: 2222 2228 4063 6174 3d22 736d 6169 6e22  """(@cat="smain"
+000048e0: 206f 7220 4063 6174 3d22 7768 7122 206f   or @cat="whq" o
+000048f0: 7220 2562 6172 6573 7631 2520 2922 2222  r %baresv1% )"""
+00004900: 0d0a 6d65 7461 7665 7262 203d 2022 2222  ..metaverb = """
+00004910: 2840 6c65 6d6d 613d 227a 6567 6765 6e22  (@lemma="zeggen"
+00004920: 206f 7220 406c 656d 6d61 3d22 6465 6e6b   or @lemma="denk
+00004930: 656e 2220 6f72 2040 6c65 6d6d 613d 2276  en" or @lemma="v
+00004940: 696e 6465 6e22 206f 7220 406c 656d 6d61  inden" or @lemma
+00004950: 3d22 7672 6167 656e 2220 6f72 2040 6c65  ="vragen" or @le
+00004960: 6d6d 613d 2273 6368 7265 6575 7765 6e22  mma="schreeuwen"
+00004970: 206f 7220 406c 656d 6d61 3d22 666c 7569   or @lemma="flui
+00004980: 7374 6572 656e 2220 2922 2222 0d0a 6d65  steren" )"""..me
+00004990: 7461 736d 6169 6e20 3d20 2222 2228 4063  tasmain = """(@c
+000049a0: 6174 3d22 736d 6169 6e22 2061 6e64 206e  at="smain" and n
+000049b0: 6f74 2840 7265 6c3d 2263 6e6a 2229 2061  ot(@rel="cnj") a
+000049c0: 6e64 206e 6f64 655b 4072 656c 3d22 6864  nd node[@rel="hd
+000049d0: 2220 616e 6420 256d 6574 6176 6572 6225  " and %metaverb%
+000049e0: 5d29 2022 2222 0d0a 6d65 7461 7376 3120  ]) """..metasv1 
+000049f0: 3d20 2222 2228 4063 6174 3d22 7376 3122  = """(@cat="sv1"
+00004a00: 2061 6e64 206e 6f74 2840 7265 6c3d 2263   and not(@rel="c
+00004a10: 6e6a 2229 2061 6e64 206e 6f64 655b 4072  nj") and node[@r
+00004a20: 656c 3d22 6864 2220 616e 6420 256d 6574  el="hd" and %met
+00004a30: 6176 6572 6225 5d29 2022 2222 0d0a 0d0a  averb%]) """....
+00004a40: 6261 7265 7376 3120 3d20 2222 2228 2040  baresv1 = """( @
+00004a50: 6361 743d 2273 7631 2220 616e 6420 6e6f  cat="sv1" and no
+00004a60: 7428 7061 7265 6e74 3a3a 6e6f 6465 5b28  t(parent::node[(
+00004a70: 4063 6174 3d22 7768 7122 206f 7220 4063  @cat="whq" or @c
+00004a80: 6174 3d22 7768 7265 6c22 295d 2929 2222  at="whrel")]))""
+00004a90: 220d 0a0d 0a0d 0a64 656c 7076 5f6e 6f6e  "......delpv_non
+00004aa0: 6669 6e63 6174 203d 2022 2222 2840 6361  fincat = """(@ca
+00004ab0: 743d 2270 7072 6573 2220 6f72 2040 6361  t="ppres" or @ca
+00004ac0: 743d 2270 7061 7274 2220 6f72 2040 6361  t="ppart" or @ca
+00004ad0: 743d 2274 6922 206f 7220 4063 6174 3d22  t="ti" or @cat="
+00004ae0: 6f74 6922 206f 7220 4063 6174 3d22 6168  oti" or @cat="ah
+00004af0: 6922 206f 7220 2840 6361 743d 2269 6e66  i" or (@cat="inf
+00004b00: 2220 616e 6420 4070 6f73 6974 6965 213d  " and @positie!=
+00004b10: 226e 6f6d 2229 2029 2022 2222 0d0a 6465  "nom") ) """..de
+00004b20: 6c70 765f 636c 6175 7365 6361 7420 3d20  lpv_clausecat = 
+00004b30: 2222 2228 4063 6174 3d22 736d 6169 6e22  """(@cat="smain"
+00004b40: 206f 7220 4063 6174 3d22 7373 7562 2220   or @cat="ssub" 
+00004b50: 6f72 2040 6361 743d 2273 7631 2220 6f72  or @cat="sv1" or
+00004b60: 2040 6361 743d 2270 7072 6573 2220 6f72   @cat="ppres" or
+00004b70: 2040 6361 743d 2270 7061 7274 2220 6f72   @cat="ppart" or
+00004b80: 2040 6361 743d 2274 6922 206f 7220 4063   @cat="ti" or @c
+00004b90: 6174 3d22 6f74 6922 206f 7220 4063 6174  at="oti" or @cat
+00004ba0: 3d22 6168 6922 206f 7220 4063 6174 3d22  ="ahi" or @cat="
+00004bb0: 696e 6622 2922 2222 0d0a 6465 6c70 765f  inf")"""..delpv_
+00004bc0: 6e6f 6e66 696e 7777 203d 2022 2222 2840  nonfinww = """(@
+00004bd0: 7074 3d22 7777 2220 616e 6420 2840 7776  pt="ww" and (@wv
+00004be0: 6f72 6d3d 2274 6422 206f 7220 2840 7776  orm="td" or (@wv
+00004bf0: 6f72 6d3d 2269 6e66 2220 616e 6420 4070  orm="inf" and @p
+00004c00: 6f73 6974 6965 213d 226e 6f6d 2229 206f  ositie!="nom") o
+00004c10: 7220 4077 766f 726d 3d22 7664 2229 2029  r @wvorm="vd") )
+00004c20: 2222 220d 0a0d 0a63 6f72 6564 656c 7076  """....coredelpv
+00004c30: 203d 2022 2222 2828 2564 656c 7076 5f6e   = """((%delpv_n
+00004c40: 6f6e 6669 6e63 6174 2520 6f72 2025 6465  onfincat% or %de
+00004c50: 6c70 765f 6e6f 6e66 696e 7777 2520 2920  lpv_nonfinww% ) 
+00004c60: 616e 6420 6e6f 7428 616e 6365 7374 6f72  and not(ancestor
+00004c70: 3a3a 6e6f 6465 5b25 6465 6c70 765f 636c  ::node[%delpv_cl
+00004c80: 6175 7365 6361 7425 5d29 2029 2222 220d  ausecat%]) )""".
+00004c90: 0a0d 0a72 6f62 7573 7464 656c 7076 203d  ...robustdelpv =
+00004ca0: 2022 2222 286e 6f74 2840 7265 6c3d 2264   """(not(@rel="d
+00004cb0: 7022 2061 6e64 2040 6265 6769 6e20 3e20  p" and @begin > 
+00004cc0: 616e 6365 7374 6f72 3a3a 6e6f 6465 5b40  ancestor::node[@
+00004cd0: 6361 743d 2274 6f70 225d 2f64 6573 6365  cat="top"]/desce
+00004ce0: 6e64 616e 743a 3a6e 6f64 655b 4072 656c  ndant::node[@rel
+00004cf0: 3d22 6470 225d 2f64 6573 6365 6e64 616e  ="dp"]/descendan
+00004d00: 743a 3a6e 6f64 655b 4070 743d 2277 7722  t::node[@pt="ww"
+00004d10: 2061 6e64 2040 7776 6f72 6d3d 2270 7622   and @wvorm="pv"
+00004d20: 5d2f 4062 6567 696e 2929 2222 220d 0a0d  ]/@begin))"""...
+00004d30: 0a64 656c 7076 203d 2022 2222 2825 636f  .delpv = """(%co
+00004d40: 7265 6465 6c70 7625 2061 6e64 2025 726f  redelpv% and %ro
+00004d50: 6275 7374 6465 6c70 7625 2922 2222 0d0a  bustdelpv%)"""..
+00004d60: 0d0a 566f 6269 6a20 3d20 2222 2228 4070  ..Vobij = """(@p
+00004d70: 743d 2262 7722 2061 6e64 2028 636f 6e74  t="bw" and (cont
+00004d80: 6169 6e73 2840 6672 616d 652c 2265 725f  ains(@frame,"er_
+00004d90: 6164 7665 7262 2220 2920 6f72 2063 6f6e  adverb" ) or con
+00004da0: 7461 696e 7328 4066 7261 6d65 2c20 2274  tains(@frame, "t
+00004db0: 6d70 5f61 6476 6572 6222 2920 6f72 2063  mp_adverb") or c
+00004dc0: 6f6e 7461 696e 7328 4066 7261 6d65 2c20  ontains(@frame, 
+00004dd0: 2277 6161 725f 6164 7665 7262 2229 206f  "waar_adverb") o
+00004de0: 7220 406c 656d 6d61 3d22 6461 6172 6f6d  r @lemma="daarom
+00004df0: 2229 2061 6e64 200d 0a40 6c65 6d6d 6121  ") and ..@lemma!
+00004e00: 3d22 6572 2220 616e 6420 406c 656d 6d61  ="er" and @lemma
+00004e10: 213d 2264 6161 7222 2061 6e64 2040 6c65  !="daar" and @le
+00004e20: 6d6d 6121 3d22 6869 6572 2220 616e 6420  mma!="hier" and 
+00004e30: 406c 656d 6d61 213d 2277 6161 7222 2061  @lemma!="waar" a
+00004e40: 6e64 2028 7374 6172 7473 2d77 6974 6828  nd (starts-with(
+00004e50: 406c 656d 6d61 2c20 2765 7227 2920 6f72  @lemma, 'er') or
+00004e60: 2073 7461 7274 732d 7769 7468 2840 6c65   starts-with(@le
+00004e70: 6d6d 612c 2027 6461 6172 2729 206f 7220  mma, 'daar') or 
+00004e80: 7374 6172 7473 2d77 6974 6828 406c 656d  starts-with(@lem
+00004e90: 6d61 2c20 2768 6965 7227 2920 6f72 2073  ma, 'hier') or s
+00004ea0: 7461 7274 732d 7769 7468 2840 6c65 6d6d  tarts-with(@lemm
+00004eb0: 612c 2027 7761 6172 2729 2929 2222 220d  a, 'waar')))""".
+00004ec0: 0a0d 0a54 6172 7370 5f56 7a4e 203d 2022  ...Tarsp_VzN = "
+00004ed0: 2222 2825 767a 6e31 7870 6174 6825 206f  ""(%vzn1xpath% o
+00004ee0: 7220 2576 7a6e 3278 7061 7468 2520 2920  r %vzn2xpath% ) 
+00004ef0: 2222 220d 0a0d 0a76 7a6e 3178 7061 7468  """....vzn1xpath
+00004f00: 203d 2022 2222 2840 6361 743d 2270 7022   = """(@cat="pp"
+00004f10: 2061 6e64 2028 6e6f 6465 5b40 7074 3d22   and (node[@pt="
+00004f20: 767a 225d 2061 6e64 206e 6f64 655b 2840  vz"] and node[(@
+00004f30: 7074 3d22 6e22 206f 7220 4070 743d 2276  pt="n" or @pt="v
+00004f40: 6e77 2229 2061 6e64 206e 6f74 2028 2552  nw") and not (%R
+00004f50: 7072 6f6e 6f75 6e25 2920 616e 6420 4072  pronoun%) and @r
+00004f60: 656c 3d22 6f62 6a31 225d 2061 6e64 206e  el="obj1"] and n
+00004f70: 6f74 286e 6f64 655b 4070 743d 2276 7a22  ot(node[@pt="vz"
+00004f80: 2061 6e64 2040 767a 7479 7065 3d22 6669   and @vztype="fi
+00004f90: 6e22 5d29 2929 2222 220d 0a76 7a6e 3278  n"])))"""..vzn2x
+00004fa0: 7061 7468 203d 2022 2222 286e 6f64 655b  path = """(node[
+00004fb0: 406c 656d 6d61 3d22 696e 2220 616e 6420  @lemma="in" and 
+00004fc0: 4072 656c 3d22 6d77 7022 5d20 616e 6420  @rel="mwp"] and 
+00004fd0: 6e6f 6465 5b40 6c65 6d6d 613d 2264 657a  node[@lemma="dez
+00004fe0: 6522 2061 6e64 2040 7265 6c3d 226d 7770  e" and @rel="mwp
+00004ff0: 225d 2922 2222 0d0a 767a 6e33 7870 6174  "])"""..vzn3xpat
+00005000: 6820 3d20 2222 2228 4070 743d 2276 7a22  h = """(@pt="vz"
+00005010: 2061 6e64 202e 2e2f 6e6f 6465 5b28 406c   and ../node[(@l
+00005020: 656d 6d61 3d22 6469 7422 206f 7220 406c  emma="dit" or @l
+00005030: 656d 6d61 3d22 6461 7422 2920 2061 6e64  emma="dat")  and
+00005040: 2040 6265 6769 6e3e 3d2e 2e2f 6e6f 6465   @begin>=../node
+00005050: 5b40 7074 3d22 767a 225d 2f40 656e 6420  [@pt="vz"]/@end 
+00005060: 616e 6420 636f 756e 7428 6e6f 6465 293c  and count(node)<
+00005070: 3d33 5d20 2922 2222 0d0a 0d0a 6e6f 5270  =3] )"""....noRp
+00005080: 726f 6e6f 756e 7820 3d20 2222 226e 6f74  ronounx = """not
+00005090: 2861 6e63 6573 746f 723a 3a6e 6f64 655b  (ancestor::node[
+000050a0: 4063 6174 3d22 746f 7022 5d2f 6465 7363  @cat="top"]/desc
+000050b0: 656e 6461 6e74 3a3a 6e6f 6465 5b25 5270  endant::node[%Rp
+000050c0: 726f 6e6f 756e 7825 5d29 2222 220d 0a0d  ronounx%])"""...
+000050d0: 0a74 7261 6e73 6974 6976 6576 7a20 3d20  .transitivevz = 
+000050e0: 2222 2228 2040 6c65 6d6d 613d 2761 616e  """( @lemma='aan
+000050f0: 2720 6f72 2040 6c65 6d6d 613d 2762 696a  ' or @lemma='bij
+00005100: 2720 6f72 2040 6c65 6d6d 613d 2764 6f6f  ' or @lemma='doo
+00005110: 7227 206f 7220 406c 656d 6d61 3d27 696e  r' or @lemma='in
+00005120: 2720 6f72 2040 6c65 6d6d 613d 276e 6161  ' or @lemma='naa
+00005130: 7227 206f 7220 406c 656d 6d61 3d27 6e61  r' or @lemma='na
+00005140: 6172 746f 6527 2020 6f72 200d 0a20 2020  artoe'  or ..   
+00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005160: 2040 6c65 6d6d 613d 276f 7027 206f 7220   @lemma='op' or 
+00005170: 2040 6c65 6d6d 613d 276f 7665 7227 206f   @lemma='over' o
+00005180: 7220 2020 406c 656d 6d61 3d27 7465 6765  r   @lemma='tege
+00005190: 6e27 206f 7220 406c 656d 6d61 3d27 746f  n' or @lemma='to
+000051a0: 6527 206f 7220 2040 6c65 6d6d 613d 2774  e' or  @lemma='t
+000051b0: 7573 7365 6e27 206f 7220 406c 656d 6d61  ussen' or @lemma
+000051c0: 3d27 7569 7427 206f 720d 0a09 0909 0909  ='uit' or.......
+000051d0: 406c 656d 6d61 3d27 7661 6e27 206f 7220  @lemma='van' or 
+000051e0: 2040 6c65 6d6d 613d 2776 6f6f 7227 0d0a   @lemma='voor'..
+000051f0: 0909 0909 0929 2222 220d 0a0d 0a52 7072  .....)"""....Rpr
+00005200: 6f6e 6f75 6e78 203d 2022 2222 2825 5270  onounx = """(%Rp
+00005210: 726f 6e6f 756e 2520 6f72 2040 6c65 6d6d  ronoun% or @lemm
+00005220: 613d 2264 6161 727a 6f22 206f 7220 406c  a="daarzo" or @l
+00005230: 656d 6d61 3d22 6869 6572 7a6f 2229 2022  emma="hierzo") "
+00005240: 2222 0d0a 0d0a 666f 6c6c 6f77 6564 6279  ""....followedby
+00005250: 6465 7420 3d20 2222 2228 4065 6e64 3d61  det = """(@end=a
+00005260: 6e63 6573 746f 723a 3a6e 6f64 655b 4063  ncestor::node[@c
+00005270: 6174 3d22 746f 7022 5d2f 6465 7363 656e  at="top"]/descen
+00005280: 6461 6e74 3a3a 6e6f 6465 5b25 6465 7425  dant::node[%det%
+00005290: 5d2f 4062 6567 696e 2922 2222 0d0a 0d0a  ]/@begin)"""....
+000052a0: 6465 7420 3d20 2222 2228 4070 743d 226c  det = """(@pt="l
+000052b0: 6964 2220 6f72 2040 6c65 6d6d 613d 2264  id" or @lemma="d
+000052c0: 6974 2220 6f72 2040 6c65 6d6d 613d 2264  it" or @lemma="d
+000052d0: 657a 6522 206f 7220 406c 656d 6d61 3d22  eze" or @lemma="
+000052e0: 6469 6522 206f 7220 406c 656d 6d61 3d22  die" or @lemma="
+000052f0: 6461 7422 206f 7220 2840 7074 3d22 766e  dat" or (@pt="vn
+00005300: 7722 2061 6e64 2040 7677 7479 7065 3d22  w" and @vwtype="
+00005310: 6265 7a22 2920 2920 2222 220d 0a0d 0a0d  bez") ) """.....
+00005320: 0a76 7277 6f6e 6470 6c75 7320 3d20 2222  .vrwondplus = ""
+00005330: 2228 2577 6871 7376 3125 206f 7220 2562  "(%whqsv1% or %b
+00005340: 6173 6963 7672 776f 6e64 706c 7573 2520  asicvrwondplus% 
+00005350: 6f72 2025 6261 7369 6376 7277 6f6e 6470  or %basicvrwondp
+00005360: 6c75 736e 6f73 7562 6a25 2922 2222 0d0a  lusnosubj%)"""..
+00005370: 0d0a 7768 7173 7631 203d 2022 2222 2840  ..whqsv1 = """(@
+00005380: 6361 743d 2277 6871 2229 2061 6e64 206e  cat="whq") and n
+00005390: 6f64 655b 4063 6174 3d22 7376 3122 2061  ode[@cat="sv1" a
+000053a0: 6e64 2040 7265 6c3d 2262 6f64 7922 5d20  nd @rel="body"] 
+000053b0: 616e 6420 636f 756e 7428 6e6f 6465 293d  and count(node)=
+000053c0: 3122 2222 0d0a 0d0a 6261 7369 6376 7277  1"""....basicvrw
+000053d0: 6f6e 6470 6c75 7320 3d20 2222 2228 0d0a  ondplus = """(..
+000053e0: 2040 6361 743d 2273 7631 2220 616e 6420   @cat="sv1" and 
+000053f0: 4072 656c 3d22 2d2d 2220 616e 6420 616e  @rel="--" and an
+00005400: 6365 7374 6f72 3a3a 6e6f 6465 5b40 6361  cestor::node[@ca
+00005410: 743d 2274 6f70 2220 616e 6420 6e6f 6465  t="top" and node
+00005420: 5b40 6c65 6d6d 613d 223f 225d 5d20 616e  [@lemma="?"]] an
+00005430: 640d 0a20 2020 2020 2020 206e 6f64 655b  d..        node[
+00005440: 4072 656c 3d22 6864 2220 616e 6420 2840  @rel="hd" and (@
+00005450: 6c65 6d6d 613d 227a 696a 6e22 206f 7220  lemma="zijn" or 
+00005460: 406c 656d 6d61 3d22 646f 656e 2220 6f72  @lemma="doen" or
+00005470: 2040 6c65 6d6d 613d 2268 6574 656e 2220   @lemma="heten" 
+00005480: 6f72 2040 6c65 6d6d 613d 226d 6f65 7465  or @lemma="moete
+00005490: 6e22 295d 2061 6e64 200d 0a20 2020 2020  n")] and ..     
+000054a0: 2020 206e 6f64 655b 4072 656c 3d22 7375     node[@rel="su
+000054b0: 2220 5d20 616e 640d 0a20 2020 2020 2020  " ] and..       
+000054c0: 206e 6f74 286e 6f64 655b 4072 656c 3d22   not(node[@rel="
+000054d0: 7375 2220 616e 6420 6e6f 6465 5b40 7265  su" and node[@re
+000054e0: 6c3d 226d 6f64 225d 5d29 2061 6e64 0d0a  l="mod"]]) and..
+000054f0: 2020 2020 2020 2020 6e6f 7428 6e6f 6465          not(node
+00005500: 5b28 4072 656c 3d22 6f62 6a31 2220 6f72  [(@rel="obj1" or
+00005510: 2040 7265 6c3d 2270 7265 6463 2220 6f72   @rel="predc" or
+00005520: 2040 7265 6c3d 226f 626a 3222 206f 7220   @rel="obj2" or 
+00005530: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00005540: 2020 2020 4072 656c 3d22 7663 2220 6f72      @rel="vc" or
+00005550: 2040 7265 6c3d 226c 6422 206f 7220 4072   @rel="ld" or @r
+00005560: 656c 3d22 7063 2220 6f72 2040 7265 6c3d  el="pc" or @rel=
+00005570: 2273 6522 295d 2920 616e 640d 0a20 2020  "se")]) and..   
+00005580: 2020 2020 206e 6f74 286e 6f64 655b 4072       not(node[@r
+00005590: 656c 3d22 6864 2220 616e 6420 406c 656d  el="hd" and @lem
+000055a0: 6d61 3d22 7a69 6a6e 225d 2061 6e64 206e  ma="zijn"] and n
+000055b0: 6f64 655b 4072 656c 3d22 6d6f 6422 2061  ode[@rel="mod" a
+000055c0: 6e64 2028 4063 6174 3d22 7070 2220 6f72  nd (@cat="pp" or
+000055d0: 2040 6361 743d 2263 7022 295d 2920 616e   @cat="cp")]) an
+000055e0: 640d 0a20 2020 2020 2020 206e 6f74 286e  d..        not(n
+000055f0: 6f64 655b 4072 656c 3d22 6864 2220 616e  ode[@rel="hd" an
+00005600: 6420 406c 656d 6d61 3d22 7a69 6a6e 225d  d @lemma="zijn"]
+00005610: 2061 6e64 206e 6f64 655b 4072 656c 3d22   and node[@rel="
+00005620: 6d6f 6422 2061 6e64 2025 5270 726f 6e6f  mod" and %Rprono
+00005630: 756e 255d 2920 616e 640d 0a09 096e 6f74  un%]) and....not
+00005640: 286e 6f64 655b 4072 656c 3d22 6d6f 6422  (node[@rel="mod"
+00005650: 2061 6e64 2040 6c65 6d6d 613d 226e 6965   and @lemma="nie
+00005660: 7422 5d20 616e 640d 0a09 096e 6f74 286e  t"] and....not(n
+00005670: 6f64 655b 4072 656c 3d22 6d6f 6422 2061  ode[@rel="mod" a
+00005680: 6e64 2040 6c65 6d6d 6121 3d22 6461 6e22  nd @lemma!="dan"
+00005690: 2061 6e64 2040 6c65 6d6d 6121 3d22 6e6f   and @lemma!="no
+000056a0: 7522 2061 6e64 2040 6c65 6d6d 6121 3d22  u" and @lemma!="
+000056b0: 7765 6572 225d 290d 0a09 0929 0d0a 2922  weer"])....)..)"
+000056c0: 2222 0d0a 0d0a 6261 7369 6376 7277 6f6e  ""....basicvrwon
+000056d0: 6470 6c75 736e 6f73 7562 6a20 3d20 2222  dplusnosubj = ""
+000056e0: 220d 0a28 200d 0a20 4063 6174 3d22 7376  "..( .. @cat="sv
+000056f0: 3122 2061 6e64 2040 7265 6c3d 222d 2d22  1" and @rel="--"
+00005700: 2061 6e64 2061 6e63 6573 746f 723a 3a6e   and ancestor::n
+00005710: 6f64 655b 4063 6174 3d22 746f 7022 2061  ode[@cat="top" a
+00005720: 6e64 206e 6f64 655b 406c 656d 6d61 3d22  nd node[@lemma="
+00005730: 3f22 5d5d 2061 6e64 0d0a 2020 2020 2020  ?"]] and..      
+00005740: 2020 6e6f 6465 5b40 7265 6c3d 2268 6422    node[@rel="hd"
+00005750: 2061 6e64 2040 7074 3d22 7777 2220 616e   and @pt="ww" an
+00005760: 6420 4077 766f 726d 3d22 7076 2220 616e  d @wvorm="pv" an
+00005770: 6420 4073 7479 7065 213d 2269 6d70 6172  d @stype!="impar
+00005780: 6174 6976 6522 5d20 616e 6420 0d0a 2020  ative"] and ..  
+00005790: 2020 2020 2020 6e6f 7428 6e6f 6465 5b40        not(node[@
+000057a0: 7265 6c3d 2276 6322 5d29 2061 6e64 0d0a  rel="vc"]) and..
+000057b0: 2020 2020 2020 2020 6e6f 7428 6e6f 6465          not(node
+000057c0: 5b40 6361 743d 226e 7022 2061 6e64 206e  [@cat="np" and n
+000057d0: 6f64 655b 4072 656c 3d22 6d6f 6422 5d5d  ode[@rel="mod"]]
+000057e0: 2920 616e 640d 0a20 2020 2020 2020 206e  ) and..        n
+000057f0: 6f74 286e 6f64 655b 4063 6174 3d22 6e70  ot(node[@cat="np
+00005800: 2220 616e 6420 6e6f 6465 5b40 7265 6c3d  " and node[@rel=
+00005810: 2264 6574 2220 616e 6420 0d0a 2020 2020  "det" and ..    
+00005820: 2020 2020 2020 2020 2020 2840 6c65 6d6d            (@lemm
+00005830: 6120 3d20 2264 6974 2220 6f72 2040 6c65  a = "dit" or @le
+00005840: 6d6d 613d 2264 6174 2220 6f72 2040 6c65  mma="dat" or @le
+00005850: 6d6d 613d 2264 6965 2220 6f72 2040 6c65  mma="die" or @le
+00005860: 6d6d 613d 2268 6574 2220 6f72 2040 6c65  mma="het" or @le
+00005870: 6d6d 613d 2264 6522 2920 5d5d 2920 616e  mma="de") ]]) an
+00005880: 640d 0a09 096e 6f74 286e 6f64 655b 4063  d....not(node[@c
+00005890: 6174 3d22 636f 6e6a 225d 2920 616e 640d  at="conj"]) and.
+000058a0: 0a20 2020 2020 2020 206e 6f74 286e 6f64  .        not(nod
+000058b0: 655b 4072 656c 3d22 6d6f 6422 2061 6e64  e[@rel="mod" and
+000058c0: 2040 6361 743d 2273 7631 225d 2920 616e   @cat="sv1"]) an
+000058d0: 640d 0a20 2020 2020 2020 206e 6f74 286e  d..        not(n
+000058e0: 6f64 655b 4072 656c 3d22 7375 2220 5d29  ode[@rel="su" ])
+000058f0: 2061 6e64 0d0a 0909 6e6f 7428 6e6f 6465   and....not(node
+00005900: 5b40 7265 6c3d 226d 6f64 2220 616e 6420  [@rel="mod" and 
+00005910: 406c 656d 6d61 213d 2264 616e 2220 616e  @lemma!="dan" an
+00005920: 6420 406c 656d 6d61 213d 226e 6f75 2220  d @lemma!="nou" 
+00005930: 616e 6420 406c 656d 6d61 213d 2277 6565  and @lemma!="wee
+00005940: 7222 2061 6e64 2040 6c65 6d6d 6121 3d22  r" and @lemma!="
+00005950: 6572 225d 2920 616e 640d 0a09 0928 6e6f  er"]) and....(no
+00005960: 7428 6e6f 6465 5b25 696e 7472 6d6f 6461  t(node[%intrmoda
+00005970: 6c76 6572 6225 5d20 616e 6420 6e6f 6465  lverb%] and node
+00005980: 5b40 7265 6c3d 226f 626a 3122 5d29 290d  [@rel="obj1"])).
+00005990: 0a09 0961 6e64 2063 6f75 6e74 286e 6f64  ...and count(nod
+000059a0: 6529 203c 3d20 330d 0a29 0d0a 2222 220d  e) <= 3..)..""".
+000059b0: 0a0d 0a69 6e74 726d 6f64 616c 7665 7262  ...intrmodalverb
+000059c0: 203d 2022 2222 2820 4070 743d 2277 7722   = """( @pt="ww"
+000059d0: 2061 6e64 200d 0a20 2020 2020 2020 2020   and ..         
+000059e0: 2020 2020 2020 2020 2020 2020 2020 2840                (@
+000059f0: 6c65 6d6d 613d 226b 756e 6e65 6e22 206f  lemma="kunnen" o
+00005a00: 720d 0a09 0909 0909 2020 2040 6c65 6d6d  r.......   @lemm
+00005a10: 613d 226d 6f65 7465 6e22 206f 720d 0a09  a="moeten" or...
+00005a20: 0909 0909 2020 2040 6c65 6d6d 613d 226d  ....   @lemma="m
+00005a30: 6f67 656e 2220 6f72 0d0a 0909 0909 0920  ogen" or....... 
+00005a40: 2020 406c 656d 6d61 3d22 6761 616e 2220    @lemma="gaan" 
+00005a50: 0d0a 0909 0909 0920 2020 290d 0a0d 0a29  .......   )....)
+00005a60: 2022 2222 20                              """
```

### Comparing `sastadev-0.1.5/src/sastadev/data/macros/sastamacros2.txt` & `sastadev-0.2.0/src/sastadev/data/macros/sastamacros2.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/methods/ASTA_07062021.xlsx` & `sastadev-0.2.0/src/sastadev/data/methods/ASTA_07062021.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/methods/ASTA_Index_Current.xlsx` & `sastadev-0.2.0/src/sastadev/data/methods/ASTA_Index_Current_old.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/methods/STAP_07062021.xlsx` & `sastadev-0.2.0/src/sastadev/data/methods/STAP_07062021.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/methods/STAP_Index_Current.xlsx` & `sastadev-0.2.0/src/sastadev/data/methods/STAP_Index_Current.xlsx`

 * *Files 22% similar despite different names*

```diff
@@ -103,1004 +103,995 @@
 00000660: de62 f8ae 01d5 4253 edad 86b0 b737 a0ea  .b....BS.....7..
 00000670: 93cf 9b7f d796 a6e9 0d3f 8839 4cec d299  .........?.9L...
 00000680: 15c8 7362 67d9 ae7c c86c 21f5 f91a 5553  ..sbg..|.l!...US
 00000690: 6839 69b0 629e 723a 2279 5f64 6cc0 f344  h9i.b.r:"y_dl..D
 000006a0: 9bbf 13fd 7c2d 4e9c c852 2234 12f8 32cf  ....|-N..R"4..2.
 000006b0: 47c7 25a0 f57f 5ab4 34f1 cb9d 79c4 3709  G.%...Z.4...y.7.
 000006c0: c3ab c8f0 c982 8b1f a8de 0100 00ff ff03  ................
-000006d0: 0050 4b03 0414 0006 0008 0000 0021 00db  .PK..........!..
-000006e0: 46c4 2dba 0300 000e 0900 000f 0000 0078  F.-............x
-000006f0: 6c2f 776f 726b 626f 6f6b 2e78 6d6c ac55  l/workbook.xml.U
-00000700: 516f a338 107e 3fe9 fe03 87fa 4ac1 0408  Qo.8.~?.....J...
-00000710: a026 ab26 045d a5ed aa6a 73dd 9748 9503  .&.&.]...js..H..
-00000720: 2678 0398 b34d 9368 b5ff 7dc7 10d2 64b3  &x...M.h..}...d.
-00000730: 5ae5 ba87 121b 7bcc e76f c6df 8c6f 3e6c  Z.....{..o...o>l
-00000740: cb42 7b25 5c50 568d 7474 6de9 1aa9 1296  .B{%\PV.ttm.....
-00000750: d26a 35d2 ff99 c786 af6b 42e2 2ac5 05ab  .j5......kB.*...
-00000760: c848 df11 a17f 18ff f9c7 cd86 f1f5 92b1  .H..............
-00000770: b506 0095 18e9 b994 7568 9a22 c949 89c5  ........uh.".I..
-00000780: 35ab 4905 968c f112 4b18 f295 296a 4e70  5.I.....K...)jNp
-00000790: 2a72 4264 5998 b665 7966 8969 a577 0821  *rBdY..eyf.i.w.!
-000007a0: bf04 8365 194d 48c4 92a6 2495 ec40 3829  ...e.MH...$..@8)
-000007b0: b004 fa22 a7b5 e8d1 cae4 12b8 12f3 7553  ..."..........uS
-000007c0: 1b09 2b6b 8058 d282 ca5d 0baa 6b65 12de  ..+k.X...]..ke..
-000007d0: ad2a c6f1 b200 b7b7 c8d5 b61c 7e1e fc91  .*..........~...
-000007e0: 058d ddef 04a6 b3ad 4a9a 7026 5826 af01  ........J.p&X&..
-000007f0: daec 489f f98f 2c13 a193 106c cf63 7019  ..H...,....l.cp.
-00000800: 9263 72f2 4ad5 191e 5871 ef9d acbc 0396  .cr.J...Xq......
-00000810: f706 86ac df46 4320 ad56 2b21 04ef 9d68  .....FC .V+!...h
-00000820: ee81 9bad 8f6f 325a 90e7 4eba 1aae eb4f  .....o2Z..N....O
-00000830: b854 2755 e85a 8185 9ca5 5492 74a4 0f61  .T'U.Z....T.t..a
-00000840: c836 e464 8237 f5a4 a105 586d d7b3 906e  .6.d.7....Xm...n
-00000850: 8e0f 727e e05a 4a32 dc14 720e 42ee e121  ..r~.ZJ2..r.B..!
-00000860: 333c 2fb0 5db5 1284 715b 48c2 2b2c c994  3</.]...q[H.+,..
-00000870: 5512 74b8 f7eb 7735 d762 4f73 060a d71e  U.t...w5.bOs....
-00000880: c9bf 0de5 0412 0bf4 05be 428b 9310 2fc5  ..........B.../.
-00000890: 0396 b9d6 f062 a447 e122 e2ac 5eb2 ede2  .....b.G."..^...
-000008a0: 0b24 ec97 f5a2 dcd5 9cad 382e c5a2 dec9  .$........8.....
-000008b0: 9c55 0b01 91c0 90ce 046c ed7b 4a5e 1725  .U.......l.{J^.%
-000008c0: 015b 2a16 470a c6e7 e9f2 1f34 8c13 1518  .[*.G......4....
-000008d0: 1322 d3b1 efde 7f8c 1238 c1c3 5ea7 0f92  .".......8..^...
-000008e0: 6bf0 7e17 7d04 864f f815 4e0e f491 ee13  k.~.}..O..N.....
-000008f0: fb0e 8e06 0d5e aa84 87e8 e5ab 3df1 ec81  .....^......=...
-00000900: ed05 863d 8c23 c399 4553 2370 2753 6310  ...=.#..ES#p'Sc.
-00000910: 3b9e ed7b 4374 8b82 6fe0 0cf7 c284 e146  ;..{Ct..o......F
-00000920: e67b 5128 e891 ee80 02ce 4cf7 78db 5b90  .{Q(......L.x.[.
-00000930: 1536 347d a3f1 d5da 3f86 ea7f 687a db37  .64}....?...hz.7
-00000940: e5b0 2a7f cf94 6cc4 9b7c d450 db7e a655  ..*...l..|.P.~.U
-00000950: ca36 a02e dff3 c1ab 5d3f 3690 0dc3 4d6b  .6......]?6...Mk
-00000960: fd4c 5399 c392 c072 0e73 7f13 baca 8132  .LS....r.s.....2
-00000970: 727d 3509 79a2 a88d f413 4a51 4729 86c7  r}5.y.....JQG)..
-00000980: 50cd 0925 f388 535b 6981 5bdb 6b55 9b1d  P..%..S[i.[.kU..
-00000990: 4faa fa22 28e9 aa6f a3ac 6b3c 547b f0bb  O.."(..o..k<T{..
-000009a0: b44d 84b3 d550 e80e abe1 fdb0 da6e cfbc  .M...P.......n..
-000009b0: df04 9286 5624 5539 085b 1e8d f61b bf6c  ....V$U9.[.....l
-000009c0: 8baa bc7e 89a9 4a9d 084b bcc4 82a8 d44c  ...~..J..K.....L
-000009d0: 70d1 9252 64c0 e79c a629 5137 913e eeb8  p..Rd....)Q7.>..
-000009e0: fe75 757b 85c2 abf9 1572 fc1b f308 1844  .uu{.....r.....D
-000009f0: 76ba 2920 2590 beaa 6b3d 0b90 6507 8a24  v.) %...k=..e..$
-00000a00: d9ca 8f42 b63d 640e 8578 22c7 ba1d 5a81  ...B.=d..x"...Z.
-00000a10: 6358 b381 6b38 7e60 1bbe 33b0 8da9 13d9  cX..k8~`..3.....
-00000a20: 3377 388b 6613 5729 4a5d 6de1 ff51 e0db  3w8.f.W)J]m..Q..
-00000a30: 040e fb3b 53b1 cc31 9773 8e93 35dc b48f  ...;S..1.s..5...
-00000a40: 249b 4038 94d7 2a8f 80ef 31d9 89eb 4fac  $.@8..*...1...O.
-00000a50: 0150 7462 141b 0e0a 2c63 32f1 1cc3 8de2  .Ptb....,c2.....
-00000a60: 813b 44d1 74e6 c66f 6495 fbd9 3bcb ab6f  .;D.t..od...;..o
-00000a70: b65f 132c 1b28 3daa eab4 e350 b5f1 7ef6  ._.,.(=....P..~.
-00000a80: 3099 7513 fbf3 3da9 16e1 63a4 1cd9 7ffd  0.u...=...c.....
-00000a90: ab85 4fe0 7d41 2e5c 1c3f 5fb8 70fa e97e  ..O.}A.\.?_.p..~
-00000aa0: 7edf 86f2 a70e 7401 566d 2b0b b33f 96f1  ~.....t.Vm+..?..
-00000ab0: 7700 0000 ffff 0300 504b 0304 1400 0600  w.......PK......
-00000ac0: 0800 0000 2100 4aa9 a661 fa00 0000 4703  ....!.J..a....G.
-00000ad0: 0000 1a00 0801 786c 2f5f 7265 6c73 2f77  ......xl/_rels/w
-00000ae0: 6f72 6b62 6f6f 6b2e 786d 6c2e 7265 6c73  orkbook.xml.rels
-00000af0: 20a2 0401 28a0 0001 0000 0000 0000 0000   ...(...........
-00000b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bf0: 0000 0000 0000 0000 bc92 cd6a c430 0c84  ...........j.0..
-00000c00: ef85 be83 d1bd 7192 fe50 ca3a 7b29 85bd  ......q..P.:{)..
-00000c10: b6db 0730 b112 874d 6c63 a93f 79fb 9a94  ...0...Mlc.?y...
-00000c20: ee36 b0a4 97d0 a324 34f3 31cc 66fb 39f4  .6.....$4.1.f.9.
-00000c30: e21d 2375 de29 28b2 1c04 bada 9bce b50a  ..#u.)(.........
-00000c40: 5ef7 4f57 f720 88b5 33ba f70e 158c 48b0  ^.OW. ..3.....H.
-00000c50: ad2e 2f36 cfd8 6b4e 4f64 bb40 22a9 3852  ../6..kNOd.@".8R
-00000c60: 6099 c383 9454 5b1c 3465 3ea0 4b97 c6c7  `....T[.4e>.K...
-00000c70: 4173 1a63 2b83 ae0f ba45 59e6 f99d 8cbf  As.c+....EY.....
-00000c80: 35a0 9a69 8a9d 5110 77e6 1ac4 7e0c c9f9  5..i..Q.w...~...
-00000c90: 6f6d df34 5d8d 8fbe 7e1b d0f1 190b c989  om.4]...~.......
-00000ca0: 0b93 a08e 2db2 8269 fc5e 1659 0205 799e  ....-..i.^.Y..y.
-00000cb0: a15c 93e1 c3c7 0359 443e 711c 5724 a74b  .\.....YD>q.W$.K
-00000cc0: b904 53fc 33cc 6232 b76b c290 d511 cd0b  ..S.3.b2.k......
-00000cd0: c754 3e3a a533 5b2f 2573 b32a 0c8f 7dea  .T>:.3[/%s.*..}.
-00000ce0: fab1 2b34 cd3f f672 56ff ea0b 0000 ffff  ..+4.?.rV.......
-00000cf0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00000d00: dd19 99f8 1c0d 0000 844f 0000 1800 0000  .........O......
-00000d10: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00000d20: 6565 7431 2e78 6d6c 9c94 5d6f da30 1486  eet1.xml..]o.0..
-00000d30: ef27 ed3f 58be 6f12 2721 5044 5a55 add0  .'.?X.o.'!PDZU..
-00000d40: 3a4d 53d5 76db b571 1cb0 9ac4 996d 0ab4  :MS.v..q.....m..
-00000d50: da7f dfb1 f301 1bb4 8a8a 2036 4ece 73ce  .......... 6N.s.
-00000d60: 7b3e 32bb dc96 057a e64a 0b59 a598 7801  {>2....z.J.Y..x.
-00000d70: 46bc 6232 13d5 32c5 3f1e e767 138c b4a1  F.b2..2.?..g....
-00000d80: 5546 0b59 f114 efb8 c697 179f 3fcd 3652  UF.Y........?.6R
-00000d90: 3de9 15e7 0601 a1d2 295e 1953 4f7d 5fb3  =.......)^.SO}_.
-00000da0: 152f a9f6 64cd 2bb8 934b 5552 037f d5d2  ./..d.+..KUR....
-00000db0: d7b5 e234 7346 65e1 8741 90f8 2515 156e  ...4sFe..A..%..n
-00000dc0: 0853 3584 21f3 5c30 7e23 d9ba e495 6920  .S5.!.\0~#....i 
-00000dd0: 8a17 d440 fc7a 256a ddd1 4a36 0457 52f5  ...@.z%j..J6.WR.
-00000de0: b4ae cf98 2c6b 402c 4421 ccce 4131 2ad9  ....,k@,D!..A1*.
-00000df0: f476 5949 4517 05e8 de92 9832 b455 f00d  .vYIE......2.U..
-00000e00: e117 756e dcf9 91a7 5230 25b5 cc8d 0764  ..un....R0%....d
-00000e10: bf89 f958 feb9 7fee 53d6 938e f50f c290  ...X....S.......
-00000e20: d857 fc59 d802 ee51 e1c7 4222 a39e 15ee  .W.Y...Q..B"....
-00000e30: 61d1 0761 490f b3e9 52d3 b5c8 52fc 1ab4  a..aI...R...R...
-00000e40: 9f33 5889 bd04 fb4b 77ef 0fbe 9865 022a  .3X....Kw....e.*
-00000e50: 6c55 21c5 f314 5f91 e923 8927 d8bf 98b9  lU!..._..#.'....
-00000e60: 0efa 29f8 461f ec91 a18b 075e 7066 3878  ..).F......^pf8x
-00000e70: 2118 bd48 593e 305a f0ef b605 0b38 0ba0  !..HY>0Z.....8..
-00000e80: b96d db2e a47c b2e6 b7f0 6000 9e6a 5a71  .m...|....`..jZq
-00000e90: b47d a8a1 f829 1e61 b46b b700 31b2 fec6  .}...).a.k..1...
-00000ea0: 7373 cd0b 007c 859c 5066 c433 bf03 8b14  ss...|..Pf.3....
-00000eb0: 2fa4 31b2 bc17 cb95 7143 62e0 2c57 f285  /.1.....qCb.,W..
-00000ec0: 572e 4a17 8c8d dff2 530c a8f6 d186 d130  W.J.....S......0
-00000ed0: e7e0 44ff 760a 616b c5fd 67d6 38b1 4174  ..D.v.ak..g.8.At
-00000ee0: ce1b c32b 08a6 3584 ed9b 8627 5c3e ee5d  ...+..5....'\>.]
-00000ef0: c216 2cfd 3ea1 87fb 2eb9 7337 c177 0a65  ..,.>.....s7.w.e
-00000f00: 3ca7 ebc2 5ccb e297 c8cc 2ac5 136f 3c1e  <...\.....*..o<.
-00000f10: 4771 3486 9cb5 37ef e5e6 0bb7 0981 74c7  Gq4...7.......t.
-00000f20: 5e0c 65b7 7333 cd76 375c 3318 5848 b817  ^.e.s3.v7\3.XH..
-00000f30: 599f 4c16 e000 aea8 14f6 c503 f346 b76e  Y.L..........F.n
-00000f40: dd1c c3b5 d9d9 1974 327b 13d0 ef4c 606d  .......t2{...L`m
-00000f50: 4dc8 c40b c9c4 46d3 1b20 b6d6 50a3 3660  M.....F.. ..P.6`
-00000f60: a7b6 0740 533a 0044 d901 869a c273 ce14  ...@S:.D.....s..
-00000f70: d6d6 340e bc38 2671 9084 ff30 165c 9bb9  ..4..8&q...0.\..
-00000f80: 6d2b 10f8 4e28 49cb 1bf7 bc28 3c48 ee20  m+..N(I....(<H. 
-00000f90: 39f0 a276 31c1 dac9 49bc d128 4e86 67e4  9..v1...I..(N.g.
-00000fa0: bc45 c0da 216c 9775 d947 03d5 1098 b3a6  .E..!l.u.G......
-00000fb0: 9a76 e09a 7292 e054 2c43 817d 7bc0 a605  .v..r..T,C.}{...
-00000fc0: 26e4 0868 fdbe 9364 d215 9cec f51d b6f0  &..h...d........
-00000fd0: e92e ebb4 8407 5a92 93b5 1928 26ec c524  ......Z....(&..$
-00000fe0: d164 df7b 6f45 e2bb 49f9 0b00 00ff ff00  .d.{oE..I.......
-00000ff0: 0000 ffff 9c9c e96e dc38 1084 5fc5 9807  .......n.8.._...
-00001000: 8887 ba27 b00d ec1c ce64 0eed 9517 30bc  ...'.....d....0.
-00001010: 06f2 27c9 22f6 5e6f bf12 a919 91d5 45a9  ..'.".^o......E.
-00001020: 993f c146 f8a6 d464 179b 5253 d9bb d7cf  .?.F...d..RS....
-00001030: 2f2f 6fdb a7b7 a787 bbef dffe b9f9 7ebf  //o...........~.
-00001040: 308b 9bd7 3f9f bebe 76ff f53e 5b76 7fb1  0...?...v..>[v..
-00001050: 979e ff7a 7dfb f6e5 f1db f72f 4f6f f6c2  ...z}....../Oo..
-00001060: bfa6 787a 7eff c77f db97 d7e7 97af ddb5  ..xz~...........
-00001070: e5bb 7cf1 70f7 dc4b fcd4 6b58 aabb feda  ..|.p..K..kX....
-00001080: 5dfd fba1 b9bb fdfb e1ee f679 20d6 92c8  ]..........y ...
-00001090: 4262 2389 3c24 b692 5885 c44e 12cb 9078  Bb#.<$..X..N...x
-000010a0: 9484 01e4 0341 4ca8 b227 080c e723 4142  .....AL..'...#AB
-000010b0: 9183 248a 9038 3aa2 59dc 5ca7 b50c 8913  ..$..8:.Y.\.....
-000010c0: 1b0e 4472 660c 0ca8 650c 44f3 3361 4a98  ..Drf...e.D.3aJ.
-000010d0: bb5f 1803 f7fa 9531 10f3 6f8c 013b fcce  ._.....1..o..;..
-000010e0: 1888 f993 64aa eb0c de76 0be0 ba0a 3258  ....d....v....2X
-000010f0: 059f 7bd7 17c5 e266 d2f7 fdaf ee17 dd9f  ..{....f........
-00001100: d704 e535 185f 2235 3a5f 2205 187b 2b91  ...5._"5:_"..{+.
-00001110: 157a 5f22 0d20 7ba2 02eb f4a3 442a c8df  .z_". {.....D*..
-00001120: 81a8 c0a0 8f0e 5979 f362 7062 4ef3 c19c  ......Yy.bpbN...
-00001130: e791 5622 6639 2e92 20c5 f90f a5b8 ff15  ..V"f9.. .......
-00001140: a418 6b9b 446a f0ea 4622 b874 b612 1129  ..k.Dj..F".t...)
-00001150: 2608 5626 8260 8a25 2252 4c54 30c5 0e09  &.V&.`.%"RLT0...
-00001160: 528c ae3d cd07 739e 475a 8944 53dc add7  R..=..s.GZ.DS...
-00001170: 602f eb57 71d6 bceb 2ae8 e432 ee7f 0639  `/.Wq...*..2...9
-00001180: 86a5 b396 480d b566 2391 12b2 b395 88c8  ....H..f#.......
-00001190: b144 1a28 fa7b a282 3996 4805 55e7 4054  .D.(.{..9.H.U.@T
-000011a0: 30c7 0e09 730c 32a7 f960 cef3 482b 113f  0...s.2..`..H+.?
-000011b0: c7f6 21e3 1391 8914 f3f2 8756 7aff abd0  ..!........Vz...
-000011c0: 0505 6c6f 6b89 d490 9c8d 444a 98b2 ad44  ..lok.....DJ...D
-000011d0: 840b 24d2 408a f744 055d 2091 0a0a d381  ..$.@..D.] .....
-000011e0: a8a0 0b1c 12ba 0064 4ef3 c19c e791 5622  .......dN.....V"
-000011f0: d195 5e41 8a27 d777 0f43 6661 65ae 2552  ..^A.'.w.Cfae.%R
-00001200: 8fe6 b2fe db48 a4c4 2754 8988 cc12 04fc  .....H..'T......
-00001210: b127 0866 5622 1594 a303 51c1 cc3a c474  .'.fV"....Q..:.t
-00001220: 0ffd d7e7 971a 2c7f 9a0f e63c 8fb4 1289  ......,....<....
-00001230: 66b6 4ec9 6c0f 4366 6136 d712 a961 1e36  f.N.l.Cfa6...a.6
-00001240: 1229 6136 b712 1199 9548 0316 da13 15cc  .)a6.....H......
-00001250: ac44 2a28 3107 a282 9975 4898 59b0 fc69  .D*(1....uH.Y..i
-00001260: 3e98 f33c d24a 249a d96e 1b16 bb73 dd3d  >..<.J$..n...s.=
-00001270: c04d aedd fe47 9061 5875 6b89 d430 ab1b  .M...G.aXuk..0..
-00001280: 8994 30ab 5b89 880c 4ba4 8189 df13 15cc  ..0.[...K.......
-00001290: b044 4486 890a 66d8 21e1 2336 d8ed 341f  .DD...f.!.#6..4.
-000012a0: cc79 1e69 2512 cd70 174e 90e1 c9cc f630  .y.i%..p.N.....0
-000012b0: 6416 56dd 5a22 353c 986d 2452 c234 6c25  d.V.Z"5<.m$R.4l%
-000012c0: 2232 4b10 70d9 a344 cc12 8ae5 9ec8 60f6  "2K.p..D......`.
-000012d0: 2552 41bc 07a2 82d9 7748 b827 e3fa 9e0f  %RA.....wH.'....
-000012e0: e63c 8fb4 6cd8 9117 acbe dc88 056e b2d5  .<..l........n..
-000012f0: bbae fa4f b78f 5cdb c97f 8f2e 6079 aead  ...O..\.....`y..
-00001300: 7868 9706 a67f 4398 1266 6e4b 18e1 06c6  xh....C..fnK....
-00001310: 403c 8f84 314b f0cc 9e09 a121 0853 41d0  @<..1K.....!.SA.
-00001320: 07a6 8396 1898 d013 b0a0 4e8a 80ce 0aa6  ..........N.....
-00001330: a5a3 8fd9 a26f c2f8 1dc6 692f b896 4de0  .....o....i/..M.
-00001340: 0558 206b 2399 06dc bf21 4c09 53bf 258c  .X k#....!L.S.%.
-00001350: f482 bcd7 0a66 75cf 7444 9aa5 4e05 cc81  .....fu.tD..N...
-00001360: e988 343b 9d20 cd39 14c5 9322 a0b3 8269  ..4;. .9..."...i
-00001370: 0913 adfd a66f c5e8 d34c 9a5e d83a b38a  .....o...L.^.:..
-00001380: b0e4 45d7 58ea 94d8 3c23 3a32 cda4 d784  ..E.X...<#:2....
-00001390: d59d e988 3493 069a 48b3 a283 36dc 2b4c  ....4...H...6.+L
-000013a0: 3308 9d14 019d 154c 4b98 789a b18d 36bd  3......LK.x...6.
-000013b0: 9a65 f3a6 8051 ac8d 641a ec9f 11a6 82f4  .e...Q..d.......
-000013c0: 6c09 23d3 4cee 2556 b3a2 87c6 e201 db1d  l.#.L.%V........
-000013d0: 583c 6235 b336 1abe 8231 2198 c4b3 8269  X<b5.6...1!....i
-000013e0: 0913 4f33 b6d2 a6d3 ccfa 37a2 6a33 085f  ..O3......7.j3._
-000013f0: c50c 8344 dd56 f4d1 9850 26ce 7114 ad34  ...D.V...P&.q..4
-00001400: 2254 8954 2b9a 6983 4eb0 a233 916a 453b  "T.T+.i.N..3.jE;
-00001410: 8d04 b482 196a e934 8e51 077d 7183 edb2  .....j.4.Q.}q...
-00001420: e954 9326 0d1e a1ad ad64 58b9 8d11 6b9a  .T.&.....dX...k.
-00001430: 29e1 5b19 5192 8b9a 09e1 8b19 1312 c59b  ).[.Q...........
-00001440: 0989 5c2b 5a66 c3cd 825c 1b88 e8a4 88e8  ..\+Zf...\......
-00001450: ac60 5a36 d9cb 58ae 93fa 6686 b46d 0c76  .`Z6..X...f..m.v
-00001460: ce28 84bd 710a e17b 1a81 64ae 5948 90c7  .(..q..{..d.YH..
-00001470: 3d13 12b9 6642 22d7 8a26 da70 b330 d762  =...fB"..&.p.0.b
-00001480: a756 b4d1 1451 b76c 1ea3 b9c6 4e9a f234  .V...Q.l....N..4
-00001490: c490 968e c1ae 1a83 3291 75a2 9489 1732  ........2.u....2
-000014a0: 456b 8ddd 2d17 8f67 8aee 1a1d 9bc8 fa7c  Ek..-..g.......|
-000014b0: 83ed 4484 b008 9f15 4ccb 02f2 12ea 4e3e  ..D.....L.....N>
-000014c0: 0628 7c18 1ccb 6958 cdb1 cb36 5dcd 4973  .(|...iX...6].Is
-000014d0: 2713 b966 109e 7b18 0689 8d5b d164 6342  '..f..{....[.dcB
-000014e0: b9d8 b815 7d36 2664 44ae e75b 6d27 2224  ....}6&dD..[m'"$
-000014f0: 73ad 68a4 b180 64ae 9d50 d0ba 35f9 b8b2  s.h...d..P..5...
-00001500: c264 f7dd 19ff 9d4b bbc4 4957 27c3 b6aa  .d.....K..IW'...
-00001510: 6110 1e8a 5048 bc80 39a5 ae06 5ecf 1964  a...PH..9...^..d
-00001520: 6127 77cb f164 84dc 0d33 f191 4524 d34e  a'w..d...3..E$.N
-00001530: 3a5f 627f 5634 d014 01b5 2c20 9976 77b3  :_b.V4...., .vw.
-00001540: 7089 471a 2af6 2b2d f59b f6f0 4d97 df50  p.G.*.+-....M..P
-00001550: 31a2 bb46 2158 bd3b 0ae1 1107 8130 45c7  1..F!X.;.....0E.
-00001560: 8109 5b55 38fd 0aa1 9645 14db 0eb3 9437  ..[U8....E.....7
-00001570: 9aa3 a5ef 17ab c56d f715 5bf0 a150 cad3  .......m..[..P..
-00001580: f231 bb1c 9e0a 9994 07b1 63e6 1e1f 4834  .1........c...H4
-00001590: b8c7 4f55 fb5d e636 b6aa 1f94 dd59 8ec3  ..OU.].6.....Y..
-000015a0: 1522 9cb2 8d1c b3cb 6984 1826 16a8 a9f8  ."......i..&....
-000015b0: 8e99 5b04 5dd7 0975 726c 2d4f ea58 9a25  ..[.]..url-O.X.%
-000015c0: 2f4f 6945 1e2d 4d65 525a 5dc7 fcf2 3594  /OiE.-MeRZ]...5.
-000015d0: 1894 d74a 31ef fb5e dbf4 a82e bd02 a1e3  ...J1..^........
-000015e0: 395b a373 f9ac 43e8 78d6 d6e8 c4bc 9d7b  9[.s..C.x......{
-000015f0: ded6 e8c4 cc9d 7be6 d6e8 3877 4b2f e79e  ......{...8wK/..
-00001600: 9735 3a31 33e7 9e99 353a 9792 8ef3 5c78  .5:13...5:....\x
-00001610: 6656 e858 9cd9 b048 f38f c5a9 4e9a 7ffa  fV.X...H....N...
-00001620: af22 bb83 3b39 cf45 9a7f 2c4e 75d2 fc53  ."..;9.E..,Nu..S
-00001630: c4fc 53a4 f9c7 e234 9e34 ff14 31ff 1469  ..S....4.4..1..i
-00001640: feb1 388b a74c f38f c5a9 8e57 0d15 3e2c  ..8..L.....W..>,
-00001650: 2f27 0fe8 e7d2 2b87 1a9d 583d 2cd3 fc6c  /'....+...X=,..l
-00001660: 713a ae34 1f96 b13a 56a6 f9d0 e234 9e34  q:.4...:V....4.4
-00001670: 1f96 b13a 56a6 f9d0 e234 9e34 1f96 b13a  ...:V....4.4...:
-00001680: 56a5 f9d0 e22c 9e2a cd3f 16a7 3a69 fea9  V....,.*.?..:i..
-00001690: 62fb 6995 560f 2d4e e349 f361 15f3 6195  b.i.V.-N.I.a..a.
-000016a0: e643 8bd3 78d2 fc53 c5ea 5895 e61f 8bb3  .C..x..S..X.....
-000016b0: 78ea b4fa 6371 aa93 e69f fe93 23ba 7fd5  x...cq......#...
-000016c0: 69fe b138 8d27 cd3f 756c 3fad d3fc 6371  i..8.'.?ul?...cq
-000016d0: 1a4f 9a7f ead8 7e5a a7d5 318b d378 d27c  .O....~Z..1..x.|
-000016e0: 58c7 7c58 a7f9 d0e2 2c9e 26ad 8e59 9cea  X.|X....,.&..Y..
-000016f0: 8c7e 2eed 3fa5 9a7c 9c6f 62db 6933 da59  .~..?..|.ob.i3.Y
-00001700: 2313 7373 33ba 5923 132b 86cd 6866 8d4c  #.ss3.Y#.+..hf.L
-00001710: cccb cde8 658d 4cac 1436 a305 3532 b19d  ....e.L..6..52..
-00001720: b419 1da8 9189 19b0 190d 382f b3b3 f4fd  ..........8/....
-00001730: c27b fb1e aed8 2769 d7e9 1dae 14e2 0578  .{....'i.......x
-00001740: 357a 5411 b1a5 9945 5749 16b5 3495 49b2  5zT....EWI..4.I.
-00001750: e82a 66d1 5592 b72c 4da3 49f2 d62a e6ad  .*f.U..,M.I..*..
-00001760: d558 2635 531c ab92 abb4 aa64 7136 aaee  .X&5S......dq6..
-00001770: ebc2 b1b9 ab78 ac76 3c57 4adb 68cd 3256  .....x.v<WJ.h.2V
-00001780: 9acc 326d ab75 3c8f 296d b3ed bead 8bec  ..2m.u<.)m......
-00001790: da66 99b6 bd39 9ec7 94b6 c199 65ac be18  .f...9......e...
-000017a0: ff63 284d eeae 9ffb e0bb 5577 6c7e 7541  .c(M......Uwl~uA
-000017b0: 39df 2372 381d 9cfd 24c0 758d 5542 b14a  9.#r8...$.u.UB.J
-000017c0: 6ebc ef05 5442 6ebd 7523 9463 f357 dc6c  n...TBn.u#.c.W.l
-000017d0: ffcb 0c87 9fa4 3d68 ec09 59c2 e0e2 89f3  ......=h..Y.....
-000017e0: 7706 4548 b1ad c1d8 ae7f 4244 b197 2ce3  w.EH......BD..,.
-000017f0: 75fb 35d3 7ded ad8b d9ce fcda 3f3f 348b  u.5.}.......??4.
-00001800: 5327 657e f557 08c5 cabf c952 bcbd 73f8  S'e~.W.....R..s.
-00001810: fda2 beb6 af1f e5a5 0ff2 d23e b814 9e9f  ...........>....
-00001820: 7987 02f3 93db 45e0 1645 1001 5eea 22c0  y.....E..E..^.".
-00001830: 4b5d 04de 2588 206d 0d44 4f02 8c6d e5eb  K]..%. m.DO..m..
-00001840: 0d17 edfc 1bdb cc4f 108a 2e01 dbce 4f10  .......O......O.
-00001850: 8a2e 01af fbaf 5902 d1f6 bff1 faff 2aa1  ......Y.......*.
-00001860: e83e 687b fafa a145 8f00 4c9e 56de 2d4e  .>h{...E..L.V.-N
-00001870: 1765 ee3f 4bcd 2f4a 8b73 21ff 694a 2114  .e.?K./J.s!.iJ!.
-00001880: 7b9c 32de 3180 6ab2 630f 54dd 3f1d 4fda  {.2.1.j.c.T.?.O.
-00001890: 022d ce87 9652 dc77 c69e 1bdc 2ff2 f1b8  .-...R.w..../...
-000018a0: ec72 49f6 be8d 7738 a0a9 2416 1fb4 c382  .rI...w8..$.....
-000018b0: e09d 0e68 8486 d381 d22b 8ac3 a5f1 45e3  ...h.....+....E.
-000018c0: 8311 978e 974b 6428 45ca 46b1 3316 f7df  .....Kd(E.F.3...
-000018d0: 6b1e e5a5 2e02 b796 6c50 30e0 94ed a4bb  k.......lP0.....
-000018e0: 9ddb 4ec6 d175 b7c3 4bdd edf0 5237 e0e8  ..N..u..K...R7..
-000018f0: 3e64 4f34 f4ab 397a 0062 ec51 c470 32af  >dO4..9z.b.Q.p2.
-00001900: 79ec 8b1e 5d98 c4b3 0bc7 53d3 dbe3 8894  y...].....S.....
-00001910: 9844 3dbf 1dff a731 ff03 0000 ffff 0000  .D=....1........
-00001920: 00ff ff5c 90c1 6ec2 3010 447f c5f2 3d98  ...\..n.0.D...=.
-00001930: 240e 018b 2045 1024 0e9c e80f b889 43ac  $... E.$......C.
-00001940: 2659 6bbd a8a8 55ff bd0e 811e 7adb d995  &Yk...U.....z...
-00001950: 66de ce56 df08 8eb6 2783 0c4d 5bf0 3256  f..V....'..M[.2V
-00001960: 6fb1 5c73 7647 75b3 4dc1 bf8f 5595 6552  o.\svGu.M...U.eR
-00001970: 9651 76a8 aa48 aed6 fba8 2cf3 4d14 a752  .Qv..H....,.M..R
-00001980: ae0e b994 a94c 7fb8 d86d 3d20 5d48 9379  .....L...m= ]H.y
-00001990: 3a25 ea3c 3b0d fde8 d5bd c726 2978 47e4  :%.<;......&)xG.
-000019a0: 9410 beee cca0 fd62 b035 8287 9616 350c  .......b.5....5.
-000019b0: 02da d6d6 4678 8746 37be 3386 865e 24cb  ....Fx.F7.3..^$.
-000019c0: 3817 68eb aed1 a413 3ee7 ec61 6c2c 5918  8.h.....>..al,Y.
-000019d0: e7ac 2a51 d594 f5a4 f877 3d25 eaf4 bc8a  ..*Q.....w=%....
-000019e0: 3fc8 ddd6 e9ab 396b bcda d1b3 deb4 54f0  ?.....9k......T.
-000019f0: e522 e70c edb5 7bcd 04ee b1cd 387b 0722  ."....{.....8{."
-00001a00: 185e aa0b 8006 2795 72d6 0284 fe66 1108  .^....'.r....f..
-00001a10: 26df 8ba1 9b63 4e3b 8317 fb65 0abe e10c  &....cN;...e....
-00001a20: d09a 31f4 13a8 0bee 4259 a82d 853c 35d5  ..1.....BY.-.<5.
-00001a30: 8ca7 269e f0c5 27e0 c7e3 f5dd 2f00 0000  ..&...'...../...
-00001a40: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00001a50: 2100 b163 99a9 e804 0000 c610 0000 1800  !..c............
-00001a60: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00001a70: 7368 6565 7432 2e78 6d6c 9c93 db6a e330  sheet2.xml...j.0
-00001a80: 1086 ef17 fa0e 42f7 b16c e7d0 d6c4 296c  ......B..l....)l
-00001a90: 4bd8 422e 9665 0fd7 8a3c 8e45 24cb 2b29  K.B..e...<.E$.+)
-00001aa0: 2796 7df7 1dc9 751a 082c a1c6 d68c edd1  '.}...u..,......
-00001ab0: f7cf 48a3 f9d3 512b b207 eba4 694b 9a25  ..H...Q+....iK.%
-00001ac0: 2925 d00a 53c9 7653 d21f df97 a307 4a9c  )%..S.vS......J.
-00001ad0: e76d c595 69a1 a427 70f4 6971 f769 7e30  .m..i..'p.iq.i~0
-00001ae0: 76eb 1a00 4f90 d0ba 9236 de77 0563 4e34  v...O....6.w.cN4
-00001af0: a0b9 4b4c 072d fea9 8dd5 dce3 abdd 30d7  ..KL.-........0.
-00001b00: 59e0 559c a415 cbd3 74c6 3497 2ded 0985  Y.U.....t.4.-...
-00001b10: bd85 61ea 5a0a 7831 62a7 a1f5 3dc4 82e2  ..a.Z.x1b...=...
-00001b20: 1ef3 778d ecdc 40d3 e216 9ce6 76bb eb46  ..w...@.....v..F
-00001b30: c2e8 0e11 6ba9 a43f 4528 255a 14af 9bd6  ....k..?E(%Z....
-00001b40: 58be 5658 f731 9b70 418e 16ef 1c9f f120  X.VX.1.pA...... 
-00001b50: 13bf 5f29 6929 ac71 a6f6 0992 599f f375  .._)i).q....Y..u
-00001b60: f98f ec91 7171 265d d77f 1326 9b30 0b7b  ....qq&]...&.0.{
-00001b70: 1936 f01d 957f 2ca5 6c7a 66e5 efb0 f107  .6....,.lzf.....
-00001b80: 61b3 332c 2c97 2d76 b22a e99f f4ed 1aa1  a.3,,.-v.*......
-00001b90: cdc2 908e d22c 0c17 d75f ba98 5712 7738  .....,..._..W.w8
-00001ba0: 5445 2cd4 25fd 9c17 ab7c 46d9 621e 1be8  TE,.%....|F.b...
-00001bb0: a784 83bb f089 37dd 0a6a ff0c 4a61 f03d  ......7..j..Ja.=
-00001bc0: 25a1 41d7 c66c 43e4 2b0a a7c8 74a0 4084  %.A..lC.+...t.@.
-00001bd0: 5621 1ccd 1efa e855 36c1 26ff 1d65 828f  V!.....U6.&..e..
-00001be0: 1aec 2c72 e90f 82cb d8d4 5f2d a9a0 e63b  ..,r......_-...;
-00001bf0: e5bf 99c3 1790 9bc6 e309 9a24 088b 5d51  ...........$..]Q
-00001c00: 54a7 1770 02db 14c5 9371 c00a a390 8123  T..p.....q.....#
-00001c10: d112 8f1b 2e8b e6c7 680f b2f2 4d49 f33c  ........h...MI.<
-00001c20: c9b3 87fb 2925 6b70 7e29 0391 12b1 73de  ....)%kp~)....s.
-00001c30: e85f 7d48 f606 ea11 2816 1168 07c4 7fe3  ._}H....(..h....
-00001c40: 33dc d738 2138 c38c 6932 9d4e 6651 f65a  3..8!8..i2.NfQ.Z
-00001c50: 8ac5 a4ff 0100 00ff ff00 0000 ffff 9c56  ...............V
-00001c60: 516e c230 0cbd 0aea 0128 490b 0554 fab1  Qn.0.....(I..T..
-00001c70: 06a1 49bd 0462 487c b189 22b6 dd7e 4e94  ..I..bH|.."..~N.
-00001c80: d4b1 134a ba2f c071 5eec 17bf 17ea fe72  ...J./.q^......r
-00001c90: 3edf d5f1 7e6c eadb e7f7 ecb6 cb64 36eb  >...~l.......d6.
-00001ca0: bf8e d71e be6d 05fc b8dc 7759 059f 3fa2  .....m....wY..?.
-00001cb0: 3c9e b61f bfea dc9f ce57 082e e645 d6d4  <........W...E..
-00001cc0: 27bd e70d d621 d2c3 ef47 2365 9d3f 9a3a  '....!...G#e.?.:
-00001cd0: 3fd9 c5d6 5f14 055d dceb e376 9928 3d00  ?..._..]...v.(=.
-00001ce0: 51d2 9c03 01a8 e862 6701 961e 4081 0039  Q......bg...@..9
-00001cf0: 7435 b456 b0d6 c65a daeb 645e d872 389b  t5.V...Z..d^.r8.
-00001d00: e042 f101 6572 3d5f 8f93 d692 9e57 8c17  .B..er=_.....W..
-00001d10: 8df9 8a17 02b0 66bc 5800 c2cb 93fa 2187  ......f.X.....!.
-00001d20: d43f ca8b 4ee6 856d d885 f987 ca05 5d7c  .?..N..m......]|
-00001d30: 278b 22ce 6815 6174 59cd 572f c610 b6e1  '.".h.atY.W/....
-00001d40: 18b2 496b c922 1b31 a50f 84ae 8a2c b753  ..Ik.".1.....,.S
-00001d50: bbb7 119f 6389 fc99 b13f 1048 7e01 1680  ....c....?.H~...
-00001d60: 5cc0 9376 6152 922f 40e9 645a aa8d 94ba  \..vaR./@.dZ....
-00001d70: 7832 989b 09b8 2d24 2379 6c1c 9546 a287  x2....-$#yl..F..
-00001d80: da08 e107 b549 ca10 8b7f 788a 32bb e899  .....I....x.2...
-00001d90: 2e34 7a29 3a09 1b61 a3d9 3908 722d 382a  .4z):..a..9.r-8*
-00001da0: b46e 31e5 5e84 ce66 f5da 5078 33da 5927  .n1.^..f..Px3.Y'
-00001db0: db6c ab77 0dad 154c 58ca 60b2 0222 f6ca  .l.w...LX.`.."..
-00001dc0: a7b8 73fb 0825 68e2 9492 291e aa40 4f01  ..s..%h...)..@O.
-00001dd0: 2583 aff2 61d5 6f40 c446 5fb9 2879 3ad8  %...a.o@.F_.(y:.
-00001de0: e3a0 0c26 a364 7056 27f5 ce65 1102 5001  ...&.dpV'..e..P.
-00001df0: 9480 2966 a984 754b cf57 5c28 3213 606f  ..)f..uK.W\(2.`o
-00001e00: e936 2074 366b cd86 22d0 68a8 e516 6a1a  .6 t6k..".h...j.
-00001e10: 7378 2542 3374 a108 327a 5702 72e8 5de2  sx%B3t..2zW.r.].
-00001e20: a979 0974 af04 e4d0 a0cc 7ef3 52f1 4993  .y.t......~.R.I.
-00001e30: e847 af91 4d32 e5d9 8542 3624 3a46 0272  .G..M2...B6$:F.r
-00001e40: 6818 667f bc66 348c 0464 2b7b 6fec e4e0  h.f..f4..d+{o...
-00001e50: 0401 1b28 e904 e450 d1f2 a9a2 252a 3a01  ...(...P....%*:.
-00001e60: d9ea d2af d997 2a51 a144 1526 2087 2234  ......*Q.D.& ."4
-00001e70: fbe3 3ca3 0813 9043 0dca 5083 39fe c9fe  ..<....C..P.9...
-00001e80: 0300 00ff ff00 0000 ffff 3c8f 416e 8430  ..........<.An.0
-00001e90: 0c45 af12 f900 6486 aa45 4584 4d67 d345  .E....d..EE.Mg.E
-00001ea0: 579c 2025 0e89 4a70 e478 34a3 9ebe 0189  W. %..Jp.x4.....
-00001eb0: eefc bdf8 effd a110 cb24 5650 317a 03b7  .........$VP1z..
-00001ec0: aebf b56f a09e 69dd 4aff 5cd9 b506 8248  ...o..i.J.\....H
-00001ed0: eeb5 2e73 c064 4b93 e2cc 54c8 4b33 53d2  ...s.dK...T.K3S.
-00001ee0: e47d 9c51 97cc 685d 0988 9256 dd5e ae9d  .}.Q..h]...V.^..
-00001ef0: e638 0767 c5b6 300e 3be6 8336 1725 d276  .8.g..0.;..6.%.v
-00001f00: a240 8f83 fe17 1887 6c17 fcb2 bcc4 ada8  .@......l.......
-00001f10: 15bd 18b8 341d 288e 4b38 6fa1 7c7c 5f41  ....4.(.K8o.||_A
-00001f20: 7d93 08a5 3385 4a47 ded3 0b28 4f24 67a8  }...3.JG...(O$g.
-00001f30: 8cbd 7742 b967 956d 469e e22f 1a78 0745  ..wB.g.mF../.x.E
-00001f40: 1c71 abdb ab92 815c 0dd9 46a9 bc3e 3a03  .q.....\..F..>:.
-00001f50: fce9 ae87 e083 f8e7 d835 fe01 0000 ffff  .........5......
-00001f60: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00001f70: c117 10be 4e07 0000 c620 0000 1300 0000  ....N.... ......
-00001f80: 786c 2f74 6865 6d65 2f74 6865 6d65 312e  xl/theme/theme1.
-00001f90: 786d 6cec 59cd 8b1b 3714 bf17 fa3f 0c73  xml.Y...7....?.s
-00001fa0: 77fc 35e3 8f25 dee0 cf6c 93dd 2464 9d94  w.5..%...l..$d..
-00001fb0: 1cb5 b6ec 5156 3332 92bc 1b13 0225 39f5  ....QV32.....%9.
-00001fc0: 5228 a4a5 9742 6f3d 94d2 4003 0dbd f48f  R(...Bo=..@.....
-00001fd0: 0924 b4e9 1fd1 27cd d823 ade5 249b 6c4a  .$....'..#..$.lJ
-00001fe0: 5a76 0d8b 47fe bda7 a7f7 9e7e 7af3 74f1  Zv..G......~z.t.
-00001ff0: d2bd 987a 4798 0bc2 9296 5fbe 50f2 3d9c  ...zG....._.P.=.
-00002000: 8cd8 9824 d396 7f6b 3828 347c 4f48 948c  ...$...k8(4|OH..
-00002010: 1165 096e f90b 2cfc 4bdb 9f7e 7211 6dc9  .e.n..,.K..~r.m.
-00002020: 08c7 d803 f944 6ca1 961f 4939 db2a 16c5  .....Dl...I9.*..
-00002030: 0886 91b8 c066 3881 df26 8cc7 48c2 239f  .....f8..&..H.#.
-00002040: 16c7 1c1d 83de 9816 2ba5 52ad 1823 92f8  ........+.R..#..
-00002050: 5e82 6250 7b7d 3221 23ec 0d95 4a7f 7ba9  ^.bP{}2!#...J.{.
-00002060: bc4f e131 9142 0d8c 28df 57aa b125 a1b1  .O.1.B..(.W..%..
-00002070: e3c3 b242 8885 e852 ee1d 21da f261 9e31  ...B...R..!..a.1
-00002080: 3b1e e27b d2f7 2812 127e 68f9 25fd e717  ;..{..(..~h.%...
-00002090: b72f 16d1 5626 44e5 0659 436e a0ff 32b9  ./..V&D..YCn..2.
-000020a0: 4c60 7c58 d173 f2e9 c16a d220 0883 5a7b  L`|X.s...j. ..Z{
-000020b0: a55f 03a8 5cc7 f5eb fd5a bfb6 d2a7 0168  ._..\....Z.....h
-000020c0: 3482 95a6 b6d8 3aeb 956e 9061 0d50 fad5  4.....:..n.a.P..
-000020d0: a1bb 57ef 55cb 16de d05f 5db3 b91d aa8f  ..W.U...._].....
-000020e0: 85d7 a054 7fb0 861f 0cba e045 0baf 4129  ...T.......E..A)
-000020f0: 3e5c c387 9d66 a767 ebd7 a014 5f5b c3d7  >\...f.g...._[..
-00002100: 4bed 5e50 b7f4 6b50 4449 72b8 862e 85b5  K.^P..kPDIr.....
-00002110: 6a77 b9da 1564 c2e8 8e13 de0c 8341 bd92  jw...d.......A..
-00002120: 29cf 5190 0dab ec52 534c 5822 37e5 5a8c  ).Q....RSLX"7.Z.
-00002130: ee32 3e00 8002 5224 49e2 c9c5 0c4f d008  .2>...R$I....O..
-00002140: b2b8 8b28 39e0 c4db 25d3 0812 6f86 1226  ...(9...%...o..&
-00002150: 60b8 5429 0d4a 55f8 af3e 81fe a623 8ab6  `.T).JU..>...#..
-00002160: 3032 a495 5d60 8958 1b52 f678 62c4 c94c  02..]`.X.R.xb..L
-00002170: b6fc 2ba0 d537 202f 9e3d 7bfe f0e9 f387  ..+..7 /.={.....
-00002180: bf3d 7ff4 e8f9 c35f b2b9 b52a 4b6e 0725  .=....._...*Kn.%
-00002190: 5353 eed5 8f5f fffd fd17 de5f bffe f0ea  SS..._....._....
-000021a0: f137 e9d4 27f1 c2c4 bffc f9cb 97bf fff1  .7..'...........
-000021b0: 3af5 b0e2 dc15 2fbe 7df2 f2e9 9317 df7d  :...../.}......}
-000021c0: f5e7 4f8f 1dda db1c 1d98 f021 89b1 f0ae  ..O........!....
-000021d0: e163 ef26 8b61 810e fbf1 013f 9dc4 3042  .c.&.a.....?..0B
-000021e0: c492 4011 e876 a8ee cbc8 025e 5b20 eac2  ..@..v.....^[ ..
-000021f0: 75b0 edc2 db1c 58c6 05bc 3cbf 6bd9 ba1f  u.....X...<.k...
-00002200: f1b9 248e 99af 46b1 05dc 638c 7618 773a  ..$...F...c.v.w:
-00002210: e0aa 9acb f0f0 709e 4cdd 93f3 b989 bb89  ......p.L.......
-00002220: d091 6bee 2e4a ac00 f7e7 33a0 57e2 52d9  ..k..J....3.W.R.
-00002230: 8db0 65e6 0d8a 1289 a638 c1d2 53bf b143  ..e......8..S..C
-00002240: 8c1d abbb 4388 e5d7 3d32 e24c b089 f4ee  ....C...=2.L....
-00002250: 10af 8388 d325 4372 6025 522e b443 6288  .....%Cr`%R..Cb.
-00002260: cbc2 6520 84da f2cd de6d afc3 a86b d53d  ..e .....m...k.=
-00002270: 7c64 2361 5b20 ea30 7e88 a9e5 c6cb 682e  |d#a[ .0~.....h.
-00002280: 51ec 5239 4431 351d be8b 64e4 3272 7fc1  Q.R9D15...d.2r..
-00002290: 4726 ae2f 2444 7a8a 29f3 fa63 2c84 4be6  G&./$Dz.)..c,.K.
-000022a0: 3a87 f51a 41bf 0a0c e30e fb1e 5dc4 3692  :...A.......].6.
-000022b0: 4b72 e8d2 b98b 1833 913d 76d8 8d50 3c73  Kr.....3.=v..P<s
-000022c0: da4c 92c8 c47e 260e 2145 9177 8349 177c  .L...~&.!E.w.I.|
-000022d0: 8fd9 3b44 3d43 1c50 b231 dcb7 09b6 c2fd  ..;D=C.P.1......
-000022e0: 6622 b805 e46a 9a94 2788 fa65 ce1d b1bc  f"...j..'..e....
-000022f0: 8c99 bd1f 1774 82b0 8b65 da3c b6d8 b5cd  .....t...e.<....
-00002300: 8933 3b3a f3a9 95da bb18 5374 8cc6 187b  .3;:......St...{
-00002310: b73e 7358 d061 33cb e7b9 d157 2260 951d  .>sX.a3....W"`..
-00002320: ec4a ac2b c8ce 55f5 9c60 0165 92aa 6bd6  .J.+..U..`.e..k.
-00002330: 2972 9708 2b65 f7f1 946d b067 6f71 8278  )r..+e...m.goq.x
-00002340: 1628 8911 dfa4 f91a 44dd 4a5d 38e5 9c54  .(......D.J]8..T
-00002350: 7a9d 8e0e 4de0 3502 e51f e48b d329 d705  z...M.5......)..
-00002360: e830 92bb bf49 eb8d 0859 6797 7a16 ee7c  .0...I...Yg.z..|
-00002370: 5d70 2b7e 6fb3 c760 5fde 3ded be04 197c  ]p+~o..`_.=....|
-00002380: 6a19 20f6 b7f6 cd10 516b 823c 6186 080a  j. .....Qk.<a...
-00002390: 0c17 dd82 8815 fe5c 449d ab5a 6cee 949b  .......\D..Zl...
-000023a0: d89b 360f 0314 4656 bd13 93e4 8dc5 cf89  ..6...FV........
-000023b0: b227 fc77 ca1e 7701 7306 058f 5bf1 fb94  .'.w..w.s...[...
-000023c0: 3a9b 2865 e744 81b3 09f7 1f2c 6b7a 689e  :.(e.D.....,kzh.
-000023d0: dcc0 7092 ac73 d679 5573 5ed5 f8ff fbaa  ..p..s.yUs^.....
-000023e0: 66d3 5e3e af65 ce6b 99f3 5ac6 f5f6 f541  f.^>.e.k..Z....A
-000023f0: 6a99 bc7c 81ca 26ef f2e8 9e4f bcb1 e533  j..|..&....O...3
-00002400: 2194 eecb 05c5 bb42 777d 04bc d18c 0730  !......Bw}.....0
-00002410: a8db 51ba 27b9 6a01 ce22 f89a 3598 2cdc  ..Q.'.j.."..5.,.
-00002420: 9423 2de3 7126 3f27 32da 8fd0 0c5a 4365  .#-.q&?'2....ZCe
-00002430: ddc0 9c8a 4cf5 5478 3326 a063 a487 752b  ....L.Tx3&.c..u+
-00002440: 159f d0ad fb4e f378 8f8d d34e 67b9 acba  .....N.x...Ng...
-00002450: 9aa9 0b05 92f9 7829 5c8d 4397 4aa6 e85a  ......x)\.C.J..Z
-00002460: 3def dead d4eb 7ee8 5477 5997 0628 d9d3  =.....~.TwY..(..
-00002470: 1861 4c66 1b51 7518 515f 0e42 145e 6784  .aLf.Qu.Q_.B.^g.
-00002480: 5ed9 9958 d174 58d1 50ea 97a1 5a46 71e5  ^..X.tX.P...ZFq.
-00002490: 0a30 6d15 1578 e5f6 e045 bde5 8741 da41  .0m..x...E...A.A
-000024a0: 8666 1c94 e763 15a7 b499 bc8c ae0a ce99  .f...c..........
-000024b0: 467a 9333 a999 0150 622f 3320 8f74 53d9  Fz.3...Pb/3 .tS.
-000024c0: ba71 796a 7569 aabd 45a4 2d23 8c74 b38d  .qyjui..E.-#.t..
-000024d0: 30d2 3082 17e1 2c3b cd96 fb59 c6ba 9987  0.0...,;...Y....
-000024e0: d432 4fb9 62b9 1b72 33ea 8d0f 116b 4522  .2O.b..r3....kE"
-000024f0: 27b8 8126 2653 d0c4 3b6e f9b5 6a08 b72a  '..&&S..;n..j..*
-00002500: 2334 6bf9 13e8 18c3 d778 06b9 23d4 5b17  #4k......x..#.[.
-00002510: a253 b876 1949 9e6e f877 6196 1917 b287  .S.v.I.n.wa.....
-00002520: 4494 3a5c 934e ca06 3191 987b 94c4 2d5f  D.:\.N..1..{..-_
-00002530: 2d7f 950d 34d1 1ca2 6d2b 5780 103e 5ae3  -...4...m+W..>Z.
-00002540: 9a40 2b1f 9b71 1074 3bc8 7832 c123 6986  .@+..q.t;.x2.#i.
-00002550: dd18 519e 4e1f 81e1 53ae 70fe aac5 df1d  ..Q.N...S.p.....
-00002560: ac24 d91c c2bd 1f8d 8fbd 033a e737 11a4  .$.........:.7..
-00002570: 5858 2f2b 078e 8980 8b83 72ea cd31 819b  XX/+......r..1..
-00002580: b015 91e5 f977 e260 ca68 d7bc 8ad2 3994  .....w.`.h....9.
-00002590: 8e23 3a8b 5076 a298 649e c235 89ae ccd1  .#:.Pv..d..5....
-000025a0: 4f2b 1f18 4fd9 9ac1 a1eb 2e3c 98aa 03f6  O+..O......<....
-000025b0: bd4f dd37 1fd5 ca73 0669 e667 a6c5 2aea  .O.7...s.i.g..*.
-000025c0: d474 93e9 873b e40d abf2 43d4 b22a a56e  .t...;....C..*.n
-000025d0: fd4e 2d72 ae6b 2eb9 0e12 d579 4abc e1d4  .N-r.k.....yJ...
-000025e0: 7d8b 03c1 302d 9fcc 324d 59bc 4ec3 8ab3  }...0-..2MY.N...
-000025f0: b351 dbb4 332c 080c 4fd4 36f8 6d75 4638  .Q..3,..O.6.muF8
-00002600: 3df1 ae27 3fc8 9dcc 5a75 402c eb4a 9df8  =..'?...Zu@,.J..
-00002610: faca dcbc d566 0777 813c 7a70 7f38 a752  .....f.w.<zp.8.R
-00002620: e850 426f 9723 28fa d21b c894 3660 8bdc  .PBo.#(.....6`..
-00002630: 9359 8d08 dfbc 3927 2dff 7e29 6c07 dd4a  .Y....9'-.~)l..J
-00002640: d82d 941a 61bf 1054 8352 a111 b6ab 8576  .-..a..T.R.....v
-00002650: 1856 cbfd b05c ea75 2a0f e060 9151 5c0e  .V...\.u*..`.Q\.
-00002660: d3eb fa01 5c61 d045 7669 afc7 d72e eee3  ....\a.Evi......
-00002670: e52d cd85 118b 8b4c 5fcc 17b5 e1fa e2be  .-.....L_.......
-00002680: 5cd9 7c71 ef11 209d fbb5 caa0 596d 766a  \.|q.. .....Ymvj
-00002690: 8566 b53d 2804 bd4e a3d0 ecd6 3a85 5ead  .f.=(..N....:.^.
-000026a0: 5bef 0d7a ddb0 d11c 3cf0 bd23 0d0e dad5  [..z....<..#....
-000026b0: 6e50 eb37 0ab5 72b7 5b08 6a25 657e a359  nP.7..r.[.j%e~.Y
-000026c0: a807 954a 3ba8 b71b fda0 fd20 2b63 60e5  ...J;...... +c`.
-000026d0: 297d 64be 00f7 6abb b6ff 0100 00ff ff03  )}d...j.........
-000026e0: 0050 4b03 0414 0006 0008 0000 0021 0040  .PK..........!.@
-000026f0: b3d4 95e4 0300 0012 1100 000d 0000 0078  ...............x
-00002700: 6c2f 7374 796c 6573 2e78 6d6c d458 4b6f  l/styles.xml.XKo
-00002710: db38 10be 2fb0 ff81 e05d d1c3 926b 1992  .8../....]...k..
-00002720: 8a3a 8e80 02dd a040 b2c0 5e69 9972 8852  .:.....@..^i.r.R
-00002730: a496 a213 7917 fbdf 77a8 872d 276e ead8  ....y...w..-'n..
-00002740: 699b 1e6c 9323 6ae6 9b37 c7d1 fbba e0e8  i..l.#j..7......
-00002750: 9eaa 8a49 1163 f7c2 c188 8a4c 2e99 58c5  ...I.c.....L..X.
-00002760: f8cf dbd4 9a60 5469 2296 844b 4163 bca1  .....`Ti"..KAc..
-00002770: 157e 9ffc fe5b 54e9 0da7 3777 946a 042c  .~...[T...7w.j.,
-00002780: 4415 e33b adcb a96d 57d9 1d2d 4875 214b  D..;...mW..-Hu!K
-00002790: 2ae0 492e 5541 346c d5ca ae4a 45c9 b232  *.I.UA4l...JE..2
-000027a0: 2f15 dcf6 1c67 6c17 8409 dc72 9816 d931  /....gl....r...1
-000027b0: 4c0a a2be ac4b 2b93 4549 345b 30ce f4a6  L....K+.EI4[0...
-000027c0: e185 5191 4d3f ae84 5464 c101 6aed fa24  ..Q.M?..Td..j..$
-000027d0: 43b5 3b56 1eaa 552f a4a1 3e91 53b0 4cc9  C.;V..U/..>.S.L.
-000027e0: 4ae6 fa02 f8da 32cf 5946 9fc2 0ded d026  J.....2.YF.....&
-000027f0: d98e 1370 3e8d 931b d88e b7a7 7bad 4ee4  ...p>.......{.N.
-00002800: e4db 8ade 33e3 3e9c 44b9 14ba 4299 5c0b  ....3.>.D...B.\.
-00002810: 1d63 1f80 1a13 4cbf 08f9 2052 f308 3cdc  .c....L... R..<.
-00002820: 9d4a a2ea 1f74 4f38 505c 6c27 5126 b954  .J...tO8P\l'Q&.T
-00002830: 4883 ebc0 720d 4590 82b6 272e 0967 0bc5  H...r.E...'..g..
-00002840: ccb1 9c14 8c6f 5ab2 6708 8db7 bb73 0503  .....oZ.g....s..
-00002850: db1b a26d 70b4 6892 6861 4ebd 4d59 72ad  ...mp.h.haN.MYr.
-00002860: 1855 e89a 3e3c d66d f444 8d17 a870 1cdb  .U..><.m.D...p..
-00002870: c648 1558 8971 bef5 9967 dc03 8424 82e0  .H.X.q...g...$..
-00002880: d654 8914 36a8 5bdf 6e4a 708e 803c 6cd1  .T..6.[.nJp..<l.
-00002890: 35e7 be71 7aa5 c8c6 f582 c10b 7623 10fc  5..qz.......v#..
-000028a0: 22d5 12f2 7e17 2d3d 2989 38cd 3578 4db1  "...~.-=).8.5xM.
-000028b0: d59d f9d5 b284 ef85 d41a 7223 8996 8cac  ..........r#....
-000028c0: a420 dc38 ba65 72f8 4da8 1b50 2262 acef  . .8.er.M..P"b..
-000028d0: 20c5 1f45 5888 9166 2648 9d8b 5118 86ef   ..EX..f&H..Q...
-000028e0: 8260 12b8 a1e7 c3a7 093e bb91 dd88 3e8b  .`.......>....>.
-000028f0: 0d40 ef91 9fc5 a755 fedb ba9f 25c4 987d  .@.....U....%..}
-00002900: cfea bf94 eafb 01f3 e6a1 77a1 0b09 9851  ..........w....Q
-00002910: ce6f 4ca8 fe95 6fb3 c194 c93a 4762 5da4  .oL...o....:Gb].
-00002920: 85fe b884 38c5 c814 b57e 09a9 d72d db0c  ....8....~...-..
-00002930: 6837 2623 86dc 5ade 43b6 e393 f8a2 3adf  h7&#..Z.C.....:.
-00002940: 0ad8 43e5 431e f5b0 5c58 1e86 b57d 1d91  ..C.C...\X...}..
-00002950: b2e4 9beb 75b1 a02a 6dfa b2a9 f52d d5f4  ....u..*m....-..
-00002960: 87ae f27f 5584 31c2 4922 c030 2f66 ea41  ....U.1.I".0/f.A
-00002970: fbea d47e 0ef7 ac29 63df 0df9 be71 dadd  ...~...)c....q..
-00002980: 7922 476f 48af 9f60 3cd3 d076 5177 1c00  y"GoH..`<..vQw..
-00002990: 0885 d708 edce 971d 80e7 6212 7cf4 fa02  ..........b.|...
-000029a0: 5bf1 1f38 5b89 82b6 c996 4470 b56a b7e8  [..8[.....Dp.j..
-000029b0: 4191 f296 d67d 12da 75fe 4cd2 7c17 803f  A....}..u.L.|..?
-000029c0: c922 bb18 f811 1682 7a77 4c59 e9cb e17e  ."......zwLY...~
-000029d0: cc3c ceff 7301 1fd5 551e e1fd 6a00 c114  .<..s...U...j...
-000029e0: a759 66ae f419 8417 6d6f e24f a2e8 8522  .Yf.....mo.O..."
-000029f0: ff5e 4b4d 3f2b 9ab3 fa50 8d7d 5505 0e65  .^KM?+...P.}U..e
-00002a00: 40d3 4fa1 830e daf4 5e93 deb6 5b64 e695  @.O.....^...[d..
-00002a10: 185f 9bb6 c607 3e5e ac19 87ab e681 060d  ._....>^........
-00002a20: 3c97 f5ae e53b e68e accd e8d8 5c06 b652  <....;......\..R
-00002a30: 40c5 25cd c99a ebdb edc3 18ef d67f d025  @.%............%
-00002a40: 5b17 50a2 ba53 9fd9 bdd4 0d8b 18ef d69f  [.P..S..........
-00002a50: cc5d da1d 1b19 90e3 9f2a b8e8 c12f 8201  .].......*.../..
-00002a60: 24c6 ff5e cdde 85f3 abd4 b326 ce6c 62f9  $..^.......&.lb.
-00002a70: 231a 5861 309b 5b81 7f39 9bcf d3d0 f19c  #.Xa0.[..9......
-00002a80: cbff 0603 ec19 e36b 336f 4361 71fd 69c5  .......k3oCaq.i.
-00002a90: 61c8 559d b21d f89b 1d2d c683 4d0b bf99  a.U......-..M...
-00002aa0: 2200 f610 7be8 8d9d 0f81 eb58 e9c8 712d  "...{......X..q-
-00002ab0: 7f4c 26d6 643c 0aac 3470 bdf9 d89f 5d05  .L&.d<..4p....].
-00002ac0: 6930 c01e 9c38 e63a b6eb b603 b301 1f4c  i0...8.:.......L
-00002ad0: 352b 2867 a2f7 55ef a121 159c 04db 6794  5+(g..U..!....g.
-00002ae0: b07b 4fd8 bb3f 3392 ff01 0000 ffff 0300  .{O..?3.........
-00002af0: 504b 0304 1400 0600 0800 0000 2100 fcff  PK..........!...
-00002b00: 017b a806 0000 8318 0000 1400 0000 786c  .{............xl
-00002b10: 2f73 6861 7265 6453 7472 696e 6773 2e78  /sharedStrings.x
-00002b20: 6d6c 9419 5d4f dc38 f01d 89ff e0b3 8400  ml..]O.8........
-00002b30: e9ca b2d0 6d7b 88a5 147a 4595 aab6 27da  ....m{...zE...'.
-00002b40: 7d39 21e4 4d86 dd40 62a7 8937 29fc fa1b  }9!.M..@b..7)...
-00002b50: 3b09 493c 4eae e589 cc78 c633 e3f9 ded3  ;.I<N....x.3....
-00002b60: b73f 9398 1590 e591 9273 3e3d 38e4 0c64  .?.......s>=8..d
-00002b70: a0c2 48ae e6fc fbb7 0f2f de70 966b 2143  ..H....../.p.k!C
-00002b80: 112b 0973 fe08 397f 7bb6 bd75 9ae7 9a21  .+.s..9.{..u...!
-00002b90: adcc e77c ad75 7a32 99e4 c11a 1291 1fa8  ...|.uz2........
-00002ba0: 1424 62ee 5496 088d 9fd9 6a92 a719 8830  .$b.T.....j....0
-00002bb0: 5f03 e824 9e1c 1d1e be9a 2422 929c 056a  _..$......$"...j
-00002bc0: 23f5 9c1f bd7e c9d9 4646 3f36 7059 41a6  #....~..FF?6pYA.
-00002bd0: b319 3f3b cda3 b353 7df6 5143 723a d167  ..?;...S}.QCr:.g
-00002be0: a713 f35d c152 b182 dc05 5e0a 0d2b 953d  ...].R....^..+.=
-00002bf0: baf0 ebcd 3210 da85 7e10 39b8 b07f 3640  ....2...~.9...6@
-00002c00: c92f 5592 80d4 e4ba c5a5 4bfe f1bd 0bf9  ./U.......K.....
-00002c10: 0405 c42e 50c4 3a42 9d08 c328 49e3 88aa  ....P.:B...(I...
-00002c20: f525 8b56 9114 848d 2c59 0880 cfc7 56f0  .%.V....,Y....V.
-00002c30: e4de 719e 413c 47b3 8781 1f43 c04b 480f  ..q.A<G....C.KH.
-00002c40: 2cab 5c43 1cae 210a 89d8 3264 e7a9 9e33  ,.\C..!...2d...3
-00002c50: 990e a144 784f ae43 8a65 e925 88e4 5d25  ...DxO.C.e.%..]%
-00002c60: a317 6b14 4814 9182 187d e152 c7d1 7d08  ..k.H....}.R..}.
-00002c70: 286b a154 5642 4684 b5a6 51cb fba9 4b98  (k.TVBF...Q...K.
-00002c80: 00e0 f987 5fa1 3df2 892c 95de 4b45 86be  ...._.=..,..KE..
-00002c90: 7272 2255 08ff 9ea3 dbcd 77d3 74f7 66df  rr"U......w.t.f.
-00002ca0: 77de 7f96 61b4 312b 236a 7fe3 d219 a59e  w...a.1+#j......
-00002cb0: 40e7 100f a937 9954 771b fb71 a326 dfde  @....7.Tw..q.&..
-00002cc0: 62f8 67d8 fa25 e469 ca6f f6c9 550d 23a3  b.g..%.i.o..U.#.
-00002cd0: 8439 d2b2 d9b3 e2f1 34a8 6186 bdca 2aa1  .9......4.a...*.
-00002ce0: 791c f2fd ee8d c60e ad2c 372e 0add 8317  y........,7.....
-00002cf0: 4ffc 66f0 fa86 f6a8 be0c 2faa efef 28d7  O.f......./...(.
-00002d00: 2848 4dda 4a6e ce34 e72a 89d0 c023 8a37  (HM.Jn.4.*...#.7
-00002d10: 5a9a 20f2 298a ea77 14dd b38f cd65 63a7  Z. .)..w.....ec.
-00002d20: da26 7b26 62b8 ecd0 37c6 b28a cb92 ef0f  .&{&b...7.......
-00002d30: 5a7e 4000 eb1f 861a a38d ff2e 71ef a95a  Z~@.........q..Z
-00002d40: 0d1a bbf8 b418 d584 6853 bd6f 636b fb58  ........hS.ock.X
-00002d50: cfb2 d6e6 1a7d c131 17ad 78f7 c81b af78  .....}.1..x....x
-00002d60: 16d2 75fb eeab ff8a 77f8 3ca4 2b77 3f1a  ..u.....w.<.+w?.
-00002d70: 5abb d97b 7b11 d133 751b 150d 891b a575  Z..{{..3u......u
-00002d80: 64f4 d14d 7478 9ce4 faf0 9064 3084 91cc  d..Mtx.....d0...
-00002d90: 84b0 6337 8b20 eca5 0736 f3c0 5e79 60af  ..c7. ...6..^y`.
-00002da0: 3db0 371e d85f 1436 3df4 c03c 7a4c 891e  =.7.._.6=..<zL..
-00002db0: 124b a9c4 2623 7a78 c0ee c4e5 a264 885d  .K..&#zx.....d.]
-00002dc0: cc10 3645 9c52 322f b029 01e9 d2e6 0281  ..6E.R2/.)......
-00002dd0: d84f 98c2 676a 29ac 42d2 1960 8f14 0396  .O..gj).B..`....
-00002de0: 15a6 b1ba d0a4 1c6b a5a2 d0d6 e312 3334  .......k......34
-00002df0: 3921 8548 2c82 debe 8cee 0b05 2bac 5a0f  9!.H,.......+.Z.
-00002e00: c0b0 0a8b 18d5 a3c7 9e20 beb3 9d58 b402  ......... ...X..
-00002e10: 5bda 3a2c d931 b05a 4557 34e4 5edd ebf2  [.:,.1.ZEW4.^...
-00002e20: 6785 902c 8d05 f668 bf47 e333 8042 f318  g..,...h.G.3.B..
-00002e30: b906 6f73 af98 1137 9811 2798 1117 9811  ..os...7..'.....
-00002e40: 479e 1137 9e11 279e 1117 9e11 c77c 45e4  G..7..'......|E.
-00002e50: 69aa 5f5a 1885 b146 a103 f0c1 2255 1acf  i._Z...F...."U..
-00002e60: c243 584f 8873 882c 124b 8881 1d11 158b  .CXO.s.,.K......
-00002e70: 1647 94ed e088 da1d 1c31 4007 474c d1c1  .G.......1@.GL..
-00002e80: 11a3 7470 24be 3b38 12e7 1d1c 316b 8b3b  ..tp$.;8....1k.;
-00002e90: 2606 eee0 46ec 724c ec72 71c1 946b e3af  &...F.rL.rq..k..
-00002ea0: a409 5c90 56fc 3349 3c57 572e e8f3 b50b  ..\.V.3I<WW.....
-00002eb0: c1db c8e4 f085 9c5a 7c23 748b 0b20 9d27  .......Z|#t.. .'
-00002ec0: 3223 b02a ae0f 0a59 1eb8 3c36 91b6 a980  2#.*...Y..<6....
-00002ed0: 3dd9 ecc6 d282 9598 5b30 0989 3867 2fa6  =.......[0..8g/.
-00002ee0: 98ab f2c0 976d 883d 716c 7399 070a a70d  .....m.=qls.....
-00002ef0: f889 8348 4414 3429 0933 11c9 9341 0620  ...HD.4).3...A. 
-00002f00: 3dc9 171b 7974 7ff7 78ad 1933 aafd d9aa  =...yt..x..3....
-00002f10: 59ff 8b50 9720 cd54 00b9 47d2 8ca4 e3eb  Y..P. .T..G.....
-00002f20: c3e9 4850 1c13 9c56 5a88 7828 3f11 4154  ..HP...VZ.x(?.AT
-00002f30: 4e6c 8237 7a4a e6d4 5332 a723 a135 9601  Nl.7zJ..S2.#.5..
-00002f40: 5c29 5690 4461 8835 0958 8cf5 4963 dacf  \)V.Da.5.X..Ic..
-00002f50: a27b 6095 5bfc ffe9 198b 855c 6155 ebd1  .{`.[......\aU..
-00002f60: d1ca 72f5 69f1 dde5 76f5 69e6 811e 7982  ..r.i...v.i...y.
-00002f70: f1b6 32ad 2f6e 94cf 889e de61 3a92 5346  ..2./n.....a:.SF
-00002f80: 5e79 24f3 9157 8138 8e52 1d99 1d05 0e42  ^y$..W.8.R.....B
-00002f90: 7aa0 14cb 08f4 8b22 5610 e10c e81b 8195  z......"V.......
-00002fa0: 34bb 1274 25b9 c439 af7e 096a d1bf df91  4..t%..9.~.j....
-00002fb0: c482 9c17 3563 17f7 a562 fa9d c661 47ea  ....5c...b...aG.
-00002fc0: 77a3 4237 ac47 6446 f6be bec2 2c71 4ef2  w.B7.GdF....,qN.
-00002fd0: 5404 b8dc c175 410e 5901 fcec b9f8 7566  T....uA.Y.....uf
-00002fe0: 975e 2b5f 0da9 a9ca 912b 524a 9534 b3d0  .^+_.....+RJ.4..
-00002ff0: f331 5df2 e751 f68f 390f 41f7 8ed8 3e3a  .1]..Q..9.A...>:
-00003000: 2937 7cbf 9e4c cd9c 880c 9119 b663 380f  )7|..L.......c8.
-00003010: 32dc 3239 5b9f 5a2c 9cff 6248 1231 e780  2.29[.Z,..bH.1..
-00003020: 3b24 3378 d69f 8910 590f 50e2 5bf7 00ea  ;$3x....Y.P.[...
-00003030: aef7 196e f2fa fe76 6cd9 abc7 ae20 0b2b  ...n...vl.... .+
-00003040: 050e 0e3a 13f5 6e20 ef77 adc4 f5a8 9457  ...:..n .w.....W
-00003050: 9b2c 2385 5529 48ab 1bec 070e 059d af3c  .,#.U)H........<
-00003060: df2c bb9f c5b4 f355 ae7f b45f a83b 2fd7  .,.....U..._.;/.
-00003070: 7dea 726d c8f7 6ff6 51e3 8eb4 d524 1b62  }.rm..o.Q....$.b
-00003080: d3f8 80a3 e4f6 d6f6 d650 93c2 7624 94b7  .........P..v$..
-00003090: d7df de7d bdbd b8b8 d53b ecd7 0ea6 c307  ...}.....;......
-000030a0: 7b0c d5ce 10bf 9dba 9e90 03e3 ce57 f754  {............W.T
-000030b0: 69c1 7134 725c 619c d2ce 62eb faf9 ce5b  i.q4r\a...b....[
-000030c0: 3ef6 dd9e 6dd7 7b57 5e04 f6b5 fbe3 2b43  >...m.{W^.....+C
-000030d0: 57b3 0f89 15ce be8e 8bb6 8fce e68c ebc8  W...............
-000030e0: e007 d0b8 8310 59e5 88f4 8419 f1ca d259  ......Y........Y
-000030f0: 10e0 1458 0f9d cdfc ca58 3b20 527b f422  ...X.....X; R{."
-00003100: 164b 6be5 b9e6 3289 4ba9 f3a2 d48f 29c6  .Kk...2.K.....).
-00003110: e912 9e2a 7faf c4c0 e544 3518 cdf9 71bb  ...*.....D5...q.
-00003120: 5de9 009b 6586 f1ee f668 e23d 5b78 a1aa  ]...e....h.=[x..
-00003130: bf0c 4259 6c8c 8bb0 39de 9b92 6d92 206e  ..BYl...9...m. n
-00003140: 84a5 9774 96be 8623 110f 38c4 89d4 87fb  ...t...#..8.....
-00003150: 800d 8adb 598c 3a51 fdf0 269c abcd 59b3  ....Y.:Q..&...Y.
-00003160: cfe3 368c 6fda 9d40 e521 55b8 3e6f 281a  ..6.o..@.!U.>o(.
-00003170: a089 d93e 9071 1bd7 ed2e a35d 15d6 ac5b  ...>.q.....]...[
-00003180: 1f69 5681 983f 972a 7ce4 9817 bafb 0c13  .iV..?.*|.......
-00003190: fb88 c294 3480 d162 3580 919b 20c6 6442  ....4..b5... .dB
-000031a0: 732c 1a30 232d d85d 146b c8dc 746c 3b78  s,.0#-.].k..tl;x
-000031b0: cf62 7c23 3739 84a4 d5a9 c09d 1662 823f  .b|#79.......b.?
-000031c0: 229c fd07 0000 ffff 0300 504b 0304 1400  ".........PK....
-000031d0: 0600 0800 0000 2100 3b6d 324b c100 0000  ......!.;m2K....
-000031e0: 4201 0000 2300 0000 786c 2f77 6f72 6b73  B...#...xl/works
-000031f0: 6865 6574 732f 5f72 656c 732f 7368 6565  heets/_rels/shee
-00003200: 7431 2e78 6d6c 2e72 656c 7384 8fc1 8ac2  t1.xml.rels.....
-00003210: 3014 45f7 03fe 4378 7b93 d685 0c43 5337  0.E...Cx{....CS7
-00003220: 22b8 55e7 0362 fada 06db 9790 f714 fd7b  ".U..b.........{
-00003230: b31c 65c0 e5e5 70cf e536 9bfb 3ca9 1b66  ..e...p..6..<..f
-00003240: 0e91 2cd4 ba02 85e4 6317 68b0 f07b da2d  ..,.....c.h..{.-
-00003250: bf41 b138 eadc 1409 2d3c 9061 d32e be9a  .A.8....-<.a....
-00003260: 034e 4e4a 89c7 9058 150b b185 5124 fd18  .NNJ...X....Q$..
-00003270: c37e c4d9 b18e 09a9 903e e6d9 4989 7930  .~.......>..I.y0
-00003280: c9f9 8b1b d0ac aa6a 6df2 5f07 b42f 4eb5  .......jm._../N.
-00003290: ef2c e47d 5783 3a3d 5259 feec 8e7d 1f3c  .,.}W.:=RY...}.<
-000032a0: 6ea3 bfce 48f2 cf84 4939 9060 3ea2 4839  n...H...I9.`>.H9
-000032b0: c845 edf2 8062 41eb 77f6 9e6b 7d0e 04a6  .E...bA.w..k}...
-000032c0: 6dcc cbf3 f609 0000 ffff 0300 504b 0304  m...........PK..
-000032d0: 1400 0600 0800 0000 2100 13c4 2c13 c200  ........!...,...
-000032e0: 0000 4201 0000 2300 0000 786c 2f77 6f72  ..B...#...xl/wor
-000032f0: 6b73 6865 6574 732f 5f72 656c 732f 7368  ksheets/_rels/sh
-00003300: 6565 7432 2e78 6d6c 2e72 656c 7384 8fc1  eet2.xml.rels...
-00003310: 6ac3 3010 44ef 85fc 83d8 7b24 3b87 508a  j.0.D.....{$;.P.
-00003320: 255f 4a21 d726 fd00 455e dba2 f64a 68b7  %_J!.&..E^...Jh.
-00003330: 25f9 fbe8 d884 428e c363 de30 5d7f 5917  %.....B..c.0].Y.
-00003340: f58b 8563 220b ad6e 4021 8534 449a 2c7c  ...c"..n@!.4D.,|
-00003350: 9d3e b6af a058 3c0d 7e49 8416 aec8 d0bb  .>...X<.~I......
-00003360: cd4b f789 8b97 5ae2 3966 56d5 426c 6116  .K....Z.9fV.Bla.
-00003370: c96f c670 9871 f5ac 5346 aa64 4c65 f552  .o.p.q..SF.dLe.R
-00003380: 6399 4cf6 e1db 4f68 764d b337 e5af 03dc  c.L...OhvM.7....
-00003390: 9d53 1d06 0be5 30b4 a04e d75c 979f bbd3  .S....0..N.\....
-000033a0: 38c6 80ef 29fc ac48 f2cf 84c9 2592 6039  8...)..H....%.`9
-000033b0: a248 3dc8 55ed cb84 6241 eb47 f698 77fa  .H=.U...bA.G..w.
-000033c0: 1c09 8ceb ccdd 7377 0300 00ff ff03 0050  ......sw.......P
-000033d0: 4b03 0414 0006 0008 0000 0021 00ae 0bfd  K..........!....
-000033e0: 89bb 0100 002c 1500 0027 0000 0078 6c2f  .....,...'...xl/
-000033f0: 7072 696e 7465 7253 6574 7469 6e67 732f  printerSettings/
-00003400: 7072 696e 7465 7253 6574 7469 6e67 7331  printerSettings1
-00003410: 2e62 696e ec94 cd4a e350 14c7 ff69 fca8  .bin...J.P...i..
-00003420: ce62 2c08 6e66 3114 5762 194b e3c7 4e4b  .b,.nf1.Wb.K..NK
-00003430: d33a 95c6 84a6 1537 b328 3642 a026 254d  .:.....7.(6B.&%M
-00003440: 9119 1941 e62d c407 99e5 2c5d fa00 b376  ...A.-....,]...v
-00003450: 253e 801b fddf d822 ce14 29e2 4638 379c  %>....."..).F87.
-00003460: 7b3e eeb9 e7e6 feb8 1c0b 3e0e 1021 448f  {>........>..!D.
-00003470: 7288 189f e1d0 f711 2476 cca8 8a98 a860  r.......$v.....`
-00003480: d4d0 26f4 a9bf 70e6 f52f 1a34 cce0 fc83  ..&...p../.4....
-00003490: 916e d3fa 88fd 548a 7a3f a573 2ec2 18b9  .n....T.z?.s....
-000034a0: fb75 416d b04d e914 45e9 7b8e edaa fbec  .uAm.M..E.{.....
-000034b0: 18b3 badb cce2 128b fa72 66f3 dbc9 e94b  .........rf....K
-000034c0: a74d 268b 9349 ad37 fc55 29f5 8e08 0cdf  .M&..I.7.U).....
-000034d0: d538 bf7c c924 d76a eca8 dc39 fcc6 0956  .8.|.$.j...9...V
-000034e0: b0c1 575e a1ce 732e 2287 32d6 5060 2c47  ..W^..s.".2.P`,G
-000034f0: 31b1 ce2f c79c 02e3 655a 2bf4 0dfa 79ea  1../....eZ+...y.
-00003500: 12bd 0256 13ef 272b d6cb ae59 aba1 19f8  ...V..'+...Y....
-00003510: 91d7 5396 d3ea 7a91 ebff f050 3460 47be  ..S...z....P4`G.
-00003520: 17c4 add8 0f03 3876 bd51 2f56 1ba8 7bbd  ......8v.Q/V..{.
-00003530: b0d3 4f62 34ed aeb2 f228 859d 30b2 c2b6  ..Ob4....(..0...
-00003540: f768 fd7f b3e5 0cb0 6798 d6f0 ee17 b3dd  .h......g.......
-00003550: ec27 a6dd 5074 ca9d 66a7 8deb 63eb d7ed  .'..Pt..f...c...
-00003560: f4d7 853f ab67 578c d506 6b48 3fd5 53b9  ...?.gW...kH?.S.
-00003570: ca5f 1a68 e56f 51f6 943f 07de 3f64 9fe9  ._.h.oQ..?..?d..
-00003580: e308 5ed2 599a ec37 1efb 8c83 16ad 1e8e  ..^.Y..7........
-00003590: b91e a1cd e47f 336d ae05 63e6 9658 e33b  ......3m..c..X.;
-000035a0: baec 5c2e 77a8 f354 278b 1993 2104 8480  ..\.w..T'...!...
-000035b0: 1010 0242 4008 0801 2120 0484 8010 1002  ...B@...! ......
-000035c0: 4240 0808 8171 083c 0000 00ff ff03 0050  B@...q.<.......P
-000035d0: 4b03 0414 0006 0008 0000 0021 00fa 5660  K..........!..V`
-000035e0: d383 0500 00d4 1b00 0027 0000 0078 6c2f  .........'...xl/
-000035f0: 7072 696e 7465 7253 6574 7469 6e67 732f  printerSettings/
-00003600: 7072 696e 7465 7253 6574 7469 6e67 7332  printerSettings2
-00003610: 2e62 696e 8a61 8861 2860 2862 c864 c863  .bin.a.a(`(b.d.c
-00003620: 2861 d063 2805 423d 203b 0728 ee04 2413  (a.c(.B= ;.(..$.
-00003630: 1992 19b2 1970 0346 1666 b63b 0c3f a482  .....p.F.f.;.?..
-00003640: ff37 3032 3270 32cc e236 e148 6160 64e0  .7022p2..6.Ha`d.
-00003650: 6788 6062 6260 0293 8c0c 8e0c 2678 cc20  g.`bb`......&x. 
-00003660: 558a 11aa 8105 4833 0131 8c8f 6e4e 4090  U.....H3.1..nN@.
-00003670: 67d8 2301 2a5a 0c35 4a02 4c0b a883 2003  g.#.*Z.5J.L... .
-00003680: 0308 43c0 0186 2dcc b86c 8349 b888 0b30  ..C...-..l.I...0
-00003690: 0498 3033 6874 805c 0f01 8c58 7cb0 c0c4  ..03ht.\...X|...
-000036a0: 8399 1528 fd9f 810f 8819 1910 aaa9 ef9f  ...(............
-000036b0: 5113 076f 08e0 4adb b85c 7c00 2811 ec1b  Q..o..J..\|.(...
-000036c0: e205 9217 60d8 c010 c190 0acc ddf9 0c15  ....`...........
-000036d0: 0c0a 0cee 0c01 0c2e 403a 8021 1848 8631  ........@:.!.H.1
-000036e0: 1803 733a 049b 3098 03d9 6640 6c00 d4e7  ..s:..0...f@l...
-000036f0: 939a 9892 9997 ee9a 929e cac0 1090 989e  ................
-00003700: 1a9c 5995 cae0 6802 6607 a5a6 67e6 e731  ..Y...h.f...g..1
-00003710: 30b8 9416 e4a4 5640 29bf fc90 d2dc a49c  0.....V@).......
-00003720: 5486 a0d4 e2fc 9cd2 1290 0a33 0383 0a20  T..........3... 
-00003730: 4e29 c824 2574 5dc4 1918 0cfd 8222 40fe  N).$%t]......"@.
-00003740: e601 b289 059d 8566 f338 80f9 6439 b300  .......f.8..d9..
-00003750: 500b 2303 bbc2 6391 0850 e1c0 e01b ecec  P.#...c..P......
-00003760: 06a2 bba0 5950 076a 2433 b0bc 02d9 6209  ....YP.j$3....b.
-00003770: f472 1058 0f23 c347 3654 fbf4 f543 f392  .r.X.#.G6T...C..
-00003780: f373 0b8a 528b 8b53 5374 5d12 4b12 f5f5  .s..R..SSt].K...
-00003790: 1902 a65d 7f62 c0fc 91cd d97b ee54 6f0f  ...].b.....{.To.
-000037a0: d144 91e3 e76b 8a45 7535 4f6a 4f7d b6f8  .D...k.Eu5OjO}..
-000037b0: d29e a28b 35f1 6b1d de85 9e79 a4b4 7df5  ....5.k....y..}.
-000037c0: 04bd 33be 795d 9f02 b97d b92e bb7e 3359  ..3.y]...}...~3Y
-000037d0: 31d5 3684 83ab 6ac7 8a35 1ccc c6e6 b66b  1.6...j..5.....k
-000037e0: 54d6 f4dc da91 3151 618b 0647 cfb9 99ff  T.....1Qa..G....
-000037f0: cfcc 3d18 656a f4fd ffec ffe5 cf6a eecf  ..=.ej.......j..
-00003800: b1fc fc92 ffca 9573 3b5f 8b7e 7cc8 ff86  .......s;_.~|...
-00003810: e317 f3c3 8435 c7c4 4f77 562d 3aca cd1e  .....5..OwV-:...
-00003820: ca16 af5d e4bb 7c53 c5cc d249 1c53 99ab  ...]..|S...I.S..
-00003830: 9395 bcf5 2cdc 7730 fcd1 e85d 2a10 a35e  ....,.w0...]*..^
-00003840: 27b8 c373 8760 cce4 939b da2d a7a5 f016  '..s.`.....-....
-00003850: bd5a c297 b8a1 ccd4 bbdd 70be ccaa cbc7  .Z........p.....
-00003860: 94cd ca14 7784 37f5 5bfd 98d1 bc5b b6e6  ....w.7.[....[..
-00003870: cec1 bd7c 760f 1fd8 b1cf 2ff9 90f9 e18f  ...|v...../.....
-00003880: d434 e36f 42e7 6e55 9c3b 56c7 f2fd 44ef  .4.oB.nU.;V...D.
-00003890: f3c0 8b15 4eae 8b39 937f ab5c 6cad ef3f  ....N..9...\l..?
-000038a0: 7bea 866a f362 9353 caa5 92fb b265 4f8b  {..j.b.S.....eO.
-000038b0: 1644 729d 0e2d d8f5 c3f9 d897 eaa3 926d  .Dr..-.........m
-000038c0: 6fa7 4e78 7e4c e456 5931 5768 df46 c64a  o.Nx~L.VY1Wh.F.J
-000038d0: 61fd 141f e5f5 c555 7dbe db92 764f 11dc  a......U}...vO..
-000038e0: 9ddd 7c65 62a5 e4bc 3ca9 4439 ed37 7d3f  ..|eb...<.D9.7}?
-000038f0: 8b26 47b8 9df9 72e8 f103 d773 cbef 35af  .&G...r....s..5.
-00003900: 4e5d 2a3f 6371 84fd a16a 9dd3 7f58 f2a6  N]*?cq...j...X..
-00003910: 7c5c ff80 f361 fcb1 e09f 4722 5be6 ea3c  |\...a....G"[..<
-00003920: fc38 eba0 62e6 6991 0fdf 4ba6 85f8 0665  .8..b.i...K....e
-00003930: 6b05 6fbe 1f33 adb9 f6c1 dc4b f397 ce5a  k.o..3.....K...Z
-00003940: e217 713e 6299 6b5c 2cf3 62ef 048f c35a  ..q>b.k\,.b....Z
-00003950: edbe b2a6 c1f6 065f 17ae 34f6 b09c 71e0  ......._..4...q.
-00003960: 53a4 b196 f036 ade4 30ad 84d8 f8c3 a593  S....6..0.......
-00003970: 4a6b bb15 db9c 5cef fcd8 cefb e5cb 4e8f  Jk....\.......N.
-00003980: bb07 9ad3 d6c4 069d d73f 11b7 55a5 fae4  .........?..U...
-00003990: ff74 ffd0 4f1b 3a43 fccf 5ef1 d3bd e2f8  .t..O.:C..^.....
-000039a0: 72cb ecad 73bf 05b3 56b3 bf34 2836 de6d  r...s...V..4(6.m
-000039b0: a7b5 34e9 5f70 e631 5dbd 554b a2b8 0299  ..4._p.1].UK....
-000039c0: 5796 88de 143d c476 6db5 e5f6 55a1 13bb  W....=.vm...U...
-000039d0: aecd 2c2f 0960 bc2f a872 b565 9bd7 946d  ..,/.`./.r.e...m
-000039e0: 598c e55c dba5 1ae3 e6a9 4ee7 5ad9 f1fc  Y..\......N.Z...
-000039f0: cc52 21bb cf2b dac2 030e cc3a 5fa7 f7ff  .R!..+.....:_...
-00003a00: 99f4 fea3 5ba6 fef5 8acb ecd8 26d1 a25a  ....[.......&..Z
-00003a10: f9ef d404 ff9b 4bfc 1257 a9ef 59ba d2b1  ......K..W..Y...
-00003a20: a0ef 8da3 73c2 fc0f 1b36 d9df 59fe c0ec  ....s....6..Y...
-00003a30: a3fa d4c0 a8d7 cea1 e70d aea9 26af 3f20  ............&.? 
-00003a40: deba fc00 f3a1 fb53 625f b07e e8f9 6168  .......Sb_.~..ah
-00003a50: 25a5 156a be67 91af 4ee6 03af 8732 77df  %..j.g..N....2w.
-00003a60: 5dcc 2a98 fde3 fad9 df6e 0fce a66f bcc3  ].*......n...o..
-00003a70: 5a7e 42e6 fb81 ee47 f7d9 ff8b c9b1 9efe  Z~B....G........
-00003a80: beea d881 c243 8fd3 f671 5668 1f99 7de5  .....C...qVh..}.
-00003a90: ecbb 7ace e2d9 3382 1f14 3dbc 9eb0 ff83  ..z...3...=.....
-00003aa0: 7441 eb87 e8cf 8c2d f511 9e75 511b 3a2e  tA.....-...uQ.:.
-00003ab0: 6a99 7b4f e2ce bfaf 3d7f 19b7 f787 03b7  j.{O....=.......
-00003ac0: 75e2 b669 5ffa b8d1 eadb 71ae d56f fe74  u..i_.....q..o.t
-00003ad0: 7e56 53f9 efc3 d7f3 f377 be59 0aab d88e  ~VS......w.Y....
-00003ae0: 8f4b be3f 8999 c93a f570 fabc bc7b 8abb  .K.?...:.p...{..
-00003af0: 1ea7 856f 7df5 fe8b 3dd3 7f20 6060 60fb  ...o}...=.. ```.
-00003b00: e8ec ef6b cac4 2004 2c9a 2a80 cd8b 5460  ...k.. .,.*...T`
-00003b10: 3343 0fcc 4e05 5673 7cc0 62c8 8cc1 90c1  3C..N.Vs|.b.....
-00003b20: 0248 5a30 9832 f040 ab3e 1106 19a0 28a4  .HZ0.2.@.>....(.
-00003b30: 88d2 0336 272c 198c c085 9621 b0c8 0241  ...6',.....!...A
-00003b40: 31b0 bc31 508d 1e50 c610 4c1b 0255 1900  1..1P..P..L..U..
-00003b50: f916 409e 38d0 9c8b 35ce ec12 a355 2929  ..@.8...5....U))
-00003b60: e5f1 a8da d110 180d 81d1 1018 0d81 d110  ................
-00003b70: 180d 81d1 1018 0d81 d110 180d 81d1 1018  ................
-00003b80: 0d81 d110 180d 81d1 1018 0d81 c117 0200  ................
-00003b90: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00003ba0: 0000 0021 009a 47b4 c45b 0100 007b 0200  ...!..G..[...{..
-00003bb0: 0011 0008 0164 6f63 5072 6f70 732f 636f  .....docProps/co
-00003bc0: 7265 2e78 6d6c 20a2 0401 28a0 0001 0000  re.xml ...(.....
-00003bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003cc0: 0000 0000 0000 0000 0000 0000 0000 7c92  ..............|.
-00003cd0: 5f4f 8330 14c5 df4d fc0e a44f 9a08 a56c  _O.0...M...O...l
-00003ce0: 73ae 0196 f867 0f8b 8b26 6234 be35 eddd  s....g...&b4.5..
-00003cf0: 8683 42da 2adb b7b7 c086 98a9 8fed 39f7  ..B.*.........9.
-00003d00: d773 6e1a 4eb7 79e6 7c82 d269 2123 443c  .sn.N.y.|..i!#D<
-00003d10: 1f39 2079 2152 b98a d073 3273 af90 a30d  .9 y!R...s2s....
-00003d20: 9382 6585 8408 ed40 a369 7c7a 12f2 92f2  ..e....@.i|z....
-00003d30: 42c1 a32a 4a50 2605 ed58 92d4 9497 115a  B..*JP&..X.....Z
-00003d40: 1b53 528c 355f 43ce b467 1dd2 8acb 42e5  .SR.5_C..g....B.
-00003d50: ccd8 a35a e192 f10d 5b01 0e7c ff12 e760  ...Z....[..|...`
-00003d60: 9860 86e1 1ae8 961d 11ed 9182 77c8 f243  .`..........w..C
-00003d70: 650d 4070 0c19 e420 8dc6 c423 f8db 6b40  e.@p... ...#..k@
-00003d80: e5fa d781 46e9 39f3 d4ec 4adb 691f b7cf  ....F.9...J.i...
-00003d90: 16bc 153b f756 a79d b1aa 2aaf 1a34 316c  ...;.V....*..41l
-00003da0: 7e82 5f17 f74f 4d55 3795 f5ae 38a0 3814  ~._..OMU7...8.8.
-00003db0: 9c72 05cc 142a 7e10 e9fb e6c2 997b 77de  .r...*~......{w.
-00003dc0: dc5b 78ce d99c c9f3 10f7 1cf5 3633 a6cd  .[x.........63..
-00003dd0: c22e 7e99 82b8 defd 3574 6cb4 2f35 c5da  ..~.....5tl./5..
-00003de0: e740 3836 2a6d 8b1d 9497 c1cd 6d32 4371  .@86*m......m2Cq
-00003df0: e093 89eb 4fdc 2048 c890 fa63 ea0f dfea  ....O. H...c....
-00003e00: 1c3f e6eb e8ed 45be 4ff3 2f31 18b8 fec8  .?....E.O./1....
-00003e10: 0dc6 0921 948c 2819 f788 0740 1ce2 a3ef  ...!..(....@....
-00003e20: 127f 0100 00ff ff03 0050 4b03 0414 0006  .........PK.....
-00003e30: 0008 0000 0021 008b 9767 eb98 0100 0044  .....!...g.....D
-00003e40: 0300 0010 0008 0164 6f63 5072 6f70 732f  .......docProps/
-00003e50: 6170 702e 786d 6c20 a204 0128 a000 0100  app.xml ...(....
-00003e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f50: 0000 0000 0000 0000 0000 0000 0000 009c  ................
-00003f60: 9341 8bdb 3010 85ef 85fe 07a3 fb46 4e5a  .A..0........FNZ
-00003f70: 9612 642d 25db b287 9606 e2dd 3dab f238  ..d-%.......=..8
-00003f80: 162b 4b42 336b 92fe fa4a 36eb 38ed a1d0  .+KB3k...J6.8...
-00003f90: dbcc bcc7 d3e7 912c ee4e bd2d 0688 68bc  .......,.N.-..h.
-00003fa0: abd8 7a55 b202 9cf6 8d71 c78a 3dd6 5f6f  ..zU.....q..=._o
-00003fb0: 3eb1 0249 b946 59ef a062 6740 7627 dfbf  >..I.FY..bg@v'..
-00003fc0: 13fb e803 4432 8045 8a70 58b1 8e28 6c39  ....D2.E.pX..(l9
-00003fd0: 47dd 41af 7095 6497 94d6 c75e 516a e391  G.A.p.d....^Qj..
-00003fe0: fbb6 351a eebd 7eed c111 df94 e52d 8713  ..5...~......-..
-00003ff0: 816b a0b9 0973 209b 12b7 03fd 6f68 e375  .k...s .....oh.u
-00004000: e6c3 a7fa 1c12 b014 b527 656b d383 2c05  .........'ek..,.
-00004010: bf34 e273 08d6 6845 e9eb e577 a3a3 47df  .4.s..hE...w..G.
-00004020: 52f1 e5a4 c10a be14 45a2 3e80 7e8d 86ce  R.......E.>.~...
-00004030: 3963 d98a 8356 1676 e940 d92a 8b20 f865  9c...V.v.@.*. .e
-00004040: 201e 40e5 65ee 9589 28c5 40db 0134 f958   .@.e...(.@..4.X
-00004050: a0f9 95d6 b961 c54f 8590 312b 36a8 6894  .....a.O..1+6.h.
-00004060: a384 9b6d 5333 d636 2045 f9ec e30b 7600  ...mS3.6 E....v.
-00004070: 8482 27c3 341c cba5 7759 9b8f 7233 1a52  ..'.4...wY..r3.R
-00004080: 716d cc01 1348 12ae 116b 4316 f047 bb57  qm...H...kC..G.W
-00004090: 91fe 453c 324c bc13 ce21 f3ad 977c 33e9  ..E<2L...!...|3.
-000040a0: 284d 384b f471 1b09 e28f 6377 be0f ca9d  (M8K.q....cw....
-000040b0: 9330 57df 8c7b c1c7 50fb 7b45 f0b6 e9eb  .0W..{..P.{E....
-000040c0: a138 742a 4293 2e67 be89 7920 1ed2 92a3  .8t*B..g..y ....
-000040d0: cd21 bb4e b923 346f 9ebf 85fc 2e9e a69f  .!.N.#4o........
-000040e0: 42ae 6f57 e587 325d f962 26f8 e5f9 cbdf  B.oW..2].b&.....
-000040f0: 0000 00ff ff03 0050 4b01 022d 0014 0006  .......PK..-....
-00004100: 0008 0000 0021 0021 8c46 3a73 0100 008c  .....!.!.F:s....
-00004110: 0500 0013 0000 0000 0000 0000 0000 0000  ................
-00004120: 0000 0000 005b 436f 6e74 656e 745f 5479  .....[Content_Ty
-00004130: 7065 735d 2e78 6d6c 504b 0102 2d00 1400  pes].xmlPK..-...
-00004140: 0600 0800 0000 2100 b555 3023 f400 0000  ......!..U0#....
-00004150: 4c02 0000 0b00 0000 0000 0000 0000 0000  L...............
-00004160: 0000 ac03 0000 5f72 656c 732f 2e72 656c  ......_rels/.rel
-00004170: 7350 4b01 022d 0014 0006 0008 0000 0021  sPK..-.........!
-00004180: 00db 46c4 2dba 0300 000e 0900 000f 0000  ..F.-...........
-00004190: 0000 0000 0000 0000 0000 00d1 0600 0078  ...............x
-000041a0: 6c2f 776f 726b 626f 6f6b 2e78 6d6c 504b  l/workbook.xmlPK
-000041b0: 0102 2d00 1400 0600 0800 0000 2100 4aa9  ..-.........!.J.
-000041c0: a661 fa00 0000 4703 0000 1a00 0000 0000  .a....G.........
-000041d0: 0000 0000 0000 0000 b80a 0000 786c 2f5f  ............xl/_
-000041e0: 7265 6c73 2f77 6f72 6b62 6f6f 6b2e 786d  rels/workbook.xm
-000041f0: 6c2e 7265 6c73 504b 0102 2d00 1400 0600  l.relsPK..-.....
-00004200: 0800 0000 2100 dd19 99f8 1c0d 0000 844f  ....!..........O
-00004210: 0000 1800 0000 0000 0000 0000 0000 0000  ................
-00004220: f20c 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-00004230: 732f 7368 6565 7431 2e78 6d6c 504b 0102  s/sheet1.xmlPK..
-00004240: 2d00 1400 0600 0800 0000 2100 b163 99a9  -.........!..c..
-00004250: e804 0000 c610 0000 1800 0000 0000 0000  ................
-00004260: 0000 0000 0000 441a 0000 786c 2f77 6f72  ......D...xl/wor
-00004270: 6b73 6865 6574 732f 7368 6565 7432 2e78  ksheets/sheet2.x
-00004280: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-00004290: 2100 c117 10be 4e07 0000 c620 0000 1300  !.....N.... ....
-000042a0: 0000 0000 0000 0000 0000 0000 621f 0000  ............b...
-000042b0: 786c 2f74 6865 6d65 2f74 6865 6d65 312e  xl/theme/theme1.
-000042c0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-000042d0: 0021 0040 b3d4 95e4 0300 0012 1100 000d  .!.@............
-000042e0: 0000 0000 0000 0000 0000 0000 00e1 2600  ..............&.
-000042f0: 0078 6c2f 7374 796c 6573 2e78 6d6c 504b  .xl/styles.xmlPK
-00004300: 0102 2d00 1400 0600 0800 0000 2100 fcff  ..-.........!...
-00004310: 017b a806 0000 8318 0000 1400 0000 0000  .{..............
-00004320: 0000 0000 0000 0000 f02a 0000 786c 2f73  .........*..xl/s
-00004330: 6861 7265 6453 7472 696e 6773 2e78 6d6c  haredStrings.xml
-00004340: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00004350: 3b6d 324b c100 0000 4201 0000 2300 0000  ;m2K....B...#...
-00004360: 0000 0000 0000 0000 0000 ca31 0000 786c  ...........1..xl
-00004370: 2f77 6f72 6b73 6865 6574 732f 5f72 656c  /worksheets/_rel
-00004380: 732f 7368 6565 7431 2e78 6d6c 2e72 656c  s/sheet1.xml.rel
-00004390: 7350 4b01 022d 0014 0006 0008 0000 0021  sPK..-.........!
-000043a0: 0013 c42c 13c2 0000 0042 0100 0023 0000  ...,.....B...#..
-000043b0: 0000 0000 0000 0000 0000 00cc 3200 0078  ............2..x
-000043c0: 6c2f 776f 726b 7368 6565 7473 2f5f 7265  l/worksheets/_re
-000043d0: 6c73 2f73 6865 6574 322e 786d 6c2e 7265  ls/sheet2.xml.re
-000043e0: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
-000043f0: 2100 ae0b fd89 bb01 0000 2c15 0000 2700  !.........,...'.
-00004400: 0000 0000 0000 0000 0000 0000 cf33 0000  .............3..
-00004410: 786c 2f70 7269 6e74 6572 5365 7474 696e  xl/printerSettin
-00004420: 6773 2f70 7269 6e74 6572 5365 7474 696e  gs/printerSettin
-00004430: 6773 312e 6269 6e50 4b01 022d 0014 0006  gs1.binPK..-....
-00004440: 0008 0000 0021 00fa 5660 d383 0500 00d4  .....!..V`......
-00004450: 1b00 0027 0000 0000 0000 0000 0000 0000  ...'............
-00004460: 00cf 3500 0078 6c2f 7072 696e 7465 7253  ..5..xl/printerS
-00004470: 6574 7469 6e67 732f 7072 696e 7465 7253  ettings/printerS
-00004480: 6574 7469 6e67 7332 2e62 696e 504b 0102  ettings2.binPK..
-00004490: 2d00 1400 0600 0800 0000 2100 9a47 b4c4  -.........!..G..
-000044a0: 5b01 0000 7b02 0000 1100 0000 0000 0000  [...{...........
-000044b0: 0000 0000 0000 973b 0000 646f 6350 726f  .......;..docPro
-000044c0: 7073 2f63 6f72 652e 786d 6c50 4b01 022d  ps/core.xmlPK..-
-000044d0: 0014 0006 0008 0000 0021 008b 9767 eb98  .........!...g..
-000044e0: 0100 0044 0300 0010 0000 0000 0000 0000  ...D............
-000044f0: 0000 0000 0029 3e00 0064 6f63 5072 6f70  .....)>..docProp
-00004500: 732f 6170 702e 786d 6c50 4b05 0600 0000  s/app.xmlPK.....
-00004510: 000f 000f 0012 0400 00f7 4000 0000 00    ..........@....
+000006d0: 0050 4b03 0414 0006 0008 0000 0021 004a  .PK..........!.J
+000006e0: a9a6 61fa 0000 0047 0300 001a 0008 0178  ..a....G.......x
+000006f0: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
+00000700: 2e78 6d6c 2e72 656c 7320 a204 0128 a000  .xml.rels ...(..
+00000710: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000007f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000810: 00bc 92cd 6ac4 300c 84ef 85be 83d1 bd71  ....j.0........q
+00000820: 92fe 50ca 3a7b 2985 bdb6 db07 30b1 1287  ..P.:{).....0...
+00000830: 4d6c 63a9 3f79 fb9a 94ee 36b0 a497 d0a3  Mlc.?y....6.....
+00000840: 2434 f331 cc66 fb39 f4e2 1d23 75de 2928  $4.1.f.9...#u.)(
+00000850: b21c 04ba da9b ceb5 0a5e f74f 57f7 2088  .........^.OW. .
+00000860: b533 baf7 0e15 8c48 b0ad 2e2f 36cf d86b  .3.....H.../6..k
+00000870: 4e4f 64bb 4022 a938 5260 99c3 8394 545b  NOd.@".8R`....T[
+00000880: 1c34 653e a04b 97c6 c741 731a 632b 83ae  .4e>.K...As.c+..
+00000890: 0fba 4559 e6f9 9d8c bf35 a09a 698a 9d51  ..EY.....5..i..Q
+000008a0: 1077 e61a c47e 0cc9 f96f 6ddf 345d 8d8f  .w...~...om.4]..
+000008b0: be7e 1bd0 f119 0bc9 890b 93a0 8e2d b282  .~...........-..
+000008c0: 69fc 5e16 5902 0579 9ea1 5c93 e1c3 c703  i.^.Y..y..\.....
+000008d0: 5944 3e71 1c57 24a7 4bb9 0453 fc33 cc62  YD>q.W$.K..S.3.b
+000008e0: 32b7 6bc2 90d5 11cd 0bc7 543e 3aa5 335b  2.k.......T>:.3[
+000008f0: 2f25 73b3 2a0c 8f7d eafa b12b 34cd 3ff6  /%s.*..}...+4.?.
+00000900: 7256 ffea 0b00 00ff ff03 0050 4b03 0414  rV.........PK...
+00000910: 0006 0008 0000 0021 00a9 fa2f 40ae 0300  .......!.../@...
+00000920: 0007 0900 000f 0000 0078 6c2f 776f 726b  .........xl/work
+00000930: 626f 6f6b 2e78 6d6c ac55 5d6f e238 147d  book.xml.U]o.8.}
+00000940: 5f69 ff43 d6ea 6bea 3824 01a2 c2a8 24a0  _i.C..k.8$....$.
+00000950: ad34 1d55 fd9a 4764 1243 ac26 71d6 760a  .4.U..Gd.C.&q.v.
+00000960: d568 fefb 5e27 2485 6134 623b 8bc0 8e3f  .h..^'$.a4b;...?
+00000970: 383e e7fa dc9b ab4f bb22 b75e 9954 5c94  8>.....O.".^.T\.
+00000980: 1344 2e1d 64b1 3211 292f 3713 f4f4 b8b0  .D..d.2.)/7.....
+00000990: 47c8 529a 9629 cd45 c926 e88d 29f4 69fa  G.R..).E.&..).i.
+000009a0: e71f 575b 215f 5642 bc58 0050 aa09 cab4  ..W[!_VB.X.P....
+000009b0: ae42 8c55 92b1 82aa 4b51 b112 56d6 4216  .B.U....KQ..V.B.
+000009c0: 54c3 506e b0aa 24a3 a9ca 18d3 458e 5dc7  T.Pn..$.....E.].
+000009d0: 0970 4179 895a 8450 9e83 21d6 6b9e b058  .pAy.Z.P..!.k..X
+000009e0: 2475 c14a dd82 4896 530d f455 c62b d5a1  $u.J..H.S..U.+..
+000009f0: 15c9 3970 0595 2f75 6527 a2a8 0062 c573  ..9p../ue'...b.s
+00000a00: aedf 1a50 6415 4978 b329 85a4 ab1c 64ef  ...Pd.Ix.)....d.
+00000a10: 886f ed24 7c03 f811 071a b73b 0996 4e8e  .o.$|......;..N.
+00000a20: 2a78 2285 126b 7d09 d0b8 257d a29f 3898  *x"..k}...%}..8.
+00000a30: 90a3 10ec 4e63 701e 9287 257b e5e6 0e7b  ....Ncp...%{...{
+00000a40: 5632 f820 aba0 c70a dec1 88f3 db68 04ac  V2. .........h..
+00000a50: d578 2584 e07d 10cd efb9 b968 7ab5 e639  .x%..}.....hz..9
+00000a60: 7b6e ad6b d1aa fa42 0b73 5339 b272 aaf4  {n.k...B.sS9.r..
+00000a70: 3ce5 9aa5 1334 84a1 d8b2 a309 5957 b39a  <....4......YW..
+00000a80: e7b0 4a88 e38e 109e f676 be93 56ca d6b4  ..J......v..V...
+00000a90: cef5 2318 b983 878d 4130 767d b313 8c71  ..#.....A0v}...q
+00000aa0: 9d6b 264b aa59 244a 0d3e dceb fa5d cf35  .k&K.Y$J.>...].5
+00000ab0: d851 26c0 e1d6 3dfb a7e6 9241 6281 bf40  .Q&...=....Ab..@
+00000ac0: 2bb4 3409 e94a dd51 9d59 b5cc 2708 3f29  +.4..J.Q.Y..'.?)
+00000ad0: 108f e9c0 f546 be1b e00d d758 8172 9ab2  .....F.....X.r..
+00000ae0: d765 4593 17ba 6158 c9a4 9fc4 29d5 1417  .eE...aX....)...
+00000af0: 4c67 2255 f8c0 bff4 3459 fe83 8369 62c2  Lg"U....4Y...ib.
+00000b00: 8221 2e2d f7f6 f9c7 1881 0419 762e bdd3  .!.-........v...
+00000b10: d282 e79b f833 f07d a0af 706f e08e 749f  .....3.}..po..t.
+00000b20: d637 e662 06cb 3291 2159 7e8b fdc8 0b88  .7.b..2.!Y~.....
+00000b30: 1bd9 736f 3cb4 a3a1 e7db d751 ecda b301  ..so<......Q....
+00000b40: 99cf 67f1 200a a2f1 7710 2383 3011 b4d6  ..g. ...w.#.0...
+00000b50: d9de 1206 7a82 3cb8 ff93 a55b baeb 5688  ....z.<....[..V.
+00000b60: 13d6 3c7d a7f1 cdd9 7f6c d3ff d074 6bdf  ..<}.....l...tk.
+00000b70: 8d60 53fc 9e39 dbaa 77f3 98a1 b5fb cacb  .`S..9..w.......
+00000b80: 546c 1b45 6fdd b3ef 80be 6db3 f095 a73a  Tl.Eo.....m....:
+00000b90: 9ba0 81e3 7afd dcdf 8c6f 3260 4bc6 8199  ....z....o2`K...
+00000ba0: 8404 31ac 26e8 884d dcb2 59c0 c736 cd11  ..1.&..M..Y..6..
+00000bb0: 1b7c 40a7 29b1 40ab e9ad b249 8b07 5376  .|@.).@....I..Sv
+00000bc0: 09d4 72d3 3701 4696 0ccd 19f2 2625 46cf  ..r.7.F.....&%F.
+00000bd0: c96e a870 fd6e 78ee 77bb cd75 7787 40b6  .n.p.nx.w..uw.@.
+00000be0: f092 a526 f9e0 c883 d1fe e0e5 2e2f 8bcb  ...&........./..
+00000bf0: e582 9b9c 89c1 802b aa98 c9c9 84e6 0d29  .......+.......)
+00000c00: 4306 3467 3c4d 9979 05a1 69cb f5af 8beb  C.4g<M.y..i.....
+00000c10: 0b12 5e3c 5d10 6f74 850f 80c1 5fc7 8702  ..^<].ot...._...
+00000c20: 5202 796b ba46 d918 927a 6c48 b29d feac  R.yk.F...zlH....
+00000c30: 74d3 43ca 7088 27f1 9ceb a133 f66c 673e  t.C.p.'....3.lg>
+00000c40: f06d 6f34 76ed 9137 70ed c88b ddb9 3f9c  .mo4v..7p.....?.
+00000c50: c7f3 996f cc64 de69 e1ff 51d9 9bcc 0dbb  ...o.d.i..Q.....
+00000c60: 97a5 6199 51a9 1f25 a427 bc62 efd9 7a06  ..a.Q..%.'.b..z.
+00000c70: e130 aa4d 0a01 df43 b233 7f34 7306 40d1  .0.M...C.3.4s.@.
+00000c80: 5b90 85ed 91b1 63cf 6681 67fb f162 e00f  [.....c.f.g..b..
+00000c90: 491c cdfd c53b 5923 7ffd c1ba 3ac2 cdbf  I....;Y#....:...
+00000ca0: 19d5 35d4 1c53 6e9a 7168 dac5 7eb6 9f5c  ..5..Sn.qh..~..\
+00000cb0: b713 fbfb 3d2a 14e1 7d6c 84ec fffd ab8d  ....=*..}l......
+00000cc0: 0fa0 3e67 676e 5e3c 9fb9 31fa 72fb 78db  ..>ggn^<..1.r.x.
+00000cd0: 84f2 a702 da00 9bb6 b105 eeae 65fa 2f00  ............e./.
+00000ce0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00000cf0: 0000 2100 d543 1936 c503 0000 d00e 0000  ..!..C.6........
+00000d00: 0d00 0000 786c 2f73 7479 6c65 732e 786d  ....xl/styles.xm
+00000d10: 6cd4 57cb 6edb 3814 dd17 987f 20b8 57f4  l.W.n.8..... .W.
+00000d20: b0e4 5a86 a4a2 8e23 a040 1b14 4806 982d  ..Z....#.@..H..-
+00000d30: 2d53 3651 8ad4 5074 22cf a0ff de4b 3d6c  -S6Q..Pt"....K=l
+00000d40: 3971 d2c4 4e81 7691 98bc 22cf 3df7 4932  9q..N.v...".=.I2
+00000d50: fa50 171c dd51 5531 2962 ec5e 3818 5191  .P...QU1)b.^8.Q.
+00000d60: c925 13ab 18ff 7d9b 5a13 8c2a 4dc4 9270  .%....}.Z..*M..p
+00000d70: 2968 8cb7 b4c2 1f92 bfde 4595 de72 7ab3  )h........E..rz.
+00000d80: a654 2380 1055 8cd7 5a97 53db aeb2 352d  .T#..U..Z.S...5-
+00000d90: 4875 214b 2ae0 4b2e 5541 344c d5ca ae4a  Hu!K*.K.UA4L...J
+00000da0: 45c9 b232 9b0a 6e7b 8e33 b60b c204 6e11  E..2..n{.3....n.
+00000db0: a645 f612 9082 a86f 9bd2 ca64 5112 cd16  .E.....o...dQ...
+00000dc0: 8c33 bd6d b030 2ab2 e9a7 9590 8a2c 3850  .3.m.0*......,8P
+00000dd0: ad5d 9f64 a876 c7ca 43b5 ea95 34d2 477a  .].d.v..C...4.Gz
+00000de0: 0a96 2959 c95c 5f00 ae2d f39c 65f4 31dd  ..)Y.\_..-..e.1.
+00000df0: d00e 6d92 ed91 00f9 3424 37b0 1def c0f6  ..m.....4$7.....
+00000e00: 5a9d 88e4 db8a de31 133e 9c44 b914 ba42  Z......1.>.D...B
+00000e10: 99dc 081d 631f 881a 174c bf09 792f 52f3  ....c....L..y/R.
+00000e20: 0922 dcad 4aa2 ea3f 7447 3848 5c6c 2751  ."..J..?tG8H\l'Q
+00000e30: 26b9 5448 43e8 c073 8d44 9082 b62b 2e09  &.THC..s.D...+..
+00000e40: 670b c5cc b29c 148c 6f5b b167 044d b4bb  g.......o[.g.M..
+00000e50: 7505 03df 1ba1 6d78 b46c 9268 6156 fd9e  u.....mx.l.haV..
+00000e60: bae4 4631 aad0 35bd 7f68 dbe8 9119 af30  ..F1..5..h.....0
+00000e70: e165 b08d 932a f012 e37c 1733 cf84 0704  .e...*...|.3....
+00000e80: 4904 c9ad a912 294c 5037 bedd 9610 1c01  I.....)LP7......
+00000e90: 75d8 b26b d6fd 64f5 4a91 adeb 0583 0d76  u..k..d.J......v
+00000ea0: a310 e222 d512 ea7e 9f2d bd28 8938 cd35  ..."...~.-.(.8.5
+00000eb0: 444d b1d5 dafc 6a59 c2ff 85d4 1a6a 2389  DM....jY.....j#.
+00000ec0: 968c aca4 20dc 04ba 0539 be13 fa06 b488  .... ....9......
+00000ed0: 18eb 3594 f883 0c0b 31d2 cc24 a973 310a  ..5.....1..$.s1.
+00000ee0: c3f0 7d10 4c02 37f4 7cf8 6b92 cf6e 7437  ..}.L.7.|.k..nt7
+00000ef0: aacf 8201 ea3d f3b3 705a e37f 6efb 594a  .....=..pZ..n.YJ
+00000f00: 8cdb 0fbc fe47 997e 9830 bf3d f52e 75a1  .....G.~.0.=..u.
+00000f10: 0033 caf9 8d49 d57f f25d 3598 3659 e748  .3...I...]5.6Y.H
+00000f20: 6c8a b4d0 9f96 90a7 1899 a6d6 0fa1 f4ba  l...............
+00000f30: 615b 01ed c454 c410 adc5 1ec2 9afa 7e3d  a[...T........~=
+00000f40: 2eaa f39d 8283 dd3e d451 4fcb 85e1 715a  .......>.QO...qZ
+00000f50: bbed 8894 25df 5e6f 8a05 5569 732e 9b5e  ....%.^o..Uis..^
+00000f60: df4a cdf9 d075 fe27 5518 279c a402 1cf3  .J...u.'U.'.....
+00000f70: 6a50 0f8e afce ece7 78cf 9a36 762a f3d1  jP......x..6v*..
+00000f80: 5b2a 01c6 bf3a 02c0 f72d 54b4 0efd c8d9  [*...:...-T.....
+00000f90: 4a14 b48d 7b12 c129 df4e d1bd 22e5 2dad  J...{..).N..".-.
+00000fa0: fb7c b0eb fc99 f8bd 11a5 e752 e429 1590  .|.........R.)..
+00000fb0: bb2f 4991 3eb5 5bab f709 73ae 175e d413  ./I.>.[...s..^..
+00000fc0: 1e30 7cd2 e770 07d7 2c33 17b2 0c22 42db  .0|..p..,3..."B.
+00000fd0: 7bd4 23c7 bf52 e5bf 1ba9 e957 4573 561f  {.#..R.....WEsV.
+00000fe0: ab90 3735 e058 d234 dd10 fadf a0c9 1eb4  ..75.X.4........
+00000ff0: d85d b344 e6b6 19e3 6bd3 94f8 20aa 8b0d  .].D....k... ...
+00001000: e370 5138 d25e 0173 59ef 1bb6 636e 38da  .pQ8.^.sY...cn8.
+00001010: 5cfc 9b56 bed3 0226 2e69 4e36 5cdf ee3e  \..V...&.iN6\..>
+00001020: c678 3ffe 4297 6c53 40e5 76ab beb2 3ba9  .x?.B.lS@.v...;.
+00001030: 1b88 18ef c79f cd4d c81d 1b1d 5016 9f2b  .......M....P..+
+00001040: 38a6 e117 c1f5 31c6 ff5f cdde 87f3 abd4  8.....1.._......
+00001050: b326 ce6c 62f9 231a 5861 309b 5b81 7f39  .&.lb.#.Xa0.[..9
+00001060: 9bcf d3d0 f19c cbef 83e7 c719 8f8f e6b5  ................
+00001070: 04b5 e8fa d38a c313 4575 c676 e46f f6b2  ........Eu.v.o..
+00001080: 180f 262d fde6 0e08 b487 dc43 6fec 7c0c  ..&-.......Co.|.
+00001090: 5cc7 4a47 8e6b f963 32b1 26e3 5160 a581  \.JG.k.c2.&.Q`..
+000010a0: ebcd c7fe ec2a 4883 01f7 e0c4 478a 63bb  .....*H.....G.c.
+000010b0: 6efb dc31 e483 a966 05e5 4cf4 b1ea 2334  n..1...f..L...#4
+000010c0: 9442 9060 fa8c 1176 1f09 7bff 144d 7e00  .B.`...v..{..M~.
+000010d0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+000010e0: 0000 2100 927a 24c4 ae06 0000 9a18 0000  ..!..z$.........
+000010f0: 1400 0000 786c 2f73 6861 7265 6453 7472  ....xl/sharedStr
+00001100: 696e 6773 2e78 6d6c 9419 5d4f dc38 f01d  ings.xml..]O.8..
+00001110: 89ff e0b3 8400 e9ca b270 4b7b 88a5 14ee  .........pK{....
+00001120: 4095 50db 132d 2f27 84bc c9b0 1b48 ec34  @.P..-/'.....H.4
+00001130: f126 855f 7f63 2721 89c7 c9b5 3c91 19cf  .&._.c'!....<...
+00001140: 7866 3cdf 7bf2 fe47 12b3 02b2 3c52 72ce  xf<.{..G....<Rr.
+00001150: a77b fb9c 810c 5418 c9e5 9c7f fb7a f9e6  .{....T......z..
+00001160: 1d67 b916 3214 b192 30e7 cf90 f3f7 a79b  .g..2...0.......
+00001170: 1b27 79ae 19d2 ca7c ce57 5aa7 c793 491e  .'y....|.WZ...I.
+00001180: ac20 11f9 9e4a 4122 e641 6589 d0f8 992d  . ...JA".Ae....-
+00001190: 2779 9a81 08f3 1580 4ee2 c9c1 fefe d124  'y......N......$
+000011a0: 1191 e42c 506b a9e7 fce0 ed8c b3b5 8cbe  ...,Pk..........
+000011b0: afe1 a282 4c67 47fc f424 8f4e 4ff4 e947  ....LgG..$.NO..G
+000011c0: 0dc9 c944 9f9e 4ccc 7705 4bc5 1272 1778  ...D..L.w.K..r.x
+000011d0: 2134 2c55 f6ec c26f d68b 4068 177a 2972  !4,U...o..@h.z)r
+000011e0: 7061 ffac 8192 5fa8 2401 a9c9 75b7 172e  pa...._.$...u...
+000011f0: f9c7 bf5c c835 1410 bb40 11eb 0875 220c  ...\.5...@...u".
+00001200: a324 8d23 aad6 e72c 5a46 5210 36b2 6421  .$.#...,ZFR.6.d!
+00001210: 003e 1f5b c28b 7bc7 5906 f11c cd1e 067e  .>.[..{.Y......~
+00001220: 0c01 2f20 ddb3 ac72 0d71 b882 2824 62cb  ../ ...r.q..($b.
+00001230: 909d a57a ce64 3a84 12e1 23b9 0e29 16a5  ...z.d:...#..)..
+00001240: 9720 920f 958c 5eac 5120 5144 0a62 f45b  . ....^.Q QD.b.[
+00001250: 973a 8e1e 4340 590b a5b2 1232 22ac 358d  .:..C@Y....2".5.
+00001260: 5a3c 4e5d c204 00cf 3ffd 0ced 814f 64a9  Z<N]....?....Od.
+00001270: f44e 2a32 f495 e363 a942 f8f7 0cdd 6ebe  .N*2...c.B....n.
+00001280: 9da6 db77 bbbe f3fe b30c a38d 5919 51fb  ...w........Y.Q.
+00001290: 3b97 ce28 f502 3a87 7848 bdc9 a4ba dbd8  ;..(..:.xH......
+000012a0: 8f1b 35f9 e606 c33f c3d6 2f21 4f53 7eb7  ..5....?../!OS~.
+000012b0: 4bae 6a18 1925 cc91 96cd 8e15 8fa7 410d  K.j..%........A.
+000012c0: 33ec 5556 09cd e390 ef76 6f34 7668 65b9  3.UV.....vo4vhe.
+000012d0: 7351 e81e bc78 e177 83d7 37b4 07f5 6578  sQ...x.w..7...ex
+000012e0: 517d 7f47 b946 416a d256 7273 a639 5749  Q}.G.FAj.Vrs.9WI
+000012f0: 8406 1e51 bcd1 d204 914f 5154 bfa3 e88e  ...Q.....OQT....
+00001300: 7d6c 2e1b 3bd5 36d9 3111 c365 87be 3196  }l..;.6.1..e..1.
+00001310: 555c 967c 77d0 f203 0258 ff30 d418 6dfc  U\.|w....X.0..m.
+00001320: 5789 7b4f d56a d0d8 c5a7 c5a8 2644 9bea  W.{O.j......&D..
+00001330: 7d1b 5bdb c77a 95b5 36d7 e80b 8eb9 68c5  }.[..z..6.....h.
+00001340: bb47 de78 c5ab 90ae db77 5ffd 67bc c3e7  .G.x.....w_.g...
+00001350: 215d b9fb d1d0 dacd dedb 8b88 9ea9 dba8  !]..............
+00001360: 6848 dc28 ad23 a38f 6ea2 c3e3 2437 fbfb  hH.(.#..n...$7..
+00001370: 2483 218c 6426 841d ba59 0461 7f78 6033  $.!.d&...Y.a.x`3
+00001380: 0fec c803 7beb 81bd f3c0 fea4 b0e9 be07  ....{...........
+00001390: e6d1 634a f490 584a 2536 19d1 d313 7627  ..cJ..XJ%6....v'
+000013a0: 2e17 2543 ec62 86b0 29e2 9492 7981 4d09  ..%C.b..)...y.M.
+000013b0: 4897 3617 08c4 7ec2 143e 534b 6119 92ce  H.6...~..>SKa...
+000013c0: 007b a418 b0ac 308d d585 26e5 582b 1585  .{....0...&.X+..
+000013d0: b61e 9798 a1c9 0929 4462 11f4 f645 f458  .......)Db...E.X
+000013e0: 2858 62d5 7a02 8655 58c4 a81e 3df6 02f1  (Xb.z..UX...=...
+000013f0: 83ed c4a2 25d8 d2d6 61c9 0e81 d52a baa2  ....%...a....*..
+00001400: 21f7 ea5e 973f 2b84 6469 2cb0 47fb 351a  !..^.?+.di,.G.5.
+00001410: 9f01 149a c7c8 3578 9b7b c58c b8c1 8c38  ......5x.{.....8
+00001420: c18c b8c0 8c38 f28c b8f1 8c38 f18c b8f0  .....8.....8....
+00001430: 8c38 e611 91a7 a97e 6961 14c6 1a85 0ec0  .8.....~ia......
+00001440: 078b 5469 3c0b 0f61 3d21 ce21 b248 2c20  ..Ti<..a=!.!.H, 
+00001450: 0676 4054 2c5a 1c51 b683 236a 7770 c400  .v@T,Z.Q..#jwp..
+00001460: 1d1c 3145 0747 8cd2 c191 f8ee e048 9c77  ..1E.G.......H.w
+00001470: 70c4 ac2d ee90 18b8 831b b1cb 21b1 cbf9  p..-........!...
+00001480: 3953 ae8d bf90 26f0 96b4 e29f 48e2 b9ba  9S....&.....H...
+00001490: 7241 9f6e 5c08 de46 2687 cfe4 d4ed 5742  rA.n\..F&.....WB
+000014a0: 777b 0ea4 f344 6604 56c5 f55e 21cb 3d97  w{...Df.V..^!.=.
+000014b0: c73a d236 15b0 179b dd58 5ab0 1273 0b26  .:.6.....XZ..s.&
+000014c0: 2111 e7ec cd14 7355 1ef8 b20d b127 8e6d  !.....sU.....'.m
+000014d0: 2ef3 40e1 b401 3f70 1089 8882 2625 6126  ..@...?p....&%a&
+000014e0: 2279 32c8 00a4 27f9 6223 8fee ef1e af35  "y2...'.b#.....5
+000014f0: 6346 b5df 5b35 eb7f 11ea 12a4 990a 20f7  cF..[5........ .
+00001500: 489a 9174 7cb3 3f1d 098a 4382 d34a 0b11  H..t|.?...C..J..
+00001510: 0fe5 2722 88ca 894d f046 4fc9 9c7a 4ae6  ..'"...M.FO..zJ.
+00001520: 7424 b4c6 3280 2bc5 1292 280c b126 018b  t$..2.+...(..&..
+00001530: b13e 694c fb59 f408 ac72 8bff 3f3d 63b1  .>iL.Y...r..?=c.
+00001540: 904b ac6a 3d3a 5a59 aeae 6fbf b9dc aeae  .K.j=:ZY..o.....
+00001550: 671e e881 2718 ef2b d3fa e246 f98c e8e9  g...'..+...F....
+00001560: 1da6 2339 65e4 9547 321f 7915 88e3 28d5  ..#9e..G2.y...(.
+00001570: 91d9 51e0 20a4 074a b18c 40bf 2962 0511  ..Q. ..J..@.)b..
+00001580: ce80 be11 5849 b32b 4157 920b 9cf3 ea97  ....XI.+AW......
+00001590: a016 fdfb 0349 2cc8 f9b6 66ec e23e 574c  .....I,...f..>WL
+000015a0: bfd1 38ec 48fd 6154 e886 f588 ccc8 ded7  ..8.H.aT........
+000015b0: 5798 25ce 719e 8a00 973b b82e c821 2b80  W.%.q....;...!+.
+000015c0: 9fbe 16bf ceec d26b e5ab 2135 5539 7245  .......k..!5U9rE
+000015d0: 4aa9 9266 167a 3da6 4bfe 3aca fe36 e721  J..f.z=.K.:..6.!
+000015e0: e8de 11db 4727 e59a efd6 93a9 9913 9121  ....G'.........!
+000015f0: 32c3 760c e741 865b 2667 eb53 8b85 f35f  2.v..A.[&g.S..._
+00001600: 0c49 22e6 1c70 8764 06cf fa33 1122 eb01  .I"..p.d...3."..
+00001610: 4a7c eb1e 403d f43e c375 5edf df8e 2d3b  J|..@=.>.u^...-;
+00001620: f5d8 1564 61a5 c0de 5e67 a2de 0ee4 e3b6  ...da...^g......
+00001630: 95b8 1e95 f26a 9365 a4b0 2a05 6975 83fd  .....j.e..*.iu..
+00001640: c0a1 a0f3 95e7 eb45 f7b3 9876 beca d5f7  .......E...v....
+00001650: f60b 75e7 e5aa 4f5d ae0c f9ee dd2e 6adc  ..u...O]......j.
+00001660: 91b6 9a64 436c 1a9f 7094 dcdc d8dc 186a  ...dCl..p......j
+00001670: 52d8 9684 f2fe e6eb 872f f7e7 e7f7 7a8b  R......../....z.
+00001680: fddc c174 f860 8fa1 da1a e2b7 55d7 1372  ...t.`......U..r
+00001690: 60dc f9ea 9e2a 2d38 8e46 8e2b 8c53 da59  `....*-8.F.+.S.Y
+000016a0: 6c55 3fdf 59cb c7be dbab ed7a efca 8bc0  lU?.Y......z....
+000016b0: be76 7f7c 65e8 6af6 21b1 c2d9 d771 d1f6  .v.|e.j.!....q..
+000016c0: d1d9 9c71 1d19 fc00 1a77 1022 ab1c 919e  ...q.....w."....
+000016d0: 3023 5e59 3a0b 029c 02eb a1b3 995f 196b  0#^Y:........_.k
+000016e0: 0744 6a8f 5ec4 6269 ad3c d75c 2671 2975  .Dj.^.bi.<.\&q)u
+000016f0: 5694 fa39 c538 5dc0 4be5 ef95 18b8 9ca8  V..9.8].K.......
+00001700: 06a3 393f 6cb7 2b1d 60b3 cc30 dedd 1e4d  ..9?l.+.`..0...M
+00001710: bc67 0b2f 54f5 9741 288b 8d71 1136 c77b  .g./T..A(..q.6.{
+00001720: 53b2 4d12 c48d b0f4 92ce d2d7 7024 e209  S.M.........p$..
+00001730: 8738 91fa 7097 d8a0 b89d c5a8 13d5 0f6f  .8..p..........o
+00001740: c2b9 da9c 35fb 3c6e c3f8 aedd 0954 1e52  ....5.<n.....T.R
+00001750: 85eb eb86 a201 9a98 ed03 19b7 71dd ee32  ............q..2
+00001760: da55 61cd baf5 9166 1588 f973 a1c2 678e  .Ua....f...s..g.
+00001770: 79a1 bbcf 30b1 8f28 4c49 0318 2d96 0318  y...0..(LI..-...
+00001780: b90e 624c 2634 c7a2 0133 d282 3d44 b186  ..bL&4...3..=D..
+00001790: cc4d c7b6 83f7 2cc6 d772 9d43 485a 9d0a  .M....,..r.CHZ..
+000017a0: 4c5a 886b 6c41 b3ee 767b 82bf 2d9c fe07  LZ.klA..v{..-...
+000017b0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+000017c0: 0000 2100 13c4 2c13 c200 0000 4201 0000  ..!...,.....B...
+000017d0: 2300 0000 786c 2f77 6f72 6b73 6865 6574  #...xl/worksheet
+000017e0: 732f 5f72 656c 732f 7368 6565 7432 2e78  s/_rels/sheet2.x
+000017f0: 6d6c 2e72 656c 7384 8fc1 6ac3 3010 44ef  ml.rels...j.0.D.
+00001800: 85fc 83d8 7b24 3b87 508a 255f 4a21 d726  ....{$;.P.%_J!.&
+00001810: fd00 455e dba2 f64a 68b7 25f9 fbe8 d884  ..E^...Jh.%.....
+00001820: 428e c363 de30 5d7f 5917 f58b 8563 220b  B..c.0].Y....c".
+00001830: ad6e 4021 8534 449a 2c7c 9d3e b6af a058  .n@!.4D.,|.>...X
+00001840: 3c0d 7e49 8416 aec8 d0bb cd4b f789 8b97  <.~I.......K....
+00001850: 5ae2 3966 56d5 426c 6116 c96f c670 9871  Z.9fV.Bla..o.p.q
+00001860: f5ac 5346 aa64 4c65 f552 6399 4cf6 e1db  ..SF.dLe.Rc.L...
+00001870: 4f68 764d b337 e5af 03dc 9d53 1d06 0be5  OhvM.7.....S....
+00001880: 30b4 a04e d75c 979f bbd3 38c6 80ef 29fc  0..N.\....8...).
+00001890: ac48 f2cf 84c9 2592 6039 a248 3dc8 55ed  .H....%.`9.H=.U.
+000018a0: cb84 6241 eb47 f698 77fa 1c09 8ceb ccdd  ..bA.G..w.......
+000018b0: 7377 0300 00ff ff03 0050 4b03 0414 0006  sw.......PK.....
+000018c0: 0008 0000 0021 00c1 1710 be4e 0700 00c6  .....!.....N....
+000018d0: 2000 0013 0000 0078 6c2f 7468 656d 652f   ......xl/theme/
+000018e0: 7468 656d 6531 2e78 6d6c ec59 cd8b 1b37  theme1.xml.Y...7
+000018f0: 14bf 17fa 3f0c 7377 fc35 e38f 25de e0cf  ....?.sw.5..%...
+00001900: 6c93 dd24 649d 941c b5b6 ec51 5633 3292  l..$d......QV32.
+00001910: bc1b 1302 2539 f552 28a4 a597 426f 3d94  ....%9.R(...Bo=.
+00001920: d240 030d bdf4 8f09 24b4 e91f d127 cdd8  .@......$....'..
+00001930: 23ad e524 9b6c 4a5a 760d 8b47 febd a7a7  #..$.lJZv..G....
+00001940: f79e 7e7a f374 f1d2 bd98 7a47 980b c292  ..~z.t....zG....
+00001950: 965f be50 f23d 9c8c d898 24d3 967f 6b38  ._.P.=....$...k8
+00001960: 2834 7c4f 4894 8c11 6509 6ef9 0b2c fc4b  (4|OH...e.n..,.K
+00001970: db9f 7e72 116d c908 c7d8 03f9 446c a196  ..~r.m......Dl..
+00001980: 1f49 39db 2a16 c508 8691 b8c0 6638 81df  .I9.*.......f8..
+00001990: 268c c748 c223 9f16 c71c 1d83 de98 162b  &..H.#.........+
+000019a0: a552 ad18 2392 f85e 8262 507b 7d32 2123  .R..#..^.bP{}2!#
+000019b0: ec0d 954a 7f7b a9bc 4fe1 3191 420d 8c28  ...J.{..O.1.B..(
+000019c0: df57 aab1 25a1 b1e3 c3b2 4288 85e8 52ee  .W..%.....B...R.
+000019d0: 1d21 daf2 619e 313b 1ee2 7bd2 f728 1212  .!..a.1;..{..(..
+000019e0: 7e68 f925 fde7 17b7 2f16 d156 2644 e506  ~h.%..../..V&D..
+000019f0: 5943 6ea0 ff32 b94c 607c 58d1 73f2 e9c1  YCn..2.L`|X.s...
+00001a00: 6ad2 2008 835a 7ba5 5f03 a85c c7f5 ebfd  j. ..Z{._..\....
+00001a10: 5abf b6d2 a701 6834 8295 a6b6 d83a eb95  Z.....h4.....:..
+00001a20: 6e90 610d 50fa d5a1 bb57 ef55 cb16 ded0  n.a.P....W.U....
+00001a30: 5f5d b3b9 1daa 8f85 d7a0 547f b086 1f0c  _]........T.....
+00001a40: bae0 450b af41 293e 5cc3 879d 66a7 67eb  ..E..A)>\...f.g.
+00001a50: d7a0 145f 5bc3 d74b ed5e 50b7 f46b 5044  ..._[..K.^P..kPD
+00001a60: 4972 b886 2e85 b56a 77b9 da15 64c2 e88e  Ir.....jw...d...
+00001a70: 13de 0c83 41bd 9229 cf51 900d abec 5253  ....A..).Q....RS
+00001a80: 4c58 2237 e55a 8cee 323e 0080 0252 2449  LX"7.Z..2>...R$I
+00001a90: e2c9 c50c 4fd0 08b2 b88b 2839 e0c4 db25  ....O.....(9...%
+00001aa0: d308 126f 8612 2660 b854 290d 4a55 f8af  ...o..&`.T).JU..
+00001ab0: 3e81 fea6 238a b630 32a4 955d 6089 581b  >...#..02..]`.X.
+00001ac0: 52f6 7862 c4c9 4cb6 fc2b a0d5 3720 2f9e  R.xb..L..+..7 /.
+00001ad0: 3d7b fef0 e9f3 87bf 3d7f f4e8 f9c3 5fb2  ={......=....._.
+00001ae0: b9b5 2a4b 6e07 2553 53ee d58f 5fff fdfd  ..*Kn.%SS..._...
+00001af0: 17de 5fbf fef0 eaf1 37e9 d427 f1c2 c4bf  .._.....7..'....
+00001b00: fcf9 cb97 bfff f13a f5b0 e2dc 152f be7d  .......:...../.}
+00001b10: f2f2 e993 17df 7df5 e74f 8f1d dadb 1c1d  ......}..O......
+00001b20: 98f0 2189 b1f0 aee1 63ef 268b 6181 0efb  ..!.....c.&.a...
+00001b30: f101 3f9d c430 42c4 9240 11e8 76a8 eecb  ..?..0B..@..v...
+00001b40: c802 5e5b 20ea c275 b0ed c2db 1c58 c605  ..^[ ..u.....X..
+00001b50: bc3c bf6b d9ba 1ff1 b924 8e99 af46 b105  .<.k.....$...F..
+00001b60: dc63 8c76 1877 3ae0 aa9a cbf0 f070 9e4c  .c.v.w:......p.L
+00001b70: dd93 f3b9 89bb 89d0 916b ee2e 4aac 00f7  .........k..J...
+00001b80: e733 a057 e252 d98d b065 e60d 8a12 89a6  .3.W.R...e......
+00001b90: 38c1 d253 bfb1 438c 1dab bb43 88e5 d73d  8..S..C....C...=
+00001ba0: 32e2 4cb0 89f4 ee10 af83 88d3 2543 7260  2.L.........%Cr`
+00001bb0: 2552 2eb4 4362 88cb c265 2084 daf2 cdde  %R..Cb...e .....
+00001bc0: 6daf c3a8 6bd5 3d7c 6423 615b 20ea 307e  m...k.=|d#a[ .0~
+00001bd0: 88a9 e5c6 cb68 2e51 ec52 3944 3135 1dbe  .....h.Q.R9D15..
+00001be0: 8b64 e432 727f c147 26ae 2f24 447a 8a29  .d.2r..G&./$Dz.)
+00001bf0: f3fa 632c 844b e63a 87f5 1a41 bf0a 0ce3  ..c,.K.:...A....
+00001c00: 0efb 1e5d c436 924b 72e8 d2b9 8b18 3391  ...].6.Kr.....3.
+00001c10: 3d76 d88d 503c 73da 4c92 c8c4 7e26 0e21  =v..P<s.L...~&.!
+00001c20: 4591 7783 4917 7c8f d93b 443d 431c 50b2  E.w.I.|..;D=C.P.
+00001c30: 31dc b709 b6c2 fd66 22b8 05e4 6a9a 9427  1......f"...j..'
+00001c40: 88fa 65ce 1db1 bc8c 99bd 1f17 7482 b08b  ..e.........t...
+00001c50: 65da 3cb6 d8b5 cd89 333b 3af3 a995 dabb  e.<.....3;:.....
+00001c60: 1853 748c c618 7bb7 3e73 58d0 6133 cbe7  .St...{.>sX.a3..
+00001c70: b9d1 5722 6095 1dec 4aac 2bc8 ce55 f59c  ..W"`...J.+..U..
+00001c80: 6001 6592 aa6b d629 7297 082b 65f7 f194  `.e..k.)r..+e...
+00001c90: 6db0 676f 7182 7816 2889 11df a4f9 1a44  m.goq.x.(......D
+00001ca0: dd4a 5d38 e59c 547a 9d8e 0e4d e035 02e5  .J]8..Tz...M.5..
+00001cb0: 1fe4 8bd3 29d7 05e8 3092 bbbf 49eb 8d08  ....)...0...I...
+00001cc0: 5967 977a 16ee 7c5d 702b 7e6f b3c7 605f  Yg.z..|]p+~o..`_
+00001cd0: de3d edbe 0419 7c6a 1920 f6b7 f6cd 1051  .=....|j. .....Q
+00001ce0: 6b82 3c61 8608 0a0c 17dd 8288 15fe 5c44  k.<a..........\D
+00001cf0: 9dab 5a6c ee94 9bd8 9b36 0f03 1446 56bd  ..Zl.....6...FV.
+00001d00: 1393 e48d c5cf 89b2 27fc 77ca 1e77 0173  ........'.w..w.s
+00001d10: 0605 8f5b f1fb 943a 9b28 65e7 4481 b309  ...[...:.(e.D...
+00001d20: f71f 2c6b 7a68 9edc c070 92ac 73d6 7955  ..,kzh...p..s.yU
+00001d30: 735e d5f8 fffb aa66 d35e 3eaf 65ce 6b99  s^.....f.^>.e.k.
+00001d40: f35a c6f5 f6f5 416a 99bc 7c81 ca26 eff2  .Z....Aj..|..&..
+00001d50: e89e 4fbc b1e5 3321 94ee cb05 c5bb 4277  ..O...3!......Bw
+00001d60: 7d04 bcd1 8c07 30a8 db51 ba27 b96a 01ce  }.....0..Q.'.j..
+00001d70: 22f8 9a35 982c dc94 232d e371 263f 2732  "..5.,..#-.q&?'2
+00001d80: da8f d00c 5a43 65dd c09c 8a4c f554 7833  ....ZCe....L.Tx3
+00001d90: 26a0 63a4 8775 2b15 9fd0 adfb 4ef3 788f  &.c..u+.....N.x.
+00001da0: 8dd3 4e67 b9ac ba9a a90b 0592 f978 295c  ..Ng.........x)\
+00001db0: 8d43 974a a6e8 5a3d efde add4 eb7e e854  .C.J..Z=.....~.T
+00001dc0: 7759 9706 28d9 d318 614c 661b 5175 1851  wY..(...aLf.Qu.Q
+00001dd0: 5f0e 4214 5e67 845e d999 58d1 7458 d150  _.B.^g.^..X.tX.P
+00001de0: ea97 a15a 4671 e50a 306d 1515 78e5 f6e0  ...ZFq..0m..x...
+00001df0: 45bd e587 41da 4186 661c 94e7 6315 a7b4  E...A.A.f...c...
+00001e00: 99bc 8cae 0ace 9946 7a93 33a9 9901 5062  .......Fz.3...Pb
+00001e10: 2f33 208f 7453 d9ba 7179 6a75 69aa bd45  /3 .tS..qyjui..E
+00001e20: a42d 238c 74b3 8d30 d230 8217 e12c 3bcd  .-#.t..0.0...,;.
+00001e30: 96fb 59c6 ba99 87d4 324f b962 b91b 7233  ..Y.....2O.b..r3
+00001e40: ea8d 0f11 6b45 2227 b881 2626 53d0 c43b  ....kE"'..&&S..;
+00001e50: 6ef9 b56a 08b7 2a23 346b f913 e818 c3d7  n..j..*#4k......
+00001e60: 7806 b923 d45b 17a2 53b8 7619 499e 6ef8  x..#.[..S.v.I.n.
+00001e70: 7761 9619 17b2 8744 943a 5c93 4eca 0631  wa.....D.:\.N..1
+00001e80: 9198 7b94 c42d 5f2d 7f95 0d34 d11c a26d  ..{..-_-...4...m
+00001e90: 2b57 8010 3e5a e39a 402b 1f9b 7110 743b  +W..>Z..@+..q.t;
+00001ea0: c878 32c1 2369 86dd 1851 9e4e 1f81 e153  .x2.#i...Q.N...S
+00001eb0: ae70 feaa c5df 1dac 24d9 1cc2 bd1f 8d8f  .p......$.......
+00001ec0: bd03 3ae7 3711 a458 582f 2b07 8e89 808b  ..:.7..XX/+.....
+00001ed0: 8372 eacd 3181 9bb0 1591 e5f9 77e2 60ca  .r..1.......w.`.
+00001ee0: 68d7 bc8a d239 948e 233a 8b50 76a2 9864  h....9..#:.Pv..d
+00001ef0: 9ec2 3589 aecc d14f 2b1f 184f d99a c1a1  ..5....O+..O....
+00001f00: eb2e 3c98 aa03 f6bd 4fdd 371f d5ca 7306  ..<.....O.7...s.
+00001f10: 69e6 67a6 c52a ead4 7493 e987 3be4 0dab  i.g..*..t...;...
+00001f20: f243 d4b2 2aa5 6efd 4e2d 72ae 6b2e b90e  .C..*.n.N-r.k...
+00001f30: 12d5 794a bce1 d47d 8b03 c130 2d9f cc32  ..yJ...}...0-..2
+00001f40: 4d59 bc4e c38a b3b3 51db b433 2c08 0c4f  MY.N....Q..3,..O
+00001f50: d436 f86d 7546 383d f1ae 273f c89d cc5a  .6.muF8=..'?...Z
+00001f60: 7540 2ceb 4a9d f8fa cadc bcd5 6607 7781  u@,.J.......f.w.
+00001f70: 3c7a 707f 38a7 52e8 5042 6f97 2328 fad2  <zp.8.R.PBo.#(..
+00001f80: 1bc8 9436 608b dc93 598d 08df bc39 272d  ...6`...Y....9'-
+00001f90: ff7e 296c 07dd 4ad8 2d94 1a61 bf10 5483  .~)l..J.-..a..T.
+00001fa0: 52a1 11b6 ab85 7618 56cb fdb0 5cea 752a  R.....v.V...\.u*
+00001fb0: 0fe0 6091 515c 0ed3 ebfa 015c 61d0 4576  ..`.Q\.....\a.Ev
+00001fc0: 69af c7d7 2eee e3e5 2dcd 8511 8b8b 4c5f  i.......-.....L_
+00001fd0: cc17 b5e1 fae2 be5c d97c 71ef 1120 9dfb  .......\.|q.. ..
+00001fe0: b5ca a059 6d76 6a85 66b5 3d28 04bd 4ea3  ...Ymvj.f.=(..N.
+00001ff0: d0ec d63a 855e ad5b ef0d 7add b0d1 1c3c  ...:.^.[..z....<
+00002000: f0bd 230d 0eda d56e 50eb 370a b572 b75b  ..#....nP.7..r.[
+00002010: 086a 2565 7ea3 59a8 0795 4a3b a8b7 1bfd  .j%e~.Y...J;....
+00002020: a0fd 202b 6360 e529 7d64 be00 f76a bbb6  .. +c`.)}d...j..
+00002030: ff01 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+00002040: 0800 0000 2100 3b6d 324b c100 0000 4201  ....!.;m2K....B.
+00002050: 0000 2300 0000 786c 2f77 6f72 6b73 6865  ..#...xl/workshe
+00002060: 6574 732f 5f72 656c 732f 7368 6565 7431  ets/_rels/sheet1
+00002070: 2e78 6d6c 2e72 656c 7384 8fc1 8ac2 3014  .xml.rels.....0.
+00002080: 45f7 03fe 4378 7b93 d685 0c43 5337 22b8  E...Cx{....CS7".
+00002090: 55e7 0362 fada 06db 9790 f714 fd7b b31c  U..b.........{..
+000020a0: 65c0 e5e5 70cf e536 9bfb 3ca9 1b66 0e91  e...p..6..<..f..
+000020b0: 2cd4 ba02 85e4 6317 68b0 f07b da2d bf41  ,.....c.h..{.-.A
+000020c0: b138 eadc 1409 2d3c 9061 d32e be9a 034e  .8....-<.a.....N
+000020d0: 4e4a 89c7 9058 150b b185 5124 fd18 c37e  NJ...X....Q$...~
+000020e0: c4d9 b18e 09a9 903e e6d9 4989 7930 c9f9  .......>..I.y0..
+000020f0: 8b1b d0ac aa6a 6df2 5f07 b42f 4eb5 ef2c  .....jm._../N..,
+00002100: e47d 5783 3a3d 5259 feec 8e7d 1f3c 6ea3  .}W.:=RY...}.<n.
+00002110: bfce 48f2 cf84 4939 9060 3ea2 4839 c845  ..H...I9.`>.H9.E
+00002120: edf2 8062 41eb 77f6 9e6b 7d0e 04a6 6dcc  ...bA.w..k}...m.
+00002130: cbf3 f609 0000 ffff 0300 504b 0304 1400  ..........PK....
+00002140: 0600 0800 0000 2100 406b a56b 7e0c 0000  ......!.@k.k~...
+00002150: e54d 0000 1800 0000 786c 2f77 6f72 6b73  .M......xl/works
+00002160: 6865 6574 732f 7368 6565 7431 2e78 6d6c  heets/sheet1.xml
+00002170: 9c54 5d6f da30 147d 9fb4 ff60 f9bd 240e  .T]o.0.}...`..$.
+00002180: 34a3 88b4 aa5a a175 9aa6 aa5d b767 e3dc  4....Z.u...].g..
+00002190: 80d5 24ce 6c53 a0d3 fefb ae9d 2fba 7e2c  ..$.lS....../.~,
+000021a0: 2a82 d838 39e7 9e7b eebd 999f ed8a 9c3c  *..89..{.......<
+000021b0: 8036 5295 0965 a390 1228 854a 65b9 4ae8  .6R..e...(.Je.J.
+000021c0: ddf7 c5d1 9412 6379 99f2 5c95 90d0 3d18  ......cy..\...=.
+000021d0: 7a76 faf1 c37c abf4 bd59 0358 820c a549  zv...|...Y.X...I
+000021e0: e8da da6a 1604 46ac a1e0 66a4 2a28 f14e  ...j..F...f.*(.N
+000021f0: a674 c12d fed5 abc0 541a 78ea 4145 1e44  .t.-....T.x.AE.D
+00002200: 6118 0705 9725 ad19 667a 0887 ca32 29e0  a....%..fz...2).
+00002210: 5289 4d01 a5ad 4934 e4dc a27e b396 9569  R.M...I4...~...i
+00002220: d90a 3184 aee0 fa7e 531d 0955 5448 b194  ..1....~S..UTH..
+00002230: b9b4 7b4f 4a49 2166 57ab 5269 becc 31ef  ..{OJI!fW.Ri..1.
+00002240: 1d9b 7041 761a bf11 fec6 6d18 7ffe 2c52  ..pAv.....m...,R
+00002250: 2185 5646 6576 84cc 41ad f979 fa27 c149  !.VFev..A..y.'.I
+00002260: c045 c7f4 3cff 4134 6c12 6878 90ae 803d  .E..<.A4l.hx...=
+00002270: 55f4 3e49 ecb8 e38a 7ab2 f13b c9e2 8ecc  U.>I....z..;....
+00002280: d9a5 671b 9926 f477 d87c 8e70 65ee 12f6  ..g..&.w.|.pe...
+00002290: 97f6 de1f 7a3a 4f25 56d8 6545 3464 093d  ....z:O%V.eE4d.=
+000022a0: 67b3 3b36 99d2 e074 ee3b e887 84ad 39d8  g.;6...t.;....9.
+000022b0: 13cb 97b7 9083 b080 5118 258f 4a15 b782  ........Q.%.J...
+000022c0: e7f0 cdb5 608e 6721 36b7 6bdb a552 f70e  ....`.g!6.k..R..
+000022d0: 7e85 0f86 18a9 e225 90dd 6d85 c54f e831  ~......%..m..O.1
+000022e0: 25fb 668b 2456 555f 21b3 1790 23c1 17f4  %.f.$VU_!...#...
+000022f0: 840b 2b1f e01a 1109 5d2a 6b55 7123 576b  ..+.....]*kUq#Wk
+00002300: eb87 c4e2 59a6 d523 945e a517 e3f4 3bfe  ....Y..#.^....;.
+00002310: 8422 55f3 68cd 5173 2e30 88f9 e533 c4ad  ."U.h.Qs.0...3..
+00002320: 4bee 1f58 1dc4 8968 83d7 c073 14d3 0071  K..X...h...s...q
+00002330: fb2a f085 90d7 588d 0689 5b44 069d a187  .*....X...[D....
+00002340: fbd6 dc85 9fe0 6b4d 96dc c085 ca7f cad4  ......kM........
+00002350: ae9d 9b94 a490 f14d 6efb c3e9 683a 8ec2  .......Mn...h:..
+00002360: 318b d0c5 e6e6 8dda 7e06 6711 42f0 d4cf  1.......~.g.B...
+00002370: cb2c dd5f 8211 38c0 5880 9157 2f54 8e01  .,._..8.X..W/T..
+00002380: f14a 0ae9 5e44 387f 7ce7 d76d 1def 90da  .J..^D8.|..m....
+00002390: d8bd 9bc9 1658 43d0 0f0f c1b5 81b0 e988  .....XC.........
+000023a0: c593 3076 6a3a 0811 1b83 556b b370 f977  ..0vj:....Uk.p.w
+000023b0: 51d1 184f 31e9 2986 42f1 390f c5b5 893e  Q..O1.).B.9....>
+000023c0: 0947 4fc0 4b30 76e1 3a0c 737b 4343 dc10  .GO.K0v.:.s{CC..
+000023d0: 7dea 88c6 d181 ab83 f2c0 77b6 1783 6b6b  }.........w...kk
+000023e0: 45fc 54cc 1b02 4e1a 30ae 2dd8 b55a 6b39  E.T...N.0.-..Zk9
+000023f0: 1998 87eb 8fba 846e eada 9e79 9725 aceb  .......n...y.%..
+00002400: 06dc 3454 313b a042 afde 4888 b565 8d7a  ..4T1;.B..H..e.z
+00002410: 25ff efa6 3666 d4c7 64f1 8b85 1868 48d4  %...6f..d....hH.
+00002420: 3628 8bc7 d3be c35e 5312 f889 f80b 0000  6(.....^S.......
+00002430: ffff 0000 00ff ff94 9ceb 6edb 4610 855f  ..........n.F.._
+00002440: c5d0 03d4 5ade 15d8 062a 29ae 2293 ec35  ....Z....*)."..5
+00002450: 0f60 b806 f227 4911 bb69 fbf6 2597 92c5  .`...'I..i..%...
+00002460: 3d73 86bb f3a7 6885 4f47 c39d 33b3 cb21  =s....h.OG..3..!
+00002470: dd9b 974f cfcf affb c7d7 c7bb 9b6f 5fff  ...O.........o_.
+00002480: b9fa 76bb 72ab ab97 bf1e bfbc 0cff f62e  ..v.r...........
+00002490: 1bff c37f f4f4 f7cb ebd7 cff7 5fbf 7d7e  ............_.}~
+000024a0: 7cf5 1ffc eb8a c7a7 777f feb7 7f7e 797a  |.......w....~yz
+000024b0: fe32 7cb6 fe21 5bdd dd3c 8d12 3fbe 7d6d  .2|..![..<..?.}m
+000024c0: f8fc 65f8 f4fb 5d73 73fd fdee e6fa e944  ..e...]ss......D
+000024d0: 6c25 9185 c44e 1279 48ec 25b1 0989 f792  l%...N.yH.%.....
+000024e0: 5887 c4bd 241c 203f 11c4 852a 0782 c0e5  X...$. ?...*....
+000024f0: 7c20 4828 7294 4411 120f 1351 aeae de96  | H(r.D....Q....
+00002500: b50c 8996 5d0e 44d2 3106 2ea8 670c 44f3  ....].D.1...g.D.
+00002510: 3361 4a88 e717 c6c0 fafe ca18 88e7 37c6  3aJ...........7.
+00002520: c075 fdce 18b0 cc1f 8c81 ebfa 2899 ea6d  .u..........(..m
+00002530: 95af 8722 79ab 940c 2ae5 d358 1945 b1ba  ..."y...*..X.E..
+00002540: 5aac 8df1 5bb7 abe1 9f6f 49cc 6b28 0e89  Z...[....oI.k(..
+00002550: d458 1d12 29c0 fc7b 896c b03e 24d2 0072  .X..)..{.l.>$..r
+00002560: 202a 50cb 1f24 5241 fe8e 4405 2efa 6142   *P..$RA..D...aB
+00002570: aad9 ba38 5c98 361e 4c17 477a 89b8 f5c5  ...8\.6.L.Gz....
+00002580: b841 8a73 96e2 6a1d 49f1 f82d 4831 f63f  .A.s..j.I..-H1.?
+00002590: 89d4 e0d5 9d44 4a28 9dbd 4444 8a09 82dd  .....DJ(..DD....
+000025a0: 8b20 9862 8988 1413 154c f184 0429 46d7  . .b.....L...)F.
+000025b0: b6f1 60ba 38d2 4b44 4df1 50af c17e 3756  ..`.8.KDM.P..~7V
+000025c0: 713e 5864 b188 c72f 4186 a170 b612 a9a1  q>Xd.../A..p....
+000025d0: d3ec 2452 426e f612 1119 9648 036d f840  ..$RBn.....H.m.@
+000025e0: 5430 c312 a9a0 e71c 890a 6678 42c2 0c83  T0........fxB...
+000025f0: 4c1b 0fa6 8b23 bd44 e619 f6c7 908f 4446  L....#.D......DF
+00002600: 69e5 c39e 2a4c e0a2 753e 7e2b 7441 0115  i...*L..u>~+tA..
+00002610: ba95 480d c9d9 49a4 8425 db4b 44b8 4022  ..H...I..%.KD.@"
+00002620: 0da4 f840 54d0 0512 a9a0 2d1d 890a ba60  ...@T.....-....`
+00002630: 4242 1780 4c1b 0fa6 8b23 bd44 d43a 1fc2  BB..L....#.D.:..
+00002640: 0952 bc58 df23 0c99 85ca dc4a a4be 98cb  .R.X.#.....J....
+00002650: fb6f 2791 12cf b012 1199 2508 f8e3 4010  .o'.......%...@.
+00002660: ccac 442a 6847 47a2 8299 9d90 7ab6 49d7  ..D*hGG.....z.I.
+00002670: e0f8 361e 4b17 477a 89a8 891d a249 4fec  ..6.K.Gz.....IO.
+00002680: 0843 6261 31b7 12a9 6119 7612 2961 31f7  .Cba1...a.v.)a1.
+00002690: 1211 8995 4803 0e3a 1015 4cac 442a e830  ....H..:..L.D*.0
+000026a0: 47a2 8289 9d90 20b1 60f8 361e 4b17 477a  G..... .`.6.K.Gz
+000026b0: 89a8 896d 4853 6e62 67af f14b 9060 a8b9  ...mHSnbg..K.`..
+000026c0: ad44 6a58 d49d 44f0 d666 2f11 9160 8934  .DjX..D..f/..`.4
+000026d0: b0ee 07a2 8209 9688 4830 51c1 044f 48d0  ........H0Q..OH.
+000026e0: 9373 705b 1b0f a68b 23bd 44d4 0c6f e8b6  .sp[....#.D..o..
+000026f0: 1b39 7b8d 5f82 0c43 f16d 2552 c3f1 6c27  .9{._..C.m%R..l'
+00002700: 9112 9663 2f11 9161 8280 dbee 25e2 d6d0  ...c/..a....%...
+00002710: 330f 4406 5d20 910a e23d 1215 74c1 8484  3.D.] ...=..t...
+00002720: 3b33 d679 3c98 2e8e f4ec b295 9b2c 37d4  ;3.y<........,7.
+00002730: b43c 7d45 6fa4 fdd7 c008 d0f9 b684 6960  .<}Eo.........i`
+00002740: f177 8429 61dd f684 115e 600c c473 4f18  .w.)a....^`..sO.
+00002750: b706 c71c 9810 da81 3015 047d 643a 6888  ........0..}d:h.
+00002760: 1313 3a02 caa9 4d08 a84b 607a 7af5 9a29  ..:...M..K`zz..)
+00002770: c631 cc7c 0ee9 a72b 439c cb83 c769 7833  .1.|...+C....ix3
+00002780: 9fae 1450 265b 2799 066a 6047 9812 52b0  ...P&['..j`G..R.
+00002790: 278c f484 fcad 0dac ee81 e988 744b 9d0a  '...........tK..
+000027a0: 9823 d311 e99e 74c2 6d00 5a63 9b10 5097  .#....t.m.Zc..P.
+000027b0: c0f4 8451 7702 4787 69d1 7493 3118 0ed3  ...Qw.G.i.t.1...
+000027c0: bc72 d826 1a31 6b96 3a25 8ed3 888e 4c37  .r.&.1k.:%....L7
+000027d0: 993e 61af 673a 22dd 64a4 26d2 9d30 533b  .>a.g:".d.&..0S;
+000027e0: fd56 986e 106a 1302 ea12 989e 307a baf9  .V.n.j......0z..
+000027f0: 602d 56dd 72ac 53c0 d56c 9d64 1a9c ac11  `-V.r.S..l.d....
+00002800: a6c2 d11a 6164 bac9 6f89 ea4e 98ae b178  ....ad..o..N...x
+00002810: c07e 4716 8fa8 6e36 60c3 fb33 2604 8bd8  .~G...n6`..3&...
+00002820: 2530 3d61 f474 b321 9b8b 5637 9bf1 886e  %0=a.t.!..V7...n
+00002830: ce20 bc5f 730c 12fd 3c61 d6c6 8432 f134  . ._s...<a...2.4
+00002840: 2861 dc46 842a 91f2 8481 db49 27a8 f04c  (a.F.*.....I'..L
+00002850: a43c 61e4 4602 dac0 0af5 7419 2f51 0793  .<a.F.....t./Q..
+00002860: 73c7 476a b10a 2703 1d7c 20b7 f5d2 6147  s.Gj..'..| ...aG
+00002870: 774e d438 5382 e3d8 9e28 c922 6742 781b  wN.8S....(."gBx.
+00002880: c784 4453 6742 22e7 09e3 b5d3 8f05 3977  ..DSgB".......9w
+00002890: 1051 9b10 5197 c0f4 6cb1 d75a cec7 a98d  .Q..Q...l..Z....
+000028a0: fdcc 4666 3d0e a76d 63b3 80bb 3ee7 709e  ..Ff=..mc...>.p.
+000028b0: 4e21 bcab 2390 cc39 fb35 c8e7 8109 899c  N!..#..9.5......
+000028c0: 3321 9173 096d 446b 9f98 30e7 6227 2742  3!.s.mDk..0.b''B
+000028d0: a2b5 c799 9ead a39a 731c bf25 3d3f 7164  ........s..%=?qd
+000028e0: 0ce4 7010 c7a0 4ce4 9c28 65e2 f62d 611a  ..p...L..(e..-a.
+000028f0: c77e 2d17 87b7 8481 1cbd 3691 f3f8 4cae  .~-.......6...L.
+00002900: 2542 d892 bb04 a667 01cd d239 3d2b 3941  %B.....g...9=+9A
+00002910: e151 f1d2 54c3 de8e 93b9 e57b 3232 10ca  .Q..T......{22..
+00002920: 44ae 1984 4f4a 1c83 c436 9e30 9863 42b9  D...OJ...6.0.cB.
+00002930: d8c6 1366 734c c889 5cc7 c773 2d11 92b9  ...fsL..\..s-...
+00002940: 4e18 beb1 8064 ae27 a1f9 b4d7 e597 c20a  N....d.'........
+00002950: 73cd 6674 d1e7 a38e 8c7f 329c c352 089f  s.ft......2..R..
+00002960: a150 48dc 9b25 8cea 9850 8e0f 5208 8469  .PH..%...P..R..i
+00002970: f8c0 8464 cee3 c3b8 36e1 c7ba 04a6 6701  ...d....6.....g.
+00002980: c99c 93d1 5fae cc5e 323a 908b 1dd7 fdb7  ...._..^2:......
+00002990: e058 56e0 408e 4250 c2ef 2984 8f46 0884  .XV.@.BP..)..F..
+000029a0: a97a 3831 4153 2bf0 a494 20d4 b388 b41d  .z81AS+... .....
+000029b0: 31c3 9b9d a5ee f8e0 e9db 55b5 ba1e 5e8f  1.........U...^.
+000029c0: 0bde 2ec2 03f4 b2cc f999 ab90 c133 d9b2  .............3..
+000029d0: ccf9 9821 6470 9b5f 9699 7637 7251 969d  ...!dp._..v7rQ..
+000029e0: e321 3b3f b410 d160 535a 8ee6 6c7d 94c9  .!;?...`SZ..l}..
+000029f0: d1e7 8b32 9e66 99ca 7154 b92c 731e c189  ...2.f..qT.,s...
+00002a00: 6870 04b6 2c73 7e5f 4ac8 cc46 2bee dd38  hp..,s~_J..F+..8
+00002a10: 835b d639 cf0c 84ce ccc6 293a e757 3f84  .[.9......):.W?.
+00002a20: cecc c729 3a9a 91f3 9991 5374 3427 e733  ...):.....St4'.3
+00002a30: 27a7 e868 56ce 6756 4ed1 d1bc 9ccf bc9c  '..hV.gVN.......
+00002a40: a2a3 99b9 9899 3941 c7e3 cccd 85cd 3f1e  ......9A......?.
+00002a50: a73a 36ff 8c8f 7b86 1b3c d932 0a9b 7f3c  .:6...{..<.2...<
+00002a60: 4e75 6cfe 2934 ff14 36ff 789c c663 f34f  Nul.)4..6.x..c.O
+00002a70: a1f9 a7b0 f9c7 e32c 9ed2 e61f 8f53 9d59  .......,.....S.Y
+00002a80: 374c f061 a9b5 c372 d60e 5374 b47e 58da  7L.a...r..St.~X.
+00002a90: fcec 717a 5d36 1f96 5a1f 2b6d 3ef4 388d  ..qz]6..Z.+m>.8.
+00002aa0: c7e6 c352 eb63 a5cd 871e a7f1 d87c 586a  ...R.c.......|Xj
+00002ab0: 7d6c 7ceb ee3c 444a c8bb c759 3c95 cd3f  }l|..<DJ...Y<..?
+00002ac0: 1ea7 3a36 ff54 da7e 5ad9 faa1 c769 3c36  ..:6.T.~Z....i<6
+00002ad0: 1f56 9a0f 2b9b 0f3d 4ee3 b1f9 a7d2 fa58  .V..+..=N......X
+00002ae0: 65f3 8fc7 593c b5ad ff78 9cea d8fc 536b  e...Y<...x....Sk
+00002af0: fda7 b6f9 c7e3 341e 9b7f 6a6d 3fad 6dfe  ......4...jm?.m.
+00002b00: f138 8dc7 e69f 5adb 4f6b 5b1f f338 8dc7  .8....Z.Ok[..8..
+00002b10: e6c3 5af3 616d f3a1 c759 3ce3 9b6a 863e  ..Z.am...Y<..j.>
+00002b20: e671 aa63 f373 a3ed a78d cdcf 1ea7 f1d8  .q.c.s..........
+00002b30: fcdc 68fd b0b1 f9d9 e334 1e9b 9f1b ad1f  ..h......4......
+00002b40: 3636 1f7a 9cc6 63f3 61a3 f9b0 b1f9 d0e3  66.z..c.a.......
+00002b50: 2c9e 8dcd 871e a73a 361f 6e34 1f6e 6c3e  ,......:6.n4.nl>
+00002b60: f438 8dc7 e69f 8dd6 0f37 36ff 789c c663  .8.......76.x..c
+00002b70: eb87 1bad 1f6e 6c79 f738 8b67 78cb d0d4  .....nly.8.gx...
+00002b80: 8026 9e2b d952 efd6 5aee ddda 96fc 89e7  .&.+.R..Z.......
+00002b90: 31d9 dad0 f096 9d72 7fe9 d6b6 c44d 3c8f  1......r.....M<.
+00002ba0: c9d6 42dc 5a3b 93bb f9eb 5009 87e0 89a7  ..B.Z;....P.....
+00002bb0: 31f9 d734 4ecf 6493 94d4 75f2 4fff 2d4a  1..4N.d...u.O.-J
+00002bc0: 5ac5 b9f9 bb01 4931 4d3d bb11 3352 e79f  Z.....I1M=..3R..
+00002bd0: 545a 62d2 aace f9e7 5f16 253d 77b6 0dc0  TZb....._.%=w...
+00002be0: 9d1e d9c8 c987 f383 7d4b 4cda 3d95 9b4f  ........}KL.=..O
+00002bf0: f453 56fc 6d70 8ed3 3ce7 ff24 dc10 d3e9  .SV.mp..<..$....
+00002c00: 4fc8 c9d5 65c6 5ee0 79ea f1cc 58c1 9ee7  O...e.^.y...X...
+00002c10: 4ac6 0ace 5417 f8d9 b565 9db4 7380 cb2e  J...T....e..s...
+00002c20: 1b42 199f e74e 38bd b8d9 b83b 4548 9d77  .B...N8....;EH.w
+00002c30: bbd9 c03b 4948 dd0e c6e7 88a7 3372 9290  ...;IH......3r..
+00002c40: 768f e5f2 cb6e 9024 a436 b9fc 72aa 4812  v....n.$.6..r.H.
+00002c50: 527b 5c7e 3956 2409 69c7 5237 9b7b 2709  R{\~9V$.i.R7.{'.
+00002c60: a91d 6e36 f84e 1252 ad3d 9b7c c785 de3b  ..n6.N.R.=.|...;
+00002c70: 8f0f 7f53 3b76 6fff aec1 c3f9 23d2 1466  ...S;vo.....#..f
+00002c80: d3f0 24ed a9e3 79ed f0b1 f56c 1c9e 2274  ..$...y....l.."t
+00002c90: 1a87 17b3 20d5 09b9 2b6c b6f5 38ad 483f  .... ...+l..8.H?
+00002ca0: f49e 9a44 4a4a d419 b9f3 d36a 43b7 51a7  ...DJJ.....jC.Q.
+00002cb0: dbce 38de 9e78 7e71 c67d 504e b8af 2fff  ..8..x~q.}PN../.
+00002cc0: 7792 ff01 0000 ffff 0000 00ff ff5c 90c1  w............\..
+00002cd0: 6ec2 3010 447f c5f2 3d98 240e 018b 2045  n.0.D...=.$... E
+00002ce0: 1024 0e9c 503f c04d 1c62 35c9 5aeb 4545  .$..P?.M.b5.Z.EE
+00002cf0: adfa ef75 08f4 d0db ceae 34f3 76b6 fa46  ...u......4.v..F
+00002d00: 70b4 3d19 6468 da82 97b1 7a8b e59a b33b  p.=.dh....z....;
+00002d10: aa9b 6d0a fe7d acaa 2c93 b28c b243 5545  ..m..}..,....CUE
+00002d20: 72b5 de47 6599 6fa2 3895 7275 c8a5 4c65  r..Ge.o.8.ru..Le
+00002d30: fac3 c56e eb01 e942 9acc d329 51e7 d969  ...n...B...)Q..i
+00002d40: e847 afee 3d36 49c1 3b22 a784 f075 6706  .G..=6I.;"...ug.
+00002d50: ed17 83ad 113c b4b4 a861 10d0 b6b6 36c2  .....<...a....6.
+00002d60: 3b34 baf1 9d31 34f4 2259 c6b9 405b 778d  ;4...14."Y..@[w.
+00002d70: 269d f039 670f 6363 c9c2 3867 5589 aaa6  &..9g.cc..8gU...
+00002d80: ac27 c5bf eb29 51a7 e755 fc41 eeb6 4e5f  .'...)Q..U.A..N_
+00002d90: cd59 e3d5 8e9e f5a6 a582 2f17 3967 68af  .Y......../.9gh.
+00002da0: dd6b 2670 8f6d c6d9 3b10 c1f0 525d 0034  .k&p.m..;...R].4
+00002db0: 38a9 94b3 1620 f437 8b40 30f9 5e0c dd1c  8.... .7.@0.^...
+00002dc0: 73da 19bc d82f 53f0 0d67 80d6 8ca1 9f40  s..../S..g.....@
+00002dd0: 5d70 17ca 426d 29e4 a9a9 663c 35f1 842f  ]p..Bm)...f<5../
+00002de0: 3e01 3f1e afef 7e01 0000 ffff 0300 504b  >.?...~.......PK
+00002df0: 0304 1400 0600 0800 0000 2100 904f 860a  ..........!..O..
+00002e00: f804 0000 d710 0000 1800 0000 786c 2f77  ............xl/w
+00002e10: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
+00002e20: 2e78 6d6c 9c93 db8a db30 1086 ef0b 7d07  .xml.....0....}.
+00002e30: a1fb 58b6 7368 d6c4 59e8 2ea1 0b7b 514a  ..X.sh..Y....{QJ
+00002e40: 0fd7 8a3c 8e45 24cb 9594 13a5 efde 91bc  ...<.E$.........
+00002e50: 4e02 8112 d6d8 922c cd7c ff8c 345a 3c1e  N......,.|..4Z<.
+00002e60: b522 7bb0 4e9a b6a4 5992 5202 ad30 956c  ."{.N...Y.R..0.l
+00002e70: 3725 fdf1 7d35 9a53 e23c 6f2b ae4c 0b25  7%..}5.S.<o+.L.%
+00002e80: 3d81 a38f cb8f 1f16 0763 b7ae 01f0 0409  =........c......
+00002e90: ad2b 69e3 7d57 30e6 4403 9abb c474 d0e2  .+i.}W0.D....t..
+00002ea0: 4a6d ace6 1e7f ed86 b9ce 02af a293 562c  Jm............V,
+00002eb0: 4fd3 19d3 5cb6 b427 14f6 1e86 a96b 29e0  O...\..'.....k).
+00002ec0: d988 9d86 d6f7 100b 8a7b 8cdf 35b2 7303  .........{..5.s.
+00002ed0: 4d8b 7b70 9adb edae 1b09 a33b 44ac a592  M.{p.......;D...
+00002ee0: fe14 a194 6851 bc6c 5a63 f95a 61de c76c  ....hQ.lZc.Za..l
+00002ef0: c205 395a 7c73 fcc6 834c 9cbf 51d2 5258  ..9Z|s...L..Q.RX
+00002f00: e34c ed13 24b3 3ee6 dbf4 1fd8 03e3 e24c  .L..$.>........L
+00002f10: bacd ff2e 4c36 6116 f632 1ce0 0595 bf2f  ....L6a..2...../
+00002f20: a46c 7a66 e517 d8f8 9db0 d919 16b6 cb16  .lzf............
+00002f30: 3b59 95f4 4ffa f68c b0cf 4293 8ed2 2c34  ;Y..O.....B...,4
+00002f40: 57cf 5fba 5c54 124f 3864 452c d425 fd9c  W._.\T.O8dE,.%..
+00002f50: 17af f98c b2e5 2216 d04f 0907 7735 26de  ......"..O..w5&.
+00002f60: 74af 50fb 2750 0a8d 3f51 120a 746d cc36  t.P.'P..?Q..tm.6
+00002f70: 58be a070 8a4c 070a 4428 15c2 b1db 436f  X..p.L..D(....Co
+00002f80: fd9a 4db0 c87f 4799 3046 0d76 16b9 1e0f  ..M...G.0F.v....
+00002f90: 82ab 58d4 5f2d 5973 074f 46fd 9295 6ff0  ..X._-Ys.OF...o.
+00002fa0: f6e0 e5a9 a0e6 3be5 2f93 f364 3ece d371  ......;./..d>..q
+00002fb0: 964f cf8b dfcc e10b c84d e3d1 0567 6309  .O.......M...gc.
+00002fc0: 15d5 e919 9cc0 9ac6 4893 3cc4 208c 4241  ........H.<. .BA
+00002fd0: 6c89 9678 3771 0f35 3fc6 fed0 ebe5 7992  l..x7q.5?.....y.
+00002fe0: cd26 e92c a0d7 e0fc 4a06 2225 62e7 bcd1  .&.,....J."%b...
+00002ff0: 4350 6fa8 1e82 8946 08f6 03e4 bff6 1996  CPo....F........
+00003000: 4174 0883 c163 9aa0 e0ad 088b 01ff 0300  At...c..........
+00003010: 00ff ff00 0000 ffff 9456 db6e 8330 0cfd  .........V.n.0..
+00003020: 952a 1f30 48a0 5701 0f23 5535 899f 400c  .*.0H.W..#U5..@.
+00003030: a94f dd54 aa6e fbfb 3990 62ec a434 bcb5  .O.T.n..9.b..4..
+00003040: 8e73 6c9f f89c 36eb ce6d 7bd3 f5ad 2eb2  .sl...6..m{.....
+00003050: ebd7 cfea 9a0b 2556 dd77 7de9 e0d3 41c2  ......%V.w}...A.
+00003060: 97f3 2d17 bb58 ac7e 655a 3787 cf3f dd76  ..-..X.~eZ7..?.v
+00003070: 4d7b 8160 fca6 4491 35e6 ce3b e441 a483  M{.`..D.5..;.A..
+00003080: eff7 42a9 2cba 1759 d4d8 c372 7a28 137a  ..B.,..Y...rz(.z
+00003090: 7834 e572 21a1 c008 2053 9a73 2200 5b7a  x4.r!... S.s".[z
+000030a0: 5859 0039 0148 1020 82a9 c6d1 1236 dadc  XY.9.H. .....6..
+000030b0: 4847 93cc 1b5b 8fb5 096e eaa1 2c81 bee6  HG...[...n..,...
+000030c0: f04b b884 136f 182b 06f1 152b 0460 c758  .K...o.+...+.`.X
+000030d0: b100 8495 27dd af97 b062 9279 637b f65c  ....'....b.yc{.\
+000030e0: 9083 cb10 d3c3 0f72 28fd 7c6e 3d7c a6bb  .......r(.|n=|..
+000030f0: 172b 0897 b02a dbb2 921c b2f5 d2a6 5c2e  .+...*........\.
+00003100: f622 b20b 7b1c 0264 2715 92d7 6ffc 8920  ."..{..d'...o.. 
+00003110: 72f6 2d00 61ff c9ac 3016 91db dcce 6893  r.-.a...0.....h.
+00003120: 4c3a 1d02 d029 f44e 5672 bf00 b684 64a4  L:...).NVr....d.
+00003130: 8ead a236 48a4 e610 a0ec a028 4917 2669  ...6H......(I.&i
+00003140: b199 e8fe 1629 6923 f32f 424f d952 560f  .....)i#./BO.RV.
+00003150: 08f2 26b8 26b4 6d48 0a7f 1469 b269 bb43  ..&.&.mH...i.i.C
+00003160: c4f3 2cc6 5017 1352 9a5b e303 254c 51ba  ..,.P..R.[..%LQ.
+00003170: c7a4 f53d a6ca 17b8 b2d7 4cf7 888d d64d  ...=......L....M
+00003180: 0959 e29c 5a0e d639 1194 8df8 08f1 7a67  .Y..Z..9......zg
+00003190: 0cd1 59f3 9453 f363 bf08 da1c b207 19fd  ..Y..S.c........
+000031a0: f4a1 f1ca 26d1 f171 f7e9 f84b 2c52 cbc1  ....&..q...K,R..
+000031b0: 23a7 e38f aec9 652a 378b 36cd 64d3 971e  #.....e*7.6.d...
+000031c0: 223e 62d1 44d3 03d4 9ff5 15e9 58a0 8df8  ">b.D.......X...
+000031d0: 80d1 b102 801d c792 4f2d 4ba2 6705 003b  ........O-K.g..;
+000031e0: b6d4 5fef 7f9a 38c9 0a5d e835 709f 4c38  .._...8..].5p.L8
+000031f0: b611 0f15 0a7d 2200 d8b1 89fe babf 63b4  .....}".......c.
+00003200: 8900 e041 ed93 7d53 a3fe 1d2a 50c8 01c0  ...A..}S...*P...
+00003210: 8e8e d5f8 a7c8 0146 1d07 003b 0255 5381  .......F...;.US.
+00003220: 12ed 29d4 5e00 b023 bdfe ba9f 6394 5e00  ..).^..#....c.^.
+00003230: b0a3 3ce5 2a2f c23f d3ff 0000 00ff ff00  ..<.*/.?........
+00003240: 0000 ffff 3c8f 416e 8430 0c45 af12 f900  ....<.An.0.E....
+00003250: 6486 aa45 4584 4d67 d345 579c 2025 0e89  d..EE.Mg.EW. %..
+00003260: 4a70 e478 34a3 9ebe 0189 eefc bdf8 effd  Jp.x4...........
+00003270: a110 cb24 5650 317a 03b7 aebf b56f a09e  ...$VP1z.....o..
+00003280: 69dd 4aff 5cd9 b506 8248 eeb5 2e73 c064  i.J.\....H...s.d
+00003290: 4b93 e2cc 54c8 4b33 53d2 e47d 9c51 97cc  K...T.K3S..}.Q..
+000032a0: 685d 0988 9256 dd5e ae9d e638 0767 c5b6  h]...V.^...8.g..
+000032b0: 300e 3be6 8336 1725 d276 a240 8f83 fe17  0.;..6.%.v.@....
+000032c0: 1887 6c17 fcb2 bcc4 ada8 15bd 18b8 341d  ..l...........4.
+000032d0: 288e 4b38 6fa1 7c7c 5f41 7d93 08a5 3385  (.K8o.||_A}...3.
+000032e0: 4a47 ded3 0b28 4f24 67a8 8cbd 7742 b967  JG...(O$g...wB.g
+000032f0: 956d 469e e22f 1a78 0745 1c71 abdb ab92  .mF../.x.E.q....
+00003300: 815c 0dd9 46a9 bc3e 3a03 fce9 ae87 e083  .\..F..>:.......
+00003310: f8e7 d835 fe01 0000 ffff 0300 504b 0304  ...5........PK..
+00003320: 1400 0600 0800 0000 2100 5e08 1521 9f01  ........!.^..!..
+00003330: 0000 4e03 0000 1000 0801 646f 6350 726f  ..N.......docPro
+00003340: 7073 2f61 7070 2e78 6d6c 20a2 0401 28a0  ps/app.xml ...(.
+00003350: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+00003360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000033a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000033b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000033c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000033d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000033e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000033f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003450: 0000 9c93 418b db30 1085 ef85 fe07 a3fb  ....A..0........
+00003460: 464e 5a96 1264 2d25 dbb2 872e 0dc4 bb3d  FNZ..d-%.......=
+00003470: 4fe5 712c 5696 8c66 d624 fdf5 956d d671  O.q,V..f.$...m.q
+00003480: da43 a1b7 9979 8fa7 cf23 4bdd 9d5a 97f5  .C...y...#K..Z..
+00003490: 18c9 065f 88f5 2a17 197a 132a eb8f 8578  ..._..*..z.*...x
+000034a0: 2abf de7c 1219 31f8 0a5c f058 8833 92b8  *..|..1..\.X.3..
+000034b0: d3ef dfa9 7d0c 1d46 b648 598a f054 8886  ....}..F.HY..T..
+000034c0: b9db 4a49 a6c1 1668 9564 9f94 3ac4 1638  ..JI...h.d..:..8
+000034d0: b5f1 2843 5d5b 83f7 c1bc b6e8 596e f2fc  ..(C][......Yn..
+000034e0: 56e2 89d1 5758 dd74 73a0 9812 b73d ff6f  V...WX.ts....=.o
+000034f0: 6815 ccc0 47cf e5b9 4bc0 5a95 81c1 95b6  h...G...K.Z.....
+00003500: 459d 2b79 69d4 e7ae 73d6 00a7 afd7 8fd6  E.+yi...s.......
+00003510: c440 a1e6 ec11 8cf5 1ca8 c9be 9c0c 3a25  .@............:%
+00003520: 9736 95f8 0f68 5ea3 e5f3 90b6 6cd5 c180  .6...h^.....l...
+00003530: c35d 3a5a d7e0 0895 bc0c d403 c2b0 d63d  .]:Z...........=
+00003540: d848 5af5 bced d170 8819 d95f 69b1 1b91  .HZ....p..._i...
+00003550: fd04 c201 b810 3d44 0b9e 13f8 609b 9ab1  ......=D....`...
+00003560: 761d 71d4 3f42 7ca1 0691 49c9 6498 8663  v.q.?B|...I.d..c
+00003570: b9f4 2e6b fb51 6f46 432a ae8d 43c0 0492  ...k.QoFC*..C...
+00003580: 846b c4d2 b243 fa5e ef21 f2bf 8847 8689  .k...C.^.!...G..
+00003590: 77c2 390c 7ceb 25df 4c3a 4a13 ce12 7ddc  w.9.|.%.L:J...}.
+000035a0: 4682 f8e3 d85d 683b f0e7 24cc d537 eb5f  F....]h;..$..7._
+000035b0: e8a9 2bc3 3d30 be6d fa7a a80e 0d44 acd2  ..+.=0.m.z...D..
+000035c0: e5cc 3731 0fd4 435a 7274 43c8 ae01 7fc4  ..71..CZrtC.....
+000035d0: eacd f3b7 30fc 21cf d3f3 d0eb db55 fe21  ....0.!......U.!
+000035e0: 4f57 be98 2979 7908 fa37 0000 00ff ff03  OW..)yy..7......
+000035f0: 0050 4b03 0414 0006 0008 0000 0021 0003  .PK..........!..
+00003600: 3b96 6a69 0100 007e 0200 0011 0008 0164  ;.ji...~.......d
+00003610: 6f63 5072 6f70 732f 636f 7265 2e78 6d6c  ocProps/core.xml
+00003620: 20a2 0401 28a0 0001 0000 0000 0000 0000   ...(...........
+00003630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000036a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000036b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000036c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000036d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000036e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000036f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003720: 0000 0000 0000 0000 7c92 5f4b c330 14c5  ........|._K.0..
+00003730: df05 bf43 c993 826d 926e 4e17 da0e a6ee  ...C...m.nN.....
+00003740: 6138 14ac 28be 85e4 6eab 6bd3 92c4 fdf9  a8..(...n.k.....
+00003750: f6a6 ed56 3714 1f93 7bce 2fe7 5c12 8db6  ...V7...{./.\...
+00003760: 45ee ad41 9bac 5431 a201 411e 2851 ca4c  E..A..T1..A.(Q.L
+00003770: 2d62 f49a 4efc 5be4 19cb 95e4 79a9 2046  -b..N.[.....y. F
+00003780: 3b30 6894 9c9f 45a2 62a2 d4f0 accb 0ab4  ;0h...E.b.......
+00003790: cdc0 788e a40c 1355 8c96 d656 0c63 2396  ..x....U...V.c#.
+000037a0: 5070 1338 8572 c379 a90b 6edd 512f 70c5  Pp.8.r.y..n.Q/p.
+000037b0: c58a 2f00 8784 0c70 0196 4b6e 39ae 817e  ../....p..Kn9..~
+000037c0: d511 d11e 2945 87ac be74 de00 a4c0 9043  ....)E...t.....C
+000037d0: 01ca 1a4c 038a 7fb4 1674 61fe 3434 9323  ...L.....ta.44.#
+000037e0: 6591 d95d e53a ede3 1eb3 a568 879d 7a6b  e..].:.....h..zk
+000037f0: b24e b8d9 6c82 4daf 89e1 f253 fc3e 7b7c  .N..l.M....S.>{|
+00003800: 69aa fa99 aa77 2500 2591 144c 68e0 b6d4  i....w%.%..Lh...
+00003810: c993 cc3e 5757 de34 7808 a6c1 2cf0 2ea6  ...>WW.4x...,...
+00003820: 5c5d 46f8 4851 6f33 e7c6 cedc e2e7 19c8  \]F.HQo3........
+00003830: f12e 1997 4ba8 fbd5 3e6f cd95 7341 6ec1  ....K...>o..sAn.
+00003840: f97e 6bdd 634d b7f6 4590 9e4b cbda 6e87  .~k.cM..E..K..n.
+00003850: c95b efee 3e9d a024 2474 e893 a11f 8629  .[..>..$$t.....)
+00003860: ed33 72c3 48ff a38e 72e2 afd3 b717 c53e  .3r.H...r......>
+00003870: d0bf c4b0 e753 ead3 eb94 0c19 19b0 5e78  .....S........^x
+00003880: 443c 0092 26f7 e98f 49be 0100 00ff ff03  D<..&...I.......
+00003890: 0050 4b03 0414 0006 0008 0000 0021 00ae  .PK..........!..
+000038a0: 0bfd 89bb 0100 002c 1500 0027 0000 0078  .......,...'...x
+000038b0: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
+000038c0: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
+000038d0: 7331 2e62 696e ec94 cd4a e350 14c7 ff69  s1.bin...J.P...i
+000038e0: fca8 ce62 2c08 6e66 3114 5762 194b e3c7  ...b,.nf1.Wb.K..
+000038f0: 4e4b d33a 95c6 84a6 1537 b328 3642 a026  NK.:.....7.(6B.&
+00003900: 254d 9119 1941 e62d c407 99e5 2c5d fa00  %M...A.-....,]..
+00003910: b376 253e 801b fddf d822 ce14 29e2 4638  .v%>....."..).F8
+00003920: 379c 7b3e eeb9 e7e6 feb8 1c0b 3e0e 1021  7.{>........>..!
+00003930: 448f 7288 189f e1d0 f711 2476 cca8 8a98  D.r.......$v....
+00003940: a860 d4d0 26f4 a9bf 70e6 f52f 1a34 cce0  .`..&...p../.4..
+00003950: fc83 916e d3fa 88fd 548a 7a3f a573 2ec2  ...n....T.z?.s..
+00003960: 18b9 fb75 416d b04d e914 45e9 7b8e edaa  ...uAm.M..E.{...
+00003970: fbec 18b3 badb cce2 128b fa72 66f3 dbc9  ...........rf...
+00003980: e94b a74d 268b 9349 ad37 fc55 29f5 8e08  .K.M&..I.7.U)...
+00003990: 0cdf d538 bf7c c924 d76a eca8 dc39 fcc6  ...8.|.$.j...9..
+000039a0: 0956 b0c1 575e a1ce 732e 2287 32d6 5060  .V..W^..s.".2.P`
+000039b0: 2c47 31b1 ce2f c79c 02e3 655a 2bf4 0dfa  ,G1../....eZ+...
+000039c0: 79ea 12bd 0256 13ef 272b d6cb ae59 aba1  y....V..'+...Y..
+000039d0: 19f8 91d7 5396 d3ea 7a91 ebff f050 3460  ....S...z....P4`
+000039e0: 47be 17c4 add8 0f03 3876 bd51 2f56 1ba8  G.......8v.Q/V..
+000039f0: 7bbd b0d3 4f62 34ed aeb2 f228 859d 30b2  {...Ob4....(..0.
+00003a00: c2b6 f768 fd7f b3e5 0cb0 6798 d6f0 ee17  ...h......g.....
+00003a10: b3dd ec27 a6dd 5074 ca9d 66a7 8deb 63eb  ...'..Pt..f...c.
+00003a20: d7ed f4d7 853f ab67 578c d506 6b48 3fd5  .....?.gW...kH?.
+00003a30: 53b9 ca5f 1a68 e56f 51f6 943f 07de 3f64  S.._.h.oQ..?..?d
+00003a40: 9fe9 e308 5ed2 599a ec37 1efb 8c83 16ad  ....^.Y..7......
+00003a50: 1e8e b91e a1cd e47f 336d ae05 63e6 9658  ........3m..c..X
+00003a60: e33b baec 5c2e 77a8 f354 278b 1993 2104  .;..\.w..T'...!.
+00003a70: 8480 1010 0242 4008 0801 2120 0484 8010  .....B@...! ....
+00003a80: 1002 4240 0808 8171 083c 0000 00ff ff03  ..B@...q.<......
+00003a90: 0050 4b03 0414 0006 0008 0000 0021 00fa  .PK..........!..
+00003aa0: 5660 d383 0500 00d4 1b00 0027 0000 0078  V`.........'...x
+00003ab0: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
+00003ac0: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
+00003ad0: 7332 2e62 696e 8a61 8861 2860 2862 c864  s2.bin.a.a(`(b.d
+00003ae0: c863 2861 d063 2805 423d 203b 0728 ee04  .c(a.c(.B= ;.(..
+00003af0: 2413 1992 19b2 1970 0346 1666 b63b 0c3f  $......p.F.f.;.?
+00003b00: a482 ff37 3032 3270 32cc e236 e148 6160  ...7022p2..6.Ha`
+00003b10: 64e0 6788 6062 6260 0293 8c0c 8e0c 2678  d.g.`bb`......&x
+00003b20: cc20 558a 11aa 8105 4833 0131 8c8f 6e4e  . U.....H3.1..nN
+00003b30: 4090 67d8 2301 2a5a 0c35 4a02 4c0b a883  @.g.#.*Z.5J.L...
+00003b40: 2003 0308 43c0 0186 2dcc b86c 8349 b888   ...C...-..l.I..
+00003b50: 0b30 0498 3033 6874 805c 0f01 8c58 7cb0  .0..03ht.\...X|.
+00003b60: c0c4 8399 1528 fd9f 810f 8819 1910 aaa9  .....(..........
+00003b70: ef9f 5113 076f 08e0 4adb b85c 7c00 2811  ..Q..o..J..\|.(.
+00003b80: ec1b e205 9217 60d8 c010 c190 0acc ddf9  ......`.........
+00003b90: 0c15 0c0a 0cee 0c01 0c2e 403a 8021 1848  ..........@:.!.H
+00003ba0: 8631 1803 733a 049b 3098 03d9 6640 6c00  .1..s:..0...f@l.
+00003bb0: d4e7 939a 9892 9997 ee9a 929e cac0 1090  ................
+00003bc0: 989e 1a9c 5995 cae0 6802 6607 a5a6 67e6  ....Y...h.f...g.
+00003bd0: e731 30b8 9416 e4a4 5640 29bf fc90 d2dc  .10.....V@).....
+00003be0: a49c 5486 a0d4 e2fc 9cd2 1290 0a33 0383  ..T..........3..
+00003bf0: 0a20 4e29 c824 2574 5dc4 1918 0cfd 8222  . N).$%t]......"
+00003c00: 40fe e601 b289 059d 8566 f338 80f9 6439  @........f.8..d9
+00003c10: b300 500b 2303 bbc2 6391 0850 e1c0 e01b  ..P.#...c..P....
+00003c20: ecec 06a2 bba0 5950 076a 2433 b0bc 02d9  ......YP.j$3....
+00003c30: 6209 f472 1058 0f23 c347 3654 fbf4 f543  b..r.X.#.G6T...C
+00003c40: f392 f373 0b8a 528b 8b53 5374 5d12 4b12  ...s..R..SSt].K.
+00003c50: f5f5 1902 a65d 7f62 c0fc 91cd d97b ee54  .....].b.....{.T
+00003c60: 6f0f d144 91e3 e76b 8a45 7535 4f6a 4f7d  o..D...k.Eu5OjO}
+00003c70: b6f8 d29e a28b 35f1 6b1d de85 9e79 a4b4  ......5.k....y..
+00003c80: 7df5 04bd 33be 795d 9f02 b97d b92e bb7e  }...3.y]...}...~
+00003c90: 3359 31d5 3684 83ab 6ac7 8a35 1ccc c6e6  3Y1.6...j..5....
+00003ca0: b66b 54d6 f4dc da91 3151 618b 0647 cfb9  .kT.....1Qa..G..
+00003cb0: 99ff cfcc 3d18 656a f4fd ffec ffe5 cf6a  ....=.ej.......j
+00003cc0: eecf b1fc fc92 ffca 9573 3b5f 8b7e 7cc8  .........s;_.~|.
+00003cd0: ff86 e317 f3c3 8435 c7c4 4f77 562d 3aca  .......5..OwV-:.
+00003ce0: cd1e ca16 af5d e4bb 7c53 c5cc d249 1c53  .....]..|S...I.S
+00003cf0: 99ab 9395 bcf5 2cdc 7730 fcd1 e85d 2a10  ......,.w0...]*.
+00003d00: a35e 27b8 c373 8760 cce4 939b da2d a7a5  .^'..s.`.....-..
+00003d10: f016 bd5a c297 b8a1 ccd4 bbdd 70be ccaa  ...Z........p...
+00003d20: cbc7 94cd ca14 7784 37f5 5bfd 98d1 bc5b  ......w.7.[....[
+00003d30: b6e6 cec1 bd7c 760f 1fd8 b1cf 2ff9 90f9  .....|v...../...
+00003d40: e18f d434 e36f 42e7 6e55 9c3b 56c7 f2fd  ...4.oB.nU.;V...
+00003d50: 44ef f3c0 8b15 4eae 8b39 937f ab5c 6cad  D.....N..9...\l.
+00003d60: ef3f 7bea 866a f362 9353 caa5 92fb b265  .?{..j.b.S.....e
+00003d70: 4f8b 1644 729d 0e2d d8f5 c3f9 d897 eaa3  O..Dr..-........
+00003d80: 926d 6fa7 4e78 7e4c e456 5931 5768 df46  .mo.Nx~L.VY1Wh.F
+00003d90: c64a 61fd 141f e5f5 c555 7dbe db92 764f  .Ja......U}...vO
+00003da0: 11dc 9ddd 7c65 62a5 e4bc 3ca9 4439 ed37  ....|eb...<.D9.7
+00003db0: 7d3f 8b26 47b8 9df9 72e8 f103 d773 cbef  }?.&G...r....s..
+00003dc0: 35af 4e5d 2a3f 6371 84fd a16a 9dd3 7f58  5.N]*?cq...j...X
+00003dd0: f2a6 7c5c ff80 f361 fcb1 e09f 4722 5be6  ..|\...a....G"[.
+00003de0: ea3c fc38 eba0 62e6 6991 0fdf 4ba6 85f8  .<.8..b.i...K...
+00003df0: 0665 6b05 6fbe 1f33 adb9 f6c1 dc4b f397  .ek.o..3.....K..
+00003e00: ce5a e217 713e 6299 6b5c 2cf3 62ef 048f  .Z..q>b.k\,.b...
+00003e10: c35a edbe b2a6 c1f6 065f 17ae 34f6 b09c  .Z......._..4...
+00003e20: 71e0 53a4 b196 f036 ade4 30ad 84d8 f8c3  q.S....6..0.....
+00003e30: a593 4a6b bb15 db9c 5cef fcd8 cefb e5cb  ..Jk....\.......
+00003e40: 4e8f bb07 9ad3 d6c4 069d d73f 11b7 55a5  N..........?..U.
+00003e50: fae4 ff74 ffd0 4f1b 3a43 fccf 5ef1 d3bd  ...t..O.:C..^...
+00003e60: e2f8 72cb ecad 73bf 05b3 56b3 bf34 2836  ..r...s...V..4(6
+00003e70: de6d a7b5 34e9 5f70 e631 5dbd 554b a2b8  .m..4._p.1].UK..
+00003e80: 0299 5796 88de 143d c476 6db5 e5f6 55a1  ..W....=.vm...U.
+00003e90: 13bb aecd 2c2f 0960 bc2f a872 b565 9bd7  ....,/.`./.r.e..
+00003ea0: 946d 598c e55c dba5 1ae3 e6a9 4ee7 5ad9  .mY..\......N.Z.
+00003eb0: f1fc cc52 21bb cf2b dac2 030e cc3a 5fa7  ...R!..+.....:_.
+00003ec0: f7ff 99f4 fea3 5ba6 fef5 8acb ecd8 26d1  ......[.......&.
+00003ed0: a25a f9ef d404 ff9b 4bfc 1257 a9ef 59ba  .Z......K..W..Y.
+00003ee0: d2b1 a0ef 8da3 73c2 fc0f 1b36 d9df 59fe  ......s....6..Y.
+00003ef0: c0ec a3fa d4c0 a8d7 cea1 e70d aea9 26af  ..............&.
+00003f00: 3f20 deba fc00 f3a1 fb53 625f b07e e8f9  ? .......Sb_.~..
+00003f10: 6168 25a5 156a be67 91af 4ee6 03af 8732  ah%..j.g..N....2
+00003f20: 77df 5dcc 2a98 fde3 fad9 df6e 0fce a66f  w.].*......n...o
+00003f30: bcc3 5a7e 42e6 fb81 ee47 f7d9 ff8b c9b1  ..Z~B....G......
+00003f40: 9efe beea d881 c243 8fd3 f671 5668 1f99  .......C...qVh..
+00003f50: 7de5 ecbb 7ace e2d9 3382 1f14 3dbc 9eb0  }...z...3...=...
+00003f60: ff83 7441 eb87 e8cf 8c2d f511 9e75 511b  ..tA.....-...uQ.
+00003f70: 3a2e 6a99 7b4f e2ce bfaf 3d7f 19b7 f787  :.j.{O....=.....
+00003f80: 03b7 75e2 b669 5ffa b8d1 eadb 71ae d56f  ..u..i_.....q..o
+00003f90: fe74 7e56 53f9 efc3 d7f3 f377 be59 0aab  .t~VS......w.Y..
+00003fa0: d88e 8f4b be3f 8999 c93a f570 fabc bc7b  ...K.?...:.p...{
+00003fb0: 8abb 1ea7 856f 7df5 fe8b 3dd3 7f20 6060  .....o}...=.. ``
+00003fc0: 60fb e8ec ef6b cac4 2004 2c9a 2a80 cd8b  `....k.. .,.*...
+00003fd0: 5460 3343 0fcc 4e05 5673 7cc0 62c8 8cc1  T`3C..N.Vs|.b...
+00003fe0: 90c1 0248 5a30 9832 f040 ab3e 1106 19a0  ...HZ0.2.@.>....
+00003ff0: 28a4 88d2 0336 272c 198c c085 9621 b0c8  (....6',.....!..
+00004000: 0241 31b0 bc31 508d 1e50 c610 4c1b 0255  .A1..1P..P..L..U
+00004010: 1900 f916 409e 38d0 9c8b 35ce ec12 a355  ....@.8...5....U
+00004020: 2929 e5f1 a8da d110 180d 81d1 1018 0d81  ))..............
+00004030: d110 180d 81d1 1018 0d81 d110 180d 81d1  ................
+00004040: 1018 0d81 d110 180d 81d1 1018 0d81 c117  ................
+00004050: 0200 0000 00ff ff03 0050 4b01 022d 0014  .........PK..-..
+00004060: 0006 0008 0000 0021 0021 8c46 3a73 0100  .......!.!.F:s..
+00004070: 008c 0500 0013 0000 0000 0000 0000 0000  ................
+00004080: 0000 0000 0000 005b 436f 6e74 656e 745f  .......[Content_
+00004090: 5479 7065 735d 2e78 6d6c 504b 0102 2d00  Types].xmlPK..-.
+000040a0: 1400 0600 0800 0000 2100 b555 3023 f400  ........!..U0#..
+000040b0: 0000 4c02 0000 0b00 0000 0000 0000 0000  ..L.............
+000040c0: 0000 0000 ac03 0000 5f72 656c 732f 2e72  ........_rels/.r
+000040d0: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
+000040e0: 0021 004a a9a6 61fa 0000 0047 0300 001a  .!.J..a....G....
+000040f0: 0000 0000 0000 0000 0000 0000 00d1 0600  ................
+00004100: 0078 6c2f 5f72 656c 732f 776f 726b 626f  .xl/_rels/workbo
+00004110: 6f6b 2e78 6d6c 2e72 656c 7350 4b01 022d  ok.xml.relsPK..-
+00004120: 0014 0006 0008 0000 0021 00a9 fa2f 40ae  .........!.../@.
+00004130: 0300 0007 0900 000f 0000 0000 0000 0000  ................
+00004140: 0000 0000 000b 0900 0078 6c2f 776f 726b  .........xl/work
+00004150: 626f 6f6b 2e78 6d6c 504b 0102 2d00 1400  book.xmlPK..-...
+00004160: 0600 0800 0000 2100 d543 1936 c503 0000  ......!..C.6....
+00004170: d00e 0000 0d00 0000 0000 0000 0000 0000  ................
+00004180: 0000 e60c 0000 786c 2f73 7479 6c65 732e  ......xl/styles.
+00004190: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+000041a0: 0021 0092 7a24 c4ae 0600 009a 1800 0014  .!..z$..........
+000041b0: 0000 0000 0000 0000 0000 0000 00d6 1000  ................
+000041c0: 0078 6c2f 7368 6172 6564 5374 7269 6e67  .xl/sharedString
+000041d0: 732e 786d 6c50 4b01 022d 0014 0006 0008  s.xmlPK..-......
+000041e0: 0000 0021 0013 c42c 13c2 0000 0042 0100  ...!...,.....B..
+000041f0: 0023 0000 0000 0000 0000 0000 0000 00b6  .#..............
+00004200: 1700 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00004210: 2f5f 7265 6c73 2f73 6865 6574 322e 786d  /_rels/sheet2.xm
+00004220: 6c2e 7265 6c73 504b 0102 2d00 1400 0600  l.relsPK..-.....
+00004230: 0800 0000 2100 c117 10be 4e07 0000 c620  ....!.....N.... 
+00004240: 0000 1300 0000 0000 0000 0000 0000 0000  ................
+00004250: b918 0000 786c 2f74 6865 6d65 2f74 6865  ....xl/theme/the
+00004260: 6d65 312e 786d 6c50 4b01 022d 0014 0006  me1.xmlPK..-....
+00004270: 0008 0000 0021 003b 6d32 4bc1 0000 0042  .....!.;m2K....B
+00004280: 0100 0023 0000 0000 0000 0000 0000 0000  ...#............
+00004290: 0038 2000 0078 6c2f 776f 726b 7368 6565  .8 ..xl/workshee
+000042a0: 7473 2f5f 7265 6c73 2f73 6865 6574 312e  ts/_rels/sheet1.
+000042b0: 786d 6c2e 7265 6c73 504b 0102 2d00 1400  xml.relsPK..-...
+000042c0: 0600 0800 0000 2100 406b a56b 7e0c 0000  ......!.@k.k~...
+000042d0: e54d 0000 1800 0000 0000 0000 0000 0000  .M..............
+000042e0: 0000 3a21 0000 786c 2f77 6f72 6b73 6865  ..:!..xl/workshe
+000042f0: 6574 732f 7368 6565 7431 2e78 6d6c 504b  ets/sheet1.xmlPK
+00004300: 0102 2d00 1400 0600 0800 0000 2100 904f  ..-.........!..O
+00004310: 860a f804 0000 d710 0000 1800 0000 0000  ................
+00004320: 0000 0000 0000 0000 ee2d 0000 786c 2f77  .........-..xl/w
+00004330: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
+00004340: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00004350: 0000 2100 5e08 1521 9f01 0000 4e03 0000  ..!.^..!....N...
+00004360: 1000 0000 0000 0000 0000 0000 0000 1c33  ...............3
+00004370: 0000 646f 6350 726f 7073 2f61 7070 2e78  ..docProps/app.x
+00004380: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00004390: 2100 033b 966a 6901 0000 7e02 0000 1100  !..;.ji...~.....
+000043a0: 0000 0000 0000 0000 0000 0000 f135 0000  .............5..
+000043b0: 646f 6350 726f 7073 2f63 6f72 652e 786d  docProps/core.xm
+000043c0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+000043d0: 00ae 0bfd 89bb 0100 002c 1500 0027 0000  .........,...'..
+000043e0: 0000 0000 0000 0000 0000 0091 3800 0078  ............8..x
+000043f0: 6c2f 7072 696e 7465 7253 6574 7469 6e67  l/printerSetting
+00004400: 732f 7072 696e 7465 7253 6574 7469 6e67  s/printerSetting
+00004410: 7331 2e62 696e 504b 0102 2d00 1400 0600  s1.binPK..-.....
+00004420: 0800 0000 2100 fa56 60d3 8305 0000 d41b  ....!..V`.......
+00004430: 0000 2700 0000 0000 0000 0000 0000 0000  ..'.............
+00004440: 913a 0000 786c 2f70 7269 6e74 6572 5365  .:..xl/printerSe
+00004450: 7474 696e 6773 2f70 7269 6e74 6572 5365  ttings/printerSe
+00004460: 7474 696e 6773 322e 6269 6e50 4b05 0600  ttings2.binPK...
+00004470: 0000 000f 000f 0012 0400 0059 4000 0000  ...........Y@...
+00004480: 00                                       .
```

### Comparing `sastadev-0.1.5/src/sastadev/data/methods/TARSP Index 2022-01-07.xlsx` & `sastadev-0.2.0/src/sastadev/data/methods/TARSP Index 2022-01-07.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/methods/TARSP_07062021.xlsx` & `sastadev-0.2.0/src/sastadev/data/methods/TARSP_07062021.xlsx`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/names/Woonplaatsen/83958NED_TypedDataSet_19062020_173530.csv` & `sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/83958NED_TypedDataSet_19062020_173530.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/names/Woonplaatsen/83958NED_UntypedDataSet_19062020_173456.csv` & `sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/83958NED_UntypedDataSet_19062020_173456.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/names/Woonplaatsen/83958NED_metadata.csv` & `sastadev-0.2.0/src/sastadev/data/names/Woonplaatsen/83958NED_metadata.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/names/fn10k_versie1/fn_10kw.xml` & `sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1/fn_10kw.xml`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/names/fn10k_versie1/fn_10kw.xsl` & `sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1/fn_10kw.xsl`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/names/fn10k_versie1.zip` & `sastadev-0.2.0/src/sastadev/data/names/fn10k_versie1.zip`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden.csv` & `sastadev-0.2.0/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden_raw.txt` & `sastadev-0.2.0/src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden_raw.txt`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/names/nameparts/namepartlexicon.csv` & `sastadev-0.2.0/src/sastadev/data/names/nameparts/namepartlexicon.csv`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/data/names/voornamentop10000.xml` & `sastadev-0.2.0/src/sastadev/data/names/voornamentop10000.xml`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/dedup.py` & `sastadev-0.2.0/src/sastadev/dedup.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/deregularise.py` & `sastadev-0.2.0/src/sastadev/deregularise.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 The module *deregularise* provides functions for dealing with overgeneralisations,
 wrong overgeneralisations, and certain misspelled overgeneralisations of
 verbal inflection.
 
 It provides:
 
 * functions for generating a list of overgeneralised forms, with their corrections and a characterisation of the error made. The main function for this is *makeparadigm*.
-Generating these forms and string them in a file is done by the module *deregularise_test*
+Generating these forms and string them in a file is done by the module *update_inflectioncorrection*
 
   .. autofunction:: deregularise::makeparadigm
 
 * functions for finding the correct form for a wrongly inflected verb. The main function for this is *correctinflection*:
 
   .. autofunction:: deregularise::correctinflection
 
-The module initialises the dictionary *correction* by reading in the file with the name contained in the constant *correctionfilename*
+The module initialises the dictionary *correction* by reading in the file with the name contained in the constant *correctionfullname*
+
+  .. autodata:: deregularise::correctionfullname
+
+which uses the constsnt *correctionfilename*
 
   .. autodata:: deregularise::correctionfilename
 
-  **Remark** The generation of the corrections and the module's testing should be
-  separated.
 
   **Remark** The function does not work perfectly yet for certain past participles (
   *ge* added incorrectly, and for some forms is yields a correct form (past participle
   with e) but not the more plausible past tense singular.
 
   **Remark** The functions should be extended so that also inflection information is
   returned.
@@ -43,14 +45,15 @@
 
 # maybe also add a variant with e- as prefix instead of ge-, and also without ge-
 
 
 overgen = 'Overgeneralisation'
 noge = 'Lacking ge prefix'
 nog = 'Prefix ge without onset'
+sege = 'prefix ge pronounced as se'
 wrongovergen = 'Wrong Overgeneralisation'
 wrongen = 'Wrong -en suffix'
 nolabel = 'Correct'
 
 chat_errors = {
     'Overgeneralisation': 'm',
     'Lacking ge prefix': 'm',
@@ -59,19 +62,25 @@
     'Wrong -en suffix': 'm'
 }
 
 metaarr = {}
 metaarr['ge'] = ''
 metaarr[''] = noge
 metaarr['e'] = nog
+metaarr['se'] = sege
 
-#: The constant *correctionfilename* contains the name of the file that contains the
-#: corrections. This file is generated by the module deregularise_test.
+#: The constant *correctionfilename* contains the file name of the file that contains the
+#: corrections. This file is generated by the module update_*inflectioncorrection*.
 correctionfilename = 'inflectioncorrection.tsv.txt'
 
+#: The constant *correctionfullname* contains the full name (path + filename) of the file that contains the
+#: corrections. This file is generated by the module update_*inflectioncorrection*.
+correctionfullname = os.path.join(
+    settings.SD_DIR, 'data', correctionfilename)
+
 v_prefixes = ['her', 'ver', 'ont', 'be']
 separable_prefixes = ['aan', 'aaneen', 'aantoe', 'achter', 'achteraan', 'achterna', 'achterom', 'achterop', 'achterover', 'achteruit',
                       'adem', 'ader', 'af', 'auto', 'bakzeil', 'beet', 'bekend', 'belang', 'bellen', 'betreft',
                       'bezig', 'bij', 'bijeen', 'binnen', 'blijk', 'bloot', 'boek', 'bot', 'boven', 'buiten', 'buitenom', 'daar',
                       'dank', 'deel', 'dicht', 'dienst', 'diep', 'dol', 'dood', 'door', 'droog', 'dubbel', 'dwars', 'eruit',
                       'feest', 'fijn', 'flauw', 'gade', 'garant', 'geheim', 'gelijk', 'geluk', 'gelukkig', 'gereed', 'gering', 'gerust',
                       'gevaar', 'gevangen', 'gewaar', 'geweld', 'glad', 'goed', 'groot', 'hard', 'heen', 'heet', 'heruit', 'hoog', 'in',
@@ -386,16 +395,16 @@
             adaptedresult = result
         result = prefix + adaptedresult
     return result, wrongen
 
 
 def makewrongpastpart(stem, stemFS, takesge, prefix='ge'):
     metalabel = wrongovergen
-    if stem[-1] in tkofschip or stem[-2:] in tkofschip:
-        result = stemFS + 't'
+    if stem[-1]  in tkofschip or stem[-2:] in tkofschip:
+        result = stemFS + 'd'
     elif CV(stem):
         result = stem + stem[-1] + 't'
     elif stem[-1] not in 'd':
         result = stemFS + 't'
     else:
         result = stemFS + 'd'
     if takesge:
@@ -405,15 +414,15 @@
             adaptedresult = addtrema(result[0]) + result[1:]
         else:
             adaptedresult = result
         result = prefix + adaptedresult
     result = finaldegemination(result)
     if takesge:
         metalabel = plussym.join([metalabel, metaarr[prefix]])
-    return result, overgen
+    return result, metalabel
 
 
 def getcorrections(thestr: str, correction: Dict[str, Tuple[str, str]]) -> List[Tuple[str, str]]:
     '''
 
     The function *getcorrections* returns a list of tuples (correct form, metadata) for a (wrongly) inflected word *thestr* using the dictionary *correction*.
 
@@ -553,21 +562,28 @@
 
     epastparticiple, metalabel = makepastpart(stem, stemFS, takesge, prefix='e')
     triples.append((epastparticiple, metalabel, goodpastpart))
 
     zeropastparticiple, metalabel = makepastpart(stem, stemFS, takesge, prefix='')
     triples.append((zeropastparticiple, metalabel, goodpastpart))
 
+    sepastparticiple, metalabel = makepastpart(stem, stemFS, takesge, prefix='se')
+    triples.append((sepastparticiple, metalabel, goodpastpart))
+
+
     # perfect participle with e
     pastpartwithe, metalabel = makepastpartwithe(stem, stemFS, takesge)
     triples.append((pastpartwithe, metalabel, goodpastpartwithe))
 
     epastpartwithe, metalabel = makepastpartwithe(stem, stemFS, takesge, prefix='e')
     triples.append((epastpartwithe, metalabel, goodpastpartwithe))
 
+    sepastpartwithe, metalabel = makepastpartwithe(stem, stemFS, takesge, prefix='se')
+    triples.append((sepastpartwithe, metalabel, goodpastpartwithe))
+
     # put off temporarily because past tense are more important
     # zeropastpartwithe, metalabel = makepastpartwithe(stem, stemFS, takesge, prefix='')
     # triples.append((zeropastpartwithe, metalabel, goodpastpartwithe))
 
     # perfect participle misspelled t ipv d gevalt
     wrongpastpart, metalabel = makewrongpastpart(stem, stemFS, takesge)
     triples.append((wrongpastpart, metalabel, goodpastpart))
@@ -625,14 +641,15 @@
 # eigenlijk nog de inflectiecode erbij@@@
 
 #: The dictionary *correction* consists of items with a string as key and a tuple of
 #: two strings (corrected form, metadata) as value. This dictionary is filled by
 #: reading from the file with the name in the constant *correctionfilename* upon
 #: initialisation of the module *deregularise*
 correction: Dict[str, Tuple[str, str]] = {}
-correctionfile = open(os.path.join(settings.SD_DIR, 'data', correctionfilename), 'r', encoding='utf8')
-myreader = csv.reader(correctionfile, delimiter=tab)
-for row in myreader:
-    wrong = row[0]
-    good = row[1]
-    meta = row[2]
-    correction[wrong] = good, meta
+
+with open(correctionfullname, 'r', encoding='utf8') as correctionfile:
+    myreader = csv.reader(correctionfile, delimiter=tab)
+    for row in myreader:
+        wrong = row[0]
+        good = row[1]
+        meta = row[2]
+        correction[wrong] = good, meta
```

### Comparing `sastadev-0.1.5/src/sastadev/exampletrees.py` & `sastadev-0.2.0/src/sastadev/exampletrees.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/expandquery.py` & `sastadev-0.2.0/src/sastadev/expandquery.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/external_functions.py` & `sastadev-0.2.0/src/sastadev/external_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 
 '''
 
 import re
 from typing import Callable, Dict
 
 from sastadev.allresults import QueryFunction
-from sastadev.asta_queries import asta_bijzin, asta_delpv, asta_lex, asta_noun
+from sastadev.asta_queries import (asta_bijzin, asta_delpv, asta_lemma,
+                                   asta_lex, asta_noun, astalemmafunction)
 from sastadev.astaforms import astaform
 from sastadev.ASTApostfunctions import (KMcount, countwordsandcutoff,
                                         finietheidsindex, getalllemmas,
                                         getlexlemmas, getnounlemmas,
                                         neologisme, phonpar, sempar,
                                         wordcountperutt)
 from sastadev.compounds import getcompounds
 from sastadev.dedup import correct, mlux, onvolledig, samplesize
 from sastadev.imperatives import wond4, wond5plus, wondx, wx, wxy, wxyz, wxyz5
-from sastadev.methods import allok
+from sastadev.methods import allok, astalemmafilter
 from sastadev.queryfunctions import VzN, vobij, voslashbij, xneg_neg, xneg_x
 from sastadev.stapforms import makestapform
 from sastadev.STAPpostfunctions import GL5LVU, GLVU, BB_totaal
 from sastadev.Sziplus import sziplus6, vr5plus
 from sastadev.tarspform import mktarspform
 from sastadev.TARSPpostfunctions import (gofase, gtotaal, pf, pf2, pf3, pf4,
                                          pf5, pf6, pf7, vutotaal)
@@ -69,15 +70,16 @@
                      tarsp_screening, vutotaal, gofase, gtotaal, pf2, pf3, pf4, pf5, pf6, pf7, pf, xneg_x, xneg_neg,
                      mktarspform, VzN, vobij, voslashbij]
 
 thestapfunctions = [BB_totaal, GLVU, GL5LVU, makestapform]
 
 theastafunctions = [samplesize, mlux, neologisme, onvolledig, correct, wordcountperutt, countwordsandcutoff,
                     astaform, KMcount, finietheidsindex, getnounlemmas, getlexlemmas, getalllemmas, asta_noun,
-                    asta_bijzin, asta_lex, asta_delpv, allok, sempar, phonpar, neologisme]
+                    asta_bijzin, asta_lex, asta_delpv, allok, sempar, phonpar, astalemmafilter, asta_lemma,
+                    astalemmafunction]
 
 thefunctions = thetarspfunctions + thestapfunctions + theastafunctions
 
 str2functionmap: Dict[str, QueryFunction] = {}
 
 for f in thefunctions:
     fname = getfname(f)
```

### Comparing `sastadev-0.1.5/src/sastadev/filefunctions.py` & `sastadev-0.2.0/src/sastadev/filefunctions.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/find_ngram.py` & `sastadev-0.2.0/src/sastadev/find_ngram.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/generatemacros.py` & `sastadev-0.2.0/src/sastadev/generatemacros.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/goldcountreader.py` & `sastadev-0.2.0/src/sastadev/goldcountreader.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/iedims.py` & `sastadev-0.2.0/src/sastadev/iedims.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/imperatives.py` & `sastadev-0.2.0/src/sastadev/imperatives.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from typing import List, Set
 
 from sastadev.sastatypes import SynTree
 from sastadev.Sziplus import getnodecount
 from sastadev.treebankfunctions import getattval
+from sastadev.expandquery import expandmacros
 
 noimplemmas = {'hoeven', 'moeten', 'mogen', 'kunnen', 'hebben', 'willen', 'hebben', 'zitten'}
 noimpwords = {'ben', 'bent', 'is', 'zijn'}
 impmodlemmas = {'eens', 'maar'}
 
 
+kijkVUxpath = expandmacros('.//node[%Tarsp_kijkVU%]')
+
 impquery = '''
 .//node[@cat="sv1" and
     not(node[@rel="su"]) and
     node[@rel="hd" and @pt="ww" and @pvtijd="tgw" and @pvagr="ev"
          and @wvorm="pv" and
          not(contains(@frame,"modal")) and
          (not(@lemma="zijn") or @word="wees" or @word="weest") and
@@ -136,20 +139,28 @@
 
 
 def wx(syntree: SynTree) -> List[SynTree]:
     '''
     The function *wx* finds nodes for imperative clauses with 1 or 2 nodes.
     it uses the function *impwi* to achieve that.
     '''
-    results = impwi(syntree, {1, 2})
+    kijkvuresults = syntree.xpath(kijkVUxpath)
+    if kijkvuresults == []:
+        results = impwi(syntree, {1, 2})
+    else:
+        results = []
     return results
 
 
 def wxy(syntree):
-    results = impwi(syntree, {3})
+    kijkvuresults = syntree.xpath(kijkVUxpath)
+    if kijkvuresults == []:
+        results = impwi(syntree, {3})
+    else:
+        results = []
     return results
 
 
 def wxyz(syntree):
     results = impwi(syntree, {4})
     return results
```

### Comparing `sastadev-0.1.5/src/sastadev/imply.py` & `sastadev-0.2.0/src/sastadev/imply.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/longqueries.py` & `sastadev-0.2.0/src/sastadev/longqueries.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/macrolength.py` & `sastadev-0.2.0/src/sastadev/macrolength.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/macros.py` & `sastadev-0.2.0/src/sastadev/macros.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/metadata.py` & `sastadev-0.2.0/src/sastadev/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from typing import List
 
 from lxml import etree
 
-bpl_none, bpl_word, bpl_node, bpl_delete, bpl_indeze, bpl_extra_grammatical, bpl_wordlemma, \
-    bpl_cond, bpl_replacement = tuple(range(9))
+(bpl_none, bpl_word, bpl_node, bpl_delete, bpl_indeze, bpl_extra_grammatical,
+ bpl_wordlemma, bpl_cond, bpl_replacement) = tuple(range(9))
 defaultpenalty = 10
 defaultbackplacement = bpl_none
 
 SASTA = 'SASTA'
 space = ' '
 metakw = '##META'
 
@@ -49,15 +49,15 @@
 
 # copied from chamd
 def despace(str):
     # remove leading and trailing spaces
     # replace other sequences of spaces by underscore
     result = str.strip()
     result = re.sub(r' +', r'_', result)
-    return (result)
+    return result
 
 
 class Meta:
     def __init__(self, name, value, annotationwordlist=[], annotationposlist=[], annotatedposlist=[],
                  annotatedwordlist=[], annotationcharlist=[
     ], annotationcharposlist=[], annotatedcharlist=[],
             annotatedcharposlist=[], atype='text', cat=None, subcat=None, source=None, penalty=defaultpenalty,
@@ -80,36 +80,41 @@
         self.backplacement = backplacement
         self.fmstr = '<{}:type={}:annotationwordlist={}:annotationposlist={}:annotatedwordlist={}:annotatedposlist={}:value={}:cat={}:source={}>'
         self.xmlformat = xmlformat
 
     def __repr__(self):
         reprfmstr = 'Meta({},{},annotationwordlist={},annotationposlist={},annotatedposlist{},annotatedwordlist={},' \
                     ' atype={}, cat={}, subcat={}, source={}, penalty={}, backplacement={})'
-        result = reprfmstr.format(repr(self.name), repr(self.value), repr(self.annotationwordlist), repr(self.annotationposlist),
+        result = reprfmstr.format(repr(self.name), repr(self.value), repr(self.annotationwordlist),
+                                  repr(self.annotationposlist),
                                   repr(self.annotatedposlist), repr(
-                                      self.annotatedwordlist), repr(self.atype),
-                                  repr(self.cat), repr(self.subcat), repr(self.source), repr(self.penalty), repr(self.backplacement))
+            self.annotatedwordlist), repr(self.atype),
+            repr(self.cat), repr(self.subcat), repr(
+                self.source), repr(self.penalty),
+            repr(self.backplacement))
         return result
 
     def __str__(self):
         frm = self.fmstr.format(self.name, self.atype, str(self.annotationwordlist),
                                 str(self.annotationposlist), str(
-                                    self.annotatedwordlist), str(self.annotatedposlist),
-                                str(self.value), str(self.cat), str(self.source))
+            self.annotatedwordlist), str(self.annotatedposlist),
+            str(self.value), str(self.cat), str(self.source))
         return frm
 
     def toElement(self):
         # result = self.xmlformat.format(name=self.name, atype=self.atype, annotationwordlist=str(self.annotationwordlist),
         #                    annotationposlist=str(self.annotationposlist), annotatedwordlist=str(self.annotatedwordlist),
         #                    annotatedposlist=str(self.annotatedposlist), value=str(self.value), cat=str(self.cat),
         #                         subcat=self.subcat,  source=str(self.source), backplacement=self.backplacement,
         #                         penalty=self.penalty)
 
-        result = etree.Element('xmeta', name=self.name, atype=self.atype, annotationwordlist=str(self.annotationwordlist),
-                               annotationposlist=str(self.annotationposlist), annotatedwordlist=str(self.annotatedwordlist),
+        result = etree.Element('xmeta', name=self.name, atype=self.atype,
+                               annotationwordlist=str(self.annotationwordlist),
+                               annotationposlist=str(self.annotationposlist),
+                               annotatedwordlist=str(self.annotatedwordlist),
                                annotatedposlist=str(self.annotatedposlist), value=str(self.value), cat=str(self.cat),
                                subcat=str(self.subcat), source=str(self.source), backplacement=str(self.backplacement),
                                penalty=str(self.penalty))
         return result
 
 
 def selectmeta(name, metadatalist):
```

### Comparing `sastadev-0.1.5/src/sastadev/methodinfo.py` & `sastadev-0.2.0/src/sastadev/methodinfo.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/mismatches.py` & `sastadev-0.2.0/src/sastadev/mismatches.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from collections import Counter
 from copy import copy
+from typing import Tuple
 
 from lxml import etree
 
+from sastadev.allresults import ResultsKey, showreskey
 from sastadev.conf import settings
+from sastadev.sastatypes import Position, UttId
 from sastadev.treebankfunctions import (find1, getattval, getmarkedyield,
                                         getyield)
 
 tab = '\t'
 space = ' '
 eps = ''
 
@@ -69,123 +72,184 @@
     if 'begin' in matchtree.attrib:
         positionstr = getattval(matchtree, 'begin')
         position = int(positionstr) + 1
     else:
         position = 0
     return position
 
-#moved to treebannkfunctions
+# moved to treebannkfunctions
 # def getmarkedyield(wordlist, positions):
 #     pos = 1
 #     resultlist = []
 #     for w in wordlist:
 #         if pos in positions:
 #             resultlist.append(mark(w))
 #         else:
 #             resultlist.append(w)
 #         pos += 1
 #     return resultlist
 
 
-def mismatches(queryid, queries, theresultsminusgold, goldminustheresults, allmatches, allutts, platinumcheckfile):
+def mismatches(reskey, queries, theresultsminusgold, goldminustheresults, allmatches, allutts, platinumcheckfile):
+    reskeystr = showreskey(reskey)
+    queryid = reskey[0]
     if theresultsminusgold != {}:
         print('More examples', file=platinumcheckfile)
     for uttid in theresultsminusgold:
-        if (queryid, uttid) in allmatches:
-            for (m, syntree) in allmatches[(queryid, uttid)]:
+        if (reskey, uttid) in allmatches:
+            for (m, syntree) in allmatches[(reskey, uttid)]:
                 markedutt = getmarkedutt(m, syntree)
-                platinumcheckrow1 = [queryid, queries[queryid].cat, queries[queryid].subcat, queries[queryid].item,
+                platinumcheckrow1 = [reskeystr, queries[queryid].cat, queries[queryid].subcat, queries[queryid].item,
                                      uttid, markedutt]
                 print(tab.join(platinumcheckrow1), file=platinumcheckfile)
 
     if goldminustheresults != {}:
         print('Missed examples', file=platinumcheckfile)
     for uttid in goldminustheresults:
         if uttid in allutts:
             uttstr = space.join(allutts[uttid])
         else:
             settings.LOGGER.warning('uttid {} not in alluts'.format(uttid))
-        platinumcheckrow2 = [queryid, queries[queryid].cat, queries[queryid].subcat, queries[queryid].item, uttid,
-                             uttstr]
+        platinumcheckrow2 = [reskeystr, queries[queryid].cat, queries[queryid].subcat, queries[queryid].item, uttid,
+                             uttstr, queries[queryid].inform]
         print(tab.join(platinumcheckrow2), file=platinumcheckfile)
 
 
 def getmarkposition(position, nodeendmap, uttid):
     if position == 0:
         result = 1
     elif uttid in nodeendmap:
         if str(position) in nodeendmap[uttid]:
             result = nodeendmap[uttid][str(position)]
         else:
-            settings.LOGGER.error('getmarkposition: No mapping found for position {} in utterance {}'.format(position, uttid))
+            settings.LOGGER.error(
+                'getmarkposition: No mapping found for position {} in utterance {}'.format(position, uttid))
             result = 1
     else:
-        settings.LOGGER.error('getmarkposition: No mappings found for uttid {}'.format(uttid))
+        settings.LOGGER.error(
+            'getmarkposition: No mappings found for uttid {}'.format(uttid))
         result = 1
     return result
 
 
-def exactmismatches(queryid, queries, exactresults, exactgoldscores, allmatches, allutts, platinumcheckfile,
+def isliteralreskey(reskey: ResultsKey):
+    (key, val) = reskey
+    result = key != val
+    return result
+
+
+def literalmissedmatches(queries, exactresults, exactgoldscores, allmatches, allutts, platinumcheckfile,
+                         permsilverdatadict={}, annotationinput=False):
+    newrows = []
+    for reskey in exactgoldscores:
+        if isliteralreskey(reskey) and reskey not in exactresults:
+            print('Missed examples', file=platinumcheckfile)
+            reskeystr = showreskey(reskey)
+            queryid = reskey[0]
+            inform = queries[queryid].inform
+            for hit in exactgoldscores[reskey]:
+                (uttid, position) = hit
+                if uttid in allutts:
+                    # markposition = 1 if position == 0 else position
+                    markposition = position
+                    markedwordlist = getmarkedyield(
+                        allutts[uttid], [markposition])
+                    uttstr = space.join(markedwordlist)
+                    tree = allmatches[(reskey, uttid)][0][1] if (
+                        reskey, uttid) in allmatches else None
+                    origutt = find1(
+                        tree, './/meta[@name="origutt"]/@value') if tree is not None else '**'
+                else:
+                    settings.LOGGER.warning(
+                        'uttid {} not in allutts'.format(uttid))
+                    uttstr = ""
+                    markposition = 0
+                    tree = allmatches[(reskey, uttid)][0][1] if (
+                        reskey, uttid) in allmatches else None
+                    origutt = find1(
+                        tree, './/meta[@name="origutt"]/@value') if tree is not None else '**'
+                platinumcheckrow2 = [reskeystr, queries[queryid].cat, queries[queryid].subcat, queries[queryid].item,
+                                     str(uttid),
+                                     str(markposition),
+                                     uttstr, origutt, inform]
+                print(tab.join(platinumcheckrow2), file=platinumcheckfile)
+                key = (reskey, uttid, position)
+                usercomments = getusercomments(
+                    permsilverdatadict, key, report=False)
+                xlplatinumcheckrow2 = usercomments + \
+                    ['Missed examples'] + platinumcheckrow2
+                newrows.append(xlplatinumcheckrow2)
+    return newrows
+
+
+def exactmismatches(reskey, queries, exactresults, exactgoldscores, allmatches, allutts, platinumcheckfile,
                     permsilverdatadict={}, annotationinput=False):
-    theexactresults = exactresults[queryid] if queryid in exactresults else Counter()
-    theexactgoldscores = exactgoldscores[queryid] if queryid in exactgoldscores else Counter()
+    reskeystr = showreskey(reskey)
+    queryid = reskey[0]
+    inform = queries[queryid].inform
+    theexactresults = exactresults[reskey] if reskey in exactresults else Counter()
+    theexactgoldscores = exactgoldscores[reskey] if reskey in exactgoldscores else Counter()
     (theresultsminusgold, goldminustheresults, intersection) = exactcompare(theexactresults, theexactgoldscores)
     newrows = []
     if theresultsminusgold != []:
         print('More examples', file=platinumcheckfile)
     for hit in theresultsminusgold:
         uttid, position = hit
-        if (queryid, uttid) in allmatches or annotationinput:
-            #markposition = 1 if position == 0 else position
-            tree = allmatches[(queryid, uttid)][0][1] if (queryid, uttid) in allmatches else None
+        if (reskey, uttid) in allmatches or annotationinput:
+            # markposition = 1 if position == 0 else position
+            tree = allmatches[(reskey, uttid)][0][1] if (reskey, uttid) in allmatches else None
             origutt = find1(tree, './/meta[@name="origutt"]/@value') if tree is not None else '**'
             markposition = position
             if uttid in allutts:
                 markedwordlist = getmarkedyield(allutts[uttid], [markposition])
                 uttstr = space.join(markedwordlist)
-                platinumcheckrow1 = [queryid, queries[queryid].cat, queries[queryid].subcat, queries[queryid].item,
-                                     str(uttid), str(markposition), uttstr, origutt]
+                queryitem = reskey[1] if isliteralreskey(reskey) else queries[queryid].item
+                platinumcheckrow1 = [reskeystr, queries[queryid].cat, queries[queryid].subcat, queryitem,
+                                     str(uttid), str(markposition), uttstr, origutt, inform]
                 print(tab.join(platinumcheckrow1), file=platinumcheckfile)
-                key = (queryid, uttid, position)
+                key = (reskey, uttid, position)
                 usercomments = getusercomments(permsilverdatadict, key, report=True)
                 xlplatinumcheckrow1 = usercomments + ['More examples'] + platinumcheckrow1
                 newrows.append(xlplatinumcheckrow1)
                 # for (m, syntree) in allmatches[(queryid, uttid)]:
                 #    if getfirstwordposition(m) == position:
                 #        markedutt = getmarkedutt(m, syntree)
                 #       platinumcheckrow1 = [queryid, queries[queryid].cat, queries[queryid].subcat, queries[queryid].item,
                 #                            uttid), markedutt]
                 #        print(tab.join(platinumcheckrow1), file=platinumcheckfile)
             else:
-                settings.LOGGER.error(f'Uttid {uttid} not in allutts; reporting ignored')
+                settings.LOGGER.error(
+                    f'Uttid {uttid} not in allutts; reporting ignored')
 
     if goldminustheresults != []:
         print('Missed examples', file=platinumcheckfile)
     for hit in goldminustheresults:
         (uttid, position) = hit
         if uttid in allutts:
-            #markposition = 1 if position == 0 else position
+            # markposition = 1 if position == 0 else position
             markposition = position
             markedwordlist = getmarkedyield(allutts[uttid], [markposition])
             uttstr = space.join(markedwordlist)
-            tree = allmatches[(queryid, uttid)][0][1] if (queryid, uttid) in allmatches else None
+            tree = allmatches[(reskey, uttid)][0][1] if (reskey, uttid) in allmatches else None
             origutt = find1(tree, './/meta[@name="origutt"]/@value') if tree is not None else '**'
         else:
             settings.LOGGER.warning('uttid {} not in allutts'.format(uttid))
             uttstr = ""
             markposition = 0
-            tree = allmatches[(queryid, uttid)][0][1] if (queryid, uttid) in allmatches else None
+            tree = allmatches[(reskey, uttid)][0][1] if (queryid, uttid) in allmatches else None
             origutt = find1(tree, './/meta[@name="origutt"]/@value') if tree is not None else '**'
-        platinumcheckrow2 = [queryid, queries[queryid].cat, queries[queryid].subcat, queries[queryid].item, str(uttid),
+        platinumcheckrow2 = [reskeystr, queries[queryid].cat, queries[queryid].subcat, queries[queryid].item,
+                             str(uttid),
                              str(markposition),
-                             uttstr, origutt]
+                             uttstr, origutt, inform]
         print(tab.join(platinumcheckrow2), file=platinumcheckfile)
-        key = (queryid, uttid, position)
+        key = (reskey, uttid, position)
         usercomments = getusercomments(permsilverdatadict, key, report=False)
-        xlplatinumcheckrow2 = usercomments + ['Missed examples'] + platinumcheckrow2
+        xlplatinumcheckrow2 = usercomments + \
+            ['Missed examples'] + platinumcheckrow2
         newrows.append(xlplatinumcheckrow2)
     return newrows
 
 
 def compareunaligned(resultctr, goldctr):
     '''
 
@@ -228,15 +292,16 @@
     '''
     resultscounter = Counter(exactresults)
     goldcounter = Counter(exactgoldscores)
     intersection1 = resultscounter & goldcounter
     resultsminusgold1 = resultscounter - goldcounter
     goldminusresults1 = goldcounter - resultscounter
 
-    (resultsminusgold2, goldminusresults2, intersection2) = compareunaligned(resultsminusgold1, goldminusresults1)
+    (resultsminusgold2, goldminusresults2, intersection2) = compareunaligned(
+        resultsminusgold1, goldminusresults1)
 
     intersectionctr = intersection1 + intersection2
     resultsminusgoldctr = resultsminusgold1 - resultsminusgold2
     goldminusresultsctr = goldminusresults1 - goldminusresults2
 
     intersection = counter2list(intersectionctr)
     resultsminusgold = counter2list(resultsminusgoldctr)
@@ -247,19 +312,25 @@
 
 def counter2list(ctr):
     result1 = [el for el in ctr for k in range(ctr[el])]
     result = sorted(result1)
     return result
 
 
-def getusercomments(permsilverdict, key, report=False):
+def getusercomments(permsilverdict, key: Tuple[ResultsKey, UttId, Position], report=False):
+    reskey, uttid, pos = key
+    olderkey = (reskey[0], uttid, pos)
     if key in permsilverdict:
         therow = permsilverdict[key]
         usercomments = therow[usercommentbegin:usercommentuntil]
         result = usercomments
+    elif olderkey in permsilverdict:
+        therow = permsilverdict[olderkey]
+        usercomments = therow[usercommentbegin:usercommentuntil]
+        result = usercomments
     else:
         count = usercommentuntil - usercommentbegin
         resultlist = [usercommentdefaultvalue for _ in range(count)]
         result = resultlist
         if report:
             settings.LOGGER.warning('No silver remark for key: {}'.format(key))
     return result
@@ -267,15 +338,16 @@
 
 def testcompare():
     testresults = [(1, 2), (1, 2), (1, 2), (1, 5), (1, 6), (2, 0), (2, 4)]
     goldresults = [(1, 2), (2, 4), (2, 6), (1, 0), (3, 5)]
     reftestminusgold = [(1, 2), (1, 5), (1, 6)]
     refgoldminustest = [(3, 5)]
     refintersection = [(1, 2), (1, 2), (2, 4), (2, 6)]
-    (testminusgold, goldminustest, intersection) = exactcompare(testresults, goldresults)
+    (testminusgold, goldminustest, intersection) = exactcompare(
+        testresults, goldresults)
     for (l, r, g) in zip(['R-G', 'G-R', 'R*G'], [testminusgold, goldminustest, intersection],
                          [reftestminusgold, refgoldminustest, refintersection]):
         if r == g:
             print('{}: OK {} == {}'.format(l, r, g))
         else:
             print('{}: NO: {} != {}'.format(l, r, g))
```

### Comparing `sastadev-0.1.5/src/sastadev/mksilver.py` & `sastadev-0.2.0/src/sastadev/mksilver.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/mwe2pep.py` & `sastadev-0.2.0/src/sastadev/mwe2pep.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/namepartlexicon.py` & `sastadev-0.2.0/src/sastadev/namepartlexicon.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/phonetics.py` & `sastadev-0.2.0/src/sastadev/phonetics.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/query.py` & `sastadev-0.2.0/src/sastadev/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,29 +22,30 @@
 def clean(valstr):
     result = valstr.strip().lower()
     return result
 
 
 class Query:
     def __init__(self, id, cat, subcat, level, item, altitems, implies, original, pages, fase, query, inform,
-                 screening, process, stars, filter, variants, unused1, unused2, comments):
+                 screening, process, literal, stars, filter, variants, unused1, unused2, comments):
         self.id = id
         self.cat = cat
         self.subcat = subcat
         self.level = level
         self.item = item
         self.altitems = altitems
         self.implies = implies
         self.original = original
         self.pages = pages
         self.fase = fase
         self.query = query
         self.inform = inform
         self.screening = screening
         self.process = getprocess(process)
+        self.literal = literal
         self.stars = clean(stars)
         self.filter = filter
         self.variants = variants
         self.unused1 = unused1
         self.unused2 = unused2
         self.comments = comments
 
@@ -73,7 +74,12 @@
     result = (query.process == post_process)
     return result
 
 
 def query_exists(query):
     result = query.query != "" and query.query is not None
     return result
+
+
+def is_literal(query):
+    result = query.literal != ''
+    return result
```

### Comparing `sastadev-0.1.5/src/sastadev/queryfunctions.py` & `sastadev-0.2.0/src/sastadev/queryfunctions.py`

 * *Files 11% similar despite different names*

```diff
@@ -106,17 +106,16 @@
     for RPnode in RPnodes:
         # find the head node
         headnode = find1(RPnode, 'node[@rel="hd"]')
 
         # find the obj1node
         obj1node = find1(RPnode, 'node[@rel="obj1"]')
 
-        # check if they are adjacent
         if headnode is not None and obj1node is not None:
-            if pred(headnode, obj1node, stree):
+            if pred(obj1node, headnode, stree):
                 results.append(RPnode)
     return results
 
 
 def vobij(stree: SynTree) -> List[SynTree]:
     '''
 
@@ -131,15 +130,15 @@
 
     * The function *auxvobij*  finds adjacent R-pronoun + adposition cases:
 
       .. autofunction:: queryfunctions::auxvobij
 
     '''
     results1 = stree.xpath(vobijxpath)
-    results2 = auxvobij(stree, adjacent)
+    results2 = auxvobij(stree, vobijpred)
     results = results1 + results2
     return results
 
 
 def voslashbij(stree: SynTree) -> List[SynTree]:
     '''
 
@@ -151,7 +150,19 @@
     .. autofunction:: queryfunctions::auxvobij
           :noindex:
 
 
     '''
     results = auxvobij(stree, notadjacent)
     return results
+
+def vobijpred(obj1node, headnode, stree) -> bool:
+    #check for adjacency  (er naar is ok, er gisteren naar not)
+    cond1 = adjacent(headnode, obj1node, stree)
+
+    # check whether the obj1node precedes the headnode: daar naar is ok, naar daar is not ok
+    headposition = int(getattval(headnode, 'end'))
+    obj1position = int(getattval(obj1node, 'end'))
+    cond2 = obj1position < headposition
+    result = cond1 and cond2
+    return result
+
```

### Comparing `sastadev-0.1.5/src/sastadev/rawalpinoparsing.py` & `sastadev-0.2.0/src/sastadev/rawalpinoparsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import re
 import urllib.parse
 import urllib.request
+from typing import Optional
 
 from lxml import etree  # type: ignore
 
 from sastadev.treebankfunctions import showtree
 
 # from memoize import memoize
 
@@ -72,15 +73,14 @@
             # print(streebytes.decode('utf8'))
             stree = etree.fromstring(streebytes)
             return stree
         else:
             logging.error('parsing failed:', r1.status, r1.reason, sent)
             return None
 
-
 def escape_alpino_input(instr: str) -> str:
     '''
     The function escape_alpino_input takes as input a string *str* and returns this string with symbols with a
     special meaning for Alpino escaped, in particular the square bracket symbols [ and ] used for bracketed input.
     :param instr:
     :return:
     '''
```

### Comparing `sastadev-0.1.5/src/sastadev/readcsv.py` & `sastadev-0.2.0/src/sastadev/readcsv.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/readmethod.py` & `sastadev-0.2.0/src/sastadev/readmethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,17 +128,17 @@
     return True
 
 
 def read_method(methodname: str, methodfilename: FileName) -> Method:
     header, data = xlsx.getxlsxdata(methodfilename)
 
     idcol, catcol, subcatcol, levelcol, itemcol, altcol, impliescol, \
-        originalcol, pagescol, fasecol, querycol, informcol, screeningcol, processcol, starscol, filtercol, \
-        variantscol, unused1col, unused2col, commentscol = \
-        0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19
+    originalcol, pagescol, fasecol, querycol, informcol, screeningcol, processcol, literalcol, starscol, filtercol, \
+    variantscol, unused1col, unused2col, commentscol = \
+        0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20
 
     headerrow = 0
 
     queries: QueryDict = {}
     item2idmap: Item_Level2QIdDict = {}
     altcodes: AltCodeDict = {}
 
@@ -155,22 +155,24 @@
             original: bool = getboolean(row[originalcol])
             pages: str = str(get_pages(row[pagescol]))
             fase: int = getint(row[fasecol])
             query: str = row[querycol]
             inform: str = row[informcol]
             screening: str = row[screeningcol]
             process: str = row[processcol].strip()
+            literal: str = row[literalcol].strip()
             stars: str = row[starscol].strip()
             filter: str = row[filtercol].strip()
             variants: str = row[variantscol]
             unused1: str = row[unused1col]
             unused2: str = row[unused2col]
             comments: str = row[commentscol]
 
-            queries[id] = Query(id, cat, subcat, level, item, altitems, implies, original, pages, fase, query, inform, screening, process,
+            queries[id] = Query(id, cat, subcat, level, item, altitems, implies, original, pages, fase, query,
+                                inform, screening, process, literal,
                                 stars, filter, variants, unused1, unused2, comments)
             if queries[id].process in [post_process, form_process]:
                 postquerylist.append(id)
             lcitem = item.lower()
             lclevel = level.lower()
             if (lcitem, lclevel) in item2idmap:
                 settings.LOGGER.error('Duplicate (item, level) pair for {} and {}'.format(
```

### Comparing `sastadev-0.1.5/src/sastadev/reduceresults.py` & `sastadev-0.2.0/src/sastadev/reduceresults.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from collections import Counter
 from typing import Any, Dict, List
 
-from sastadev.allresults import AllResults
+from sastadev.allresults import (AllResults, ExactResultsDict, MatchesDict,
+                                 ResultsKey)
 from sastadev.methods import lastuttqidcondition, maxsamplesize
-from sastadev.sastatypes import (AnalysedTrees, ExactResultsDict, FileName,
-                                 Matches, MatchesDict, MethodName, Position,
-                                 QId, ResultsCounter, ResultsDict,
+from sastadev.sastatypes import (AnalysedTrees, FileName, Matches, MethodName,
+                                 Position, QId, ResultsCounter, ResultsDict,
                                  SampleSizeTuple, UttId, UttWordDict)
 from sastadev.treebankfunctions import getnodeyield
 
 
 def exact2results(exactresults: ExactResultsDict) -> ResultsDict:
     """
     :param exactresults: dictionary key= queryid, value is a list of (uttid, position) pairs
     :return: dictionary (key=queryid, value is a Counter uttid: count)
     """
     results: ResultsDict = {}
-    for qid in exactresults:
-        uttidlist = [uttid for (uttid, _) in exactresults[qid]]
+    for reskey in exactresults:
+        uttidlist = [uttid for (uttid, _) in exactresults[reskey]]
         resultvalue = Counter(uttidlist)
-        results[qid] = resultvalue
+        results[reskey] = resultvalue
     return results
 
 
 def reduceallresults(allresults: AllResults, samplesizetuple: SampleSizeTuple, methodname: MethodName) -> AllResults:
     '''
     reduces *allresults* by taking into account the samplesizetuple
     :param allresults:
@@ -37,29 +37,29 @@
         return allresults
     elif maxuttcount is not None and uttcount < maxuttcount:
         return allresults
     elif allresults.annotationinput:
         newexactresults: ExactResultsDict = reduceexactresults(allresults.exactresults,
                                                                uttidlist, cutoffpoint, methodname)  # done
         newcoreresults: Dict[QId, ResultsCounter] = exact2results(
-            newexactresults)   # done
+            newexactresults)  # done
         newallutts: UttWordDict = reduceallutts(
             allresults.allutts, uttidlist)  # done
         newallresults = AllResults(allresults.uttcount, newcoreresults, newexactresults, allresults.postresults,
                                    allresults.allmatches, allresults.filename, allresults.analysedtrees,
                                    newallutts, allresults.annotationinput)
     else:
 
         newuttcount: int = len(uttidlist)  # done
         newexactresults: ExactResultsDict = reduceexactresults(allresults.exactresults,
                                                                uttidlist, cutoffpoint, methodname)  # done
-        newcoreresults: Dict[QId, ResultsCounter] = exact2results(
-            newexactresults)   # done
+        newcoreresults: Dict[ResultsKey, ResultsCounter] = exact2results(
+            newexactresults)  # done
         # @@ I assume these need no change
-        newpostresults: Dict[QId, Any] = allresults.postresults
+        newpostresults: Dict[ResultsKey, Any] = allresults.postresults
         newallmatches: MatchesDict = reducematches(
             allresults.allmatches, uttidlist, cutoffpoint, methodname)  # done
         newfilename: FileName = allresults.filename  # done
         newanalysedtrees: AnalysedTrees = reduceanalysedtrees(
             allresults.analysedtrees, uttidlist)  # done
         newallutts: UttWordDict = reduceallutts(
             allresults.allutts, uttidlist)  # done
@@ -71,63 +71,64 @@
 
 
 def reduceexactresults(exactresultsdict: Dict[QId, ExactResultsDict], uttidlist: List[UttId],
                        cutoffpoint: Position, methodname: MethodName) -> Dict[QId, ResultsCounter]:
     newexactresultsdict = {}
     lastuttid = uttidlist[-1]
 
-    for qid in exactresultsdict:
+    for reskey in exactresultsdict:
         newexactresults = []
-        for uttid, position in exactresultsdict[qid]:
+        for uttid, position in exactresultsdict[reskey]:
             if (uttid in uttidlist and uttid != lastuttid) or \
-               (uttid == lastuttid and cutoffpoint is not None
-                    and not (position > cutoffpoint) and lastuttqidcondition[methodname](qid)):
+                    (uttid == lastuttid and cutoffpoint is not None and
+                     not (position > cutoffpoint) and lastuttqidcondition[methodname](reskey)):
                 newexactresults.append((uttid, position))
-        newexactresultsdict[qid] = newexactresults
+        newexactresultsdict[reskey] = newexactresults
     return newexactresultsdict
 
 
 def reduceresults(resultsdict: Dict[QId, Counter], samplesizetuple: SampleSizeTuple, methodname: MethodName):
     (uttidlist, wordcount, cutoffpoint) = samplesizetuple
     uttcount = len(uttidlist)
     maxuttcount, maxwordcount = maxsamplesize[methodname].maxuttcount, maxsamplesize[methodname].maxwordcount
     if wordcount is not None and maxwordcount is not None and wordcount < maxwordcount:
         newresultsdict = resultsdict
     elif maxuttcount is not None and uttcount <= maxuttcount:
         newresultsdict = resultsdict
     else:
         newresultsdict = {}
         lastuttid = uttidlist[-1]
-        for qid in resultsdict:
+        for reskey in resultsdict:
             newresults = []
-            for uttid in resultsdict[qid]:
+            for uttid in resultsdict[reskey]:
                 if (uttid in uttidlist and uttid != lastuttid) or \
-                        (uttid == lastuttid and lastuttqidcondition[methodname](qid)):  # no condition on the position, we have no info on it
+                        (uttid == lastuttid and lastuttqidcondition[methodname](
+                            reskey)):  # no condition on the position, we have no info on it
                     newresults.append(uttid)
-            newresultsdict[qid] = Counter(newresults)
+            newresultsdict[reskey] = Counter(newresults)
     return newresultsdict
 
 
 def reducematches(matchesdict: MatchesDict, uttidlist: List[UttId], cutoffpoint: Position,
                   methodname: MethodName) -> MatchesDict:
     newmatchesdict = {}
     lastuttid = uttidlist[-1]
-    for qid, uttid in matchesdict:
+    for reskey, uttid in matchesdict:
         if uttid in uttidlist and uttid != lastuttid:
-            newmatchesdict[(qid, uttid)] = matchesdict[(qid, uttid)]
+            newmatchesdict[(reskey, uttid)] = matchesdict[(reskey, uttid)]
         else:
-            if uttid == lastuttid and lastuttqidcondition[methodname](qid):
+            if uttid == lastuttid and lastuttqidcondition[methodname](reskey):
                 newmatches: Matches = []
-                for match in matchesdict[(qid, uttid)]:
+                for match in matchesdict[(reskey, uttid)]:
                     (m, tree) = match
                     treeyield = getnodeyield(tree)
                     lefttreeyield = treeyield[: cutoffpoint]
                     if m in lefttreeyield:
                         newmatches.append((m, tree))
-                newmatchesdict[(qid, uttid)] = newmatches
+                newmatchesdict[(reskey, uttid)] = newmatches
 
     return newmatchesdict
 
 
 def reduceanalysedtrees(analysedtrees: AnalysedTrees, uttidlist: List[UttId]) -> AnalysedTrees:
     newtrees = []
     for uttid, tree in analysedtrees:
```

### Comparing `sastadev-0.1.5/src/sastadev/resultsbyutterance.py` & `sastadev-0.2.0/src/sastadev/resultsbyutterance.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/rpf1.py` & `sastadev-0.2.0/src/sastadev/rpf1.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/sasta_explanation.py` & `sastadev-0.2.0/src/sastadev/sasta_explanation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,64 @@
-
 import copy
 from typing import List, Optional
 
-from auchann.align_words import align_words
+from auchann.align_words import AlignmentSettings, align_words
 from lxml import etree
 
 # import find1, iswordnode, getattval
 import sastadev.stringfunctions as strf
 import sastadev.treebankfunctions as tbf
-from sastadev.auchannsettings import AlignmentSettings
 from sastadev.auchannsettings import settings as auchannsettings
 from sastadev.cleanCHILDEStokens import cleantext
-from sastadev.conf import settings
+from sastadev.conf import settings as sdsettings
 from sastadev.lexicon import known_word
-from sastadev.metadata import (MetaValue, bpl_node, bpl_word, fromElement,
+from sastadev.metadata import (MetaValue, bpl_replacement, fromElement,
                                mkSASTAMeta)
 from sastadev.sastatok import gettokensplusxmeta
+# import find1, iswordnode, getattval
+# import find1, iswordnode, getattval
 from sastadev.sastatoken import Token
 from sastadev.sastatypes import SynTree
 from sastadev.tokenmd import TokenListMD
 
 # import CHAT_Annotation as schat  # put off because it causes an error: AttributeError: module 'CHAT_Annotation' has no attribute 'wordpat'
 
 defaultsettings = AlignmentSettings()
 
 sentenceinitialconjunctions = {'en', 'maar'}
 # interjections = ['hee', 'hè', 'ja', 'nee', 'kijk']
 # interjections used for sentence initial words that can be absent in te beginning of a correction
-interjections = ['ja', 'nee', 'kijk', 'oh', 'he', 'hoor', 'hè', 'o', 'hee', 'mama', 'okee', 'hé', 'ah', 'oeh', 'au', 'oja', 'joh', 'jee', 'mam', 'bah', 'jawel', 'mamma', 'ho', 'boem', 'ha', 'sorry',
-                 'ooh', 'daag', 'haha', 'nou', 'papa', 'pappa', 'toe', 'maar', 'oei', 'aah', 'hallo', 'dankjewel', 'oeps', 'oo', 'toch', 'wauw', 'goh', 'aha', 'vooruit', 'dan', 'tjonge',
-                 'hèhè', 'jaja', 'hoi', 'waar', 'bb', 'help', 'meneer', 'hi', 'ach', 'ee', 'hup', 'oooh', 'heh', 'm', 'ma', 'sst', 'och', 'tja', 'lieverd', 'hahaha', 'hoera', 'pap',
-                 'echt', 'lalala', 'hopla', 'da', 'pff', 'hai', 'jongens', 'juffrouw', 'jeetje', 'tot', 'ziens', 'hihi', 'jonge', 'ohh', 'poeh', 'oef',
-                 'meisje', 'aaah', 'auw', 'meid', 'niet', 'poe', 'en', 'schat', 'wel', 'ai', 'goed', 'xxxx', 'dat', 'doei', 'tjongejonge', 'ooooh', 'hoewel',
-                 'oke', 'neenee', 'pfff', 'mens', 'ps', 'oow', 'fff', 'juf', 'mevrouw', 'baby', 'dankuwel', 'waw', 'welterusten', 'sehhahahaha', 'hihihi', 'aaaah', 'wee', 'shit',
-                 'pa', 'grr', 'weltrusten', 'pats', 'weh', 'stouterd', 'dag', 'joepie', 'neej', 'hoho', 'rara', 'joehoe', 'schatje', 'hierzo', 'pffff', 'ahh', 'ahah', 'tjee',
-                 'liefje', 'pf', 'ahaha', 'hoppa', 'ahahaha', 'verdorie', 'ssst', 'foei', 'gossie', 'ok', 'joe', 'tsja', 'gatverdamme', 'grrr', 'welnee', 'god', 'tjeetje', 'doeg',
-                 'wah', 'getver', 'ohja', 'hej', 'zak', 'alhoewel', 'neen', 'goedzo', 'ahahah', 'allee', 'jo', 'jongen', 'pardon', 'hihihihi', 'floep', 'lieve', 'gatver', 'kut', 'bro',
-                 'mja', 'tsjonge', 'hohoho', 'klopt', 'man', 'jezus', 'truste', 'ppf', 'goedemorgen', 'domoor', 'aaaaah', 'okeee', 'yes', 'ahahahaha']
+interjections = ['ja', 'nee', 'kijk', 'oh', 'he', 'hoor', 'hè', 'o', 'hee', 'mama', 'okee', 'hé', 'ah', 'oeh', 'au',
+                 'oja', 'joh', 'jee', 'mam', 'bah', 'jawel', 'mamma', 'ho', 'boem', 'ha', 'sorry',
+                 'ooh', 'daag', 'haha', 'nou', 'papa', 'pappa', 'toe', 'maar', 'oei', 'aah', 'hallo', 'dankjewel',
+                 'oeps', 'oo', 'toch', 'wauw', 'goh', 'aha', 'vooruit', 'dan', 'tjonge',
+                 'hèhè', 'jaja', 'hoi', 'waar', 'bb', 'help', 'meneer', 'hi', 'ach', 'ee', 'hup', 'oooh', 'heh', 'm',
+                 'ma', 'sst', 'och', 'tja', 'lieverd', 'hahaha', 'hoera', 'pap',
+                 'echt', 'lalala', 'hopla', 'da', 'pff', 'hai', 'jongens', 'juffrouw', 'jeetje', 'tot', 'ziens', 'hihi',
+                 'jonge', 'ohh', 'poeh', 'oef',
+                 'meisje', 'aaah', 'auw', 'meid', 'niet', 'poe', 'en', 'schat', 'wel', 'ai', 'goed', 'xxxx', 'dat',
+                 'doei', 'tjongejonge', 'ooooh', 'hoewel',
+                 'oke', 'neenee', 'pfff', 'mens', 'ps', 'oow', 'fff', 'juf', 'mevrouw', 'baby', 'dankuwel', 'waw',
+                 'welterusten', 'sehhahahaha', 'hihihi', 'aaaah', 'wee', 'shit',
+                 'pa', 'grr', 'weltrusten', 'pats', 'weh', 'stouterd', 'dag', 'joepie', 'neej', 'hoho', 'rara',
+                 'joehoe', 'schatje', 'hierzo', 'pffff', 'ahh', 'ahah', 'tjee',
+                 'liefje', 'pf', 'ahaha', 'hoppa', 'ahahaha', 'verdorie', 'ssst', 'foei', 'gossie', 'ok', 'joe', 'tsja',
+                 'gatverdamme', 'grrr', 'welnee', 'god', 'tjeetje', 'doeg',
+                 'wah', 'getver', 'ohja', 'hej', 'zak', 'alhoewel', 'neen', 'goedzo', 'ahahah', 'allee', 'jo', 'jongen',
+                 'pardon', 'hihihihi', 'floep', 'lieve', 'gatver', 'kut', 'bro',
+                 'mja', 'tsjonge', 'hohoho', 'klopt', 'man', 'jezus', 'truste', 'ppf', 'goedemorgen', 'domoor',
+                 'aaaaah', 'okeee', 'yes', 'ahahahaha']
 fillers = ['eh', 'ehm', 'ah', 'boe', 'hm', 'hmm',
            'uh', 'uhm', 'ggg', 'mmm', 'ja', 'nee']
 allfillers = fillers + ['&-' + filler for filler in fillers] + \
     interjections + ['&-' + intj for intj in interjections]
 fragments = ['o.', 't', 's', 'n', 'k', 'a.', 'a', 'i', 's.', 'd', 'n.', 'e.', 'w', 'h', 'b', 'v.', 'p', 'z', 'r',
              'l', 'f', 'm.', 'g.', '@', 'w.', 'y', 'g', 'j', 'j.', 'b.', 'k.', 'v', 'h.', 'z.', 'c.', 'f.', 'i.', 'e'] \
     + defaultsettings.fragments
 
-
 space = ' '
 CHAT_explanation = 'Explanation'
 explannwordlistxpath = f'.//xmeta[@name="{CHAT_explanation}"]/@annotationwordlist'
 explannposlistxpath = f'.//xmeta[@name="{CHAT_explanation}"]/@annotationposlist'
 
 interpunction = '.,;?!'
 
@@ -80,18 +89,18 @@
             newword = newwordlist[0]
             oldwordpos = tokenposlist[0]
             oldword = oldwordlist[0]
             newtoken = Token(newword, oldwordpos)
             oldtoken = Token(oldword, oldwordpos)
             if known_word(newword):
                 newtokens = tokenreplace(newtokens, newtoken)
-                bpl = bpl_node if known_word(oldword) else bpl_word
+                # bpl = bpl_node if known_word(oldword) else bpl_word
                 meta = mkSASTAMeta(oldtoken, newtoken, name='ExplanationasReplacement',
                                    value='ExplanationasReplacement',
-                                   cat='Lexical Error', backplacement=bpl)
+                                   cat='Lexical Error', backplacement=bpl_replacement)
                 newmetadata.append(meta)
                 result = TokenListMD(newtokens, newmetadata)
     return result
 
 
 def islet(token, tree):
     tbf.showtree(tree, 'tree bij islet')
@@ -100,22 +109,21 @@
     result = tbf.getattval(node, 'pt') == 'let'
     return result
 
 # def finaltokenmultiwordexplanation(tokensmd: TokenListMD, tree: SynTree) -> Optional[str]:
 
 
 def finaltokenmultiwordexplanation(tree: SynTree) -> Optional[str]:
-
     # get the multiword explanation and the last tokenposition it occupies
 
     # it is assumed that the chat annotations have not been extracted and no metadata have been produced
     xtokens, xmetalist = gettokensplusxmeta(tree)
 
     result = None
-#    origmetadata = tokensmd.metadata
+    #    origmetadata = tokensmd.metadata
     origmetadata = xmetalist
     explanations = [xm for xm in xmetalist if xm.name == 'Explanation']
     finalmwexplanations = []
     for xm in explanations:
         lxm = len(xm.annotationwordlist)
         lastxmpos = xm.annotationposlist[-1]
         postexplanationtokens = [
@@ -127,15 +135,16 @@
 
         if len(resttokens) >= 2 and resttokens[0].word.lower() in allfillers and \
                 resttokens[1].word.lower() in interpunction and len(xm.annotationwordlist) >= 1 and \
                 resttokens[0].word.lower() != xm.annotationwordlist[0].lower():
             prefixtokens = resttokens[0:2]
             todoxtokens = resttokens[2:]
         elif len(resttokens) >= 1 and \
-                (resttokens[0].word.lower() in allfillers or resttokens[0].word.lower() in sentenceinitialconjunctions) and \
+                (resttokens[0].word.lower() in allfillers or resttokens[
+                    0].word.lower() in sentenceinitialconjunctions) and \
                 len(xm.annotationwordlist) >= 1 and resttokens[0].word.lower() != xm.annotationwordlist[0].lower():
             prefixtokens = resttokens[0:1]
             todoxtokens = resttokens[1:]
         else:
             prefixtokens = []
             todoxtokens = resttokens
 
@@ -168,15 +177,14 @@
         result = None
         # report an error
 
     return result
 
 
 def finalmultiwordexplanation(stree: SynTree) -> Optional[str]:
-
     # get the multiword explanation and the last tokenposition it occupies
 
     explannwrdliststr = tbf.find1(stree, explannwordlistxpath)
     # print(explannwrdliststr)
     explannwrdlist = strf.string2list(explannwrdliststr, quoteignore=True)
     # print(explannwrdlist)
 
@@ -246,15 +254,15 @@
 
 def finalexplanation_adapttreebank(treebank):
     newtreebank = etree.Element('treebank')
     for tree in treebank:
         newtree = finalexplanation_adapttree(tree)
         if newtree is None:
             newtreebank.append(tree)
-            settings.LOGGER.warning('Final Explanation correction failed')
+            sdsettings.LOGGER.warning('Final Explanation correction failed')
         else:
             newtreebank.append(newtree)
     return newtreebank
 
 
 def finalexplanation_adapttree(tree: SynTree) -> SynTree:
     # @@TODO: Unfinished@@
@@ -265,15 +273,15 @@
 
         # get the original meta data:
         intreemetadataxml = tree.xpath('.//meta')
         intreemetadata = []
         for el in intreemetadataxml:
             newmeta = fromElement(el)
             intreemetadata.append(newmeta)
-#        intreemetadata = [fromElement(el) for el in intreemetadataxml]
+        #        intreemetadata = [fromElement(el) for el in intreemetadataxml]
 
         # adapt the metadata
         newmetadata = []
         for meta in intreemetadata:
             if meta.uel == 'origutt':
                 newmeta = MetaValue('pre_origutt', 'text', meta.text)
                 newmetadata.append(newmeta)
@@ -285,23 +293,23 @@
         # clean the alignment
         cleanutttokens, chatmetadata = cleantext(
             alignment, False, tokenoutput=True)
 
         newmetadata += chatmetadata
         cleanutt = space.join([token.word for token in cleanutttokens])
 
-        newtree = settings.PARSE_FUNC(cleanutt)
+        newtree = sdsettings.PARSE_FUNC(cleanutt)
         sentelem = tbf.find1(tree, './/sentence')
         sentid = sentelem.attrib['sentid']
         newsentelem = tbf.find1(newtree, './/sentence')
         newsentelem.attrib['sentid'] = sentid
         # tbf.showtree(newtree, 'newly parsed tree')
         if newtree is None:
             newtree = tree
-            settings.LOGGER.warning(
+            sdsettings.LOGGER.warning(
                 'Parsing for <{cleanutt}> failed. No changes applied')
         else:
             newmetaelements = [meta.toElement() for meta in newmetadata]
             newmetadataElement = etree.Element('metadata')
             for newmetaelement in newmetaelements:
                 newmetadataElement.append(newmetaelement)
```

### Comparing `sastadev-0.1.5/src/sastadev/sastatok.py` & `sastadev-0.2.0/src/sastadev/sastatok.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 from typing import List, Tuple
 
+import sastadev
 import sastadev.CHAT_Annotation as sastachat
 import sastadev.cleanCHILDEStokens
 from sastadev.metadata import Meta
 # from CHAT_Annotation import CHAT_patterns, interpunction, wordpat
 from sastadev.sastatoken import Token, stringlist2tokenlist
 from sastadev.sastatypes import SynTree
 from sastadev.treebankfunctions import find1
@@ -40,15 +41,14 @@
 # overlap follows p. 71
 # overlap precedes p. 71
 # p73 should actually cover the number of words inside the scope
 repetition = scopeorword + r'\s*\[/\]\s*' + word
 retracing = scopeorword + r'\s*\[//\]\s*' + word  # p73
 whitespace = r'\s+'
 
-
 # sastaspecials = [r'\[::', r'\[=', r'\[:', r'\[=\?', r'\[x', r'\<', r'\>', r'\[\?\]', r'\[/\]', r'\[//\]', r'\[///\]', r'\[%', r'\]']
 sastaspecials = list(sastachat.CHAT_patterns)
 sastapatterns = sorted(sastaspecials, key=lambda x: len(
     x), reverse=True) + [word, sastachat.interpunction]
 fullsastapatterns = alts(sastapatterns)
 fullsastare = re.compile(fullsastapatterns)
```

### Comparing `sastadev-0.1.5/src/sastadev/sastatoken.py` & `sastadev-0.2.0/src/sastadev/sastatoken.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/sentence_parser.py` & `sastadev-0.2.0/src/sastadev/sentence_parser.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/smallclauses.py` & `sastadev-0.2.0/src/sastadev/smallclauses.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 adjective.
 
 For this reason this module inserts an appropriate finite verb into these utterances. This modified utterance with
 a finite verb can be analysed by Alpino. In the resulting parse, SASTA removes the verb
 again and the resulting parse tree is subjected to the queries for analysis.
 
 For example, by inserting the finite verb *moeten* in the utterance *schoenen aan*,
-resuting in *schoenen moeten aan*, *schoenen* can be analysed as a subject noun and *aan* as predicative adjective,
+resulting in *schoenen moeten aan*, *schoenen* can be analysed as a subject noun and *aan* as predicative adjective,
 and the whole utterance as an instance of TARSP *OndVC*.
 
 The small clause utterances are often very short, and we analysed utterances with 2
 and 3 "real" words,  "real" in the sense that we excluded interjections, filled pauses,
 interpunction signs, CHAT codes such as *xxx*, etc.
 
 The different subcases are dealt with by the function *smallclauses*:
@@ -187,15 +187,15 @@
     return result
 
 
 def locadv(node):
     result = getattval(node, 'pt') in ['bw', 'vz']
     frame = getattval(node, 'frame')
     result = result and ('loc' in frame or 'er_adverb' in frame)
-    result = result or rpronoun(node)
+    result = result or (rpronoun(node) and getattval(node, 'lemma') != 'er')   # in samll clauses predicates are no clitics
     return result
 
 
 def biglocvz(node):
     result = getattval(node, 'lemma') in biglocvzs
     return result
```

### Comparing `sastadev-0.1.5/src/sastadev/smartcompoundcomparison.py` & `sastadev-0.2.0/src/sastadev/smartcompoundcomparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,26 @@
 This module provides a function to determine whether an illegal word is to be considered as a compound,
 based on its correction and the lemma of its correction.
 It works for nouns only!
 
 '''
 import editdistance
 
-# from sastadev.normalise_lemma import normaliselemma
+from sastadev.normalise_lemma import normaliselemma
 
 
 def reldistance(word, corr):
     thedistance = editdistance.distance(word, corr)
     result = thedistance / max(len(word), len(corr))
     return result
 
 
 def iscompound(word, corr, rawcorrlemma):
     debug = False
-    corrlemma = rawcorrlemma
-    # corrlemma = normaliselemma(corr, rawcorrlemma, keeplastsep=True) TODO: fix
+    corrlemma = normaliselemma(corr, rawcorrlemma, keeplastsep=True)
     corrlemmaparts = corrlemma.split('_')
     if len(corrlemmaparts) == 1:
         return False
     corrlemmaprefixlist = corrlemmaparts[:-1]
     corrlemmaprefix = ''.join(corrlemmaprefixlist)
     lcorrlemmaprefix = len(corrlemmaprefix)
     corrdistance = editdistance.distance(word, corr)
```

### Comparing `sastadev-0.1.5/src/sastadev/stapforms.py` & `sastadev-0.2.0/src/sastadev/stapforms.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import os
 from collections import defaultdict
 from io import BytesIO
 from shutil import copyfile, copyfileobj
 
 from openpyxl import load_workbook
 
-from sastadev.allresults import AllResults
+from sastadev.allresults import AllResults, mkresultskey
 from sastadev.conf import settings
 from sastadev.forms import getformfilename
 
 scoresheetname = 'STAP 1 - 5'
 maxutt = 50
 zerocount = 0
 basexl = os.path.join(settings.SD_DIR, 'data', 'form_templates', 'STAP Excel VUmc 2018.xlsx')
 
-NS = 'S001'
-OS = 'S002'
-PV = 'S003'
-SGG = 'S004'
-VT = 'S005'
-VD = 'S006'
-N = 'S007'
-BvBep = 'S008'
-zelfvnw3 = 'S009'
-BBp = 'S010'
-BBt = 'S011'
-BBo = 'S012'
+NS = mkresultskey('S001')
+OS = mkresultskey('S002')
+PV = mkresultskey('S003')
+SGG = mkresultskey('S004')
+VT = mkresultskey('S005')
+VD = mkresultskey('S006')
+N = mkresultskey('S007')
+BvBep = mkresultskey('S008')
+zelfvnw3 = mkresultskey('S009')
+BBp = mkresultskey('S010')
+BBt = mkresultskey('S011')
+BBo = mkresultskey('S012')
 
 AG = 33
 Ucol = 21
 AF = 32
 
 # order in the Excel sheet: NS	OS	PV	SGG	VT	VD	N	BvBep	zelf. vnw. 3	BB p	BB t	BB o
 # i.e.
```

### Comparing `sastadev-0.1.5/src/sastadev/stringfunctions.py` & `sastadev-0.2.0/src/sastadev/stringfunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,25 +23,25 @@
 aiguvowels = 'áéíóúý'
 gravevowels = 'àèìòù\u00FD'
 tremavowels = 'äëïöüÿ'
 circumflexvowels = 'âêîôû\u0177'
 
 consonants = 'bcdfghjklmnpqrstvwxz\u00E7'  # \u00E7 is c cedilla
 dutch_base_vowels = barevowels + aiguvowels + \
-    gravevowels + tremavowels + circumflexvowels
+                    gravevowels + tremavowels + circumflexvowels
 vowels = dutch_base_vowels
 dutch_base_diphthongs = ['aa', 'ee', 'ie', 'oo',
                          'uu', 'ij', 'ei', 'au', 'ou', 'ui', 'eu', 'oe']
 dutch_y_diphthongs = ['y' + d for d in dutch_base_vowels] + [d + 'y' for d in
                                                              dutch_base_vowels]  # ryen gaat nog fout ye alleen samen nemen aan begin van woord
 dutch_y_triphthongs = ['y' + d for d in dutch_base_diphthongs] + \
-    [d + 'y' for d in dutch_base_diphthongs]
+                      [d + 'y' for d in dutch_base_diphthongs]
 dutch_trema_diphthongs = ['äa', "ëe", 'ïe', 'öo', 'üu', 'ëi']
 dutch_diphthongs = dutch_base_diphthongs + \
-    dutch_y_diphthongs + dutch_trema_diphthongs
+                   dutch_y_diphthongs + dutch_trema_diphthongs
 dutch_base_triphthongs = ['aai', 'eeu', 'ooi', 'oei']
 dutch_y_tetraphthongs = ['y' + d for d in dutch_base_triphthongs]
 dutch_triphthongs = dutch_base_triphthongs + dutch_y_triphthongs
 dutch_tetraphthongs = dutch_y_tetraphthongs
 foreign_triphthongs = ['eau', 'oeu']
 
 hyphenprefixes = ['anti', 'contra', 'ex']
@@ -98,15 +98,15 @@
 consonants_star = star(charrange(consonants))
 
 syllableheadspat = alt([alt(dutch_tetraphthongs), alt(
     dutch_triphthongs), alt(dutch_diphthongs), alt(vowels)])
 syllableheadsre = re.compile(syllableheadspat)
 
 monosyllabicpat = r'^' + consonants_star + \
-    syllableheadspat + consonants_star + r'$'
+                  syllableheadspat + consonants_star + r'$'
 monosyllabicre = re.compile(monosyllabicpat)
 
 
 def barededup(word: str) -> str:
     '''
     The function barededup takes as input a string and
     returns a string in which  sequences of the same character are reduced to a single instance of this character
```

### Comparing `sastadev-0.1.5/src/sastadev/sva.py` & `sastadev-0.2.0/src/sastadev/sva.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/syllablecount.py` & `sastadev-0.2.0/src/sastadev/syllablecount.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 ouillpattern = r'(ou)(i)(ll)'
 ouillre = re.compile(ouillpattern)
 
 ieuwpattern = r'([EeIi]e)(u)(w)'
 ieuwre = re.compile(ieuwpattern)
 
-
 syllable_exception_dictionary = {
     'cacao': 2, 'cue': 1, 'camargue': 3, 'bye': 1, 'Paraguay': 3}
 syll1vseqs = ['aau', 'ai', 'ay', 'eoi', 'eui', 'ey', 'eau',
               'oeu', 'oey', 'oi', 'ooy', 'oy', 'uay', 'uei', 'uy']
 syll2vseqs = ['aaa', 'aaia', 'aaie', 'aaiee', 'aaii', 'aaio', 'aaioe', 'ae', 'aea', 'aee', 'aeo', 'aeu',
               'aia', 'aie', 'aii', 'aio', 'ao', 'aoe', 'aoo', 'aou', 'aue', 'ayee', 'ayeu', 'ea', 'eaa',
               'eaai', 'eae', 'eai', 'eea', 'eeaa', 'eeau', 'eee', 'eeee', 'eeei', 'eei', 'eeie', 'eeo',
@@ -36,15 +35,14 @@
               'oeiee', 'oeii', 'oeio', 'oeo', 'oeoo', 'oia', 'oie', 'ooe', 'ooia', 'ooiau', 'ooie', 'ooiee',
               'ooii', 'ooio', 'ooioo', 'oua', 'ouai', 'oue', 'ouee', 'oui', 'oyaa', 'oyau', 'oyee', 'oyeu',
               'ua', 'uaa', 'uai', 'ue', 'uee', 'ueu', 'uia', 'uiaa', 'uie', 'uii', 'uo', 'uoo', 'ya', 'yaa',
               'ye', 'yi', 'yo', 'yoo']
 syll3vseqs = ['aaieo', 'aaieoo', 'aoi', 'eao', 'eeeie',
               'eeeii', 'eoa', 'ioa', 'ioui', 'oeieo', 'oeieoo']
 
-
 voweltierpattern = f'[{vowels}]+'
 voweltierre = re.compile(voweltierpattern)
 
 vowelyvowels = [f'{v1}y{v2}' for v1 in vowels for v2 in vowels]
 
 vowelsyllpairs = [(1, dutch_base_diphthongs + dutch_trema_diphthongs + dutch_base_triphthongs + syll1vseqs),
                   (2, vowelyvowels + syll2vseqs),
@@ -111,26 +109,28 @@
     for i, char in enumerate(word):
         if char in tremavowels:
             return i
     return -1
 
 
 def test1():
-    wordlist = ['B-kant', 'ABC-biljet', 'A-B-C-actie', 'cue', 'aan', 'na', 'baan', 'cadeau', 'chaos', 'naäpen', 'be-edigen', 'haaibaai', 'iaen', 'iaën',
+    wordlist = ['B-kant', 'ABC-biljet', 'A-B-C-actie', 'cue', 'aan', 'na', 'baan', 'cadeau', 'chaos', 'naäpen',
+                'be-edigen', 'haaibaai', 'iaen', 'iaën',
                 'eeuw', 'kieuw', ]
     for word in wordlist:
         vt = getvoweltier(word)
         print(word, vt)
         for vs in vt:
             cnt = vowelsyllcount(vs)
             print(f'---{vs}: {cnt}')
 
 
 def test2():
-    reflist = [('B-kant', 2), ('ABC-biljet', 3), ('A-B-C-actie', 5), ('cue', 1), ('aan', 1), ('na', 1), ('baan', 1), ('cadeau', 2), ('chaos', 2), ('naäpen', 3),
+    reflist = [('B-kant', 2), ('ABC-biljet', 3), ('A-B-C-actie', 5), ('cue', 1), ('aan', 1), ('na', 1), ('baan', 1),
+               ('cadeau', 2), ('chaos', 2), ('naäpen', 3),
                ('be-edigen', 4), ('haaibaai', 2), ('iaen',
                                                    2), ('iaën', 3), ('eeuw', 1), ('kieuw', 1),
                ('koeieoog', 3), ('expressfout', 2), ('desavoueer', 4)]
     fail = False
     cntr = 0
     for word, refcnt in reflist:
         cntr += 1
```

### Comparing `sastadev-0.1.5/src/sastadev/targets.py` & `sastadev-0.2.0/src/sastadev/targets.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/tarspform.py` & `sastadev-0.2.0/src/sastadev/tarspform.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import xlsxwriter
 
 from sastadev import xlsx
 from sastadev.conf import settings
 from sastadev.counterfunctions import counter2liststr
 from sastadev.forms import getformfilename
+from sastadev.allresults import mkresultskey
 
 ordA = ord('A')
 comma = ','
 xlsxext = '.xlsx'
 
 idpat = r'^[TSA][0-9]{3}$'
 idcpat = r'^[TSA][0-9]{3}c$'
@@ -113,21 +114,23 @@
 
     workbook = xlsxwriter.Workbook(target, {"strings_to_numbers": True})
     worksheet = workbook.add_worksheet()
 
     for (rowctr, colctr) in basesheet:
         curval = str(basesheet[(rowctr, colctr)])
         if is_id(curval):
-            newval = getval(allresults, curval)
+            curvalreskey = mkresultskey(curval)
+            newval = getval(allresults, curvalreskey)
             # write newval to the new sheet
             newvalstr = val2str(newval)
             worksheet.write(rowctr, colctr, newvalstr)
         elif is_idc(curval):
             urval = idc2id(curval)
-            newval = getval(allresults, urval)
+            urvalreskey = mkresultskey(urval)
+            newval = getval(allresults, urvalreskey)
             cval = len(newval)
             newvalstr = val2str(cval)
             worksheet.write(rowctr, colctr, newvalstr)
         else:
             worksheet.write(rowctr, colctr, curval)
 
     #formatting
```

### Comparing `sastadev-0.1.5/src/sastadev/tblex.py` & `sastadev-0.2.0/src/sastadev/tblex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-The module *tblex* contains functiond that require function
+The module *tblex* contains functions that require functions
 from the lexicon module and from the treebankfunctions module
 """
 
 import sastadev.lexicon as lex
 from sastadev.sastatypes import SynTree
 from sastadev.treebankfunctions import (all_lower_consonantsnode, getattval,
                                         is_duplicate_spec_noun, iscompound,
```

### Comparing `sastadev-0.1.5/src/sastadev/tokeniseCHILDES.py` & `sastadev-0.2.0/src/sastadev/tokeniseCHILDES.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/tokenmd.py` & `sastadev-0.2.0/src/sastadev/tokenmd.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/top3000.py` & `sastadev-0.2.0/src/sastadev/top3000.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/treebankfunctions.py` & `sastadev-0.2.0/src/sastadev/treebankfunctions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-'''
+"""
 various treebank functions
 
-'''
+"""
 
-# import sys
 import re
 # import logging
 from copy import copy, deepcopy
+# import sys
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from lxml import etree
 
+from sastadev.anonymization import pseudonymre
 # from sastadev.lexicon import informlexiconpos, isa_namepart_uc, informlexicon, isa_namepart
 # import lexicon as lex
 from sastadev.conf import settings
 from sastadev.metadata import Meta
 from sastadev.sastatoken import Token
 from sastadev.sastatypes import (FileName, OptPhiTriple, PhiTriple, Position,
                                  PositionMap, PositionStr, Span, SynTree,
                                  UttId)
 from sastadev.stringfunctions import allconsonants
 
+# from sastadev.tblex import recognised_wordnode, recognised_lemmanode, recognised_wordnodepos, recognised_lemmanodepos
+
 
 class Metadata:
-    '''
+    """
     contains 3 elements, each a string: type, name, value
-    '''
+    """
 
     def __init__(self, thetype, thename, thevalue):
         self.type = thetype
         self.name = thename
         self.value = thevalue
 
     def md2PEP(self):
@@ -114,64 +117,67 @@
 sentencexpathquery = "//sentence/text()"
 
 uniquecounter = 0
 
 countattvalxpathtemplate = 'count(.//node[@{att}="{val}"])'
 countcompoundxpath = 'count(.//node[contains(@lemma, "_")])'
 
+monthnames = ['januari', 'februari', 'maart', 'april', 'mei', 'juni', 'juli', 'augustus',
+              'september', 'oktober', 'november', 'december']
+
 
 def adjacent(node1: SynTree, node2: SynTree, stree: SynTree) -> bool:
-    '''
+    """
     :param node1:
     :param node2:
     :param stree: syntactic structure containing *node1* and *node2*
     :return: True if *node1* is adjacent to *node2* in *stree*, False otherwise
 
     The function *adjacent* determines whether *node1* is adjacent to *node1* in syntactic structure *stree*,
     and it works correctly in inflated syntactic structures. The two nodes must be nodes for words.
-    '''
+    """
     yieldnodes = getnodeyield(stree)
     for i, n in enumerate(yieldnodes):
         if yieldnodes[i] == node1:
             prec = yieldnodes[i - 1] if i > 0 else None
             succ = yieldnodes[i + 1] if i < len(yieldnodes) - 1 else None
             result = prec == node2 or succ == node2
             return result
     return False
 
 
 def immediately_precedes(node1: SynTree, node2: SynTree, stree: SynTree) -> bool:
-    '''
+    """
     :param node1:
     :param node2:
     :param stree: syntactic structure containing *node1* and *node2*
     :return: True if *node1* immediately precedes *node2* in *stree*, False otherwise
 
     The function *immediately_precedes* determines whether *node1* immediately precedes *node1* in syntactic structure *stree*,
     and it works correctly in inflated syntactic structures. The two nodes must be nodes for words.
-    '''
+    """
     yieldnodes = getnodeyield(stree)
     for i, n in enumerate(yieldnodes):
         if yieldnodes[i] == node1:
             succ = yieldnodes[i + 1] if i < len(yieldnodes) - 1 else None
             result = succ == node2
             return result
     return False
 
 
 def immediately_follows(node1: SynTree, node2: SynTree, stree: SynTree) -> bool:
-    '''
+    """
     :param node1:
     :param node2:
     :param stree: syntactic structure containing *node1* and *node2*
     :return: True if *node1* immediately follows *node2* in *stree*, False otherwise
 
     The function *immediately_follows* determines whether *node1* immediately follows *node1* in syntactic structure *stree*,
     and it works correctly in inflated syntactic structures. The two nodes must be nodes for words.
-    '''
+    """
     return immediately_precedes(node2, node1, stree)
 
 
 def countav(stree: SynTree, att: str, val: str) -> int:
     countattvalxpath = countattvalxpathtemplate.format(att=att, val=val)
     result = stree.xpath(countattvalxpath)
     return result
@@ -323,14 +329,15 @@
     if syntree is not None:
         for child in syntree:
             if child.tag == 'sentence':
                 if 'sentid' in child.attrib:
                     results = [child.attrib['sentid']]
     return results
 
+
 # put the next one in comments, see below for a different definition
 # def getsentid(syntree: SynTree) -> Optional[UttId]:
 #     result = getqueryresult(syntree, noxpathquery=noxpathsentid)
 #     return result
 
 
 def lastconstituentof(stree: SynTree) -> SynTree:
@@ -377,20 +384,20 @@
     else:
         for child in node:
             current = reclastmainclauseof(child, current)
         result = current
     return result
 
 
-def getrelchildof(node: SynTree, rel: str) -> SynTree:
-    '''
+def getrelchildof(node: SynTree, rel: str) -> Optional[SynTree]:
+    """
     gets the first child node with rel=rel under a node.
     It should always return a word node (so should have a pt attribute; it does not deal properly with conjunction
     :return: node with grammatical relation rel
-    '''
+    """
     if node is None:
         return None
     for child in node:
         chrel = getattval(child, 'rel')
         if chrel == rel:
             return child
     return None
@@ -428,21 +435,21 @@
 
 persons = ['persoon', '3p', '3m', '3v', '3o', '3', '2v', '2b', '2', '1']
 numbers = ['getal', 'ev', 'mv']
 genders = ['genus', 'onz', 'zijd', 'fem', 'masc']
 
 
 def valmerge(v1: str, v2: str, vallist: List[str]) -> str:
-    '''
+    """
     presupposes that v1 and v2 occur in the vallist
     :param v1:
     :param v2:
     :param vallist:
     :return:
-    '''
+    """
     v1ind = vallist.index(v1)
     v2ind = vallist.index(v2)
     newind = max(v1ind, v2ind)
     result = vallist[newind]
     return result
 
 
@@ -723,20 +730,20 @@
         else:
             resultlist.append(w)
         pos += 1
     return resultlist
 
 
 def addmetadata(stree: SynTree, meta: Metadata) -> SynTree:
-    '''
+    """
     adds  meta of class Metadata to stree
     :param stree:
     :param meta: type Metadata
     :return: stree
-    '''
+    """
     if stree is None:
         result = stree
     elif meta is None:
         result = stree
     else:
         metadatanodes = stree.xpath('//metadata')
         if metadatanodes == []:
@@ -767,61 +774,61 @@
         result = ssubfound
     else:
         result = False
     return result
 
 
 def iscompound(node: SynTree) -> bool:
-    '''
+    """
     The function *iscompound* determines whether a node is a node for a compound word.
     This is the case if the *lemma* attribute contains the compound separator
     *compoundsep*
 
     .. autodata:: treebankfunctions::compoundsep
-    '''
+    """
     lemma = getattval(node, 'lemma')
     result = compoundsep in lemma
     return result
 
 
 def isdiminutive(node: SynTree) -> bool:
-    '''
+    """
     The function *isdiminutive* checks whether *node* is  a node for diminutive word.
     This is the case if the attribute *graad* has the value *dim*.
 
-    '''
+    """
     graad = getattval(node, 'graad')
     result = graad == 'dim'
     return result
 
 
 def issubstantivised_verb(node: SynTree) -> bool:
-    '''
+    """
     The function *issubstantivised_verb* checks whether a node is a node for a
     substantivised verb (i.e. if *pt* = *ww* and *positie* = *nom*)
 
-    '''
+    """
     nodept = getattval(node, 'pt')
     nodepositie = getattval(node, 'positie')
     result = nodept == 'ww' and nodepositie == 'nom'
     return result
 
 
 def getsiblings(node: SynTree) -> List[SynTree]:
-    '''
+    """
     The function *getsiblings* returns the list of sibling nodes of *node*
 
-    '''
+    """
     parent = node.getparent()
     siblings = [n for n in parent if n != node]
     return siblings
 
 
 def showtn(tokennode: SynTree) -> str:
-    '''requires the node to be a node for a token (word)'''
+    """requires the node to be a node for a token (word)"""
     if tokennode is None:
         result = ''
     else:
         word = getattval(tokennode, 'word')
         position = getattval(tokennode, 'end')
         result = position + word
     return result
@@ -829,59 +836,59 @@
 
 def showtns(tokennodelist: List[SynTree]) -> str:
     result = space.join([showtn(tn) for tn in tokennodelist])
     return result
 
 
 def all_lower_consonantsnode(node: SynTree) -> bool:
-    '''
+    """
     The function *all_lower_consonantsnode* checks whether *node* is a node for a word
     that consists of all lower case consonants.
 
-    '''
+    """
     word = getattval(node, 'word')
     result = all([c.islower() for c in word])
     result = result and allconsonants(word)
     return result
 
 
 def sasta_long(node: SynTree) -> bool:
-    '''
+    """
     The function sasta_long checks whether the length of the *word* attribute of the
     node is greater or equal to *min_sasta_length*:
 
     .. autodata:: treebankfunctions::min_sasta_length
 
-    '''
+    """
     word = getattval(node, 'word')
     result = len(word) >= min_sasta_length
     return result
 
 
 def spec_noun(node: SynTree) -> bool:
-    '''
+    """
     The function *spec_noun* checks whether the node is node of *pt* *spec* which is a
     name or name part (as determined by the attributes *pos* and *frame*).
 
-    '''
+    """
     pt = getattval(node, 'pt')
     pos = getattval(node, 'pos')
     frame = getattval(node, 'frame')
     word = getattval(node, 'word')
     result = (pt == 'spec' and (
         pos == 'name' or frame.startswith('proper_name')))
     result = result and word[0].isupper()
     return result
 
 
 def is_duplicate_spec_noun(node: SynTree) -> bool:
-    '''
+    """
     The function *is_duplicate_spec_noun* checks whether there is any duplicate of the
     word among its siblings (ignoring case).
-    '''
+    """
     siblings = getsiblings(node)
     result = True
     word = getattval(node, 'word')
     lcword = word.lower()
     for sibling in siblings:
         siblingword = getattval(sibling, 'word')
         lcsiblingword = siblingword.lower()
@@ -890,83 +897,187 @@
 
 
 def onbvnwdet(node: SynTree) -> bool:
     result = getattval(node, 'lemma') in potentialdet_onbvnws
     return result
 
 
+# this function moved to tblex
+# def asta_recognised_lexnode(node: SynTree) -> bool:
+#     """
+#     The function *asta_recognised_lexnode* determines whether *node* should count as a
+#     lexical verb in the ASTA method.
+#
+#     This is the case if *pt* equals *ww* and the node is not a substantivised verb as
+#     determined by the function *issubstantivised_verb*:
+#
+#     .. autofunction:: treebankfunctions::issubstantivised_verb
+#
+#     """
+#     if issubstantivised_verb(node):
+#         result = False
+#     else:
+#         result = getattval(node, 'pt') == 'ww'
+#     return result
+
+
+def isspecdeeleigen(node: SynTree) -> bool:
+    pt = getattval(node, 'pt')
+    spectype = getattval(node, 'spectype')
+    result = pt == 'spec' and spectype == 'deeleigeb'
+    return result
+
+
+def ismonthname(node: SynTree) -> bool:
+    lemma = getattval(node, 'lemma')
+    result = lemma in monthnames
+    return result
+
+
+# this function moved to tblex
+# def asta_recognised_nounnode(node: SynTree) -> bool:
+#     """
+#     The function *asta_recognised_nounnode* determines whether *node* should count as a
+#     noun in the ASTA method.
+#
+#     This is the case if
+#
+#     * either the node meets the conditions of *sasta_pseudonym*
+#
+#        .. autofunction:: treebankfunctions::sasta_pseudonym
+#
+#     * or the node is part of name (pt = *spec*, spectype= *deeleigen*)
+#
+#        .. autofunction:: treebankfunctions::isspecdeeleigen
+#
+#     * or the node is a month name (these are not always nouns in Alpino)
+#
+#        .. autofunction:: treebankfunctions::ismonthname
+#
+#     * or the node meets the conditions of *spec_noun*
+#
+#        .. autofunction:: treebankfunctions::spec_noun
+#
+#     * or the node meets the conditions of *is_duplicate_spec_noun*
+#
+#        .. autofunction:: treebankfunctions::is_duplicate_spec_noun
+#
+#     * or the node meets the conditions of *sasta_long*
+#
+#        .. autofunction:: treebankfunctions::sasta_long
+#
+#     * or the node meets the conditions of *recognised_wordnodepos*
+#
+#        .. autofunction:: treebankfunctions::recognised_wordnodepos
+#
+#     * or the node meets the conditions of *recognised_lemmanodepos(node, pos)*
+#
+#        .. autofunction:: treebankfunctions::recognised_lemmanodepos(node, pos)
+#
+#     However, the node should:
+#
+#     * neither consist of lower case consonants only, as determined by *all_lower_consonantsnode*:
+#
+#        .. autofunction:: treebankfunctions::all_lower_consonantsnode
+#
+#     * nor satisfy the conditions of *short_nucl_n*:
+#
+#        .. autofunction:: treebankfunctions::short_nucl_n
+#
+#     """
+#
+#     if issubstantivised_verb(node):
+#         pos = 'ww'
+#     else:
+#         pos = 'n'
+#     result = sasta_pseudonym(node)
+#     result = result or isspecdeeleigen(node)
+#     result = result or ismonthname(node)
+#     result = result or spec_noun(node)
+#     result = result or is_duplicate_spec_noun(node)
+#     result = result or sasta_long(node)
+#     result = result or recognised_wordnodepos(node, pos)
+#     result = result or recognised_lemmanodepos(node, pos)
+#     result = result and not (all_lower_consonantsnode(node))
+#     result = result and not (short_nucl_n(node))
+#     return result
+
+# this function moved to tblex
+# def asta_recognised_wordnode(node: SynTree) -> bool:
+#     result = sasta_pseudonym(node)
+#     result = result or spec_noun(node)
+#     result = result or is_duplicate_spec_noun(node)
+#     result = result or sasta_long(node)
+#     result = result or recognised_wordnode(node)
+#     result = result or recognised_lemmanode(node)
+#     result = result or isnumber(node)
+#     result = result and not (all_lower_consonantsnode(node))
+#     result = result and not (short_nucl_n(node))
+#     return result
+
+
 def isnumber(node: SynTree) -> bool:
     word = getattval(node, 'word')
     thematch = numberre.match(word)
     result = thematch is not None
     return result
 
 
 def sasta_short(inval: str) -> bool:
-    '''
+    """
     The function *sasta_short* determines whether the string *inval* is short, i.e,
     with a length smaller or equal than *sasta_short_length*:
 
     .. autodata:: treebankfunctions::sasta_short_length
 
-    '''
+    """
     result = len(inval) <= sasta_short_length
     return result
 
 
 def short_nucl_n(node: SynTree) -> bool:
-    '''
+    """
     The function *short_nucl_n* determines whether *node* is a node for a word with
     *pt* equal to *n*, relation *nucl*, and whose *word* attribute is short (as
     determined by the  function *sasta_short*)
 
     .. autofunction:: treebankfunctions::sasta_short
-    '''
+    """
     pt = getattval(node, 'pt')
     rel = getattval(node, 'rel')
     word = getattval(node, 'word')
     result = pt == 'n' and rel == 'nucl' and sasta_short(word)
     return result
 
 
-#: The constant *sasta_pseudonyms* list the strings that replace names for
-#: pseudonymisation purposes.
-sasta_pseudonyms = ['NAAM', 'VOORNAAM', 'ACHTERNAAM', 'ZIEKENHUIS', 'STRAAT', 'PLAATS', 'PLAATSNAAM', 'KIND', 'BEROEP',
-                    'OPLEIDING']
-#: The constant *pseudonym_patternlist* contains regular expressions for pseudonyms
-#: based on elements from the *sasta_pseudonyms* (pseudonym + number).
-pseudonym_patternlist = [r'^{}\d?$'.format(el) for el in sasta_pseudonyms]
-pseudonym_pattern = vertbar.join(pseudonym_patternlist)
-pseudonymre = re.compile(pseudonym_pattern)
-
-
 def sasta_pseudonym(node: SynTree) -> bool:
-    '''
+    """
     The function *sasta_pseudonym* determines whether the *word* attribute of *node* is a SASTA pseudonym.
 
     It uses the *pseudonymre* regular expression, which is created by joining
     the pseudonym regular expressions of the *pseudonym_patternlist* as alternatives. the
     pseudonym regular
     expressions have been created using the constant sasta_pseudonyms:
 
     .. autodata:: treebankfunctions::sasta_pseudonyms
        :noindex:
 
     .. autodata:: treebankfunctions::pseudonym_patternlist
 
-    '''
+    """
     word = getattval(node, 'word')
     match = pseudonymre.match(word)
     result = match is not None
     return result
 
 
 nodeformat = '{}/{}{}'
 nodeformatplus = nodeformat + '['
 
+
 # @@need to add a variant that returns a string
 
 
 def simpleshow(stree: SynTree, showchildren: bool = True, newline: bool = True) -> None:
     simpleshow2(stree, showchildren)
     if newline:
         print()
@@ -1000,33 +1111,33 @@
             # print('top', end=' ')
             for child in stree:
                 simpleshow2(child)
             # print(']', end=' ')
 
 
 def showflatxml(elem: SynTree) -> str:
-    '''
+    """
 
     :param elem: xml element
     :return: string that represents the element and its immediate children
-    '''
+    """
     start = '<{}>'.format(elem.tag)
     end = '</{}>'.format(elem.tag)
     middle = ['<{}/>'.format(child.tag) for child in elem]
     middlestr = space.join(middle)
     result = start + middlestr + end
     return result
 
 
 def uniquenodes(nodelist: List[SynTree]) -> List[SynTree]:
-    '''
+    """
 
     :param nodelist: list of nodes all from a single syntactic structure
     :return: nodelist without duplicates. Two nodes are considered duplicates if the begin and end attributes are identical
-    '''
+    """
     done = []
     resultlist = []
     for node in nodelist:
         begin = getattval(node, 'begin')
         end = getattval(node, 'end')
         cover = begin, end
         if cover not in done:
@@ -1122,20 +1233,20 @@
         for node in stree.iter():
             if 'index' in node.attrib and not bareindexnode(node):
                 theindex = node.attrib['index']
                 indexednodes[theindex] = node
     return indexednodes
 
 
-def nodecopy(node: SynTree) -> SynTree:
-    '''
+def nodecopy(node: SynTree) -> Optional[SynTree]:
+    """
     The function *nodecopy* copies a node without its children
     :param node: node, an lxml.etree Element
     :return: a node with no children, otherwise a copy of the input node
-    '''
+    """
     if node is None:
         return None
     else:
         newnode = copy(node)
         for ch in newnode:
             newnode.remove(ch)
         return newnode
@@ -1143,40 +1254,41 @@
 
 def bareindexnode(node: SynTree) -> bool:
     result = node.tag == 'node' and terminal(node) and 'index' in node.attrib and \
         'word' not in node.attrib and 'lemma' not in node.attrib and 'cat' not in node.attrib
     # print(props2str(get_node_props(node)), result, file=sys.stderr)
     return (result)
 
+
 # herdefinieren want met UD hebben terminale nodes wel children (maar geen children met tag=node)
 
 
 def terminal(node: SynTree) -> bool:
     result = isinstance(
         node, etree._Element) and node is not None and len(node) == 0
     return result
 
 
 def oldindextransform(stree: SynTree) -> SynTree:
-    '''
+    """
     produces a new stree in which all index nodes are replaced by their antecedent nodes
     :param stree: input stree
     :return: stree with all index nodes replaced by the nodes of their antecedents
-    '''
+    """
 
     indexednodesmap = getindexednodesmap(stree)
     # for ind, tree in indexednodesmap.items():
     # print(ind)
     # etree.dump(tree)
     result = indextransform2(stree, indexednodesmap)
     return result
 
 
 def indextransform(stree: SynTree) -> SynTree:
-    '''
+    """
     :param stree: input stree
     :return: stree with all index nodes replaced by the nodes of their antecedents
 
     The function *indextransform* produces a new stree in which all index nodes are replaced by their antecedent nodes.
     It first gathers the antecedents of bare index nodes in a dictionary (*basicindexednodesmap*) of index-SynTree
     items by means of the function *getbasicindexednodesmap*.
 
@@ -1188,28 +1300,28 @@
 
     .. autofunction:: treebankfunctions::getindexednodesmap
 
     Finally, the input tree is transformed by the function *indextransform2*, which uses  *indexnodesmap*:
 
     .. autofunction:: treebankfunctions::indextransform2
 
-    '''
+    """
 
     basicindexednodesmap = getbasicindexednodesmap(stree)
     # for ind, tree in indexednodesmap.items():
     # print(ind)
     # etree.dump(tree)
     indexnodesmap = getindexednodesmap(basicindexednodesmap)
     result = indextransform2(stree, indexnodesmap)
     return result
 
 
 # deze robuust maken tegen andere nodes dan node (metadata, alpino_ds etc)
 # waarschijnlijk is node.tag == 'node'in baseindexnode voldoende
-def indextransform2(stree: SynTree, indexednodesmap: Dict[str, SynTree]) -> SynTree:
+def indextransform2(stree: SynTree, indexednodesmap: Dict[str, SynTree]) -> Optional[SynTree]:
     """
     The function *indextransform2* takes as input a syntactic structure *stree* and an index-SynTree dictionary.
     It creates a new tree in which each bare index node in *stree* with index *i* is replaced by its antecedent
     (i.e. indexednodesmap[i]), except for the grammatical relation attribute *rel*.
 
     :param stree: input syntactic structure
     :param indexednodesmap: dictionary with index - SynTree items. No bare index nodes occur in the syntactic structures
@@ -1237,15 +1349,15 @@
             for child in stree:
                 newchild = indextransform2(child, indexednodesmap)
                 newstree.append(newchild)
 
         return newstree
 
 
-def getstree(fullname: FileName) -> etree._ElementTree:
+def getstree(fullname: FileName) -> Optional[SynTree]:
     try:
         thefile = open(fullname, 'r', encoding='utf8')
     except FileNotFoundError as e:
         settings.LOGGER.error('File not found: {}'.format(e))
         return None
     except etree.ParseError as e:
         settings.LOGGER.error('Parse Error: {}; file: {}'.format(e, fullname))
@@ -1282,15 +1394,15 @@
             else:
                 return tree
         else:
             return tree
 
 
 streestrings = {}
-streestrings[1] = '''
+streestrings[1] = """
 <alpino_ds version="1.6">
   <parser cats="1" skips="5" />
   <node begin="0" cat="top" end="8" id="0" rel="top">
     <node begin="0" conjtype="neven" end="1" frame="complementizer(root)" his="robust_skip" id="1" lcat="--" lemma="en" pos="comp" postag="VG(neven)" pt="vg" rel="--" root="en" sc="root" sense="en" word="en"/>
     <node begin="1" end="2" frame="--" genus="zijd" getal="ev" graad="basis" his="robust_skip" id="2" lcat="--" lemma="uhm" naamval="stan" ntype="soort" pos="--" postag="N(soort,ev,basis,zijd,stan)" pt="n" rel="--" root="uhm" sense="uhm" word="uhm"/>
     <node begin="2" conjtype="neven" end="3" frame="conj(en)" his="robust_skip" id="3" lcat="--" lemma="en" pos="vg" postag="VG(neven)" pt="vg" rel="--" root="en" sense="en" word="en"/>
     <node begin="3" end="4" frame="--" genus="zijd" getal="ev" graad="basis" his="robust_skip" id="4" lcat="--" lemma="uhm" naamval="stan" ntype="soort" pos="--" postag="N(soort,ev,basis,zijd,stan)" pt="n" rel="--" root="uhm" sense="uhm" word="uhm"/>
@@ -1324,17 +1436,17 @@
 <meta type="text" name="months" value="" />
 <meta type="text" name="role" value="Other" />
 <meta type="text" name="sex" value="" />
 <meta type="text" name="xsid" value="32" />
 <meta type="int" name="uttno" value="46" />
 </metadata>
 </alpino_ds>
-'''
+"""
 
-streestrings[2] = '''
+streestrings[2] = """
 <alpino_ds version="1.6">
   <parser cats="3" skips="0" />
   <node begin="0" cat="top" end="17" id="0" rel="top">
     <node begin="0" cat="du" end="16" id="1" rel="--">
       <node begin="0" cat="smain" end="3" id="2" rel="dp">
         <node begin="0" case="nom" def="def" end="1" frame="pronoun(nwh,fir,sg,de,nom,def)" gen="de" getal="ev" his="normal" his_1="normal" id="3" lcat="np" lemma="ik" naamval="nomin" num="sg" pdtype="pron" per="fir" persoon="1" pos="pron" postag="VNW(pers,pron,nomin,vol,1,ev)" pt="vnw" rel="su" rnum="sg" root="ik" sense="ik" status="vol" vwtype="pers" wh="nwh" word="ik"/>
         <node begin="1" end="2" frame="verb(hebben,sg1,transitive_ndev)" his="normal" his_1="normal" id="4" infl="sg1" lcat="smain" lemma="hebben" pos="verb" postag="WW(pv,tgw,ev)" pt="ww" pvagr="ev" pvtijd="tgw" rel="hd" root="heb" sc="transitive_ndev" sense="heb" stype="declarative" tense="present" word="heb" wvorm="pv"/>
@@ -1398,15 +1510,15 @@
 <meta type="text" name="months" value="" />
 <meta type="text" name="role" value="Other" />
 <meta type="text" name="sex" value="" />
 <meta type="text" name="xsid" value="29" />
 <meta type="int" name="uttno" value="42" />
 </metadata>
 </alpino_ds>
-'''
+"""
 
 strees = {}
 for el in streestrings:
     strees[el] = etree.fromstring(streestrings[el])
 
 
 def test() -> None:
@@ -1460,22 +1572,22 @@
     newsentence.text = theyieldstr
     newsentence.attrib['sentid'] = sentid
     sentencenodeparent.insert(sentencenodeindex, newsentence)
     return stree
 
 
 def transplant_node(node1: SynTree, node2: SynTree, stree: SynTree) -> SynTree:
-    '''
+    """
     replace node1 by node2 in stree
     Only do so if node1 and node2 have no children and if their spans are identical
     :param node1: node to be replaced in stree
     :param node2: node to replace node1 in stree
     :param stree: tree in which the replacement takes place
     :return: the stree in which the input parameter is modified
-    '''
+    """
     # find the parent of node1
     # determine the index of node1
     sentid = getsentid(stree)
     parentindex = get_parentandindex(node1, stree)
     if parentindex is None:
         result = stree
     else:
@@ -1501,20 +1613,20 @@
     newsentence.attrib['sentid'] = sentid
     sentencenodeparent.insert(sentencenodeindex, newsentence)
 
     return stree
 
 
 def get_parentandindex(node: SynTree, stree: SynTree) -> Optional[Tuple[SynTree, int]]:
-    '''
+    """
 
     :param node: node to find the parent of
     :param stree: stree to find the parent of node in
     :return: (parentnode::node, index::int) or None
-    '''
+    """
 
     nodespan = getspan(node)
     idx = 0
     for child in stree:
         childspan = getspan(child)
         if childspan == nodespan:
             return (stree, idx)
@@ -1531,53 +1643,57 @@
     nodeend = getattval(node, 'end')
     nodespan = (nodebegin, nodeend)
     return nodespan
 
 
 def lbrother(node: SynTree, tree: SynTree) -> Optional[SynTree]:
     nodebegin = getattval(node, 'begin')
+
     def condition(n): return getattval(n, 'end') == nodebegin
+
     result = findfirstnode(tree, condition)
     return result
 
 
 def rbrother(node: SynTree, tree: SynTree) -> Optional[SynTree]:
     nodeend = getattval(node, 'end')
+
     def condition(n): return getattval(n, 'begin') == nodeend
+
     result = findfirstnode(tree, condition)
     return result
 
 
 def infl_lbrother(node: SynTree, tree: SynTree) -> Optional[SynTree]:
-    '''
+    """
     :param node: the node for the relevant word
     :param tree: the syntactic structure that contains *node*
     :return: The function *infl_lbrother* returns the node for the word that immediately precedes the word for *node* if there is one, otherwise None
-    '''
+    """
     nodeyield = getnodeyield(tree)
     for i, n in enumerate(nodeyield):
         if nodeyield[i] == n and i > 0:
             return nodeyield[i - 1]
     return None
 
 
 def infl_rbrother(node: SynTree, tree: SynTree) -> Optional[SynTree]:
-    '''
+    """
     :param node: the node for the relevant word
     :param tree: the syntactic structure that contains *node*
     :return: The function *infl_lbrother* returns the node for the word that immediately follows the word for *node* if there is one, otherwise None
-    '''
+    """
     nodeyield = getnodeyield(tree)
     for i, n in enumerate(nodeyield):
         if nodeyield[i] == n and i < len(nodeyield) - 1:
             return nodeyield[i + 1]
     return None
 
 
-def findfirstnode(tree: SynTree, condition: Callable[[SynTree], bool]) -> SynTree:
+def findfirstnode(tree: SynTree, condition: Callable[[SynTree], bool]) -> Optional[SynTree]:
     if condition(tree):
         return tree
     else:
         for child in tree:
             result = findfirstnode(child, condition)
             if result is not None:
                 return result
@@ -1628,15 +1744,15 @@
 def strliststr2list(liststr: str, sep: str = comma) -> List[str]:
     bareliststr = liststr[1:-1]
     rawlist = bareliststr.split(sep)
     cleanlist = [x.strip()[1:-1] for x in rawlist]
     return cleanlist
 
 
-def find1(tree: SynTree, xpathquery: str) -> SynTree:
+def find1(tree: SynTree, xpathquery: str) -> Optional[SynTree]:
     if tree is None:
         return None
     results = tree.xpath(xpathquery)
     if results == []:
         result = None
     else:
         result = results[0]
@@ -1680,15 +1796,15 @@
     else:
         settings.LOGGER.error(
             'origpos {} not in reverseindex: {}'.format(origpos, reverseindex))
         result = str(0)
     return result
 
 
-def deletewordnode(tree: SynTree, begin: Position) -> SynTree:
+def deletewordnode(tree: SynTree, begin: Position) -> Optional[SynTree]:
     newtree = deepcopy(tree)
     if newtree is None:
         return newtree
     else:
         wordnodexpath = wordnodemodel.format(str(begin))
         thenode = find1(newtree, wordnodexpath)
         if thenode is not None:
@@ -1711,26 +1827,26 @@
     if tree is not None:
         etree.dump(tree, pretty_print=True)
     else:
         print('None')
 
 
 def deletechildlessparent(thenode: SynTree) -> None:
-    '''
+    """
     deletes thenode if it has no children, and if its parent is childless after that, applies itself to the parent
     :param thenode:
     :return:
-    '''
+    """
     if list(thenode) == []:
         theparent = thenode.getparent()
         theparent.remove(thenode)
         deletechildlessparent(theparent)
 
 
-def olddeletewordnodes(tree: SynTree, begins: List[Position]) -> SynTree:
+def olddeletewordnodes(tree: SynTree, begins: List[Position]) -> Optional[SynTree]:
     # print('tree:')
     # etree.dump(tree, pretty_print=True)
     newtree = deepcopy(tree)
     # print('newtree:')
     # etree.dump(newtree, pretty_print=True)
     if newtree is None:
         return newtree
@@ -1758,14 +1874,15 @@
         # done outside this function
 
         # adapt the sentence
         newtree = adaptsentence(newtree)
 
         return newtree
 
+
 # redefine: no children with tag == 'node'  (because of UD extensions )
 
 
 def childless(node: SynTree):
     children = [ch for ch in node]
     result = children == []
     return result
@@ -1774,15 +1891,15 @@
 def deletewordnodes(tree: SynTree, begins: List[Position]) -> SynTree:
     newtree = deepcopy(tree)
     newtree = deletewordnodes2(newtree, begins)
     newtree = adaptsentence(newtree)
     return newtree
 
 
-def deletewordnodes2(tree: SynTree, begins: List[Position]) -> SynTree:
+def deletewordnodes2(tree: SynTree, begins: List[Position]) -> Optional[SynTree]:
     if tree is None:
         return tree
     for child in tree:
         if child.tag == 'node':
             newchild = deletewordnodes2(child, begins)
         else:
             newchild = child
@@ -1792,15 +1909,15 @@
             childbeginint = int(childbegin)
             if childbeginint in begins and childless(child):
                 tree.remove(child)
             # if its children have been deleted earlier
             elif 'cat' in child.attrib and childless(child):
                 tree.remove(child)
     # tree  begin en end bijwerken
-    if tree. tag == 'node':
+    if tree.tag == 'node':
         newchildren = [n for n in tree]
         if newchildren != []:
             (minbegin, maxend) = getbeginend(newchildren)
             tree.attrib['begin'] = minbegin
             tree.attrib['end'] = maxend
     return tree
 
@@ -1826,15 +1943,15 @@
                         (minbegin, maxend) = getbeginend(newchildren)
                         theparent.attrib['begin'] = minbegin
                         theparent.attrib['end'] = maxend
         return tree
 
 
 def treeinflate(stree: SynTree, start: int = 10, inc: int = 10) -> None:
-    '''
+    """
     The function *treeinflate* adapts the input tree *stree* in such a way that:
 
     * for word nodes: the int value of the *begin* attribute  (ib) is changed to str(newib =(ib + 1) * 10), and the value of the *end* attribute to str(newib + 1)
     * for phrasal nodes: new values for *begin* and *end* are computed by the function *getbeginend*
     * for other nodes: the same as  for word nodes
 
     The parameters of this function are:
@@ -1844,15 +1961,15 @@
     * inc: increment, by default set to 10 (not used yet, see below)
 
     and it returns *None*.
 
     **Remark** This should be changed for words so that newib = start + (ib * inc) and
     newie =  newib + 1
 
-    '''
+    """
     # fatstree = deepcopy(stree)
     if stree is None:
         pass
     else:
         for child in stree:
             treeinflate(child, start, inc)
         children = [ch for ch in stree]
@@ -1873,15 +1990,15 @@
 
 
 def isidentitymap(dct: Dict[Any, Any]) -> bool:
     result = all([key == value for key, value in dct.items()])
     return result
 
 
-def updatetokenpos(stree: SynTree, tokenposdict: PositionMap) -> SynTree:
+def updatetokenpos(stree: SynTree, tokenposdict: PositionMap) -> Optional[SynTree]:
     if stree is None:
         return stree
     if isidentitymap(tokenposdict):
         return stree
     resulttree = deepcopy(stree)
     resulttree = updatetokenpos2(resulttree, tokenposdict)
     finaltree = updateindexnodes(resulttree)
@@ -1959,15 +2076,15 @@
         return ptsubclassdict[pt]
     else:
         return None
 
 
 def subclasscompatible(sc1, sc2):
     result = (sc1 == sc2) or \
-             (sc1 in ['pr', 'refl'] and sc2 in ['pr', 'refl']) or\
+             (sc1 in ['pr', 'refl'] and sc2 in ['pr', 'refl']) or \
              (sc1 in ['pr', 'pers'] and sc2 in ['pr', 'pers']) or \
              (sc1 in ['init', 'versm'] and sc2 in ['init', 'versm'])
     return result
 
 
 def fatparse(utterance: str, tokenlist: List[Token]) -> SynTree:
     stree = settings.PARSE_FUNC(utterance)
@@ -1980,20 +2097,20 @@
     fatstree = treewithtokenpos(fatstree, reducedtokenlist)
     if debug:
         showtree(fatstree, text='fatparse: fatstree')
     return fatstree
 
 
 def update_cleantokenisation(stree: SynTree, begin: PositionStr) -> SynTree:
-    '''
+    """
     updates the tokenisation info of the cleaned utterance
     :param stree: tree, will be modified
     :param begin: value of the begin attribute of the deleted wordnode
     :return: None
-    '''
+    """
     intbegin = int(begin)
     oldcleanedtokmeta = find1(stree, '//xmeta[@name="cleanedtokenisation"]')
     cleanedtokmeta = copy(oldcleanedtokmeta)
     oldcleanedtokposmeta = find1(
         stree, '//xmeta[@name="cleanedtokenpositions"]')
     cleanedtokposmeta = copy(oldcleanedtokposmeta)
     parent = oldcleanedtokmeta.getparent()
@@ -2034,33 +2151,33 @@
         if int(nodeend) > maxend:
             maxend = int(nodeend)
     result = (str(minbegin), str(maxend))
     return result
 
 
 def normalisebeginend(stree: SynTree) -> None:
-    '''
+    """
     :param stree: syntactic structure
     :return: stree with the values of begin and end attributes normalised
-    '''
+    """
     # etree.dump(stree, pretty_print=True)
     # begins = [getattval(node, 'begin') for node in stree.xpath('.//node[@pt or @pos]')]  # we must include indexed nodes but not have duplicates
     begins = {getattval(node, 'begin')
               for node in stree.xpath('.//node[count(node)=0]')}
     sortedbegins = sorted(list(begins), key=lambda x: int(x))
     normalisebeginend2(stree, sortedbegins)
 
 
 def normalisebeginend2(stree: SynTree, sortedbegins: List[PositionStr]) -> None:
-    '''
+    """
 
     :param stree: syntactic structure
     :param sortedbegins: sorted list of begin values of @pt or @pos nodes
     :return: None
-    '''
+    """
     children = list(stree)
     for child in children:
         normalisebeginend2(child, sortedbegins)
     if stree.tag == "node":
         if children == []:
             nodebegin = getattval(stree, 'begin')
             intnodebegin = int(nodebegin)
@@ -2072,20 +2189,20 @@
         else:
             (minbegin, maxend) = getbeginend(children)
             stree.attrib['begin'] = minbegin
             stree.attrib['end'] = maxend
 
 
 def updatebeginend(stree: SynTree, begin: PositionStr) -> None:  # do not use this anymore
-    '''
+    """
     updates the begin and end values of nodes in a tree in which a word node with begin=begin has been removed
     :param stree: Element_tree, input tree, which is modified
     :param begin: (string representation of an integer): value of the begin attribute of the word node that has been removed
     :return: None
-    '''
+    """
     children = list(stree)
     for child in children:
         updatebeginend(child, begin)
     if stree.tag == "node":
         intbegin = int(begin)
         if children == []:
             nodebegin = getattval(stree, 'begin')
```

### Comparing `sastadev-0.1.5/src/sastadev/xenx.py` & `sastadev-0.2.0/src/sastadev/xenx.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev/xlsx.py` & `sastadev-0.2.0/src/sastadev/xlsx.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/src/sastadev.egg-info/PKG-INFO` & `sastadev-0.2.0/src/sastadev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sastadev
-Version: 0.1.5
+Version: 0.2.0
 Summary: Linguistic functions for SASTA tool
 Home-page: https://github.com/UUDigitalHumanitieslab/sastadev
 Author: Research Software Lab - Centre for Digital Humanities - Utrecht University
 Author-email: digitalhumanities@uu.nl
 License: BSD-3-Clause
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `sastadev-0.1.5/src/sastadev.egg-info/SOURCES.txt` & `sastadev-0.2.0/src/sastadev.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 src/sastadev/TARSPpostfunctions.py
 src/sastadev/TARSPscreening.py
 src/sastadev/__init__.py
 src/sastadev/__main__.py
 src/sastadev/allresults.py
 src/sastadev/alpino.py
 src/sastadev/alpinoparsing.py
+src/sastadev/anonymization.py
 src/sastadev/asta_neo.py
 src/sastadev/asta_queries.py
 src/sastadev/astaforms.py
 src/sastadev/auchannsettings.py
 src/sastadev/basicreplacements.py
 src/sastadev/celexlexicon.py
+src/sastadev/chatundo.py
 src/sastadev/checkcorrection.py
 src/sastadev/cleanCHILDEStokens.py
 src/sastadev/compounds.py
 src/sastadev/conf.py
 src/sastadev/constants.py
 src/sastadev/corrector.py
 src/sastadev/correcttreebank.py
@@ -49,26 +51,29 @@
 src/sastadev/memoize.py
 src/sastadev/metadata.py
 src/sastadev/methodinfo.py
 src/sastadev/methods.py
 src/sastadev/mismatches.py
 src/sastadev/mksilver.py
 src/sastadev/mwe2pep.py
+src/sastadev/mysastadev.py
 src/sastadev/namepartlexicon.py
+src/sastadev/normalise_lemma.py
 src/sastadev/phonetics.py
 src/sastadev/py.typed
 src/sastadev/query.py
 src/sastadev/queryfunctions.py
 src/sastadev/rawalpinoparsing.py
 src/sastadev/readcsv.py
 src/sastadev/readmethod.py
 src/sastadev/reduceresults.py
 src/sastadev/resultsbyutterance.py
 src/sastadev/rpf1.py
 src/sastadev/sasta_explanation.py
+src/sastadev/sastacore.py
 src/sastadev/sastatok.py
 src/sastadev/sastatoken.py
 src/sastadev/sastatypes.py
 src/sastadev/sentence_parser.py
 src/sastadev/smallclauses.py
 src/sastadev/smartcompoundcomparison.py
 src/sastadev/stapforms.py
@@ -78,54 +83,70 @@
 src/sastadev/targets.py
 src/sastadev/tarspform.py
 src/sastadev/tblex.py
 src/sastadev/tokeniseCHILDES.py
 src/sastadev/tokenmd.py
 src/sastadev/top3000.py
 src/sastadev/treebankfunctions.py
+src/sastadev/tryderegularize.py
+src/sastadev/tryexcelfilter.py
+src/sastadev/trygaatie.py
+src/sastadev/update_inflectioncorrection.py
+src/sastadev/vuandnonwords.py
+src/sastadev/vunonwordlexicons.py
 src/sastadev/xenx.py
 src/sastadev/xlsx.py
 src/sastadev.egg-info/PKG-INFO
 src/sastadev.egg-info/SOURCES.txt
 src/sastadev.egg-info/dependency_links.txt
 src/sastadev.egg-info/entry_points.txt
 src/sastadev.egg-info/requires.txt
 src/sastadev.egg-info/top_level.txt
+src/sastadev/data/DutchIrregularVerbs.tsv
+src/sastadev/data/anonymization.json
 src/sastadev/data/expandedqueries.txt
 src/sastadev/data/inflectioncorrection.tsv.txt
+src/sastadev/data/old_inflectioncorrection.tsv.txt
 src/sastadev/data/celexlexicon/dutch/DMLCD.txt
 src/sastadev/data/celexlexicon/dutch/DMWCDOK.txt
 src/sastadev/data/celexlexicon/dutch/DSLCD.txt
 src/sastadev/data/compoundfiles/Ncompounds-attempt1.txt
 src/sastadev/data/compoundfiles/Ncompounds-attempt2.txt
 src/sastadev/data/compoundfiles/Ncompounds-attempt2.zip
 src/sastadev/data/filledpauseslexicon/filledpauseslexicon.txt
+src/sastadev/data/filledpauseslexicon/notanalyzewords.txt
+src/sastadev/data/filledpauseslexicon/oldfilledpauseslexicon.txt
+src/sastadev/data/filledpauseslexicon/vuwordslexicon.txt
 src/sastadev/data/form_templates/STAP Excel VUmc 2018.xlsx
 src/sastadev/data/form_templates/TARSP Form Current.xlsx
 src/sastadev/data/macros/newimperatives.txt
+src/sastadev/data/macros/newrobusthwwi.txt
 src/sastadev/data/macros/sastamacros1.txt
 src/sastadev/data/macros/sastamacros2.txt
 src/sastadev/data/methods/ASTA_07062021.xlsx
 src/sastadev/data/methods/ASTA_Index_Current.xlsx
+src/sastadev/data/methods/ASTA_Index_Current_old.xlsx
 src/sastadev/data/methods/STAP_07062021.xlsx
 src/sastadev/data/methods/STAP_Index_Current.xlsx
 src/sastadev/data/methods/TARSP Index 2022-01-07.xlsx
-src/sastadev/data/methods/TARSP Index Current.xlsx
 src/sastadev/data/methods/TARSP_07062021.xlsx
+src/sastadev/data/methods/TARSP_Index_Current.xlsx
 src/sastadev/data/names/fn10k_versie1.zip
 src/sastadev/data/names/voornamentop10000.xml
 src/sastadev/data/names/Woonplaatsen/83958NED_TypedDataSet_19062020_173530.csv
 src/sastadev/data/names/Woonplaatsen/83958NED_UntypedDataSet_19062020_173456.csv
 src/sastadev/data/names/Woonplaatsen/83958NED_metadata.csv
 src/sastadev/data/names/fn10k_versie1/fn_10kw.xml
 src/sastadev/data/names/fn10k_versie1/fn_10kw.xsl
 src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden.csv
 src/sastadev/data/names/hoofdsteden/wikipedia_hoofsteden_raw.txt
 src/sastadev/data/names/nameparts/namepartlexicon.csv
+src/sastadev/data/nochildwords/nochildwords.txt
 src/sastadev/data/top3000/Woordenlijsten Current.xlsx
+src/sastadev/data/wordsunknowntoalpino/wordsunknowntoalpino.txt
 tests/test_adjacency.py
 tests/test_explanation.py
 tests/test_hyphens.py
 tests/test_indexexpansion.py
 tests/test_lxml.py
 tests/test_smallclauses.py
 tests/test_vobij.py
```

### Comparing `sastadev-0.1.5/tests/__pycache__/test_adjacency.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.0/tests/__pycache__/test_adjacency.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug 29 13:46:10 2023 UTC, .py size: 13386 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -875,15 +875,15 @@
 000036a0: 019b 0064 029d 0383 027d 027c 0253 0029  ...d.....}.|.S.)
 000036b0: 034e 7a0e 2f2f 6e6f 6465 5b40 776f 7264  .Nz.//node[@word
 000036c0: 3d22 7a02 225d 2901 7204 0000 0029 035a  ="z."]).r....).Z
 000036d0: 0573 7472 6565 da04 776f 7264 da06 7265  .stree..word..re
 000036e0: 7375 6c74 a900 720c 0000 00fa 4b2f 5573  sult..r.....K/Us
 000036f0: 6572 732f 6133 3234 3835 3236 2f67 6974  ers/a3248526/git
 00003700: 2f73 6173 7461 6465 765f 7061 636b 6167  /sastadev_packag
-00003710: 652f 7361 7374 6164 6576 2d30 2e31 2e35  e/sastadev-0.1.5
+00003710: 652f 7361 7374 6164 6576 2d30 2e32 2e30  e/sastadev-0.2.0
 00003720: 2f74 6573 7473 2f74 6573 745f 6164 6a61  /tests/test_adja
 00003730: 6365 6e63 792e 7079 da07 6765 746e 6f64  cency.py..getnod
 00003740: 6583 0000 0073 0400 0000 0001 1201 720e  e....s........r.
 00003750: 0000 00da 0269 735a 056e 6f67 616c 5429  .....isZ.nogalT)
 00003760: 0172 0f00 0000 2901 7a12 2528 7079 3029  .r....).z.%(py0)
 00003770: 7320 6973 2025 2870 7933 2973 720b 0000  s is %(py3)sr...
 00003780: 0029 02da 0370 7930 da03 7079 337a 0e61  .)...py0..py3z.a
```

### Comparing `sastadev-0.1.5/tests/__pycache__/test_explanation.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.0/tests/__pycache__/test_explanation.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Apr 24 10:50:43 2024 UTC, .py size: 1345 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-00000000: 550d 0d0a 0000 0000 03e4 2866 4105 0000  U.........(fA...
+00000000: 550d 0d0a 0000 0000 286d 2b66 9e05 0000  U.......(m+f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
+00000020: 0003 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6401  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0b 0100 6400 6403 6c0c 6d0d  l.m.Z...d.d.l.m.
-00000070: 5a0d 0100 6404 5a0e 6506 6a0f 6a10 6405  Z...d.Z.e.j.j.d.
-00000080: 6406 8d01 6407 6408 8400 8301 5a11 6512  d...d.d.....Z.e.
-00000090: 6409 6b02 726e 6511 8300 0100 6401 5300  d.k.rne.....d.S.
-000000a0: 290a e900 0000 004e 2901 da0b 616c 6967  )......N)...alig
-000000b0: 6e5f 776f 7264 7329 01da 1173 6173 7461  n_words)...sasta
-000000c0: 5f65 7870 6c61 6e61 7469 6f6e fa01 207a  _explanation.. z
-000000d0: 1774 6573 7420 636f 6465 2064 6f65 7320  .test code does 
-000000e0: 6e6f 7420 776f 726b 2901 da06 7265 6173  not work)...reas
-000000f0: 6f6e 6300 0000 0000 0000 0000 0000 000c  onc.............
-00000100: 0000 000b 0000 0043 0000 0073 b800 0000  .......C...s....
-00000110: 6401 7d00 7400 a001 7c00 a101 7d01 7c01  d.}.t...|...}.|.
-00000120: a002 a100 7d02 6402 7d03 7c02 4400 5d94  ....}.d.}.|.D.].
-00000130: 7d04 7c03 6403 3700 7d03 7400 a003 7c04  }.|.d.7.}.t...|.
-00000140: 6404 a102 7d05 7400 a003 7c04 6405 a102  d...}.t...|.d...
-00000150: 7d06 7c06 6a04 7d07 7405 a006 7c04 a101  }.|.j.}.t...|...
-00000160: 5c02 7d08 7d09 7c08 6400 6b09 726c 7407  \.}.}.|.d.k.rlt.
-00000170: a008 7c08 7c09 1700 a101 6e02 6400 7d0a  ..|.|.....n.d.}.
-00000180: 7c0a 6400 6b09 7284 7409 7c07 7c0a 8302  |.d.k.r.t.|.|...
-00000190: 7d0b 6e04 6400 7d0b 7c0a 6400 6b09 721e  }.n.d.}.|.d.k.r.
-000001a0: 740a 6406 7c05 9b00 6407 7c07 9b00 6408  t.d.|...d.|...d.
-000001b0: 7c0a 9b00 6409 7c0b 9b00 640a 9d09 8301  |...d.|...d.....
-000001c0: 0100 711e 6400 5300 290b 4e7a 5344 3a5c  ..q.d.S.).NzSD:\
-000001d0: 4472 6f70 626f 785c 6a6f 6469 6a6b 5c55  Dropbox\jodijk\U
-000001e0: 7472 6563 6874 5c50 726f 6a65 6374 735c  trecht\Projects\
-000001f0: 5341 5354 4144 4154 415c 4175 7269 735c  SASTADATA\Auris\
-00000200: 6f75 7474 7265 6562 616e 6b73 5c44 4c44  outtreebanks\DLD
-00000210: 3037 5f63 6f72 7265 6374 6564 2e78 6d6c  07_corrected.xml
-00000220: 7201 0000 00e9 0100 0000 7a1f 2e2f 2f6d  r.........z..//m
-00000230: 6574 615b 406e 616d 653d 226f 7269 6775  eta[@name="origu
-00000240: 7474 225d 2f40 7661 6c75 657a 0b2e 2f2f  tt"]/@valuez..//
-00000250: 7365 6e74 656e 6365 7a06 204f 7269 673a  sentencez. Orig:
-00000260: 7a07 0a43 6c65 616e 3a7a 070a 2045 7870  z..Clean:z.. Exp
-00000270: 6c3a 7a07 0a41 6c69 676e 3a7a 020a 0a29  l:z..Align:z...)
-00000280: 0bda 0374 6266 da08 6765 7473 7472 6565  ...tbf..getstree
-00000290: da07 6765 7472 6f6f 74da 0566 696e 6431  ..getroot..find1
-000002a0: da04 7465 7874 7203 0000 005a 1966 696e  ..textr....Z.fin
-000002b0: 616c 6d75 6c74 6977 6f72 6465 7870 6c61  almultiwordexpla
-000002c0: 6e61 7469 6f6e da05 7370 6163 65da 046a  nation..space..j
-000002d0: 6f69 6e72 0200 0000 da05 7072 696e 7429  oinr......print)
-000002e0: 0c5a 0a69 6e66 756c 6c6e 616d 655a 0c66  .Z.infullnameZ.f
-000002f0: 756c 6c74 7265 6562 616e 6bda 0874 7265  ulltreebank..tre
-00000300: 6562 616e 6b5a 0974 7265 6563 6f75 6e74  ebankZ.treecount
-00000310: da04 7472 6565 5a07 6f72 6967 7574 745a  ..treeZ.origuttZ
-00000320: 0c63 6c65 616e 7574 7465 6c65 6d5a 0863  .cleanuttelemZ.c
-00000330: 6c65 616e 7574 745a 0f65 7870 6c61 6e61  leanuttZ.explana
-00000340: 7469 6f6e 6c69 7374 5a13 706f 7374 6578  tionlistZ.postex
-00000350: 706c 616e 6174 696f 6e6c 6973 745a 0e65  planationlistZ.e
-00000360: 7870 6c61 6e61 7469 6f6e 7374 725a 0961  xplanationstrZ.a
-00000370: 6c69 676e 6d65 6e74 a900 7211 0000 00fa  lignment..r.....
-00000380: 4d2f 5573 6572 732f 6133 3234 3835 3236  M/Users/a3248526
-00000390: 2f67 6974 2f73 6173 7461 6465 765f 7061  /git/sastadev_pa
-000003a0: 636b 6167 652f 7361 7374 6164 6576 2d30  ckage/sastadev-0
-000003b0: 2e31 2e35 2f74 6573 7473 2f74 6573 745f  .1.5/tests/test_
-000003c0: 6578 706c 616e 6174 696f 6e2e 7079 da04  explanation.py..
-000003d0: 7465 7374 0900 0000 7324 0000 0000 0304  test....s$......
-000003e0: 010a 0108 0104 0108 0108 030c 020c 0106  ................
-000003f0: 010e 011a 0208 010c 0204 0108 0102 011c  ................
-00000400: ff72 1300 0000 da08 5f5f 6d61 696e 5f5f  .r......__main__
-00000410: 2913 da08 6275 696c 7469 6e73 da0c 4070  )...builtins..@p
-00000420: 795f 6275 696c 7469 6e73 da19 5f70 7974  y_builtins.._pyt
-00000430: 6573 742e 6173 7365 7274 696f 6e2e 7265  est.assertion.re
-00000440: 7772 6974 65da 0961 7373 6572 7469 6f6e  write..assertion
-00000450: da07 7265 7772 6974 65da 0a40 7079 7465  ..rewrite..@pyte
-00000460: 7374 5f61 72da 0670 7974 6573 745a 1361  st_ar..pytestZ.a
-00000470: 7563 6861 6e6e 2e61 6c69 676e 5f77 6f72  uchann.align_wor
-00000480: 6473 7202 0000 00da 1a73 6173 7461 6465  dsr......sastade
-00000490: 762e 7472 6565 6261 6e6b 6675 6e63 7469  v.treebankfuncti
-000004a0: 6f6e 73da 1174 7265 6562 616e 6b66 756e  ons..treebankfun
-000004b0: 6374 696f 6e73 7207 0000 00da 0873 6173  ctionsr......sas
-000004c0: 7461 6465 7672 0300 0000 720c 0000 00da  tadevr....r.....
-000004d0: 046d 6172 6bda 0473 6b69 7072 1300 0000  .mark..skipr....
-000004e0: da08 5f5f 6e61 6d65 5f5f 7211 0000 0072  ..__name__r....r
-000004f0: 1100 0000 7211 0000 0072 1200 0000 da08  ....r....r......
-00000500: 3c6d 6f64 756c 653e 0100 0000 7314 0000  <module>....s...
-00000510: 0008 0012 0008 010c 020c 010c 0204 020c  ................
-00000520: 010a 1a08 01                             .....
+00000070: 5a0d 0100 6404 5a0e 6404 5a0e 6506 6a0f  Z...d.Z.d.Z.e.j.
+00000080: 6a10 6405 6406 8d01 6407 6408 8400 8301  j.d.d...d.d.....
+00000090: 5a11 6512 6409 6b02 7272 6511 8300 0100  Z.e.d.k.rre.....
+000000a0: 6401 5300 290a e900 0000 004e 2901 da0b  d.S.)......N)...
+000000b0: 616c 6967 6e5f 776f 7264 7329 01da 1173  align_words)...s
+000000c0: 6173 7461 5f65 7870 6c61 6e61 7469 6f6e  asta_explanation
+000000d0: fa01 207a 1074 6573 7420 6e6f 7420 776f  .. z.test not wo
+000000e0: 726b 696e 6729 01da 0672 6561 736f 6e63  rking)...reasonc
+000000f0: 0000 0000 0000 0000 0000 0000 0c00 0000  ................
+00000100: 0b00 0000 4300 0000 73b8 0000 0064 017d  ....C...s....d.}
+00000110: 0074 00a0 017c 00a1 017d 017c 01a0 02a1  .t...|...}.|....
+00000120: 007d 0264 027d 037c 0244 005d 947d 047c  .}.d.}.|.D.].}.|
+00000130: 0364 0337 007d 0374 00a0 037c 0464 04a1  .d.7.}.t...|.d..
+00000140: 027d 0574 00a0 037c 0464 05a1 027d 067c  .}.t...|.d...}.|
+00000150: 066a 047d 0774 05a0 067c 04a1 015c 027d  .j.}.t...|...\.}
+00000160: 087d 097c 0864 006b 0972 6c74 07a0 087c  .}.|.d.k.rlt...|
+00000170: 087c 0917 00a1 016e 0264 007d 0a7c 0a64  .|.....n.d.}.|.d
+00000180: 006b 0972 8474 097c 077c 0a83 027d 0b6e  .k.r.t.|.|...}.n
+00000190: 0464 007d 0b7c 0a64 006b 0972 1e74 0a64  .d.}.|.d.k.r.t.d
+000001a0: 067c 059b 0064 077c 079b 0064 087c 0a9b  .|...d.|...d.|..
+000001b0: 0064 097c 0b9b 0064 0a9d 0983 0101 0071  .d.|...d.......q
+000001c0: 1e64 0053 0029 0b4e 7a53 443a 5c44 726f  .d.S.).NzSD:\Dro
+000001d0: 7062 6f78 5c6a 6f64 696a 6b5c 5574 7265  pbox\jodijk\Utre
+000001e0: 6368 745c 5072 6f6a 6563 7473 5c53 4153  cht\Projects\SAS
+000001f0: 5441 4441 5441 5c41 7572 6973 5c6f 7574  TADATA\Auris\out
+00000200: 7472 6565 6261 6e6b 735c 444c 4430 375f  treebanks\DLD07_
+00000210: 636f 7272 6563 7465 642e 786d 6c72 0100  corrected.xmlr..
+00000220: 0000 e901 0000 007a 1f2e 2f2f 6d65 7461  .......z..//meta
+00000230: 5b40 6e61 6d65 3d22 6f72 6967 7574 7422  [@name="origutt"
+00000240: 5d2f 4076 616c 7565 7a0b 2e2f 2f73 656e  ]/@valuez..//sen
+00000250: 7465 6e63 657a 0620 4f72 6967 3a7a 070a  tencez. Orig:z..
+00000260: 436c 6561 6e3a 7a07 0a20 4578 706c 3a7a  Clean:z.. Expl:z
+00000270: 070a 416c 6967 6e3a 7a02 0a0a 290b da03  ..Align:z...)...
+00000280: 7462 66da 0867 6574 7374 7265 65da 0767  tbf..getstree..g
+00000290: 6574 726f 6f74 da05 6669 6e64 31da 0474  etroot..find1..t
+000002a0: 6578 7472 0300 0000 5a19 6669 6e61 6c6d  extr....Z.finalm
+000002b0: 756c 7469 776f 7264 6578 706c 616e 6174  ultiwordexplanat
+000002c0: 696f 6eda 0573 7061 6365 da04 6a6f 696e  ion..space..join
+000002d0: 7202 0000 00da 0570 7269 6e74 290c 5a0a  r......print).Z.
+000002e0: 696e 6675 6c6c 6e61 6d65 5a0c 6675 6c6c  infullnameZ.full
+000002f0: 7472 6565 6261 6e6b da08 7472 6565 6261  treebank..treeba
+00000300: 6e6b 5a09 7472 6565 636f 756e 74da 0474  nkZ.treecount..t
+00000310: 7265 655a 076f 7269 6775 7474 5a0c 636c  reeZ.origuttZ.cl
+00000320: 6561 6e75 7474 656c 656d 5a08 636c 6561  eanuttelemZ.clea
+00000330: 6e75 7474 5a0f 6578 706c 616e 6174 696f  nuttZ.explanatio
+00000340: 6e6c 6973 745a 1370 6f73 7465 7870 6c61  nlistZ.postexpla
+00000350: 6e61 7469 6f6e 6c69 7374 5a0e 6578 706c  nationlistZ.expl
+00000360: 616e 6174 696f 6e73 7472 5a09 616c 6967  anationstrZ.alig
+00000370: 6e6d 656e 74a9 0072 1100 0000 fa4d 2f55  nment..r.....M/U
+00000380: 7365 7273 2f61 3332 3438 3532 362f 6769  sers/a3248526/gi
+00000390: 742f 7361 7374 6164 6576 5f70 6163 6b61  t/sastadev_packa
+000003a0: 6765 2f73 6173 7461 6465 762d 302e 322e  ge/sastadev-0.2.
+000003b0: 302f 7465 7374 732f 7465 7374 5f65 7870  0/tests/test_exp
+000003c0: 6c61 6e61 7469 6f6e 2e70 79da 0474 6573  lanation.py..tes
+000003d0: 7410 0000 0073 2400 0000 0003 0401 0a01  t....s$.........
+000003e0: 0801 0401 0801 0803 0c02 0c01 0601 0e01  ................
+000003f0: 1a02 0801 0c02 0401 0801 0201 1cff 7213  ..............r.
+00000400: 0000 00da 085f 5f6d 6169 6e5f 5f29 13da  .....__main__)..
+00000410: 0862 7569 6c74 696e 73da 0c40 7079 5f62  .builtins..@py_b
+00000420: 7569 6c74 696e 73da 195f 7079 7465 7374  uiltins.._pytest
+00000430: 2e61 7373 6572 7469 6f6e 2e72 6577 7269  .assertion.rewri
+00000440: 7465 da09 6173 7365 7274 696f 6eda 0772  te..assertion..r
+00000450: 6577 7269 7465 da0a 4070 7974 6573 745f  ewrite..@pytest_
+00000460: 6172 da06 7079 7465 7374 5a13 6175 6368  ar..pytestZ.auch
+00000470: 616e 6e2e 616c 6967 6e5f 776f 7264 7372  ann.align_wordsr
+00000480: 0200 0000 da1a 7361 7374 6164 6576 2e74  ......sastadev.t
+00000490: 7265 6562 616e 6b66 756e 6374 696f 6e73  reebankfunctions
+000004a0: da11 7472 6565 6261 6e6b 6675 6e63 7469  ..treebankfuncti
+000004b0: 6f6e 7372 0700 0000 da08 7361 7374 6164  onsr......sastad
+000004c0: 6576 7203 0000 0072 0c00 0000 da04 6d61  evr....r......ma
+000004d0: 726b da04 736b 6970 7213 0000 00da 085f  rk..skipr......_
+000004e0: 5f6e 616d 655f 5f72 1100 0000 7211 0000  _name__r....r...
+000004f0: 0072 1100 0000 7212 0000 00da 083c 6d6f  .r....r......<mo
+00000500: 6475 6c65 3e01 0000 0073 1600 0000 0800  dule>....s......
+00000510: 1200 0801 0c02 0c01 0c02 0404 0405 0c01  ................
+00000520: 0a1a 0801                                ....
```

### Comparing `sastadev-0.1.5/tests/__pycache__/test_hyphens.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.0/tests/__pycache__/test_hyphens.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug 29 13:46:10 2023 UTC, .py size: 634 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 00000870: 795f 666f 726d 6174 3130 5a0b 4070 795f  y_format10Z.@py_
 00000880: 6173 7365 7274 345a 0b40 7079 5f61 7373  assert4Z.@py_ass
 00000890: 6572 7437 5a0b 4070 795f 666f 726d 6174  ert7Z.@py_format
 000008a0: 395a 0c40 7079 5f66 6f72 6d61 7431 31a9  9Z.@py_format11.
 000008b0: 0072 1500 0000 fa49 2f55 7365 7273 2f61  .r.....I/Users/a
 000008c0: 3332 3438 3532 362f 6769 742f 7361 7374  3248526/git/sast
 000008d0: 6164 6576 5f70 6163 6b61 6765 2f73 6173  adev_package/sas
-000008e0: 7461 6465 762d 302e 312e 352f 7465 7374  tadev-0.1.5/test
+000008e0: 7461 6465 762d 302e 322e 302f 7465 7374  tadev-0.2.0/test
 000008f0: 732f 7465 7374 5f68 7970 6865 6e73 2e70  s/test_hyphens.p
 00000900: 79da 0474 6573 7405 0000 0073 7e00 0000  y..test....s~...
 00000910: 0002 0400 0800 0c00 0800 0400 5600 0c00  ............V...
 00000920: 0e00 1001 0400 0a00 0400 0800 0600 7c00  ..............|.
 00000930: 0c00 0e00 1001 0400 0a00 0400 0800 0600  ................
 00000940: 8000 0c00 0e00 1001 0400 0a00 0400 0800  ................
 00000950: 0600 8000 0c00 0e00 1001 0400 0a00 0600  ................
```

### Comparing `sastadev-0.1.5/tests/__pycache__/test_indexexpansion.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.0/tests/__pycache__/test_indexexpansion.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug 29 13:46:10 2023 UTC, .py size: 6946 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
 000016f0: 0119 00a1 0193 0271 0453 00a9 0029 0372  .......q.S...).r
 00001700: 0200 0000 da0a 6672 6f6d 7374 7269 6e67  ......fromstring
 00001710: da0c 7374 7265 6573 7472 696e 6773 2902  ..streestrings).
 00001720: da02 2e30 da01 6972 0600 0000 7206 0000  ...0..ir....r...
 00001730: 00fa 502f 5573 6572 732f 6133 3234 3835  ..P/Users/a32485
 00001740: 3236 2f67 6974 2f73 6173 7461 6465 765f  26/git/sastadev_
 00001750: 7061 636b 6167 652f 7361 7374 6164 6576  package/sastadev
-00001760: 2d30 2e31 2e35 2f74 6573 7473 2f74 6573  -0.1.5/tests/tes
+00001760: 2d30 2e32 2e30 2f74 6573 7473 2f74 6573  -0.2.0/tests/tes
 00001770: 745f 696e 6465 7865 7870 616e 7369 6f6e  t_indexexpansion
 00001780: 2e70 79da 0a3c 6469 6374 636f 6d70 3e42  .py..<dictcomp>B
 00001790: 0000 0073 0600 0000 0600 0200 0200 720c  ...s..........r.
 000017a0: 0000 007a 1774 6573 7420 636f 6465 2064  ...z.test code d
 000017b0: 6f65 7320 6e6f 7420 776f 726b 2901 da06  oes not work)...
 000017c0: 7265 6173 6f6e 6300 0000 0000 0000 0000  reasonc.........
 000017d0: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
```

### Comparing `sastadev-0.1.5/tests/__pycache__/test_lxml.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.0/tests/__pycache__/test_lxml.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug 29 13:46:10 2023 UTC, .py size: 7187 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 00000250: 7265 7375 6c74 735a 0a6e 6f64 6572 6573  resultsZ.noderes
 00000260: 756c 7472 0f00 0000 da03 706f 735a 0670  ultr......posZ.p
 00000270: 6f73 6361 7472 1100 0000 7212 0000 00da  oscatr....r.....
 00000280: 0672 6573 756c 74a9 0072 1b00 0000 fa46  .result..r.....F
 00000290: 2f55 7365 7273 2f61 3332 3438 3532 362f  /Users/a3248526/
 000002a0: 6769 742f 7361 7374 6164 6576 5f70 6163  git/sastadev_pac
 000002b0: 6b61 6765 2f73 6173 7461 6465 762d 302e  kage/sastadev-0.
-000002c0: 312e 352f 7465 7374 732f 7465 7374 5f6c  1.5/tests/test_l
+000002c0: 322e 302f 7465 7374 732f 7465 7374 5f6c  2.0/tests/test_l
 000002d0: 786d 6c2e 7079 da0a 6765 7472 6573 756c  xml.py..getresul
 000002e0: 7473 2000 0000 7316 0000 0000 010a 0104  ts ...s.........
 000002f0: 0108 010a 010a 0110 010a 010a 010a 010c  ................
 00000300: 0172 1d00 0000 6300 0000 0000 0000 0000  .r....c.........
 00000310: 0000 000f 0000 0009 0000 0043 0000 0073  ...........C...s
 00000320: d801 0000 6700 7d00 7c00 a000 6401 a101  ....g.}.|...d...
 00000330: 0100 7c00 a000 6402 a101 0100 7c00 a000  ..|...d.....|...
```

### Comparing `sastadev-0.1.5/tests/__pycache__/test_smallclauses.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.0/tests/__pycache__/test_smallclauses.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug 29 13:46:10 2023 UTC, .py size: 1971 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 00000200: 06da 026f 73da 0470 6174 68da 046a 6f69  ...os..path..joi
 00000210: 6e72 0c00 0000 da08 4441 5441 524f 4f54  nr......DATAROOT
 00000220: 7202 0000 0029 035a 0764 6174 6173 6574  r....).Z.dataset
 00000230: da08 6669 6c65 6e61 6d65 da06 7265 7375  ..filename..resu
 00000240: 6c74 a900 7213 0000 00fa 4e2f 5573 6572  lt..r.....N/User
 00000250: 732f 6133 3234 3835 3236 2f67 6974 2f73  s/a3248526/git/s
 00000260: 6173 7461 6465 765f 7061 636b 6167 652f  astadev_package/
-00000270: 7361 7374 6164 6576 2d30 2e31 2e35 2f74  sastadev-0.1.5/t
+00000270: 7361 7374 6164 6576 2d30 2e32 2e30 2f74  sastadev-0.2.0/t
 00000280: 6573 7473 2f74 6573 745f 736d 616c 6c63  ests/test_smallc
 00000290: 6c61 7573 6573 2e70 79da 0567 6574 666e  lauses.py..getfn
 000002a0: 0b00 0000 7304 0000 0000 0114 0172 1500  ....s........r..
 000002b0: 0000 5a06 7363 7465 7374 7a13 736d 616c  ..Z.sctestz.smal
 000002c0: 6c63 6c61 7573 6574 6573 742e 786d 6c5a  lclausetest.xmlZ
 000002d0: 0b73 6368 6c69 6368 7469 6e67 7a0e 5441  .schlichtingz.TA
 000002e0: 5256 4232 5f49 4432 2e78 6d6c 5a09 6d69  RVB2_ID2.xmlZ.mi
```

### Comparing `sastadev-0.1.5/tests/__pycache__/test_vobij.cpython-38-pytest-7.4.0.pyc` & `sastadev-0.2.0/tests/__pycache__/test_vobij.cpython-38-pytest-7.4.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Tue Aug 29 13:46:10 2023 UTC, .py size: 14153 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -830,15 +830,15 @@
 000033d0: 0000 6900 7c00 5d14 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
 000033e0: 7400 a001 7c02 a101 9302 7104 5300 a900  t...|.....q.S...
 000033f0: 2902 7202 0000 00da 0a66 726f 6d73 7472  ).r......fromstr
 00003400: 696e 6729 03da 022e 30da 0169 da02 7473  ing)....0..i..ts
 00003410: 7208 0000 0072 0800 0000 fa47 2f55 7365  r....r.....G/Use
 00003420: 7273 2f61 3332 3438 3532 362f 6769 742f  rs/a3248526/git/
 00003430: 7361 7374 6164 6576 5f70 6163 6b61 6765  sastadev_package
-00003440: 2f73 6173 7461 6465 762d 302e 312e 352f  /sastadev-0.1.5/
+00003440: 2f73 6173 7461 6465 762d 302e 322e 302f  /sastadev-0.2.0/
 00003450: 7465 7374 732f 7465 7374 5f76 6f62 696a  tests/test_vobij
 00003460: 2e70 79da 0a3c 6469 6374 636f 6d70 3e8e  .py..<dictcomp>.
 00003470: 0000 0073 0600 0000 0600 0600 0200 720e  ...s..........r.
 00003480: 0000 005a 0234 305a 0233 3063 0000 0000  ...Z.40Z.30c....
 00003490: 0000 0000 0000 0000 0800 0000 0b00 0000  ................
 000034a0: 4300 0000 73e0 0100 0074 00a0 01a1 0044  C...s....t.....D
 000034b0: 0090 015d d05c 027d 007d 0164 0164 0284  ...].\.}.}.d.d..
```

### Comparing `sastadev-0.1.5/tests/test_adjacency.py` & `sastadev-0.2.0/tests/test_adjacency.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/tests/test_explanation.py` & `sastadev-0.2.0/tests/test_explanation.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,22 @@
 from auchann.align_words import align_words
 
 import sastadev.treebankfunctions as tbf
 from sastadev import sasta_explanation
 
 space = ' '
 
-@pytest.mark.skip(reason='test code does not work')
+#@pytest.mark.skip(reason='test code does not work')
+
+space = ' '
+
+#print(dir(sasta_explanation))
+
+
+@pytest.mark.skip(reason="test not working")
 def test():
     # treetotest = 9
     infullname = r"D:\Dropbox\jodijk\Utrecht\Projects\SASTADATA\Auris\outtreebanks\DLD07_corrected.xml"
     fulltreebank = tbf.getstree(infullname)
     treebank = fulltreebank.getroot()
     treecount = 0
     for tree in treebank:
```

### Comparing `sastadev-0.1.5/tests/test_hyphens.py` & `sastadev-0.2.0/tests/test_hyphens.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/tests/test_indexexpansion.py` & `sastadev-0.2.0/tests/test_indexexpansion.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/tests/test_lxml.py` & `sastadev-0.2.0/tests/test_lxml.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/tests/test_smallclauses.py` & `sastadev-0.2.0/tests/test_smallclauses.py`

 * *Files identical despite different names*

### Comparing `sastadev-0.1.5/tests/test_vobij.py` & `sastadev-0.2.0/tests/test_vobij.py`

 * *Files identical despite different names*

