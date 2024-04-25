# Comparing `tmp/pkscreener-0.44.20240424.291.tar.gz` & `tmp/pkscreener-0.44.20240425.292.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240424.291.tar", last modified: Wed Apr 24 11:38:28 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240425.292.tar", last modified: Thu Apr 25 22:36:09 2024, max compression
```

## Comparing `pkscreener-0.44.20240424.291.tar` & `pkscreener-0.44.20240425.292.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 11:38:28.099260 pkscreener-0.44.20240424.291/
--rw-rw-rw-   0        0        0     1086 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-24 11:38:28.099260 pkscreener-0.44.20240424.291/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 11:38:28.083638 pkscreener-0.44.20240424.291/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 11:38:28.099260 pkscreener-0.44.20240424.291/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    25815 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9868 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     7038 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    29415 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    20931 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    19689 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8120 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    17306 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   113351 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    51052 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    81600 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-24 11:38:18.000000 pkscreener-0.44.20240424.291/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   122734 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/globals.py
--rw-rw-rw-   0        0        0      595 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    48027 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    25383 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-24 11:38:28.083638 pkscreener-0.44.20240424.291/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-24 11:38:28.000000 pkscreener-0.44.20240424.291/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1318 2024-04-24 11:38:28.000000 pkscreener-0.44.20240424.291/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 11:38:28.000000 pkscreener-0.44.20240424.291/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-04-24 11:38:28.000000 pkscreener-0.44.20240424.291/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-24 11:38:28.000000 pkscreener-0.44.20240424.291/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-24 11:38:28.000000 pkscreener-0.44.20240424.291/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-24 11:38:28.099260 pkscreener-0.44.20240424.291/setup.cfg
--rw-rw-rw-   0        0        0     4727 2024-04-24 11:33:43.000000 pkscreener-0.44.20240424.291/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 22:36:09.952550 pkscreener-0.44.20240425.292/
+-rw-rw-rw-   0        0        0     1086 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-25 22:36:09.952550 pkscreener-0.44.20240425.292/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 22:36:09.936924 pkscreener-0.44.20240425.292/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 22:36:09.952550 pkscreener-0.44.20240425.292/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    25815 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     7288 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    29415 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    20931 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    20421 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8124 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    17306 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   113351 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    51289 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    81788 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-25 22:36:01.000000 pkscreener-0.44.20240425.292/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   123035 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      595 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    48027 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    25522 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-25 22:36:09.936924 pkscreener-0.44.20240425.292/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-25 22:36:09.000000 pkscreener-0.44.20240425.292/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1318 2024-04-25 22:36:09.000000 pkscreener-0.44.20240425.292/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 22:36:09.000000 pkscreener-0.44.20240425.292/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-25 22:36:09.000000 pkscreener-0.44.20240425.292/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 22:36:09.000000 pkscreener-0.44.20240425.292/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-25 22:36:09.000000 pkscreener-0.44.20240425.292/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-25 22:36:09.952550 pkscreener-0.44.20240425.292/setup.cfg
+-rw-rw-rw-   0        0        0     4727 2024-04-25 22:32:57.000000 pkscreener-0.44.20240425.292/setup.py
```

### Comparing `pkscreener-0.44.20240424.291/LICENSE` & `pkscreener-0.44.20240425.292/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/LICENSE-Others` & `pkscreener-0.44.20240425.292/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/PKG-INFO` & `pkscreener-0.44.20240425.292/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240424.291
+Version: 0.44.20240425.292
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240424.291.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240425.292.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -218,15 +218,15 @@
 |  8  |       **Trend**       | By using advance algorithms, the average trendlines are computed for `N` days and their strenght is displayed depending on steepness of trendlines. (This does NOT show any trendline on chart, it is calculated internally) | `Strong Up`, `Weak Down` etc.                                                            |
 |  9  |      **Pattern**      | If the chart or the candle itself forming any important pattern in the recent timeframe or as per the selected screening option, various important patterns will be indicated here.                                          | `Momentum Gainer`, `Inside Bar (N)`,`Bullish Engulfing` etc.                             |
 
 ## Hack it your way:
 Feel free to Edit the parameters in the `pkscreener.ini` file which will be generated by the application.
 ```
 [config]
-period = 450d
+period = 280d
 daystolookback = 22
 duration = 1d
 minprice = 20.0
 maxprice = 50000.0
 volumeratio = 2.5
 consolidationpercentage = 10.0
 shuffle = y
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.290/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.291/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.290/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.291/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.290/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.291/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240424.291/README.md` & `pkscreener-0.44.20240425.292/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 |  8  |       **Trend**       | By using advance algorithms, the average trendlines are computed for `N` days and their strenght is displayed depending on steepness of trendlines. (This does NOT show any trendline on chart, it is calculated internally) | `Strong Up`, `Weak Down` etc.                                                            |
 |  9  |      **Pattern**      | If the chart or the candle itself forming any important pattern in the recent timeframe or as per the selected screening option, various important patterns will be indicated here.                                          | `Momentum Gainer`, `Inside Bar (N)`,`Bullish Engulfing` etc.                             |
 
 ## Hack it your way:
 Feel free to Edit the parameters in the `pkscreener.ini` file which will be generated by the application.
 ```
 [config]
