# Comparing `tmp/MobileInventoryCLI-0.4.66.tar.gz` & `tmp/MobileInventoryCLI-0.4.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.66.tar", last modified: Thu Apr 25 13:28:14 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.67.tar", last modified: Thu Apr 25 19:20:28 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.66.tar` & `MobileInventoryCLI-0.4.67.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.438771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.442104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   106666 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6098 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)     3078 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
--rw-r--r--   0 carl      (1000) carl      (1000)    17392 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    69631 2024-04-25 13:24:18.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
--rw-r--r--   0 carl      (1000) carl      (1000)     1642 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-25 13:28:08.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1988 2024-04-25 13:27:53.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-25 13:28:14.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5283 2024-04-25 13:28:14.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 13:28:14.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-25 13:28:14.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-25 13:28:14.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-25 13:28:14.000000 MobileInventoryCLI-0.4.66/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.490471 MobileInventoryCLI-0.4.67/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.480471 MobileInventoryCLI-0.4.67/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.480471 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.483804 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.483804 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.483804 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.483804 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   107002 2024-04-25 19:13:35.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-04-25 19:12:03.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6098 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3078 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    17392 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    69631 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.487137 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1642 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-25 19:20:24.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2249 2024-04-25 19:20:07.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.490471 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.490471 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.490471 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.490471 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.490471 MobileInventoryCLI-0.4.67/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.490471 MobileInventoryCLI-0.4.67/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.490471 MobileInventoryCLI-0.4.67/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.490471 MobileInventoryCLI-0.4.67/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-25 13:28:26.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:20:28.490471 MobileInventoryCLI-0.4.67/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-25 19:20:28.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5356 2024-04-25 19:20:28.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 19:20:28.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-25 19:20:28.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-25 19:20:28.000000 MobileInventoryCLI-0.4.67/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-25 19:20:28.490471 MobileInventoryCLI-0.4.67/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-25 19:20:28.490471 MobileInventoryCLI-0.4.67/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-25 19:20:28.000000 MobileInventoryCLI-0.4.67/setup.py
```

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,29 @@
         print(msg)
     def split_by_len(self,string, length):
         result = []
         for i in range(0, len(string), length):
             result.append(string[i:i + length])
         return result
 
-class Entry(BASE):
+class EntryExtras:
+    def __add__(self,val):
+        return self.Price+val
+    def __sub__(self,val):
+        return self.Price-val
+    def __truediv__(self,val):
+        return self.Price/val
+    def __mul__(self,val):
+        return self.Price*val
+    def __pow__(self,val):
+        return self.Price**val
+
+
+
+class Entry(BASE,EntryExtras):
     __tablename__="Entry"
     Code=Column(String)
     Barcode=Column(String)
     #not found in prompt requested by
     '''
     #name {Entryid}
     #name {Entryid} {new_value}
@@ -868,15 +882,15 @@
 Entry.metadata.create_all(ENGINE)
 PairCollection.metadata.create_all(ENGINE)
 tables={
     'Entry':Entry,
     'PairCollection':PairCollection,
 }
 
-class DayLog(BASE):
+class DayLog(BASE,EntryExtras):
     __tablename__="DayLog"
     DayLogId=Column(Integer,primary_key=True)
     DayLogDate=Column(Date)
     Code=Column(String)
     Barcode=Column(String)
 
     #How Much Typically Comes in Load
```

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,7 +17,12 @@
 							begin similar process to t->#40 and create new item
 						if item:
 							prompt for location field to set
 							prompt for amount, or leave blank to skip
 							set InList==True so le-img can export the Entry, or qsl
 								can be used to quick-show-list
 6:27 am 04-25-2024 -- added version value
+12:16 pm 04-25-2024 -- added EntryExtras class to add operator functionality to classes Entry and DayLog, so one can 						do:
+							a=Entry(Barcode='BARCODE',Code='CODE',Name='NAME',Price=1.99)
+							#any of [+|-|*|/|**]
+							b=a+10
+							b will be 11.99
```

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.66
+Version: 0.4.67
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.67/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
 MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
```

### Comparing `MobileInventoryCLI-0.4.66/PKG-INFO` & `MobileInventoryCLI-0.4.67/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.66
+Version: 0.4.67
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.66/setup.py` & `MobileInventoryCLI-0.4.67/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.66'
+version='0.4.67'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

