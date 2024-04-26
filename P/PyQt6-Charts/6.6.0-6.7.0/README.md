# Comparing `tmp/PyQt6_Charts-6.6.0.tar.gz` & `tmp/PyQt6_Charts-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_Charts-6.6.0.tar", last modified: Wed Oct 25 10:22:50 2023, max compression
+gzip compressed data, was "PyQt6_Charts-6.7.0.tar", last modified: Sat Apr 20 16:01:58 2024, max compression
```

## Comparing `PyQt6_Charts-6.6.0.tar` & `PyQt6_Charts-6.7.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:22:50.291719 PyQt6_Charts-6.6.0/
--rw-r--r--   0 phil       (501) staff       (20)     4381 2023-10-25 10:22:49.573891 PyQt6_Charts-6.6.0/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2023-10-25 10:22:49.355902 PyQt6_Charts-6.6.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      450 2023-10-25 10:21:18.154686 PyQt6_Charts-6.6.0/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     1551 2023-10-25 10:22:50.291886 PyQt6_Charts-6.6.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1229 2023-10-25 10:22:49.575354 PyQt6_Charts-6.6.0/README
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:22:50.269975 PyQt6_Charts-6.6.0/examples/
--rw-r--r--   0 phil       (501) staff       (20)     2013 2023-10-25 10:21:18.160758 PyQt6_Charts-6.6.0/examples/areachart.py
--rw-r--r--   0 phil       (501) staff       (20)     1934 2023-10-25 10:21:18.161977 PyQt6_Charts-6.6.0/examples/barchart.py
--rw-r--r--   0 phil       (501) staff       (20)     5710 2023-10-25 10:21:18.162873 PyQt6_Charts-6.6.0/examples/barmodelmapper.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:22:50.270995 PyQt6_Charts-6.6.0/examples/boxplotchart/
--rw-r--r--   0 phil       (501) staff       (20)     1583 2023-10-25 10:21:18.163749 PyQt6_Charts-6.6.0/examples/boxplotchart/acme_data.txt
--rw-r--r--   0 phil       (501) staff       (20)     3433 2023-10-25 10:21:18.164549 PyQt6_Charts-6.6.0/examples/boxplotchart/boxplotchart.py
--rw-r--r--   0 phil       (501) staff       (20)     1587 2023-10-25 10:21:18.165354 PyQt6_Charts-6.6.0/examples/boxplotchart/boxwhisk_data.txt
--rw-r--r--   0 phil       (501) staff       (20)    12540 2023-10-25 10:21:18.166271 PyQt6_Charts-6.6.0/examples/chartthemes.py
--rw-r--r--   0 phil       (501) staff       (20)     3894 2023-10-25 10:21:18.167176 PyQt6_Charts-6.6.0/examples/donutbreakdown.py
--rw-r--r--   0 phil       (501) staff       (20)     2103 2023-10-25 10:21:18.168070 PyQt6_Charts-6.6.0/examples/horizontalbarchart.py
--rw-r--r--   0 phil       (501) staff       (20)     2100 2023-10-25 10:21:18.168979 PyQt6_Charts-6.6.0/examples/horizontalpercentbarchart.py
--rw-r--r--   0 phil       (501) staff       (20)     2100 2023-10-25 10:21:18.169924 PyQt6_Charts-6.6.0/examples/horizontalstackedbarchart.py
--rw-r--r--   0 phil       (501) staff       (20)     5747 2023-10-25 10:21:18.170864 PyQt6_Charts-6.6.0/examples/modeldata.py
--rw-r--r--   0 phil       (501) staff       (20)     1998 2023-10-25 10:21:18.171736 PyQt6_Charts-6.6.0/examples/percentbarchart.py
--rw-r--r--   0 phil       (501) staff       (20)     5662 2023-10-25 10:21:18.172520 PyQt6_Charts-6.6.0/examples/polarchart.py
--rw-r--r--   0 phil       (501) staff       (20)      793 2023-10-25 10:22:49.575826 PyQt6_Charts-6.6.0/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:22:50.271440 PyQt6_Charts-6.6.0/sip/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-10-25 10:22:50.291309 PyQt6_Charts-6.6.0/sip/QtCharts/
--rw-r--r--   0 phil       (501) staff       (20)     3697 2023-10-25 10:22:50.029009 PyQt6_Charts-6.6.0/sip/QtCharts/QtChartsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     5341 2023-10-25 10:22:50.038117 PyQt6_Charts-6.6.0/sip/QtCharts/qabstractaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     2795 2023-10-25 10:22:50.030638 PyQt6_Charts-6.6.0/sip/QtCharts/qabstractbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     6115 2023-10-25 10:22:50.028107 PyQt6_Charts-6.6.0/sip/QtCharts/qabstractseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1289 2023-10-25 10:22:50.032243 PyQt6_Charts-6.6.0/sip/QtCharts/qarealegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     2869 2023-10-25 10:22:50.047214 PyQt6_Charts-6.6.0/sip/QtCharts/qareaseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     2071 2023-10-25 10:22:50.039836 PyQt6_Charts-6.6.0/sip/QtCharts/qbarcategoryaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     1338 2023-10-25 10:22:50.042090 PyQt6_Charts-6.6.0/sip/QtCharts/qbarlegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     1197 2023-10-25 10:22:50.036079 PyQt6_Charts-6.6.0/sip/QtCharts/qbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     3837 2023-10-25 10:22:50.060912 PyQt6_Charts-6.6.0/sip/QtCharts/qbarset.sip
--rw-r--r--   0 phil       (501) staff       (20)     1310 2023-10-25 10:22:50.031710 PyQt6_Charts-6.6.0/sip/QtCharts/qboxplotlegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     2225 2023-10-25 10:22:50.058739 PyQt6_Charts-6.6.0/sip/QtCharts/qboxplotseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     2224 2023-10-25 10:22:50.029824 PyQt6_Charts-6.6.0/sip/QtCharts/qboxset.sip
--rw-r--r--   0 phil       (501) staff       (20)     1338 2023-10-25 10:22:50.035506 PyQt6_Charts-6.6.0/sip/QtCharts/qcandlesticklegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     1902 2023-10-25 10:22:50.026832 PyQt6_Charts-6.6.0/sip/QtCharts/qcandlestickmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     3169 2023-10-25 10:22:50.048427 PyQt6_Charts-6.6.0/sip/QtCharts/qcandlestickseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     2005 2023-10-25 10:22:50.058133 PyQt6_Charts-6.6.0/sip/QtCharts/qcandlestickset.sip
--rw-r--r--   0 phil       (501) staff       (20)     1985 2023-10-25 10:22:50.062056 PyQt6_Charts-6.6.0/sip/QtCharts/qcategoryaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     4333 2023-10-25 10:22:50.046499 PyQt6_Charts-6.6.0/sip/QtCharts/qchart.sip
--rw-r--r--   0 phil       (501) staff       (20)     2358 2023-10-25 10:22:50.054277 PyQt6_Charts-6.6.0/sip/QtCharts/qchartview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1945 2023-10-25 10:22:50.053607 PyQt6_Charts-6.6.0/sip/QtCharts/qcoloraxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     1707 2023-10-25 10:22:50.061462 PyQt6_Charts-6.6.0/sip/QtCharts/qdatetimeaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     6522 2023-10-25 10:22:50.050175 PyQt6_Charts-6.6.0/sip/QtCharts/qhash.sip
--rw-r--r--   0 phil       (501) staff       (20)     1809 2023-10-25 10:22:50.039227 PyQt6_Charts-6.6.0/sip/QtCharts/qhbarmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1814 2023-10-25 10:22:50.026130 PyQt6_Charts-6.6.0/sip/QtCharts/qhboxplotmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1946 2023-10-25 10:22:50.056777 PyQt6_Charts-6.6.0/sip/QtCharts/qhcandlestickmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1247 2023-10-25 10:22:50.052475 PyQt6_Charts-6.6.0/sip/QtCharts/qhorizontalbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1282 2023-10-25 10:22:50.047698 PyQt6_Charts-6.6.0/sip/QtCharts/qhorizontalpercentbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1282 2023-10-25 10:22:50.051986 PyQt6_Charts-6.6.0/sip/QtCharts/qhorizontalstackedbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1757 2023-10-25 10:22:50.051453 PyQt6_Charts-6.6.0/sip/QtCharts/qhpiemodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1711 2023-10-25 10:22:50.040421 PyQt6_Charts-6.6.0/sip/QtCharts/qhxymodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     3472 2023-10-25 10:22:50.043730 PyQt6_Charts-6.6.0/sip/QtCharts/qlegend.sip
--rw-r--r--   0 phil       (501) staff       (20)     2161 2023-10-25 10:22:50.057502 PyQt6_Charts-6.6.0/sip/QtCharts/qlegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     1193 2023-10-25 10:22:50.031164 PyQt6_Charts-6.6.0/sip/QtCharts/qlineseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1906 2023-10-25 10:22:50.045040 PyQt6_Charts-6.6.0/sip/QtCharts/qlogvalueaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     1232 2023-10-25 10:22:50.052989 PyQt6_Charts-6.6.0/sip/QtCharts/qpercentbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1324 2023-10-25 10:22:50.038634 PyQt6_Charts-6.6.0/sip/QtCharts/qpielegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     2638 2023-10-25 10:22:50.036907 PyQt6_Charts-6.6.0/sip/QtCharts/qpieseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     3064 2023-10-25 10:22:50.034953 PyQt6_Charts-6.6.0/sip/QtCharts/qpieslice.sip
--rw-r--r--   0 phil       (501) staff       (20)     1774 2023-10-25 10:22:50.059350 PyQt6_Charts-6.6.0/sip/QtCharts/qpolarchart.sip
--rw-r--r--   0 phil       (501) staff       (20)     2181 2023-10-25 10:22:50.056175 PyQt6_Charts-6.6.0/sip/QtCharts/qscatterseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1205 2023-10-25 10:22:50.044316 PyQt6_Charts-6.6.0/sip/QtCharts/qsplineseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1232 2023-10-25 10:22:50.045551 PyQt6_Charts-6.6.0/sip/QtCharts/qstackedbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     2336 2023-10-25 10:22:50.055557 PyQt6_Charts-6.6.0/sip/QtCharts/qvalueaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     1809 2023-10-25 10:22:50.041588 PyQt6_Charts-6.6.0/sip/QtCharts/qvbarmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1817 2023-10-25 10:22:50.059941 PyQt6_Charts-6.6.0/sip/QtCharts/qvboxplotmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1910 2023-10-25 10:22:50.041016 PyQt6_Charts-6.6.0/sip/QtCharts/qvcandlestickmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1757 2023-10-25 10:22:50.050837 PyQt6_Charts-6.6.0/sip/QtCharts/qvpiemodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1711 2023-10-25 10:22:50.054856 PyQt6_Charts-6.6.0/sip/QtCharts/qvxymodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1275 2023-10-25 10:22:50.042664 PyQt6_Charts-6.6.0/sip/QtCharts/qxylegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     7542 2023-10-25 10:22:50.033986 PyQt6_Charts-6.6.0/sip/QtCharts/qxyseries.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:58.572676 PyQt6_Charts-6.7.0/
+-rw-r--r--   0 phil       (501) staff       (20)     5177 2024-04-20 16:01:58.349097 PyQt6_Charts-6.7.0/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2024-04-20 16:01:58.254837 PyQt6_Charts-6.7.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      504 2024-04-20 16:01:02.992867 PyQt6_Charts-6.7.0/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     1500 2024-04-20 16:01:58.572759 PyQt6_Charts-6.7.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1132 2024-04-20 16:01:58.349694 PyQt6_Charts-6.7.0/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:58.562716 PyQt6_Charts-6.7.0/examples/
+-rw-r--r--   0 phil       (501) staff       (20)     2013 2024-04-20 16:01:02.994986 PyQt6_Charts-6.7.0/examples/areachart.py
+-rw-r--r--   0 phil       (501) staff       (20)     1934 2024-04-20 16:01:02.995305 PyQt6_Charts-6.7.0/examples/barchart.py
+-rw-r--r--   0 phil       (501) staff       (20)     5710 2024-04-20 16:01:02.995542 PyQt6_Charts-6.7.0/examples/barmodelmapper.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:58.563104 PyQt6_Charts-6.7.0/examples/boxplotchart/
+-rw-r--r--   0 phil       (501) staff       (20)     1583 2024-04-20 16:01:02.995775 PyQt6_Charts-6.7.0/examples/boxplotchart/acme_data.txt
+-rw-r--r--   0 phil       (501) staff       (20)     3433 2024-04-20 16:01:02.995972 PyQt6_Charts-6.7.0/examples/boxplotchart/boxplotchart.py
+-rw-r--r--   0 phil       (501) staff       (20)     1587 2024-04-20 16:01:02.996166 PyQt6_Charts-6.7.0/examples/boxplotchart/boxwhisk_data.txt
+-rw-r--r--   0 phil       (501) staff       (20)    12540 2024-04-20 16:01:02.996390 PyQt6_Charts-6.7.0/examples/chartthemes.py
+-rw-r--r--   0 phil       (501) staff       (20)     3894 2024-04-20 16:01:02.996580 PyQt6_Charts-6.7.0/examples/donutbreakdown.py
+-rw-r--r--   0 phil       (501) staff       (20)     2103 2024-04-20 16:01:02.996758 PyQt6_Charts-6.7.0/examples/horizontalbarchart.py
+-rw-r--r--   0 phil       (501) staff       (20)     2100 2024-04-20 16:01:02.996935 PyQt6_Charts-6.7.0/examples/horizontalpercentbarchart.py
+-rw-r--r--   0 phil       (501) staff       (20)     2100 2024-04-20 16:01:02.997109 PyQt6_Charts-6.7.0/examples/horizontalstackedbarchart.py
+-rw-r--r--   0 phil       (501) staff       (20)     5747 2024-04-20 16:01:02.997307 PyQt6_Charts-6.7.0/examples/modeldata.py
+-rw-r--r--   0 phil       (501) staff       (20)     1998 2024-04-20 16:01:02.997481 PyQt6_Charts-6.7.0/examples/percentbarchart.py
+-rw-r--r--   0 phil       (501) staff       (20)     5662 2024-04-20 16:01:02.997676 PyQt6_Charts-6.7.0/examples/polarchart.py
+-rw-r--r--   0 phil       (501) staff       (20)      761 2024-04-20 16:01:58.349894 PyQt6_Charts-6.7.0/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:58.563338 PyQt6_Charts-6.7.0/sip/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-04-20 16:01:58.572512 PyQt6_Charts-6.7.0/sip/QtCharts/
+-rw-r--r--   0 phil       (501) staff       (20)     3712 2024-04-20 16:01:58.446522 PyQt6_Charts-6.7.0/sip/QtCharts/QtChartsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5348 2024-04-20 16:01:58.450421 PyQt6_Charts-6.7.0/sip/QtCharts/qabstractaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2802 2024-04-20 16:01:58.447213 PyQt6_Charts-6.7.0/sip/QtCharts/qabstractbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6122 2024-04-20 16:01:58.446110 PyQt6_Charts-6.7.0/sip/QtCharts/qabstractseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1296 2024-04-20 16:01:58.447846 PyQt6_Charts-6.7.0/sip/QtCharts/qarealegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2876 2024-04-20 16:01:58.454401 PyQt6_Charts-6.7.0/sip/QtCharts/qareaseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2078 2024-04-20 16:01:58.451159 PyQt6_Charts-6.7.0/sip/QtCharts/qbarcategoryaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1345 2024-04-20 16:01:58.452157 PyQt6_Charts-6.7.0/sip/QtCharts/qbarlegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1204 2024-04-20 16:01:58.449496 PyQt6_Charts-6.7.0/sip/QtCharts/qbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3844 2024-04-20 16:01:58.460770 PyQt6_Charts-6.7.0/sip/QtCharts/qbarset.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1317 2024-04-20 16:01:58.447642 PyQt6_Charts-6.7.0/sip/QtCharts/qboxplotlegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2232 2024-04-20 16:01:58.459780 PyQt6_Charts-6.7.0/sip/QtCharts/qboxplotseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2231 2024-04-20 16:01:58.446845 PyQt6_Charts-6.7.0/sip/QtCharts/qboxset.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1345 2024-04-20 16:01:58.449293 PyQt6_Charts-6.7.0/sip/QtCharts/qcandlesticklegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1909 2024-04-20 16:01:58.445517 PyQt6_Charts-6.7.0/sip/QtCharts/qcandlestickmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3176 2024-04-20 16:01:58.454966 PyQt6_Charts-6.7.0/sip/QtCharts/qcandlestickseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2012 2024-04-20 16:01:58.459478 PyQt6_Charts-6.7.0/sip/QtCharts/qcandlestickset.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1992 2024-04-20 16:01:58.461313 PyQt6_Charts-6.7.0/sip/QtCharts/qcategoryaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4340 2024-04-20 16:01:58.454042 PyQt6_Charts-6.7.0/sip/QtCharts/qchart.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2365 2024-04-20 16:01:58.457695 PyQt6_Charts-6.7.0/sip/QtCharts/qchartview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1952 2024-04-20 16:01:58.457355 PyQt6_Charts-6.7.0/sip/QtCharts/qcoloraxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1714 2024-04-20 16:01:58.461028 PyQt6_Charts-6.7.0/sip/QtCharts/qdatetimeaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6522 2024-04-20 16:01:58.455897 PyQt6_Charts-6.7.0/sip/QtCharts/qhash.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1809 2024-04-20 16:01:58.450888 PyQt6_Charts-6.7.0/sip/QtCharts/qhbarmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1814 2024-04-20 16:01:58.445181 PyQt6_Charts-6.7.0/sip/QtCharts/qhboxplotmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1953 2024-04-20 16:01:58.458869 PyQt6_Charts-6.7.0/sip/QtCharts/qhcandlestickmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1254 2024-04-20 16:01:58.456858 PyQt6_Charts-6.7.0/sip/QtCharts/qhorizontalbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1289 2024-04-20 16:01:58.454612 PyQt6_Charts-6.7.0/sip/QtCharts/qhorizontalpercentbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1289 2024-04-20 16:01:58.456649 PyQt6_Charts-6.7.0/sip/QtCharts/qhorizontalstackedbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1757 2024-04-20 16:01:58.456425 PyQt6_Charts-6.7.0/sip/QtCharts/qhpiemodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1711 2024-04-20 16:01:58.451420 PyQt6_Charts-6.7.0/sip/QtCharts/qhxymodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3479 2024-04-20 16:01:58.452844 PyQt6_Charts-6.7.0/sip/QtCharts/qlegend.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2168 2024-04-20 16:01:58.459195 PyQt6_Charts-6.7.0/sip/QtCharts/qlegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1200 2024-04-20 16:01:58.447432 PyQt6_Charts-6.7.0/sip/QtCharts/qlineseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1913 2024-04-20 16:01:58.453326 PyQt6_Charts-6.7.0/sip/QtCharts/qlogvalueaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1239 2024-04-20 16:01:58.457073 PyQt6_Charts-6.7.0/sip/QtCharts/qpercentbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1331 2024-04-20 16:01:58.450631 PyQt6_Charts-6.7.0/sip/QtCharts/qpielegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2645 2024-04-20 16:01:58.449825 PyQt6_Charts-6.7.0/sip/QtCharts/qpieseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3071 2024-04-20 16:01:58.449085 PyQt6_Charts-6.7.0/sip/QtCharts/qpieslice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1781 2024-04-20 16:01:58.460009 PyQt6_Charts-6.7.0/sip/QtCharts/qpolarchart.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2188 2024-04-20 16:01:58.458598 PyQt6_Charts-6.7.0/sip/QtCharts/qscatterseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1212 2024-04-20 16:01:58.453055 PyQt6_Charts-6.7.0/sip/QtCharts/qsplineseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1239 2024-04-20 16:01:58.453548 PyQt6_Charts-6.7.0/sip/QtCharts/qstackedbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2343 2024-04-20 16:01:58.458291 PyQt6_Charts-6.7.0/sip/QtCharts/qvalueaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1809 2024-04-20 16:01:58.451948 PyQt6_Charts-6.7.0/sip/QtCharts/qvbarmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1817 2024-04-20 16:01:58.460268 PyQt6_Charts-6.7.0/sip/QtCharts/qvboxplotmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1917 2024-04-20 16:01:58.451684 PyQt6_Charts-6.7.0/sip/QtCharts/qvcandlestickmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1757 2024-04-20 16:01:58.456166 PyQt6_Charts-6.7.0/sip/QtCharts/qvpiemodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1711 2024-04-20 16:01:58.457951 PyQt6_Charts-6.7.0/sip/QtCharts/qvxymodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1282 2024-04-20 16:01:58.452378 PyQt6_Charts-6.7.0/sip/QtCharts/qxylegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7549 2024-04-20 16:01:58.448684 PyQt6_Charts-6.7.0/sip/QtCharts/qxyseries.sip
```

### Comparing `PyQt6_Charts-6.6.0/ChangeLog` & `PyQt6_Charts-6.7.0/ChangeLog`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+2024-04-04  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS:
+	Updated for Qt v6.7.0.
+	[7775a6a478c4] [6.7.0]
+
+2024-03-17  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6-Charts.msp:
+	Added support for Qt v6.7.
+	[76dd8a538581]
+
+2024-02-18  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* README, README.md, pyproject.toml:
+	Migrated from [tool.sip.metadata] to [project] in pyproject.toml.
+	[07d0ca99d4a0]
+
+	* NEWS:
+	Updated the NEWS file.
+	[ea2110a44708]
+
+	* Merged the 6.6-maint branch.
+	[72e632817962]
+
+2024-01-02  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, rb-product.toml:
+	Removed the product file.
+	[eb9fe0244abd] <6.6-maint>
+
+2023-10-25  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* .hgtags:
+	Added tag 6.6.0 for changeset 117d52b9b18f
+	[369c233d550f]
+
 2023-10-22  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, PyQt6-Charts.msp:
 	Updated for Qt v6.6.
 	[117d52b9b18f] [6.6.0]
 
 2023-04-04  Phil Thompson  <phil@riverbankcomputing.com>
```