-period = 450d
+period = 280d
 daystolookback = 22
 duration = 1d
 minprice = 20.0
 maxprice = 50000.0
 volumeratio = 2.5
 consolidationpercentage = 10.0
 shuffle = y
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.290/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.291/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.290/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.291/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.290/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.291/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240424.291/pkscreener/__init__.py` & `pkscreener-0.44.20240425.292/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/ConfigManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,28 +32,28 @@
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 from PKDevTools.classes.OutputControls import OutputControls
 parser = configparser.ConfigParser(strict=False)
 
 # Default attributes for Downloading Cache from Git repo
-default_period = "450d"
+default_period = "280d"
 default_duration = "1d"
 default_timeout = 2
 
 
 # This Class manages read/write of user configuration
 class tools(SingletonMixin, metaclass=SingletonType):
     def __init__(self):
         super(tools, self).__init__()
         self.consolidationPercentage = 10
         self.volumeRatio = 2.5
         self.minLTP = 20.0
         self.maxLTP = 50000
-        self.period = "450d"
+        self.period = "280d"
         self.duration = "1d"
         self.shuffleEnabled = True
         self.cacheEnabled = True
         self.stageTwo = True
         self.useEMA = False
         self.showunknowntrends = True
         self.enablePortfolioCalculations = False
@@ -198,15 +198,15 @@
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.GREEN
                 + "[+] PKScreener User Configuration:"
                 + colorText.END
             )
             self.period = input(
-                "[+] Enter number of days for which stock data to be downloaded (Days)(Optimal = 450): "
+                "[+] Enter number of days for which stock data to be downloaded (Days)(Optimal = 280): "
             )
             self.daysToLookback = input(
                 "[+] Number of recent trading periods (TimeFrame) to screen for Breakout/Consolidation (Days)(Optimal = 22): "
             )
             self.duration = input(
                 "[+] Enter Duration of each candle (Days)(Optimal = 1): "
             )
@@ -445,15 +445,15 @@
 
     # Toggle the duration and period for use in intraday and swing trading
     def toggleConfig(self, candleDuration, clearCache=True):
         if candleDuration is None:
             candleDuration = self.duration.lower()
         self.getConfig(parser)
         if candleDuration[-1] in ["d"]:
-            self.period = "450d"
+            self.period = "280d"
             self.cacheEnabled = True
         if candleDuration[-1] in ["m", "h"] and not self.isIntradayConfig():
             self.period = "1d"
             self.cacheEnabled = True
         if self.isIntradayConfig():
             self.duration = candleDuration if candleDuration[-1] in ["m", "h"] else "1m"
             candleType = candleDuration.replace("m","").replace("h","")
```

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/Fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,17 +96,21 @@
                 stockCode = [(f"{x}{exchangeSuffix}" if not x.endswith(exchangeSuffix) else x) for x in stockCode]
         elif isinstance(stockCode,str):
             if len(exchangeSuffix) > 0:
                 stockCode = f"{stockCode}{exchangeSuffix}" if not stockCode.endswith(exchangeSuffix) else stockCode
         if (period == '1d' or duration[-1] == "m"):
             # Since this is intraday data, we'd just need to start from the last trading session
             if start is None:
-                start = PKDateUtilities.tradingDate()
+                start = PKDateUtilities.tradingDate().strftime("%Y-%m-%d")
             if end is None:
                 end = PKDateUtilities.currentDateTime().strftime("%Y-%m-%d")
+            if start == end:
+                # If we send start and end dates for intraday, it comes back with empty dataframe
+                start = None
+                end = None
         with SuppressOutput(suppress_stdout=True, suppress_stderr=True):
             data = yf.download(
                 tickers=stockCode,
                 period=period,
                 interval=duration,
                 proxy=proxyServer,
                 progress=False,
```

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/MarketMonitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         highlightRows = []
         highlightCols = []
         if screen_df is None or screen_df.empty:
             return
 
         screen_monitor_df = screen_df.copy()
         screen_monitor_df.reset_index(inplace=True)
