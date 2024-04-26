# Comparing `tmp/mkt-retv-1.407.tar.gz` & `tmp/mkt-retv-1.408.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkt-retv-1.407.tar", last modified: Thu Apr 25 14:58:34 2024, max compression
+gzip compressed data, was "mkt-retv-1.408.tar", last modified: Thu Apr 25 15:09:39 2024, max compression
```

## Comparing `mkt-retv-1.407.tar` & `mkt-retv-1.408.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.366094 mkt-retv-1.407/
--rw-rw-rw-   0        0        0      697 2024-04-25 14:58:34.366094 mkt-retv-1.407/PKG-INFO
--rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.407/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 14:58:33.878100 mkt-retv-1.407/market_research/
--rw-rw-rw-   0        0        0        2 2023-11-21 12:45:19.000000 mkt-retv-1.407/market_research/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:58:33.972791 mkt-retv-1.407/market_research/analysis/
--rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.407/market_research/analysis/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.407/market_research/analysis/_analysis_scheme.py
--rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.407/market_research/analysis/imgemanger.py
--rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.407/market_research/analysis/sentimentmanager.py
--rw-rw-rw-   0        0        0     4939 2024-01-28 14:17:23.000000 mkt-retv-1.407/market_research/analysis/textmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.019623 mkt-retv-1.407/market_research/scraper/
--rw-rw-rw-   0        0        0      451 2024-01-24 12:15:44.000000 mkt-retv-1.407/market_research/scraper/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.407/market_research/scraper/_scaper_scheme.py
--rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.407/market_research/scraper/_visualizer_scheme.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.019623 mkt-retv-1.407/market_research/scraper/models/
--rw-rw-rw-   0        0        0        0 2023-11-21 12:44:57.000000 mkt-retv-1.407/market_research/scraper/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.068391 mkt-retv-1.407/market_research/scraper/models/pana/
--rw-rw-rw-   0        0        0        0 2023-11-21 12:44:12.000000 mkt-retv-1.407/market_research/scraper/models/pana/__init__.py
--rw-rw-rw-   0        0        0     6484 2024-01-24 12:45:30.000000 mkt-retv-1.407/market_research/scraper/models/pana/spec_p.py
--rw-rw-rw-   0        0        0    12563 2024-01-24 13:16:23.000000 mkt-retv-1.407/market_research/scraper/models/pana/spec_pjp.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.146841 mkt-retv-1.407/market_research/scraper/models/sony/
--rw-rw-rw-   0        0        0        4 2023-11-21 12:44:57.000000 mkt-retv-1.407/market_research/scraper/models/sony/__init__.py
--rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:31.000000 mkt-retv-1.407/market_research/scraper/models/sony/cleanup_s.py
--rw-rw-rw-   0        0        0    10226 2024-01-24 12:45:30.000000 mkt-retv-1.407/market_research/scraper/models/sony/sepc_sjp.py
--rw-rw-rw-   0        0        0    12121 2024-04-25 13:55:31.000000 mkt-retv-1.407/market_research/scraper/models/sony/spec_s.py
--rw-rw-rw-   0        0        0     4189 2024-04-25 14:57:40.000000 mkt-retv-1.407/market_research/scraper/models/sony/visualizer_s.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.225002 mkt-retv-1.407/market_research/scraper/rtings/
--rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.407/market_research/scraper/rtings/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.407/market_research/scraper/rtings/rtings.py
--rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.407/market_research/scraper/rtings/rurlsearcher.py
--rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.407/market_research/scraper/rtings/rvisualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.287507 mkt-retv-1.407/market_research/tools/
--rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.407/market_research/tools/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.407/market_research/tools/aimanager.py
--rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.407/market_research/tools/filemanager.py
--rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.407/market_research/tools/installer.py
--rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.407/market_research/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-04-25 14:58:34.350440 mkt-retv-1.407/mkt_retv.egg-info/
--rw-rw-rw-   0        0        0      697 2024-04-25 14:58:33.000000 mkt-retv-1.407/mkt_retv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1351 2024-04-25 14:58:33.000000 mkt-retv-1.407/mkt_retv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 14:58:33.000000 mkt-retv-1.407/mkt_retv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-25 14:58:33.000000 mkt-retv-1.407/mkt_retv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-04-25 14:58:33.000000 mkt-retv-1.407/mkt_retv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-25 14:58:33.000000 mkt-retv-1.407/mkt_retv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-25 14:58:34.366094 mkt-retv-1.407/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-04-25 14:58:14.000000 mkt-retv-1.407/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:09:39.314540 mkt-retv-1.408/
+-rw-rw-rw-   0        0        0      697 2024-04-25 15:09:39.313540 mkt-retv-1.408/PKG-INFO
+-rw-rw-rw-   0        0        0     1637 2024-01-28 21:55:38.000000 mkt-retv-1.408/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 15:09:39.225013 mkt-retv-1.408/market_research/
+-rw-rw-rw-   0        0        0        2 2023-11-21 12:45:19.000000 mkt-retv-1.408/market_research/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:09:39.234013 mkt-retv-1.408/market_research/analysis/
+-rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.408/market_research/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.408/market_research/analysis/_analysis_scheme.py
+-rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.408/market_research/analysis/imgemanger.py
+-rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.408/market_research/analysis/sentimentmanager.py
+-rw-rw-rw-   0        0        0     4939 2024-01-28 14:17:23.000000 mkt-retv-1.408/market_research/analysis/textmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:09:39.240905 mkt-retv-1.408/market_research/scraper/
+-rw-rw-rw-   0        0        0      451 2024-01-24 12:15:44.000000 mkt-retv-1.408/market_research/scraper/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.408/market_research/scraper/_scaper_scheme.py
+-rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.408/market_research/scraper/_visualizer_scheme.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:09:39.242907 mkt-retv-1.408/market_research/scraper/models/
+-rw-rw-rw-   0        0        0        0 2023-11-21 12:44:57.000000 mkt-retv-1.408/market_research/scraper/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:09:39.247914 mkt-retv-1.408/market_research/scraper/models/pana/
+-rw-rw-rw-   0        0        0        0 2023-11-21 12:44:12.000000 mkt-retv-1.408/market_research/scraper/models/pana/__init__.py
+-rw-rw-rw-   0        0        0     6486 2024-04-25 15:07:33.000000 mkt-retv-1.408/market_research/scraper/models/pana/spec_p.py
+-rw-rw-rw-   0        0        0    12572 2024-04-25 15:07:18.000000 mkt-retv-1.408/market_research/scraper/models/pana/spec_pjp.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:09:39.256914 mkt-retv-1.408/market_research/scraper/models/sony/
+-rw-rw-rw-   0        0        0        4 2023-11-21 12:44:57.000000 mkt-retv-1.408/market_research/scraper/models/sony/__init__.py
+-rw-rw-rw-   0        0        0     5265 2024-04-25 14:52:31.000000 mkt-retv-1.408/market_research/scraper/models/sony/cleanup_s.py
+-rw-rw-rw-   0        0        0    10235 2024-04-25 15:08:00.000000 mkt-retv-1.408/market_research/scraper/models/sony/sepc_sjp.py
+-rw-rw-rw-   0        0        0    12124 2024-04-25 15:08:00.000000 mkt-retv-1.408/market_research/scraper/models/sony/spec_s.py
+-rw-rw-rw-   0        0        0     4189 2024-04-25 14:57:40.000000 mkt-retv-1.408/market_research/scraper/models/sony/visualizer_s.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:09:39.265541 mkt-retv-1.408/market_research/scraper/rtings/
+-rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.408/market_research/scraper/rtings/__init__.py
+-rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.408/market_research/scraper/rtings/rtings.py
+-rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.408/market_research/scraper/rtings/rurlsearcher.py
+-rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.408/market_research/scraper/rtings/rvisualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:09:39.274542 mkt-retv-1.408/market_research/tools/
+-rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.408/market_research/tools/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.408/market_research/tools/aimanager.py
+-rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.408/market_research/tools/filemanager.py
+-rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.408/market_research/tools/installer.py
+-rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.408/market_research/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-04-25 15:09:39.311541 mkt-retv-1.408/mkt_retv.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-04-25 15:09:38.000000 mkt-retv-1.408/mkt_retv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1351 2024-04-25 15:09:39.000000 mkt-retv-1.408/mkt_retv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 15:09:38.000000 mkt-retv-1.408/mkt_retv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-25 15:09:38.000000 mkt-retv-1.408/mkt_retv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-04-25 15:09:38.000000 mkt-retv-1.408/mkt_retv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-25 15:09:38.000000 mkt-retv-1.408/mkt_retv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-25 15:09:39.315540 mkt-retv-1.408/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-04-25 15:09:31.000000 mkt-retv-1.408/setup.py
```

### Comparing `mkt-retv-1.407/PKG-INFO` & `mkt-retv-1.408/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.407
+Version: 1.408
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.407/README.md` & `mkt-retv-1.408/README.md`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/analysis/_analysis_scheme.py` & `mkt-retv-1.408/market_research/analysis/_analysis_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/analysis/imgemanger.py` & `mkt-retv-1.408/market_research/analysis/imgemanger.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/analysis/sentimentmanager.py` & `mkt-retv-1.408/market_research/analysis/sentimentmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/analysis/textmanager.py` & `mkt-retv-1.408/market_research/analysis/textmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/scraper/_scaper_scheme.py` & `mkt-retv-1.408/market_research/scraper/_scaper_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/scraper/models/pana/spec_p.py` & `mkt-retv-1.408/market_research/scraper/models/pana/spec_p.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from collections import OrderedDict
 import pandas as pd
 from market_research.scraper._scaper_scheme import Scraper
 from market_research.tools import FileManager
 class ModelScraper_p(Scraper):
 
     def __init__(self, enable_headless=True,
-                 export_prefix="model_pana_global", intput_folder_path="input", output_folder_path="results",
+                 export_prefix="pana_model_info_web", intput_folder_path="input", output_folder_path="results",
                  verbose: bool = False, wait_time=1):
         super().__init__(enable_headless=enable_headless, export_prefix=export_prefix,
                          intput_folder_path=intput_folder_path, output_folder_path=output_folder_path)
         self.tracking_log = verbose
         self.wait_time = wait_time
```