### Comparing `PyQt6_Charts-6.6.0/LICENSE` & `PyQt6_Charts-6.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/PKG-INFO` & `PyQt6_Charts-6.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 Metadata-Version: 2.1
 Name: PyQt6-Charts
-Version: 6.6.0
-Requires-Python: >=3.7
+Version: 6.7.0
+Requires-Python: >=3.8
 Summary: Python bindings for the Qt Charts library
-Home-Page: https://www.riverbankcomputing.com/software/pyqtchart/
-Author: Riverbank Computing Limited
-Author-Email: info@riverbankcomputing.com
-License: GPL v3
+Description-Content-Type: text/markdown
+Project-Url: homepage, https://www.riverbankcomputing.com/software/pyqtchart/
 Requires-Dist: PyQt6 (>=6.2.0)
+License: GPL v3
+Author-Email: Riverbank Computing Limited <info@riverbankcomputing.com>
 
-PyQt6-Charts - Python Bindings for the Qt Charts Library
-========================================================
+# PyQt6-Charts - Python Bindings for the Qt Charts Library
 
 PyQt6-Charts is a set of Python bindings for The Qt Company's Qt Charts
 library.  The bindings sit on top of PyQt6 and are implemented as a single
 module.
 
 
-Author
-------
+## Author
 
 PyQt6-Charts is copyright (c) Riverbank Computing Limited.  Its homepage is
 https://www.riverbankcomputing.com/software/pyqtchart/.
 
 Support may be obtained from the PyQt mailing list at
 https://www.riverbankcomputing.com/mailman/listinfo/pyqt/.
 
 