-        screen_monitor_df = screen_monitor_df[["Stock", "LTP", "%Chng","52Wk H","RSI","Volume"]].head(self.maxNumRowsInEachResult-1)
+        screen_monitor_df = screen_monitor_df[["Stock", "LTP", "%Chng","52Wk H","RSI/i","Volume"]].head(self.maxNumRowsInEachResult-1)
         screen_monitor_df.loc[:, "%Chng"] = screen_monitor_df.loc[:, "%Chng"].apply(
                     lambda x: Utility.tools.roundOff(str(x).split("% (")[0] + colorText.END,0)
                 )
         screen_monitor_df.loc[:, "52Wk H"] = screen_monitor_df.loc[:, "52Wk H"].apply(
             lambda x: Utility.tools.roundOff(x,0)
         )
         screen_monitor_df.loc[:, "Volume"] = screen_monitor_df.loc[:, "Volume"].apply(
@@ -103,15 +103,18 @@
             colIndex = 0
             highlightRows = [startRowIndex]
             highlightCols = []
             while rowIndex <= len(screen_monitor_df):
                 for col in screen_monitor_df.columns:
                     if rowIndex == 0:
                         # Column names to be repeated for each refresh in respective headers
-                        widgetHeader = ":".join(screenOptions.replace(":D","").split(":")[:4])
+                        cleanedScreenOptions = screenOptions.replace(":D","")
+                        widgetHeader = ":".join(cleanedScreenOptions.split(":")[:4])
+                        if "i " in screenOptions:
+                            widgetHeader = f'{":".join(widgetHeader.split(":")[:3])}:i:{cleanedScreenOptions.split("i ")[-1]}'
                         self.monitor_df.loc[startRowIndex,[f"A{startColIndex+1}"]] = colorText.BOLD+colorText.HEAD+(widgetHeader if startColIndex==firstColIndex else col)+colorText.END
                         highlightCols.append(startColIndex)
                     else:
                         self.monitor_df.loc[startRowIndex, [f"A{startColIndex+1}"]] = screen_monitor_df.iloc[rowIndex-1,colIndex]
                         colIndex += 1
                     startColIndex += 1
                 _, startColIndex= monitorPosition
```

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/PKScanRunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,19 +104,20 @@
         totalConsumers = min(minimumCount, multiprocessing.cpu_count())
         if totalConsumers == 1:
             totalConsumers = 2  # This is required for single core machine
         if PKScanRunner.configManager.cacheEnabled is True and multiprocessing.cpu_count() > 2:
             totalConsumers -= 1
         return tasks_queue, results_queue, totalConsumers, logging_queue
 
-    def populateQueues(items, tasks_queue, exit=False):
+    def populateQueues(items, tasks_queue, exit=False,userPassedArgs=None):
         # default_logger().debug(f"Unfinished items in task_queue: {tasks_queue.qsize()}")
         for item in items:
             tasks_queue.put(item)
-        if exit:
+        mayBePiped = userPassedArgs is not None and (userPassedArgs.monitor is not None or "|" in userPassedArgs.options)
+        if exit and not mayBePiped:
             # Append exit signal for each process indicated by None
             for _ in range(multiprocessing.cpu_count()):
                 tasks_queue.put(None)
 
 
     def getScanDurationParameters(testing, menuOption):
         # Number of days from past, including the backtest duration chosen by the user
@@ -229,18 +230,19 @@
     
     def getFormattedChoices(userArgs, selectedChoice):
         isIntraday = PKScanRunner.configManager.isIntradayConfig() or (
             userArgs.intraday is not None
         )
         choices = ""
         for choice in selectedChoice:
-            if len(selectedChoice[choice]) > 0:
+            choiceOption = selectedChoice[choice]
+            if len(choiceOption) > 0 and ("," not in choiceOption and "." not in choiceOption):
                 if len(choices) > 0:
                     choices = f"{choices}_"
-                choices = f"{choices}{selectedChoice[choice]}"
+                choices = f"{choices}{choiceOption}"
         if choices.endswith("_"):
             choices = choices[:-1]
         choices = f"{choices}{'_i' if isIntraday else ''}"
         return choices
 
     def refreshDatabase(consumers,stockDictPrimary,stockDictSecondary):
         for worker in consumers:
@@ -253,14 +255,17 @@
             tasks_queue, results_queue, consumers,logging_queue = PKScanRunner.prepareToRunScan(keyboardInterruptEvent,screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items)
             try:
                 if logging_queue is not None:
                     log_queue_reader = LogQueueReader(logging_queue)
                     log_queue_reader.start()
             except:
                 pass
+        # else:
+        #     # Restart the workers because the run method may have exited from a previous run
+        #     PKScanRunner.startWorkers(consumers)
         PKScanRunner.tasks_queue = tasks_queue
         PKScanRunner.results_queue = results_queue
         PKScanRunner.consumers = consumers
         screenResults, saveResults, backtest_df = scanningCb(
                     menuOption,
                     items,
                     PKScanRunner.tasks_queue,
@@ -272,15 +277,18 @@
                     screenResults,
                     saveResults,
                     backtest_df,
                     testing=testing,
                 )
 
         OutputControls().printOutput(colorText.END)
-        if userPassedArgs is not None and userPassedArgs.monitor is None:
+        if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options):
+            # Don't terminate the multiprocessing clients if we're 
+            # going to pipe the results from an earlier run
+            # or we're running in monitoring mode
             PKScanRunner.terminateAllWorkers(consumers, tasks_queue, testing)
         return screenResults, saveResults,backtest_df,tasks_queue, results_queue, consumers, logging_queue
 
     def prepareToRunScan(keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items):
         tasks_queue, results_queue, totalConsumers, logging_queue = PKScanRunner.initQueues(len(items))
         scr = ScreeningStatistics.ScreeningStatistics(PKScanRunner.configManager, default_logger())
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=PKScanRunner.configManager.isIntradayConfig())
@@ -372,15 +380,15 @@
         PKScanRunner.results_queue = None
         PKScanRunner.scr = None
         PKScanRunner.consumers = None
 
     def shutdown(frame, signum):
         OutputControls().printOutput("Shutting down for test coverage")
 
-    def runScan(testing,numStocks,iterations,items,numStocksPerIteration,tasks_queue,results_queue,originalNumberOfStocks,backtest_df, *otherArgs,resultsReceivedCb=None):
+    def runScan(userPassedArgs,testing,numStocks,iterations,items,numStocksPerIteration,tasks_queue,results_queue,originalNumberOfStocks,backtest_df, *otherArgs,resultsReceivedCb=None):
         queueCounter = 0
         counter = 0
         shouldContinue = True
         lastNonNoneResult = None
         while numStocks:
             if counter == 0 and numStocks > 0:
                 if queueCounter < int(iterations):
@@ -388,23 +396,25 @@
                         items[
                             numStocksPerIteration
                             * queueCounter : numStocksPerIteration
                             * (queueCounter + 1)
                         ],
                         tasks_queue,
                         (queueCounter + 1 == int(iterations)) and ((queueCounter + 1)*int(iterations) == originalNumberOfStocks),
+                        userPassedArgs
                     )
                 else:
                     PKScanRunner.populateQueues(
                         items[
                             numStocksPerIteration
                             * queueCounter :
                         ],
                         tasks_queue,
                         True,
+                        userPassedArgs
                     )
             result = results_queue.get()
             if result is not None:
                 lastNonNoneResult = result
             numStocks -= 1
             if resultsReceivedCb is not None:
                 shouldContinue, backtest_df = resultsReceivedCb(result, numStocks, backtest_df,*otherArgs)
```

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/PKScheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,16 +146,16 @@
                             completed=1,
                             total=1,
                             visible=False,
                         )
                     lock.acquire()
                     progress.refresh()
                     # raise any errors:
-                    for future in futures:
-                        future.result()
+                    # for future in futures:
+                    #     future.result()
                     lock.release()
 
 # if __name__ == "__main__":
 #     scheduleTasks([PKTask("Task 1",long_running_fn,),
 #                 PKTask("Task 2",long_running_fn),
 #                 PKTask("Task 3",long_running_fn),
 #                 PKTask("Task 4",long_running_fn),
```

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/StockScreener.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,19 +97,19 @@
             with hostRef.processingCounter.get_lock():
                 hostRef.processingCounter.value += 1
 
             volumeRatio, period = self.determineBasicConfigs(stock, newlyListedOnly, volumeRatio, logLevel, hostRef, configManager, screener, userArgsLog)
             # hostRef.default_logger.info(
             #     f"For stock:{stock}, stock exists in objectDictionary:{hostRef.objectDictionaryPrimary.get(stock)}, cacheEnabled:{configManager.cacheEnabled}, isTradingTime:{self.isTradingTime}, downloadOnly:{downloadOnly}"
             # )
-            data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef,hostRef.objectDictionaryPrimary, configManager, fetcher, period, testData,exchangeName)
+            data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef,hostRef.objectDictionaryPrimary, configManager, fetcher, period,None, testData,exchangeName)
             if not configManager.isIntradayConfig() and configManager.calculatersiintraday:
                 # Daily data is already available in "data" above.
                 # We need the intraday data for 1-d RSI values when config is not for intraday
-                intraday_data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef, hostRef.objectDictionarySecondary, configManager, fetcher, period, testData,exchangeName)
+                intraday_data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef, hostRef.objectDictionarySecondary, configManager, fetcher, "1d","1m", testData,exchangeName)
                 
             if data is not None:
                 if len(data) == 0 or len(data) < backtestDuration:
                     raise StockDataEmptyException(f"Data length:{len(data)}")
             else:
                 raise StockDataEmptyException(f"Data is None: {data}")
             # hostRef.default_logger.info(f"Will pre-process data:\n{data.tail(10)}")
@@ -719,38 +719,39 @@
                     # data has the last row from inputData at the top.
                 fullData, processedData = screener.preprocessData(
                         inputData, daysToLookback=configManager.daysToLookback
                     )
                 
         return fullData,processedData,data
 
-    def getRelevantDataForStock(self, totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef,objectDictionary, configManager, fetcher, period, testData=None,exchangeName="INDIA"):
+    def getRelevantDataForStock(self, totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef,objectDictionary, configManager, fetcher, period, duration, testData=None,exchangeName="INDIA"):
         hostData = objectDictionary.get(stock) if (objectDictionary is not None and len(objectDictionary) > 0) else None
         data = None
+        hostDataLength = 0 if hostData is None else (0 if "data" not in hostData.keys() else len(hostData["data"]))
         start = None
         if (period == '1d' or configManager.duration[-1] == "m"):
             if backtestDuration > 0: # We are backtesting
                 start = PKDateUtilities.nthPastTradingDateStringFromFutureDate(backtestDuration)
             else:
                 # Since this is intraday data, we'd just need to start from the last trading session
-                start = PKDateUtilities.tradingDate()
+                start = PKDateUtilities.tradingDate().strftime("%Y-%m-%d")
             end = PKDateUtilities.currentDateTime().strftime("%Y-%m-%d")
         if (
                 not shouldCache
                 or (downloadOnly and hostData is None)
                 or (hostData is None and self.isTradingTime)
-                or hostData is None
+                or hostData is None or hostDataLength == 0
             ):
             if testData is not None:
                 data = testData
             else:
                 data = fetcher.fetchStockData(
                         stock,
                         period,
-                        configManager.duration,
+                        configManager.duration if duration is None else duration,
                         hostRef.proxyServer,
                         hostRef.processingResultsCounter,
                         hostRef.processingCounter,
                         totalSymbols,
                         start=start,
                         end=start,
                         exchangeSuffix=".NS" if exchangeName == "INDIA" else ""
@@ -790,15 +791,15 @@
                     columns.append(f"temp{num_diff}")
                     num_diff -= 1
                 data = pd.DataFrame(
                         hostData["data"], columns=columns, index=hostData["index"]
                     )
                 pass
 
-        if ((shouldCache and not self.isTradingTime and (hostData is None)) or downloadOnly) \
+        if ((shouldCache and not self.isTradingTime and (hostData is None  or hostDataLength == 0)) or downloadOnly) \
             or (shouldCache and hostData is None):  # and backtestDuration == 0 # save only if we're NOT backtesting
                 if start is None and data is not None:
                     objectDictionary[stock] = data.to_dict("split")
                 if downloadOnly:
                     with hostRef.processingResultsCounter.get_lock():
                         hostRef.processingResultsCounter.value += 1
                     raise ScreeningStatistics.DownloadDataOnly
```

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/Utility.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,18 +196,18 @@
                     finalStocks = ",".join(stockList)
                     needsWriting = True
             if needsWriting:
                 with open(fileName, 'w') as f:
                     f.write(finalStocks)
         except IOError as e:  # pragma: no cover
             default_logger().debug(e, exc_info=True)