### Comparing `mkt-retv-1.407/market_research/scraper/models/pana/spec_pjp.py` & `mkt-retv-1.408/market_research/scraper/models/pana/spec_pjp.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from collections import OrderedDict
 import pandas as pd
 from market_research.scraper._scaper_scheme import Scraper
 import pickle
 class ModelScraper_pjp(Scraper):
 
     def __init__(self, enable_headless=True,
-                 export_prefix="model_sony_jp", intput_folder_path="input", output_folder_path="results",
+                 export_prefix="pana_model_info_web_jp", intput_folder_path="input", output_folder_path="results",
                  verbose: bool = False, wait_time=1):
         super().__init__(enable_headless=enable_headless, export_prefix=export_prefix,
                          intput_folder_path=intput_folder_path, output_folder_path=output_folder_path)
 
         self.tracking_log = verbose
         self.wait_time = wait_time
         self.file_manager = FileManager
```

### Comparing `mkt-retv-1.407/market_research/scraper/models/sony/cleanup_s.py` & `mkt-retv-1.408/market_research/scraper/models/sony/cleanup_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/scraper/models/sony/sepc_sjp.py` & `mkt-retv-1.408/market_research/scraper/models/sony/sepc_sjp.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from tqdm import tqdm
 from collections import OrderedDict
 import pandas as pd
 from market_research.scraper._scaper_scheme import Scraper
 class ModelScraper_sjp(Scraper):
 
     def __init__(self, enable_headless=True,
-                 export_prefix="model_sony_jp", intput_folder_path="input", output_folder_path="results",
+                 export_prefix="sony_model_info_web_jp", intput_folder_path="input", output_folder_path="results",
                  verbose: bool = False, wait_time=1):
         super().__init__(enable_headless=enable_headless, export_prefix=export_prefix,
                          intput_folder_path=intput_folder_path, output_folder_path=output_folder_path)
 
         self.tracking_log = verbose
         self.wait_time = wait_time
         self.file_manager = FileManager