-License
--------
+## License
 
 PyQt6-Charts is released under the GPL v3 license and under a commercial
 license that allows for the development of proprietary applications.
 
 
-Documentation
--------------
+## Documentation
 
 The documentation for the latest release can be found
-`here <https://www.riverbankcomputing.com/static/Docs/PyQt6/>`__.
+[here](https://www.riverbankcomputing.com/static/Docs/PyQt6/).
 
 
-Installation
-------------
+## Installation
 
-The GPL version of PyQt6-Charts can be installed from PyPI::
+The GPL version of PyQt6-Charts can be installed from PyPI:
 
     pip install PyQt6-Charts
 
-``pip`` will also build and install the bindings from the sdist package but
-Qt's ``qmake`` tool must be on ``PATH``.
+`pip` will also build and install the bindings from the sdist package but Qt's
+`qmake` tool must be on `PATH`.
 
-The ``sip-install`` tool will also install the bindings from the sdist package
+The `sip-install` tool will also install the bindings from the sdist package
 but will allow you to configure many aspects of the installation.
```

### Comparing `PyQt6_Charts-6.6.0/README` & `PyQt6_Charts-6.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,39 @@
-PyQt6-Charts - Python Bindings for the Qt Charts Library
-========================================================
+# PyQt6-Charts - Python Bindings for the Qt Charts Library
 
 PyQt6-Charts is a set of Python bindings for The Qt Company's Qt Charts
 library.  The bindings sit on top of PyQt6 and are implemented as a single
 module.
 
 
-Author
-------
+## Author
 
 PyQt6-Charts is copyright (c) Riverbank Computing Limited.  Its homepage is
 https://www.riverbankcomputing.com/software/pyqtchart/.
 
 Support may be obtained from the PyQt mailing list at
 https://www.riverbankcomputing.com/mailman/listinfo/pyqt/.
 
 
-License
--------
+## License
 
 PyQt6-Charts is released under the GPL v3 license and under a commercial
 license that allows for the development of proprietary applications.
 
 
-Documentation
--------------
+## Documentation
 
 The documentation for the latest release can be found
-`here <https://www.riverbankcomputing.com/static/Docs/PyQt6/>`__.
+[here](https://www.riverbankcomputing.com/static/Docs/PyQt6/).
 
 
-Installation
-------------
+## Installation
 
-The GPL version of PyQt6-Charts can be installed from PyPI::
+The GPL version of PyQt6-Charts can be installed from PyPI:
 
     pip install PyQt6-Charts
 
-``pip`` will also build and install the bindings from the sdist package but
-Qt's ``qmake`` tool must be on ``PATH``.
+`pip` will also build and install the bindings from the sdist package but Qt's
+`qmake` tool must be on `PATH`.
 
-The ``sip-install`` tool will also install the bindings from the sdist package
+The `sip-install` tool will also install the bindings from the sdist package
 but will allow you to configure many aspects of the installation.
```

### Comparing `PyQt6_Charts-6.6.0/examples/areachart.py` & `PyQt6_Charts-6.7.0/examples/areachart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/barchart.py` & `PyQt6_Charts-6.7.0/examples/barchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/barmodelmapper.py` & `PyQt6_Charts-6.7.0/examples/barmodelmapper.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/boxplotchart/acme_data.txt` & `PyQt6_Charts-6.7.0/examples/boxplotchart/acme_data.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/boxplotchart/boxplotchart.py` & `PyQt6_Charts-6.7.0/examples/boxplotchart/boxplotchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/boxplotchart/boxwhisk_data.txt` & `PyQt6_Charts-6.7.0/examples/boxplotchart/boxwhisk_data.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/chartthemes.py` & `PyQt6_Charts-6.7.0/examples/chartthemes.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/donutbreakdown.py` & `PyQt6_Charts-6.7.0/examples/donutbreakdown.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/horizontalbarchart.py` & `PyQt6_Charts-6.7.0/examples/horizontalbarchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/horizontalpercentbarchart.py` & `PyQt6_Charts-6.7.0/examples/horizontalpercentbarchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/horizontalstackedbarchart.py` & `PyQt6_Charts-6.7.0/examples/horizontalstackedbarchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/modeldata.py` & `PyQt6_Charts-6.7.0/examples/modeldata.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/percentbarchart.py` & `PyQt6_Charts-6.7.0/examples/percentbarchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/examples/polarchart.py` & `PyQt6_Charts-6.7.0/examples/polarchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.6.0/pyproject.toml` & `PyQt6_Charts-6.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Specify the build system for the project.
 [build-system]
-requires = ["sip >=6, <7", "PyQt-builder >=1.10, <2"]
+requires = ["sip >=6.8, <7", "PyQt-builder >=1.10, <2"]
 build-backend = "sipbuild.api"
 
-# Specify the PEP 566 metadata for the project.
-[tool.sip.metadata]
+[project]
 name = "PyQt6-Charts"
-version = "6.6.0"
-summary = "Python bindings for the Qt Charts library"
-home-page = "https://www.riverbankcomputing.com/software/pyqtchart/"
-author = "Riverbank Computing Limited"
-author-email = "info@riverbankcomputing.com"
-license = "GPL v3"
-description-file = "README"
-requires-dist = "PyQt6 (>=6.2.0)"
+version = "6.7.0"
+description = "Python bindings for the Qt Charts library"
+readme = "README.md"
+urls.homepage = "https://www.riverbankcomputing.com/software/pyqtchart/"
+dependencies = ["PyQt6 (>=6.2.0)"]
+license = {text = "GPL v3"}
+
+[[project.authors]]
+name = "Riverbank Computing Limited"
+email = "info@riverbankcomputing.com"
+
 
 # Specify a PyQt-based project.
 [tool.sip]
 project-factory = "pyqtbuild:PyQtProject"
 
 # Configure the project.
 [tool.sip.project]
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/QtChartsmod.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/QtChartsmod.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // QtChartsmod.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -21,18 +21,18 @@
 
 
 %Module(name=PyQt6.QtCharts, keyword_arguments="Optional", use_limited_api=True)
 
 %Import QtGui/QtGuimod.sip
 %Import QtWidgets/QtWidgetsmod.sip
 
-%Timeline {QtCharts_6_0_0 QtCharts_6_1_0 QtCharts_6_2_0 QtCharts_6_3_0 QtCharts_6_4_0 QtCharts_6_5_0 QtCharts_6_6_0}
+%Timeline {QtCharts_6_0_0 QtCharts_6_1_0 QtCharts_6_2_0 QtCharts_6_3_0 QtCharts_6_4_0 QtCharts_6_5_0 QtCharts_6_6_0 QtCharts_6_7_0}
 
 %Copying
-Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-Charts.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
@@ -48,16 +48,16 @@
 
 %DefaultSupertype PyQt6.sip.simplewrapper
 
 int PYQT_CHART_VERSION;
 const char *PYQT_CHART_VERSION_STR;
 
 %ModuleCode
-static int PYQT_CHART_VERSION = 0x060600;
-static const char *PYQT_CHART_VERSION_STR = "6.6.0";
+static int PYQT_CHART_VERSION = 0x060700;
+static const char *PYQT_CHART_VERSION_STR = "6.7.0";
 %End
 
 %Include qabstractaxis.sip
 %Include qabstractbarseries.sip
 %Include qabstractseries.sip
 %Include qarealegendmarker.sip
 %Include qareaseries.sip
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qabstractaxis.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qabstractaxis.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractaxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QAbstractAxis : QObject /NoDefaultCtors/
+class QAbstractAxis : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qabstractaxis.h>
 %End
 
 public:
     enum AxisType /BaseType=Flag/
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qabstractbarseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qabstractbarseries.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QAbstractBarSeries : QAbstractSeries /NoDefaultCtors/
+class QAbstractBarSeries : public QAbstractSeries /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qabstractbarseries.h>
 %End
 
 public:
     virtual ~QAbstractBarSeries();
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qabstractseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qabstractseries.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QAbstractSeries : QObject /NoDefaultCtors/
+class QAbstractSeries : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qabstractseries.h>
 %End
 
 %ConvertToSubClassCode
     static struct class_graph {
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qarealegendmarker.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qarealegendmarker.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qarealegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QAreaLegendMarker : QLegendMarker
+class QAreaLegendMarker : public QLegendMarker
 {
 %TypeHeaderCode
 #include <qarealegendmarker.h>
 %End
 
 public:
     QAreaLegendMarker(QAreaSeries *series, QLegend *legend, QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qareaseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qareaseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qareaseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QAreaSeries : QAbstractSeries
+class QAreaSeries : public QAbstractSeries
 {
 %TypeHeaderCode
 #include <qareaseries.h>
 %End
 
 public:
     explicit QAreaSeries(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qbarcategoryaxis.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qbarcategoryaxis.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbarcategoryaxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QBarCategoryAxis : QAbstractAxis
+class QBarCategoryAxis : public QAbstractAxis
 {
 %TypeHeaderCode
 #include <qbarcategoryaxis.h>
 %End
 
 public:
     explicit QBarCategoryAxis(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qbarlegendmarker.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qbarlegendmarker.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbarlegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QBarLegendMarker : QLegendMarker
+class QBarLegendMarker : public QLegendMarker
 {
 %TypeHeaderCode
 #include <qbarlegendmarker.h>
 %End
 
 public:
     QBarLegendMarker(QAbstractBarSeries *series, QBarSet *barset, QLegend *legend, QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qbarseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qbarseries.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QBarSeries : QAbstractBarSeries
+class QBarSeries : public QAbstractBarSeries
 {
 %TypeHeaderCode
 #include <qbarseries.h>
 %End
 
 public:
     explicit QBarSeries(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qbarset.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qbarset.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbarset.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QBarSet : QObject
+class QBarSet : public QObject
 {
 %TypeHeaderCode
 #include <qbarset.h>
 %End
 
 public:
     QBarSet(const QString name, QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qboxplotlegendmarker.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qboxplotlegendmarker.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qboxplotlegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QBoxPlotLegendMarker : QLegendMarker
+class QBoxPlotLegendMarker : public QLegendMarker
 {
 %TypeHeaderCode
 #include <qboxplotlegendmarker.h>
 %End
 
 public:
     QBoxPlotLegendMarker(QBoxPlotSeries *series, QLegend *legend, QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qboxplotseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qboxplotseries.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qboxplotseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QBoxPlotSeries : QAbstractSeries
+class QBoxPlotSeries : public QAbstractSeries
 {
 %TypeHeaderCode
 #include <qboxplotseries.h>
 %End
 
 public:
     explicit QBoxPlotSeries(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qboxset.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qboxset.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qboxset.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QBoxSet : QObject
+class QBoxSet : public QObject
 {
 %TypeHeaderCode
 #include <qboxset.h>
 %End
 
 public:
     enum ValuePositions /BaseType=IntEnum/
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qcandlesticklegendmarker.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qcandlesticklegendmarker.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcandlesticklegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QCandlestickLegendMarker : QLegendMarker
+class QCandlestickLegendMarker : public QLegendMarker
 {
 %TypeHeaderCode
 #include <qcandlesticklegendmarker.h>
 %End
 
 public:
     QCandlestickLegendMarker(QCandlestickSeries *series, QLegend *legend, QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qcandlestickmodelmapper.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qcandlestickmodelmapper.sip`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcandlestickmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QCandlestickModelMapper : QObject
+class QCandlestickModelMapper : public QObject
 {
 %TypeHeaderCode
 #include <qcandlestickmodelmapper.h>
 %End
 
 public:
     explicit QCandlestickModelMapper(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qcandlestickseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qcandlestickseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcandlestickseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QCandlestickSeries : QAbstractSeries
+class QCandlestickSeries : public QAbstractSeries
 {
 %TypeHeaderCode
 #include <qcandlestickseries.h>
 %End
 
 public:
     explicit QCandlestickSeries(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qcandlestickset.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qcandlestickset.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcandlestickset.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QCandlestickSet : QObject
+class QCandlestickSet : public QObject
 {
 %TypeHeaderCode
 #include <qcandlestickset.h>
 %End
 
 public:
     QCandlestickSet(qreal timestamp = 0., QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qcategoryaxis.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qcategoryaxis.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcategoryaxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QCategoryAxis : QValueAxis
+class QCategoryAxis : public QValueAxis
 {
 %TypeHeaderCode
 #include <qcategoryaxis.h>
 %End
 
 public:
     explicit QCategoryAxis(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qchart.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qchart.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qchart.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QChart : QGraphicsWidget
+class QChart : public QGraphicsWidget
 {
 %TypeHeaderCode
 #include <qchart.h>
 %End
 
 public:
     enum ChartTheme
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qchartview.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qchartview.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qchartview.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QChartView : QGraphicsView
+class QChartView : public QGraphicsView
 {
 %TypeHeaderCode
 #include <qchartview.h>
 %End
 
 public:
     enum RubberBand /BaseType=Flag/
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qcoloraxis.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qcoloraxis.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcoloraxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -18,15 +18,15 @@
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
 %If (QtCharts_6_2_0 -)
 
-class QColorAxis : QAbstractAxis
+class QColorAxis : public QAbstractAxis
 {
 %TypeHeaderCode
 #include <qcoloraxis.h>
 %End
 
 public:
     explicit QColorAxis(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qdatetimeaxis.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qdatetimeaxis.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdatetimeaxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QDateTimeAxis : QAbstractAxis
+class QDateTimeAxis : public QAbstractAxis
 {
 %TypeHeaderCode
 #include <qdatetimeaxis.h>
 %End
 
 public:
     explicit QDateTimeAxis(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qhash.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qhash.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // This is the SIP interface definition for the QHash based mapped types
 // specific to the QtCharts module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qhbarmodelmapper.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qhbarmodelmapper.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhbarmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qhboxplotmodelmapper.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qhboxplotmodelmapper.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhboxplotmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qhcandlestickmodelmapper.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qhcandlestickmodelmapper.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhcandlestickmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QHCandlestickModelMapper : QCandlestickModelMapper
+class QHCandlestickModelMapper : public QCandlestickModelMapper
 {
 %TypeHeaderCode
 #include <qhcandlestickmodelmapper.h>
 %End
 
 public:
     explicit QHCandlestickModelMapper(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qhorizontalbarseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qhorizontalbarseries.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhorizontalbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QHorizontalBarSeries : QAbstractBarSeries
+class QHorizontalBarSeries : public QAbstractBarSeries
 {
 %TypeHeaderCode
 #include <qhorizontalbarseries.h>
 %End
 
 public:
     explicit QHorizontalBarSeries(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qhorizontalpercentbarseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qhorizontalpercentbarseries.sip`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhorizontalpercentbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QHorizontalPercentBarSeries : QAbstractBarSeries
+class QHorizontalPercentBarSeries : public QAbstractBarSeries
 {
 %TypeHeaderCode
 #include <qhorizontalpercentbarseries.h>
 %End
 
 public:
     explicit QHorizontalPercentBarSeries(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qhorizontalstackedbarseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qhorizontalstackedbarseries.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhorizontalstackedbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QHorizontalStackedBarSeries : QAbstractBarSeries
+class QHorizontalStackedBarSeries : public QAbstractBarSeries
 {
 %TypeHeaderCode
 #include <qhorizontalstackedbarseries.h>
 %End
 
 public:
     explicit QHorizontalStackedBarSeries(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qhpiemodelmapper.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qhpiemodelmapper.sip`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhpiemodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qhxymodelmapper.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qhxymodelmapper.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhxymodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qlegend.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qlegend.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlegend.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QLegend : QGraphicsWidget
+class QLegend : public QGraphicsWidget
 {
 %TypeHeaderCode
 #include <qlegend.h>
 %End
 
 public:
     virtual ~QLegend();
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qlegendmarker.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qlegendmarker.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QLegendMarker : QObject /NoDefaultCtors/
+class QLegendMarker : public QObject /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qlegendmarker.h>
 %End
 
 public:
     enum LegendMarkerType
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qlineseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qlineseries.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlineseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QLineSeries : QXYSeries
+class QLineSeries : public QXYSeries
 {
 %TypeHeaderCode
 #include <qlineseries.h>
 %End
 
 public:
     explicit QLineSeries(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qlogvalueaxis.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qlogvalueaxis.sip`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlogvalueaxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QLogValueAxis : QAbstractAxis
+class QLogValueAxis : public QAbstractAxis
 {
 %TypeHeaderCode
 #include <qlogvalueaxis.h>
 %End
 
 public:
     explicit QLogValueAxis(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qpercentbarseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qpercentbarseries.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpercentbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QPercentBarSeries : QAbstractBarSeries
+class QPercentBarSeries : public QAbstractBarSeries
 {
 %TypeHeaderCode
 #include <qpercentbarseries.h>
 %End
 
 public:
     explicit QPercentBarSeries(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qpielegendmarker.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qpielegendmarker.sip`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpielegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QPieLegendMarker : QLegendMarker
+class QPieLegendMarker : public QLegendMarker
 {
 %TypeHeaderCode
 #include <qpielegendmarker.h>
 %End
 
 public:
     QPieLegendMarker(QPieSeries *series, QPieSlice *slice, QLegend *legend, QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qpieseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qpieseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpieseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QPieSeries : QAbstractSeries
+class QPieSeries : public QAbstractSeries
 {
 %TypeHeaderCode
 #include <qpieseries.h>
 %End
 
 public:
     explicit QPieSeries(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qpieslice.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qpieslice.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpieslice.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QPieSlice : QObject
+class QPieSlice : public QObject
 {
 %TypeHeaderCode
 #include <qpieslice.h>
 %End
 
 public:
     explicit QPieSlice(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qpolarchart.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qpolarchart.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpolarchart.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QPolarChart : QChart
+class QPolarChart : public QChart
 {
 %TypeHeaderCode
 #include <qpolarchart.h>
 %End
 
 public:
     enum PolarOrientation /BaseType=Flag/
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qscatterseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qscatterseries.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qscatterseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QScatterSeries : QXYSeries
+class QScatterSeries : public QXYSeries
 {
 %TypeHeaderCode
 #include <qscatterseries.h>
 %End
 
 public:
     enum MarkerShape
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qsplineseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qsplineseries.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsplineseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QSplineSeries : QLineSeries
+class QSplineSeries : public QLineSeries
 {
 %TypeHeaderCode
 #include <qsplineseries.h>
 %End
 
 public:
     explicit QSplineSeries(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qstackedbarseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qstackedbarseries.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qstackedbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QStackedBarSeries : QAbstractBarSeries
+class QStackedBarSeries : public QAbstractBarSeries
 {
 %TypeHeaderCode
 #include <qstackedbarseries.h>
 %End
 
 public:
     explicit QStackedBarSeries(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qvalueaxis.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qvalueaxis.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvalueaxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QValueAxis : QAbstractAxis
+class QValueAxis : public QAbstractAxis
 {
 %TypeHeaderCode
 #include <qvalueaxis.h>
 %End
 
 public:
     explicit QValueAxis(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qvbarmodelmapper.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qvbarmodelmapper.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvbarmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qvboxplotmodelmapper.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qvboxplotmodelmapper.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvboxplotmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qvcandlestickmodelmapper.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qvcandlestickmodelmapper.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvcandlestickmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QVCandlestickModelMapper : QCandlestickModelMapper
+class QVCandlestickModelMapper : public QCandlestickModelMapper
 {
 %TypeHeaderCode
 #include <qvcandlestickmodelmapper.h>
 %End
 
 public:
     explicit QVCandlestickModelMapper(QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qvpiemodelmapper.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qvpiemodelmapper.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvpiemodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qvxymodelmapper.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qvxymodelmapper.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvxymodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qxylegendmarker.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qxylegendmarker.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qxylegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QXYLegendMarker : QLegendMarker
+class QXYLegendMarker : public QLegendMarker
 {
 %TypeHeaderCode
 #include <qxylegendmarker.h>
 %End
 
 public:
     QXYLegendMarker(QXYSeries *series, QLegend *legend, QObject *parent /TransferThis/ = 0);
```

### Comparing `PyQt6_Charts-6.6.0/sip/QtCharts/qxyseries.sip` & `PyQt6_Charts-6.7.0/sip/QtCharts/qxyseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qxyseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2024 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -16,15 +16,15 @@
 // then you may purchase a commercial license.  For more information contact
 // info@riverbankcomputing.com.
 // 
 // This file is provided AS IS with NO WARRANTY OF ANY KIND, INCLUDING THE
 // WARRANTY OF DESIGN, MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.
 
 
-class QXYSeries : QAbstractSeries /NoDefaultCtors/
+class QXYSeries : public QAbstractSeries /NoDefaultCtors/
 {
 %TypeHeaderCode
 #include <qxyseries.h>
 %End
 
 public:
     virtual ~QXYSeries();
```