-            input(
+            OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
-                + "[+] Failed to save recently screened result table on disk! Skipping.."
+                + f"{e}\n[+] Failed to save recently screened result table on disk! Skipping.."
                 + colorText.END
             )
         except Exception as e:# pragma: no cover
             default_logger().debug(e, exc_info=True)
             pass
 
     # Load last screened result to pickle file
@@ -701,16 +701,17 @@
 
     def getLegendHelpText(table,backtestSummary):
         legendText = "\n*** 1. Stock ***: This is the NSE symbol/ticker for a company. Stocks that are NOT stage two, are coloured red. *** 2. Consol. ***: It shows the price range in which stock is trading for the last 22 trading sessions(22 trading sessions per month) *** 3. Breakout(22Prds) ***: The BO is Breakout level based on last 22 sessions. R is the resistance level (if available)."
         legendText = f"{legendText} An investor should consider both BO & R level to analyse entry / exits in their trading lessons. If the BO value is green, it means the stock has already broken out (is above BO level). If BO is in red, it means the stock is yet to break out.  *** 4. LTP ***: This is the last/latest trading/closing price of the given stock on a given date at NSE. The LTP in green/red means the"
         legendText = f"{legendText} stock price has increased / decreased since last trading session. (1.5%, 1.3%,1.8%) with LTP shows the stock price rose by 1.5%, 1.3% and 1.8% in the last 1, 2 and 3 trading sessions respectively. *** 5. %Chng ***: This is the change(rise/fall in percentage) in closing/trading price from the previous trading session's closing price. Green means that price rose from the previous"
         legendText = f"{legendText} trading session. Red means it fell.  *** 6. Volume ***: This shows the relative volume in the most recent trading day /today with respect to last 20 trading periods moving average of Volume. For example, 8.5x would mean today's volume so far is 8.5 times the average volume traded in the last 20 trading sessions. Volume in green means that volume for the date so far has been at"
         legendText = f"{legendText} least 2.5 times more than the average volume of last 20 sessions. If the volume is in red, it means the given date's volume is less than 2.5 times the avg volume of the last 20 sessions. *** 7. MA-Signal ***: It shows the price trend of the given stock by analyzing various 50-200 moving/exponential averages crossover strategies. Perform a Google search for the shown MA-Signals"
