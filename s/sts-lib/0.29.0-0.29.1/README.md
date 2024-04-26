# Comparing `tmp/sts_lib-0.29.0.tar.gz` & `tmp/sts_lib-0.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.29.0.tar", last modified: Thu Apr 25 02:19:10 2024, max compression
+gzip compressed data, was "sts_lib-0.29.1.tar", last modified: Fri Apr 26 12:43:40 2024, max compression
```

## Comparing `sts_lib-0.29.0.tar` & `sts_lib-0.29.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 02:19:10.114974 sts_lib-0.29.0/
--rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.29.0/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.29.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6869 2024-04-25 02:19:10.114974 sts_lib-0.29.0/PKG-INFO
--rw-rw-rw-   0        0        0     5416 2024-04-25 02:17:04.000000 sts_lib-0.29.0/README.md
--rw-rw-rw-   0        0        0     1728 2024-04-25 02:19:10.116974 sts_lib-0.29.0/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.29.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:19:10.076497 sts_lib-0.29.0/sts/
--rw-rw-rw-   0        0        0    52455 2024-04-25 02:17:05.000000 sts_lib-0.29.0/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.29.0/sts/__main__.py
--rw-rw-rw-   0        0        0     7551 2024-04-23 13:05:20.000000 sts_lib-0.29.0/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-25 02:19:10.076497 sts_lib-0.29.0/sts/data/
-drwxrwxrwx   0        0        0        0 2024-04-25 02:19:10.089232 sts_lib-0.29.0/sts/data/config/
--rw-rw-rw-   0        0        0      915 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      608 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      346 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      410 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      419 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      267 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      417 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      608 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      247 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      261 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      267 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      245 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      606 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      670 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      344 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-04-25 02:19:10.104005 sts_lib-0.29.0/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    22760 2024-04-25 01:31:59.000000 sts_lib-0.29.0/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-04-25 02:19:10.105998 sts_lib-0.29.0/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2024-04-25 01:40:27.000000 sts_lib-0.29.0/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-04-25 02:19:10.112976 sts_lib-0.29.0/sts_lib.egg-info/
--rw-rw-rw-   0        0        0     6869 2024-04-25 02:19:10.000000 sts_lib-0.29.0/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-04-25 02:19:10.000000 sts_lib-0.29.0/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 02:19:10.000000 sts_lib-0.29.0/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-25 02:19:10.000000 sts_lib-0.29.0/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      202 2024-04-25 02:19:10.000000 sts_lib-0.29.0/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-25 02:19:10.000000 sts_lib-0.29.0/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 12:43:40.066478 sts_lib-0.29.1/
+-rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.29.1/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.29.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6916 2024-04-26 12:43:40.066478 sts_lib-0.29.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5463 2024-04-26 12:29:18.000000 sts_lib-0.29.1/README.md
+-rw-rw-rw-   0        0        0     1728 2024-04-26 12:43:40.068475 sts_lib-0.29.1/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.29.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:43:39.999503 sts_lib-0.29.1/sts/
+-rw-rw-rw-   0        0        0    52455 2024-04-26 12:41:58.000000 sts_lib-0.29.1/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.29.1/sts/__main__.py
+-rw-rw-rw-   0        0        0     7551 2024-04-23 13:05:20.000000 sts_lib-0.29.1/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-26 12:43:40.013530 sts_lib-0.29.1/sts/data/
+drwxrwxrwx   0        0        0        0 2024-04-26 12:43:40.029518 sts_lib-0.29.1/sts/data/config/
+-rw-rw-rw-   0        0        0      915 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      608 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      346 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      410 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      419 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      267 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      417 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      608 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      247 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      261 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      267 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      245 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      606 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      670 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      344 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-04-26 12:43:40.052494 sts_lib-0.29.1/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    22760 2024-04-26 12:35:06.000000 sts_lib-0.29.1/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-04-26 12:43:40.055489 sts_lib-0.29.1/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2024-04-26 12:42:39.000000 sts_lib-0.29.1/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 12:43:40.063481 sts_lib-0.29.1/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0     6916 2024-04-26 12:43:39.000000 sts_lib-0.29.1/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-04-26 12:43:39.000000 sts_lib-0.29.1/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 12:43:39.000000 sts_lib-0.29.1/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-26 12:43:39.000000 sts_lib-0.29.1/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-04-26 12:43:39.000000 sts_lib-0.29.1/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-26 12:43:39.000000 sts_lib-0.29.1/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.29.0/LICENSE` & `sts_lib-0.29.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/PKG-INFO` & `sts_lib-0.29.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.29.0
+Version: 0.29.1
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,15 @@
 
 簡繁祕書是開源、輕巧、有彈性的中文簡繁轉換工具，也支援異體字轉換及地區慣用詞轉換。
 
 
 ## Features 特色
 
 * 支援 [OpenCC](https://github.com/BYVoid/OpenCC) 格式及 JSON、YAML 格式的詞典檔。
-* 可透過配置檔組合多個詞典檔作為具體轉換方案。組合詞典可儲存成新詞典檔以加速未來載入使用，任一詞典檔更新時皆會自動重新生成組合詞典。支援的組合方式有「並聯」、「串聯」、「反轉」、「擴充」、「過濾」等等。
+* 可透過配置檔組合多個詞典檔作為具體轉換方案。組合詞典可儲存成新詞典檔以加速未來載入使用，任一詞典檔更新時皆會自動重新生成組合詞典。支援的組合方式有「並聯」、「串聯」、「反轉」、「展開」、「篩選」等等。
 * 簡繁對應、異體字對應、地區慣用詞對應等不同的對應關係皆區分至不同的詞典檔。
 * 詞典及配置檔與程式本體分離，可自由修改、擴充。
 * 支援一對多轉換，轉換結果可輸出為純文字、HTML、JSON 等格式。
 * 支援 Unicode 組合字，例如「⿰虫鬼」視為一個字，不會因為詞典有「虫=>蟲」而被轉為「⿰蟲鬼」。
 * 支援用正規表示式略過特定文字的轉換。
 * 支援編碼轉換，可自訂輸入及輸出檔案的字元編碼。
 
@@ -109,15 +109,15 @@
 # perform a conversion for a string and process the result data generator
 [p for p in converter.convert("干了吧")]  # [StsDictConv(key=['干', '了'], values=['幹了', '乾了']), '吧']
 ```
 
 
 ## Configuration 配置
 
-如要自訂轉換方案，可參見[配置檔及詞典檔規格說明](./CONFIG.md)。
+如要自訂轉換方案，可參見[配置檔及詞典檔規格說明](https://github.com/danny0838/sts-lib/blob/master/CONFIG.md)。
 
 
 ## 線上版
 
 [簡繁祕書線上版](https://danny0838.github.io/sts-lib/)
 
 本線上轉換工具支援文字轉換及檔案轉換。前者只要在輸入區填入文字，就會自動轉換並且可以互動式校訂。後者可以用按鈕或拖放選擇一或多個檔案，就會逐一轉換後自動下載。預設檔案輸入輸出編碼皆是UTF-8，如要輸入其他編碼的檔案，可在進階選項設定。
```

### Comparing `sts_lib-0.29.0/README.md` & `sts_lib-0.29.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 簡繁祕書是開源、輕巧、有彈性的中文簡繁轉換工具，也支援異體字轉換及地區慣用詞轉換。
 
 
 ## Features 特色
 
 * 支援 [OpenCC](https://github.com/BYVoid/OpenCC) 格式及 JSON、YAML 格式的詞典檔。
-* 可透過配置檔組合多個詞典檔作為具體轉換方案。組合詞典可儲存成新詞典檔以加速未來載入使用，任一詞典檔更新時皆會自動重新生成組合詞典。支援的組合方式有「並聯」、「串聯」、「反轉」、「擴充」、「過濾」等等。
+* 可透過配置檔組合多個詞典檔作為具體轉換方案。組合詞典可儲存成新詞典檔以加速未來載入使用，任一詞典檔更新時皆會自動重新生成組合詞典。支援的組合方式有「並聯」、「串聯」、「反轉」、「展開」、「篩選」等等。
 * 簡繁對應、異體字對應、地區慣用詞對應等不同的對應關係皆區分至不同的詞典檔。
 * 詞典及配置檔與程式本體分離，可自由修改、擴充。
 * 支援一對多轉換，轉換結果可輸出為純文字、HTML、JSON 等格式。
 * 支援 Unicode 組合字，例如「⿰虫鬼」視為一個字，不會因為詞典有「虫=>蟲」而被轉為「⿰蟲鬼」。
 * 支援用正規表示式略過特定文字的轉換。
 * 支援編碼轉換，可自訂輸入及輸出檔案的字元編碼。
 
@@ -74,15 +74,15 @@
 # perform a conversion for a string and process the result data generator
 [p for p in converter.convert("干了吧")]  # [StsDictConv(key=['干', '了'], values=['幹了', '乾了']), '吧']
 ```
 
 
 ## Configuration 配置
 
-如要自訂轉換方案，可參見[配置檔及詞典檔規格說明](./CONFIG.md)。
+如要自訂轉換方案，可參見[配置檔及詞典檔規格說明](https://github.com/danny0838/sts-lib/blob/master/CONFIG.md)。
 
 
 ## 線上版
 
 [簡繁祕書線上版](https://danny0838.github.io/sts-lib/)
 
 本線上轉換工具支援文字轉換及檔案轉換。前者只要在輸入區填入文字，就會自動轉換並且可以互動式校訂。後者可以用按鈕或拖放選擇一或多個檔案，就會逐一轉換後自動下載。預設檔案輸入輸出編碼皆是UTF-8，如要輸入其他編碼的檔案，可在進階選項設定。
```

### Comparing `sts_lib-0.29.0/setup.cfg` & `sts_lib-0.29.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/__init__.py` & `sts_lib-0.29.1/sts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.29.0'
+__version__ = '0.29.1'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 
 
 class StreamList(list):
     """Convert an iterable into a serializable "list".
```

### Comparing `sts_lib-0.29.0/sts/cli.py` & `sts_lib-0.29.1/sts/cli.py`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/config/_default.json` & `sts_lib-0.29.1/sts/data/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/config/hk2s.json` & `sts_lib-0.29.1/sts/data/config/hk2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/config/s2twp.json` & `sts_lib-0.29.1/sts/data/config/s2twp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/config/tw2s.json` & `sts_lib-0.29.1/sts/data/config/tw2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/config/tw2sp.json` & `sts_lib-0.29.1/sts/data/config/tw2sp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.29.1/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.29.1/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.29.1/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.29.1/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.29.1/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.29.1/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.29.1/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.29.1/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.29.1/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.29.1/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.29.1/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.29.1/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/htmlpage.tpl.html` & `sts_lib-0.29.1/sts/data/htmlpage.tpl.html`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/scheme/st_multi.txt` & `sts_lib-0.29.1/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts/data/scheme/variant.txt` & `sts_lib-0.29.1/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.29.0/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.29.1/sts_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.29.0
+Version: 0.29.1
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -39,15 +39,15 @@
 
 簡繁祕書是開源、輕巧、有彈性的中文簡繁轉換工具，也支援異體字轉換及地區慣用詞轉換。
 
 
 ## Features 特色
 
 * 支援 [OpenCC](https://github.com/BYVoid/OpenCC) 格式及 JSON、YAML 格式的詞典檔。
-* 可透過配置檔組合多個詞典檔作為具體轉換方案。組合詞典可儲存成新詞典檔以加速未來載入使用，任一詞典檔更新時皆會自動重新生成組合詞典。支援的組合方式有「並聯」、「串聯」、「反轉」、「擴充」、「過濾」等等。
+* 可透過配置檔組合多個詞典檔作為具體轉換方案。組合詞典可儲存成新詞典檔以加速未來載入使用，任一詞典檔更新時皆會自動重新生成組合詞典。支援的組合方式有「並聯」、「串聯」、「反轉」、「展開」、「篩選」等等。
 * 簡繁對應、異體字對應、地區慣用詞對應等不同的對應關係皆區分至不同的詞典檔。
 * 詞典及配置檔與程式本體分離，可自由修改、擴充。
 * 支援一對多轉換，轉換結果可輸出為純文字、HTML、JSON 等格式。
 * 支援 Unicode 組合字，例如「⿰虫鬼」視為一個字，不會因為詞典有「虫=>蟲」而被轉為「⿰蟲鬼」。
 * 支援用正規表示式略過特定文字的轉換。
 * 支援編碼轉換，可自訂輸入及輸出檔案的字元編碼。
 
@@ -109,15 +109,15 @@
 # perform a conversion for a string and process the result data generator
 [p for p in converter.convert("干了吧")]  # [StsDictConv(key=['干', '了'], values=['幹了', '乾了']), '吧']
 ```
 
 
 ## Configuration 配置
 
-如要自訂轉換方案，可參見[配置檔及詞典檔規格說明](./CONFIG.md)。
+如要自訂轉換方案，可參見[配置檔及詞典檔規格說明](https://github.com/danny0838/sts-lib/blob/master/CONFIG.md)。
 
 
 ## 線上版
 
 [簡繁祕書線上版](https://danny0838.github.io/sts-lib/)
 
 本線上轉換工具支援文字轉換及檔案轉換。前者只要在輸入區填入文字，就會自動轉換並且可以互動式校訂。後者可以用按鈕或拖放選擇一或多個檔案，就會逐一轉換後自動下載。預設檔案輸入輸出編碼皆是UTF-8，如要輸入其他編碼的檔案，可在進階選項設定。
```

### Comparing `sts_lib-0.29.0/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.29.1/sts_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