```

### Comparing `mkt-retv-1.407/market_research/scraper/models/sony/spec_s.py` & `mkt-retv-1.408/market_research/scraper/models/sony/spec_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.action_chains import ActionChains
 from market_research.tools import FileManager
 from market_research.scraper._scaper_scheme import Scraper
 
 class ModelScraper_s(Scraper):
     def __init__(self, enable_headless=True,
-                 export_prefix="model_sony_gobal", intput_folder_path="input",  output_folder_path="results",
+                 export_prefix="sony_model_info_web", intput_folder_path="input",  output_folder_path="results",
                  verbose: bool = False, wait_time=2):
 
         super().__init__(enable_headless=enable_headless, export_prefix=export_prefix,  intput_folder_path=intput_folder_path, output_folder_path=output_folder_path)
 
         self.tracking_log = verbose
         self.wait_time = wait_time
         self.file_manager = FileManager
```

### Comparing `mkt-retv-1.407/market_research/scraper/models/sony/visualizer_s.py` & `mkt-retv-1.408/market_research/scraper/models/sony/visualizer_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/scraper/rtings/rtings.py` & `mkt-retv-1.408/market_research/scraper/rtings/rtings.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/scraper/rtings/rurlsearcher.py` & `mkt-retv-1.408/market_research/scraper/rtings/rurlsearcher.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/scraper/rtings/rvisualizer.py` & `mkt-retv-1.408/market_research/scraper/rtings/rvisualizer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/tools/aimanager.py` & `mkt-retv-1.408/market_research/tools/aimanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/tools/filemanager.py` & `mkt-retv-1.408/market_research/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/tools/installer.py` & `mkt-retv-1.408/market_research/tools/installer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/market_research/tools/webdriver.py` & `mkt-retv-1.408/market_research/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/mkt_retv.egg-info/PKG-INFO` & `mkt-retv-1.408/mkt_retv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.407
+Version: 1.408
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.407/mkt_retv.egg-info/SOURCES.txt` & `mkt-retv-1.408/mkt_retv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.407/setup.py` & `mkt-retv-1.408/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkt-retv',
-    version='1.407',
+    version='1.408',
     author='xikest',
     description='market research TV ',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy', 'pandas',
         'selenium','beautifulsoup4','requests',
```