-        legendText = f"{legendText} to learn about them more. If it is in green, the signal is bullish. Red means bearish. *** 8. RSI ***: Relative Strength Index is a momentum index which describes 14-period relative strength at the given price. Generally, below 30 is considered oversold and above 80 is considered overbought. *** 9. Trend(22Prds) ***:  This describes the average trendline computed based on the"
-        legendText = f"{legendText} last 22 trading sessions. Their strength is displayed depending on the steepness of the trendlines. (Strong / Weak) Up / Down shows how high/low the demand is respectively. A Sideways trend is the horizontal price movement that occurs when the forces of supply and demand are nearly equal. T:▲ or T:▼ shows the general moving average uptrend/downtrend from a 200 day MA perspective"
+        legendText = f"{legendText} to learn about them more. If it is in green, the signal is bullish. Red means bearish. *** 8. RSI or RSI/i***: Relative Strength Index is a momentum index which describes 14-period relative strength at the given price. Generally, below 30 is considered oversold and above 80 is considered overbought. When RSI/i has value, say, 80/41, it means that the daily RSI value is 80 while"
+        legendText = f"{legendText} the 1-minute intraday RSI is 41. *** 9. Trend(22Prds) ***:  This describes the average trendline computed based on the last 22 trading sessions. Their strength is displayed depending on the steepness of the trendlines. (Strong / Weak) Up / Down shows how high/low the demand is respectively. A Sideways trend is the horizontal price movement that occurs when the forces of supply"
+        legendText = f"{legendText} and demand are nearly equal. T:▲ or T:▼ shows the general moving average uptrend/downtrend from a 200 day MA perspective"
         legendText = f"{legendText} if the current 200DMA is more/less than the last 20/80/100 days' 200DMA. Similarly, t:▲ or t:▼ shows for 50DMA based on 9/14/20 days' 50DMA trend. MFI:▲ or MFI:▼ shows"
         legendText = f"{legendText} if the overall top 5 mutual funds and top 5 institutional investors ownership went up or down on the closing of the last month. *** 10. Pattern ***:This shows if the chart or the candle (from the candlestick chart) is"
         legendText = f"{legendText} forming any known pattern in the recent timeframe or as per the selected screening options. Do a google search for the shown pattern names to learn. *** 11. CCI ***: The Commodity Channel Index (CCI) is a technical indicator that measures the difference between the current price and the historical average price of the given stock. Generally below '- 100' is considered oversold"
         legendText = f"{legendText} and above 100 is considered overbought. If the CCI is < '-100' or CCI is > 100 and the Trend(22Prds) is Strong/Weak Up, it is shown in green. Otherwise it's in red. *** 12. 1-Pd/2-Pd etc. ***: 60.29% of (413) under 1-Pd in green shows that the given scan option was correct 60.23% of the times for 413 stocks that scanner found in the last 22 trading sessions under the same scan"
         legendText = f"{legendText} options. Similarly, 61.69 % of (154) in green under 22-Pd, means we found that 61.56% of 154 stocks (~95 stocks) prices found under the same scan options increased in 22 trading periods. 57.87% of (2661) under 'Overall' means that over the last 22 trading sessions we found 2661 stock instances under the same scanning options (for example, Momentum Gainers), out of which 57.87%"
         legendText = f"{legendText} of the stock prices increased in one or more of the last 1 or 2 or 3 or 4 or 5 or 10 or 22 or 22 trading sessions. If you want to see by what percent the prices increased, you should see the details. *** 13. 1 to 30 period gain/loss % ***: 4.17% under 1-Pd in green in the gain/loss table/grid means the stock price increased by 4.17% in the next 1 trading session. If this is in"
         legendText = f"{legendText} red, example, -5.67%, it means the price actually decreased by 5.67%. Gains are in green and losses are in red in this grid. The Date column has the date(s) on which that specific stock was found under the chosen scan options in the past 22 trading sessions. *** 14. 52Wk H/L ***: These have 52 weeks high/low prices and will be shown in red, green or yellow based on how close the"
```

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/classes/keys.py` & `pkscreener-0.44.20240425.292/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/courbd.ttf` & `pkscreener-0.44.20240425.292/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/globals.py` & `pkscreener-0.44.20240425.292/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -548,18 +548,20 @@
     return indexOption, executeOption
 
 def labelDataForPrinting(screenResults, saveResults, configManager, volumeRatio,executeOption, reversalOption):
     # Publish to gSheet with https://github.com/burnash/gspread
     global menuChoiceHierarchy, userPassedArgs
     try:
         isTrading = PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]
-        if isTrading or userPassedArgs.monitor:
+        if isTrading or userPassedArgs.monitor or ("RSIi" in saveResults.columns):
             screenResults['RSI'] = screenResults['RSI'].astype(str) + "/" + screenResults['RSIi'].astype(str)
             saveResults['RSI'] = saveResults['RSI'].astype(str) + "/" + saveResults['RSIi'].astype(str)
-        sortKey = ["Volume"] if "RSI" not in menuChoiceHierarchy else ("RSIi" if isTrading else "RSI")
+            screenResults.rename(columns={"RSI": "RSI/i"},inplace=True)
+            saveResults.rename(columns={"RSI": "RSI/i"},inplace=True)
+        sortKey = ["Volume"] if "RSI" not in menuChoiceHierarchy else ("RSIi" if (isTrading or "RSIi" in saveResults.columns) else "RSI")
         ascending = [False if "RSI" not in menuChoiceHierarchy else True]
         if executeOption == 21:
             if reversalOption in [3,5,6,7]:
                 sortKey = ["MFI"]
                 ascending = [reversalOption in [6,7]]
             elif reversalOption in [8,9]:
                 sortKey = ["FVDiff"]
@@ -1368,15 +1370,15 @@
                     configManager,
                     downloadOnly=downloadOnly,
                     defaultAnswer=defaultAnswer,
                     forceLoad=(menuOption in ["X", "B", "G", "S"]),
                     stockCodes = listStockCodes,
                     exchangeSuffix = "" if (indexOption == 15 or (configManager.defaultIndex == 15 and indexOption == 0)) else ".NS"
             )
-    if menuOption not in ["C"] and not configManager.isIntradayConfig() and configManager.calculatersiintraday:
+    if menuOption not in ["C"] and (userPassedArgs.monitor is not None or "|" in userPassedArgs.options) :#not configManager.isIntradayConfig() and configManager.calculatersiintraday:
         candleDuration = (userPassedArgs.intraday if (userPassedArgs is not None and userPassedArgs.intraday is not None) else "1m")
         configManager.toggleConfig(candleDuration=candleDuration,clearCache=False)
         # We also need to load the intraday data to be able to calculate intraday RSI
         stockDictSecondary = Utility.tools.loadStockData(
                         stockDictSecondary,
                         configManager,
                         downloadOnly=downloadOnly,
@@ -2164,15 +2166,15 @@
                     + f"{'Found' if menuOption in ['X'] else 'Analysed'} {len(lstscreen)} {'Stocks' if menuOption in ['X'] else 'Records'}"
                     + colorText.END
                 )
                 if keyboardInterruptEventFired:
                     return False, backtest_df
                 return not ((testing and len(lstscreen) >= 1) or len(lstscreen) >= max_allowed), backtest_df
             otherArgs = (menuOption, backtestPeriod, result, lstscreen, lstsave)
-            backtest_df, result =PKScanRunner.runScan(testing,numStocks,iterations,items,numStocksPerIteration,tasks_queue,results_queue,originalNumberOfStocks,backtest_df,*otherArgs,resultsReceivedCb=processResultsCallback)
+            backtest_df, result =PKScanRunner.runScan(userPassedArgs,testing,numStocks,iterations,items,numStocksPerIteration,tasks_queue,results_queue,originalNumberOfStocks,backtest_df,*otherArgs,resultsReceivedCb=processResultsCallback)
 
         OutputControls().printOutput(f"\x1b[{3 if OutputControls().enableMultipleLineOutput else 1}A")
         elapsed_time = time.time() - start_time
         if menuOption in ["X", "G", "C"]:
             # create extension
             screenResults = pd.DataFrame(lstscreen)
             saveResults = pd.DataFrame(lstsave)
@@ -2513,15 +2515,15 @@
 def takeBacktestInputs(
     menuOption=None, indexOption=None, executeOption=None, backtestPeriod=0
 ):
     g10k = '"Growth of 10k"'
     OutputControls().printOutput(
         colorText.BOLD
         + colorText.GREEN
-        + f"[+] For {g10k if menuOption == 'G' else 'backtesting'}, you can choose from (1,2,3,4,5,10,15,22,30) or any other custom periods (< 450)."
+        + f"[+] For {g10k if menuOption == 'G' else 'backtesting'}, you can choose from (1,2,3,4,5,10,15,22,30) or any other custom periods (< 280)."
     )
     try:
         if backtestPeriod == 0:
             backtestPeriod = int(
                 input(
                     colorText.BOLD
                     + colorText.FAIL
```

### Comparing `pkscreener-0.44.20240424.291/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240425.292/pkscreener/pkscreener.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [config]
-period = 450d
+period = 280d
 daystolookback = 22
 duration = 1d
 minprice = 20.0
 maxprice = 50000.0
 volumeratio = 2.5
 consolidationpercentage = 10.0
 shuffle = y
 cachestockdata = y
 onlystagetwostocks = y
 useema = n
 showunknowntrends = y
 logsenabled = n
 enableportfoliocalculations = n
 showpaststrategydata = n
-calculatersiintraday = n
+calculatersiintraday = y
 generaltimeout = 2.0
 defaultindex = 12
 longtimeout = 4.0
 maxnetworkretrycount = 10
 backtestperiod = 120
 maxbacktestwindow = 30
 morninganalysiscandlenumber = 25
```

### Comparing `pkscreener-0.44.20240424.291/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240425.292/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240425.292/pkscreener/pkscreenercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,14 +367,15 @@
                         start_time = time.time()
                     else:
                         elapsed_time = round(time.time() - start_time,2)
                         start_time = time.time()
                 monitorOption_org = MarketMonitor().currentMonitorOption()
                 monitorOption = monitorOption_org
                 lastComponent = monitorOption.split(":")[-1]
+                # previousCandleDuration = configManager.duration
                 if "i" in lastComponent:
                     # We need to switch to intraday scan
                     monitorOption = monitorOption.replace(lastComponent,"")
                     args.intraday = lastComponent.replace("i","").strip()
                     configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
                 else:
                     # We need to switch to daily scan
@@ -383,26 +384,27 @@
                 if monitorOption.startswith("|"):
                     monitorOption = monitorOption.replace("|","")
                     # We need to pipe the output from previous run into the next one
                     if resultStocks is not None:
                         resultStocks = ",".join(resultStocks)
                         monitorOption = f"{monitorOption}:{resultStocks}"
                 args.options = monitorOption.replace("::",":")
-                if MarketMonitor().monitorIndex == 1 and args.options is not None and plainResults is not None:
+                # (previousCandleDuration != configManager.duration) or 
+                if (MarketMonitor().monitorIndex == 1 and args.options is not None and plainResults is not None):
                     # Load the stock data afresh for each cycle
                     refreshStockData(args.options)
             try: 
                 results = None
                 plainResults = None
                 resultStocks = None
                 results, plainResults = main(userArgs=args)
                 if isInterrupted():
                     sys.exit(0)
-                # while pipeResults(plainResults,args):
-                #     results, plainResults = main(userArgs=args)
+                while pipeResults(plainResults,args):
+                    results, plainResults = main(userArgs=args)
             except SystemExit:
                 sys.exit(0)
             except Exception as e:
                 default_logger().debug(e, exc_info=True)
                 # Probably user cancelled an operation by choosing a cancel sub-menu somewhere
                 pass
             if plainResults is not None and not plainResults.empty:
```

### Comparing `pkscreener-0.44.20240424.291/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240425.292/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240424.291
+Version: 0.44.20240425.292
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240424.291.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240425.292.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -218,15 +218,15 @@
 |  8  |       **Trend**       | By using advance algorithms, the average trendlines are computed for `N` days and their strenght is displayed depending on steepness of trendlines. (This does NOT show any trendline on chart, it is calculated internally) | `Strong Up`, `Weak Down` etc.                                                            |
 |  9  |      **Pattern**      | If the chart or the candle itself forming any important pattern in the recent timeframe or as per the selected screening option, various important patterns will be indicated here.                                          | `Momentum Gainer`, `Inside Bar (N)`,`Bullish Engulfing` etc.                             |
 
 ## Hack it your way:
 Feel free to Edit the parameters in the `pkscreener.ini` file which will be generated by the application.
 ```
 [config]
-period = 450d
+period = 280d
 daystolookback = 22
 duration = 1d
 minprice = 20.0
 maxprice = 50000.0
 volumeratio = 2.5
 consolidationpercentage = 10.0
 shuffle = y
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.290/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.291/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.290/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.291/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.290/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240424.291/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240424.291/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240425.292/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240424.291/setup.py` & `pkscreener-0.44.20240425.292/setup.py`

 * *Files identical despite different names*

