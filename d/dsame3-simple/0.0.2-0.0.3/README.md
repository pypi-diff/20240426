# Comparing `tmp/dsame3_simple-0.0.2.tar.gz` & `tmp/dsame3_simple-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsame3_simple-0.0.2.tar", last modified: Tue Apr  2 17:25:59 2024, max compression
+gzip compressed data, was "dsame3_simple-0.0.3.tar", last modified: Fri Apr 26 03:32:25 2024, max compression
```

## Comparing `dsame3_simple-0.0.2.tar` & `dsame3_simple-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:25:59.117102 dsame3_simple-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 17:25:50.000000 dsame3_simple-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-02 17:25:59.117102 dsame3_simple-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9742 2024-04-02 17:25:50.000000 dsame3_simple-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-02 17:25:50.000000 dsame3_simple-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 17:25:59.117102 dsame3_simple-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:25:59.113102 dsame3_simple-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:25:59.117102 dsame3_simple-0.0.2/src/dsame3_simple/
--rw-r--r--   0 runner    (1001) docker     (127)   275555 2024-04-02 17:25:50.000000 dsame3_simple-0.0.2/src/dsame3_simple/defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21505 2024-04-02 17:25:50.000000 dsame3_simple-0.0.2/src/dsame3_simple/dsame.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 17:25:59.117102 dsame3_simple-0.0.2/src/dsame3_simple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-02 17:25:59.000000 dsame3_simple-0.0.2/src/dsame3_simple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-02 17:25:59.000000 dsame3_simple-0.0.2/src/dsame3_simple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 17:25:59.000000 dsame3_simple-0.0.2/src/dsame3_simple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 17:25:59.000000 dsame3_simple-0.0.2/src/dsame3_simple.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 17:25:59.000000 dsame3_simple-0.0.2/src/dsame3_simple.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:32:25.798312 dsame3_simple-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-26 03:32:21.000000 dsame3_simple-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10764 2024-04-26 03:32:25.798312 dsame3_simple-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9999 2024-04-26 03:32:21.000000 dsame3_simple-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-26 03:32:21.000000 dsame3_simple-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 03:32:25.798312 dsame3_simple-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:32:25.794312 dsame3_simple-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:32:25.794312 dsame3_simple-0.0.3/src/dsame3_simple/
+-rw-r--r--   0 runner    (1001) docker     (127)   275555 2024-04-26 03:32:21.000000 dsame3_simple-0.0.3/src/dsame3_simple/defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21951 2024-04-26 03:32:21.000000 dsame3_simple-0.0.3/src/dsame3_simple/dsame.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 03:32:25.798312 dsame3_simple-0.0.3/src/dsame3_simple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10764 2024-04-26 03:32:25.000000 dsame3_simple-0.0.3/src/dsame3_simple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-26 03:32:25.000000 dsame3_simple-0.0.3/src/dsame3_simple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 03:32:25.000000 dsame3_simple-0.0.3/src/dsame3_simple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 03:32:25.000000 dsame3_simple-0.0.3/src/dsame3_simple.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 03:32:25.000000 dsame3_simple-0.0.3/src/dsame3_simple.egg-info/top_level.txt
```

### Comparing `dsame3_simple-0.0.2/LICENSE` & `dsame3_simple-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsame3_simple-0.0.2/PKG-INFO` & `dsame3_simple-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsame3_simple
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simplified version of dsame3 to decode EAS SAME messages to readable text.
 Author: Joseph W. Metcalf, James Kitchens, Matthew R. McDougal
 Author-email: "Matthew R. McDougal" <ka0s@arrl.net>
 Project-URL: Homepage, https://github.com/ars-ka0s/dsame3_simple
 Project-URL: Bug Tracker, https://github.com/ars-ka0s/dsame3_simple/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
@@ -13,66 +13,68 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Communications :: Ham Radio
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dsame3
-Python EAS SAME Alert Message Decoder
+Python EAS SAME Alert Message Decoder, simplified
 
-**dsame3** is a program to decode [EAS](http://en.wikipedia.org/wiki/Emergency_Alert_System)/[SAME](http://en.wikipedia.org/wiki/Specific_Area_Message_Encoding) (Emergency Alert System/Specific Area Message Encoding) alert messages. These messages are primarily used by the National Weather Service for weather-related warnings. **dsame** will decode a demodulated message, filter by SAME ([US](http://www.nws.noaa.gov/nwr/coverage/county_coverage.html)/[CA](http://www.ec.gc.ca/meteo-weather/default.asp?lang=En&n=E5A4F19C-1)) and/or event code, provide readable text, or run an external program.
+**dsame3_simple** is a program to decode [EAS](http://en.wikipedia.org/wiki/Emergency_Alert_System)/[SAME](http://en.wikipedia.org/wiki/Specific_Area_Message_Encoding) (Emergency Alert System/Specific Area Message Encoding) alert messages. These messages are primarily used by the National Weather Service for weather-related warnings. **dsame** will decode a demodulated message, filter by SAME ([US](http://www.nws.noaa.gov/nwr/coverage/county_coverage.html)/[CA](http://www.ec.gc.ca/meteo-weather/default.asp?lang=En&n=E5A4F19C-1)) and/or event code, provide readable text, or run an external program.
 
 **DO NOT RELY ON THIS PROGRAM WHEN LOSS, DAMAGE, INJURY OR DEATH MAY OCCUR!**
 
-###NOTICE
+### NOTICE
 
 This program was originally written by [cuppa_joe](https://github.com/cuppa-joe/dsame), and was rewritten to include new updates and upgrade compatibility so others can modify the code without the headache of trying to work with Python 2.7. THIS IS NOT MY ORIGINAL CODE! I have modified it, and I will be updating it as necessary, since updates seem to have stopped on the original repository. 
 
-###Requirements
+Simplfied by [ars-ka0s](https://github.com/ars-ka0s) to remove several features such as transcription and recording that required specific libraries and OS support to make a pure python no dependency utility.
 
-* [Python](https://www.python.org/) 3.8+
+### Requirements
 
-###Installation
+* [Python](https://www.python.org/) 3.8+
 
-`pipx install dsame3_simple`
+### Installation
 
-Check [here](https://github.com/jamieden/dsame3/releases/latest) to download the latest release.
+`pip install dsame3_simple`
 
-###Command Line Options
+### Command Line Options
 
 ```
 usage: dsame3_simple [-h] [--msg MSG] [--same [SAME [SAME ...]]]
                      [--event [EVENT [EVENT ...]]] [--lang LANG]
                      [--loglevel {10,20,30,40,50}] [--version]
                      [--call CALL] [--command COMMAND]
 ```
-####Options
+#### Options
 
 Option            | Description                                                           | Example
 :-----------------|:----------------------------------------------------------------------|:----------------------
 `msg`             | Message to decode. Omit to read from standard input                   | `--msg "ZCZC-WXR-RWT-020103-020209-020091-020121-029047-029165-029095-029037+0030-1051700-KEAX/NWS"`
 `same`            | List of SAME codes to monitor                                         | `--same 029165 029095`
 `event`           | List of event codes to monitor                                        | `--event RWT TOR SVR`
 `loglevel`        | Set log level                                                         | `--loglevel 10`
 `call`            | Call an external program                                              | `--call alert.sh`
 `lang`            | Selects the language for the program**                                | `--lang EN`
 `command`         | External command line. Omit --call to send to standard output         | `--command "Event Code: {EEE}"`
 `wrap`            | Line length to wrap message (0 for no wrap)                           | `--wrap 80`
 
 ** The only available language options so far are English (EN) and Spanish (SP). The program defaults to English. 
 
-###Usage
+### Usage
+
+**dsame3_simple** can decode EAS messages from the command line, directly from the output of an external command, or by capturing the ouput of a shell script/batch file or external program. Use `msg` for single command line decoding. Without this option, standard input is used. Press `CTRL-C` to exit the program.
 
-**dsame3** can decode EAS messages from the command line, directly from the output of an external command, or by capturing the ouput of a shell script/batch file or external program. Use `msg` for single command line decoding. Without this option, standard input is used. Press `CTRL-C` to exit the program.
+The dsame3_simple.dsame.same_decode_string function can be used to decode programmatically as a library.
 
-###Filtering Alerts
+### Filtering Alerts
 
-There are two comands used to filter alerts. None, one or both can be specified. The `same` command is a list of SAME area codes ([United States](http://www.nws.noaa.gov/nwr/coverage/county_coverage.html)/[Canada](http://www.ec.gc.ca/meteo-weather/default.asp?lang=En&n=E5A4F19C-1)), and the `event` command is a list of event codes to monitor.
+There are two commands used to filter alerts. None, one or both can be specified. The `same` command is a list of SAME area codes ([United States](http://www.nws.noaa.gov/nwr/coverage/county_coverage.html)/[Canada](http://www.ec.gc.ca/meteo-weather/default.asp?lang=En&n=E5A4F19C-1)), and the `event` command is a list of event codes to monitor.
 
-####Event Codes
+#### Event Codes
 
 *This list includes current and proposed event codes.*
 
 Code| Description                  |Code| Description
 :--:|:-----------------------------|:--:|:-----------------------------
 ADR | Administrative Message       |AVA | Avalanche Watch
 AVW | Avalanche Warning            |BHW | Biological Hazard Warning
@@ -113,19 +115,19 @@
 WFW | Wild Fire Warning            |WSA | Winter Storm Watch
 WSW | Winter Storm Warning         |SQW | Snow Squall Warning*
 
 * Snow Squall Warnings are not conveyed to the EAS, however, it was added just in case/for futureproofing.
 
 An alert must match one of each specified alert type in order to be processed. If an alert type is omitted, any alert will match that type. In most cases, using only SAME codes to filter alerts will be the best option.
 
-###External Commands
+### External Commands
 
 The `call` option runs an external program, script/batch file for each alert.  The `command` option defines the command string sent to that program, script or batch file, or to standard output if the `call` option is omitted. The following variables can be used in command strings.
 
-####Command Variables
+#### Command Variables
 
 Variable        | Description                       | Example
 :---------------|:----------------------------------|:------------------
  {ORG}          | Organization code                 | WXR
  {EEE}          | Event code                        | RWT
  {PSSCCC}       | Geographical area (SAME) codes    | 020103-020209-020091-020121-029047-029165-029095-029037
  {TTTT}         | Purge time code                   | 0030
@@ -140,15 +142,15 @@
  {end}          | End time                          | 12:30 PM
  {length}       | Length of event                   | 30 minutes
  {seconds}      | Event length in seconds           | 1800 
  {date}         | Local date                        | 04/15/15 12:00:38
  {MESSAGE}      | Readable message                  | *(See sample text output below)*
 
 
-###Sample Commands
+### Sample Commands
 
 Decoding from a text file using standard input:
 
 `cat zczc.txt | dsame3_simple --same 029165`
 
 Call an external script with the event type and length:
 
@@ -158,20 +160,20 @@
 
 `dsame3_simple --msg "ZCZC-WXR-RWT-020103-020209-020091-020121-029047-029165-029095-029037+0030-1051700-KEAX/NWS" --text`
 
 Send an alert to a [Pushbullet](https://www.pushbullet.com) channel:
 
 `dsame3_simple --call pushbullet-channel.sh --command "{event}" "{MESSAGE}"`
 
-###Sample Text Output
+### Sample Text Output
 
 >The National Weather Service in Pleasant Hill, Missouri has issued a Required Weekly Test valid until 12:30 PM for the following counties in Kansas: Leavenworth, Wyandotte, Johnson, Miami, and for the following counties in Missouri: Clay, Platte, Jackson, Cass. (KEAX/NWS)
 
 
-###Known Issues
+### Known Issues
 
 * ~~SASMEX/SARMEX, a Mexican system for seismic alerts, is not implemented due to lack of documentation.~~ This issue has *HOPEFULLY* been resolved
 * ~~A correct and complete list of ICAO location codes used by the National Weather Service messages is not available.~~ This issue has *HOPEFULLY* been resolved
 * ~~Country detection may not be reliable for some locations with duplicate SAME codes.~~ This issue has *HOPEFULLY* been resolved
 * Date and time information may not be accurate when decoding old messages or messages from another time zone.
 * Multimon-ng will not decode the same alert in succession. This should only be an issue during testing and can be avoided by alternating test alerts.
```

### Comparing `dsame3_simple-0.0.2/README.md` & `dsame3_simple-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 # dsame3
-Python EAS SAME Alert Message Decoder
+Python EAS SAME Alert Message Decoder, simplified
 
-**dsame3** is a program to decode [EAS](http://en.wikipedia.org/wiki/Emergency_Alert_System)/[SAME](http://en.wikipedia.org/wiki/Specific_Area_Message_Encoding) (Emergency Alert System/Specific Area Message Encoding) alert messages. These messages are primarily used by the National Weather Service for weather-related warnings. **dsame** will decode a demodulated message, filter by SAME ([US](http://www.nws.noaa.gov/nwr/coverage/county_coverage.html)/[CA](http://www.ec.gc.ca/meteo-weather/default.asp?lang=En&n=E5A4F19C-1)) and/or event code, provide readable text, or run an external program.
+**dsame3_simple** is a program to decode [EAS](http://en.wikipedia.org/wiki/Emergency_Alert_System)/[SAME](http://en.wikipedia.org/wiki/Specific_Area_Message_Encoding) (Emergency Alert System/Specific Area Message Encoding) alert messages. These messages are primarily used by the National Weather Service for weather-related warnings. **dsame** will decode a demodulated message, filter by SAME ([US](http://www.nws.noaa.gov/nwr/coverage/county_coverage.html)/[CA](http://www.ec.gc.ca/meteo-weather/default.asp?lang=En&n=E5A4F19C-1)) and/or event code, provide readable text, or run an external program.
 
 **DO NOT RELY ON THIS PROGRAM WHEN LOSS, DAMAGE, INJURY OR DEATH MAY OCCUR!**
 
-###NOTICE
+### NOTICE
 
 This program was originally written by [cuppa_joe](https://github.com/cuppa-joe/dsame), and was rewritten to include new updates and upgrade compatibility so others can modify the code without the headache of trying to work with Python 2.7. THIS IS NOT MY ORIGINAL CODE! I have modified it, and I will be updating it as necessary, since updates seem to have stopped on the original repository. 
 
-###Requirements
+Simplfied by [ars-ka0s](https://github.com/ars-ka0s) to remove several features such as transcription and recording that required specific libraries and OS support to make a pure python no dependency utility.
 
-* [Python](https://www.python.org/) 3.8+
+### Requirements
 
-###Installation
+* [Python](https://www.python.org/) 3.8+
 
-`pipx install dsame3_simple`
+### Installation
 
-Check [here](https://github.com/jamieden/dsame3/releases/latest) to download the latest release.
+`pip install dsame3_simple`
 
-###Command Line Options
+### Command Line Options
 
 ```
 usage: dsame3_simple [-h] [--msg MSG] [--same [SAME [SAME ...]]]
                      [--event [EVENT [EVENT ...]]] [--lang LANG]
                      [--loglevel {10,20,30,40,50}] [--version]
                      [--call CALL] [--command COMMAND]
 ```
-####Options
+#### Options
 
 Option            | Description                                                           | Example
 :-----------------|:----------------------------------------------------------------------|:----------------------
 `msg`             | Message to decode. Omit to read from standard input                   | `--msg "ZCZC-WXR-RWT-020103-020209-020091-020121-029047-029165-029095-029037+0030-1051700-KEAX/NWS"`
 `same`            | List of SAME codes to monitor                                         | `--same 029165 029095`
 `event`           | List of event codes to monitor                                        | `--event RWT TOR SVR`
 `loglevel`        | Set log level                                                         | `--loglevel 10`
 `call`            | Call an external program                                              | `--call alert.sh`
 `lang`            | Selects the language for the program**                                | `--lang EN`
 `command`         | External command line. Omit --call to send to standard output         | `--command "Event Code: {EEE}"`
 `wrap`            | Line length to wrap message (0 for no wrap)                           | `--wrap 80`
 
 ** The only available language options so far are English (EN) and Spanish (SP). The program defaults to English. 
 
-###Usage
+### Usage
+
+**dsame3_simple** can decode EAS messages from the command line, directly from the output of an external command, or by capturing the ouput of a shell script/batch file or external program. Use `msg` for single command line decoding. Without this option, standard input is used. Press `CTRL-C` to exit the program.
 
-**dsame3** can decode EAS messages from the command line, directly from the output of an external command, or by capturing the ouput of a shell script/batch file or external program. Use `msg` for single command line decoding. Without this option, standard input is used. Press `CTRL-C` to exit the program.
+The dsame3_simple.dsame.same_decode_string function can be used to decode programmatically as a library.
 
-###Filtering Alerts
+### Filtering Alerts
 
-There are two comands used to filter alerts. None, one or both can be specified. The `same` command is a list of SAME area codes ([United States](http://www.nws.noaa.gov/nwr/coverage/county_coverage.html)/[Canada](http://www.ec.gc.ca/meteo-weather/default.asp?lang=En&n=E5A4F19C-1)), and the `event` command is a list of event codes to monitor.
+There are two commands used to filter alerts. None, one or both can be specified. The `same` command is a list of SAME area codes ([United States](http://www.nws.noaa.gov/nwr/coverage/county_coverage.html)/[Canada](http://www.ec.gc.ca/meteo-weather/default.asp?lang=En&n=E5A4F19C-1)), and the `event` command is a list of event codes to monitor.
 
-####Event Codes
+#### Event Codes
 
 *This list includes current and proposed event codes.*
 
 Code| Description                  |Code| Description
 :--:|:-----------------------------|:--:|:-----------------------------
 ADR | Administrative Message       |AVA | Avalanche Watch
 AVW | Avalanche Warning            |BHW | Biological Hazard Warning
@@ -95,19 +97,19 @@
 WFW | Wild Fire Warning            |WSA | Winter Storm Watch
 WSW | Winter Storm Warning         |SQW | Snow Squall Warning*
 
 * Snow Squall Warnings are not conveyed to the EAS, however, it was added just in case/for futureproofing.
 
 An alert must match one of each specified alert type in order to be processed. If an alert type is omitted, any alert will match that type. In most cases, using only SAME codes to filter alerts will be the best option.
 
-###External Commands
+### External Commands
 
 The `call` option runs an external program, script/batch file for each alert.  The `command` option defines the command string sent to that program, script or batch file, or to standard output if the `call` option is omitted. The following variables can be used in command strings.
 
-####Command Variables
+#### Command Variables
 
 Variable        | Description                       | Example
 :---------------|:----------------------------------|:------------------
  {ORG}          | Organization code                 | WXR
  {EEE}          | Event code                        | RWT
  {PSSCCC}       | Geographical area (SAME) codes    | 020103-020209-020091-020121-029047-029165-029095-029037
  {TTTT}         | Purge time code                   | 0030
@@ -122,15 +124,15 @@
  {end}          | End time                          | 12:30 PM
  {length}       | Length of event                   | 30 minutes
  {seconds}      | Event length in seconds           | 1800 
  {date}         | Local date                        | 04/15/15 12:00:38
  {MESSAGE}      | Readable message                  | *(See sample text output below)*
 
 
-###Sample Commands
+### Sample Commands
 
 Decoding from a text file using standard input:
 
 `cat zczc.txt | dsame3_simple --same 029165`
 
 Call an external script with the event type and length:
 
@@ -140,20 +142,20 @@
 
 `dsame3_simple --msg "ZCZC-WXR-RWT-020103-020209-020091-020121-029047-029165-029095-029037+0030-1051700-KEAX/NWS" --text`
 
 Send an alert to a [Pushbullet](https://www.pushbullet.com) channel:
 
 `dsame3_simple --call pushbullet-channel.sh --command "{event}" "{MESSAGE}"`
 
-###Sample Text Output
+### Sample Text Output
 
 >The National Weather Service in Pleasant Hill, Missouri has issued a Required Weekly Test valid until 12:30 PM for the following counties in Kansas: Leavenworth, Wyandotte, Johnson, Miami, and for the following counties in Missouri: Clay, Platte, Jackson, Cass. (KEAX/NWS)
 
 
-###Known Issues
+### Known Issues
 
 * ~~SASMEX/SARMEX, a Mexican system for seismic alerts, is not implemented due to lack of documentation.~~ This issue has *HOPEFULLY* been resolved
 * ~~A correct and complete list of ICAO location codes used by the National Weather Service messages is not available.~~ This issue has *HOPEFULLY* been resolved
 * ~~Country detection may not be reliable for some locations with duplicate SAME codes.~~ This issue has *HOPEFULLY* been resolved
 * Date and time information may not be accurate when decoding old messages or messages from another time zone.
 * Multimon-ng will not decode the same alert in succession. This should only be an issue during testing and can be avoided by alternating test alerts.
```

### Comparing `dsame3_simple-0.0.2/pyproject.toml` & `dsame3_simple-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dsame3_simple"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
 ]
 authors = [
     { name="Joseph W. Metcalf" },
     { name="James Kitchens" },
     { name="Matthew R. McDougal" },
     { name="Matthew R. McDougal", email="ka0s@arrl.net" }
```

### Comparing `dsame3_simple-0.0.2/src/dsame3_simple/defs.py` & `dsame3_simple-0.0.3/src/dsame3_simple/defs.py`

 * *Files identical despite different names*

### Comparing `dsame3_simple-0.0.2/src/dsame3_simple/dsame.py` & `dsame3_simple-0.0.3/src/dsame3_simple/dsame.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,16 +360,27 @@
                 bad_list = MX_bad_list
             elif COUNTRY == 'US':
                 bad_list = US_bad_list
             for code in bad_list:
                 PSSCCC_list.remove(code)
             PSSCCC_list.sort()
             if check_watch(same_watch, PSSCCC_list, event_watch, EEE):
-                msgs += [readable_message(ORG, EEE, PSSCCC_list, TTTT, JJJHHMM, STATION, TYPE, LLLLLLLL, COUNTRY,
-                                           lang, wraplen, True)]
+                msg = {
+                    'originator': ORG,
+                    'event': EEE,
+                    'country': COUNTRY,
+                    'areas': PSSCCC_list,
+                    'start_time': alert_start(JJJHHMM),
+                    'duration': alert_length(TTTT),
+                    'end_time': alert_end(JJJHHMM, TTTT),
+                    'station': LLLLLLLL,
+                    'msg': readable_message(ORG, EEE, PSSCCC_list, TTTT, JJJHHMM, STATION, TYPE, LLLLLLLL, COUNTRY,
+                                           lang, wraplen, True)
+                }
+                msgs += [msg]
         else:
             if endidx == -1:
                 return msgs
             else:
                 tail = same[msgidx:+len('NNNN')]
         # Move ahead and look for more
         same = tail
```

### Comparing `dsame3_simple-0.0.2/src/dsame3_simple.egg-info/PKG-INFO` & `dsame3_simple-0.0.3/src/dsame3_simple.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsame3_simple
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simplified version of dsame3 to decode EAS SAME messages to readable text.
 Author: Joseph W. Metcalf, James Kitchens, Matthew R. McDougal
 Author-email: "Matthew R. McDougal" <ka0s@arrl.net>
 Project-URL: Homepage, https://github.com/ars-ka0s/dsame3_simple
 Project-URL: Bug Tracker, https://github.com/ars-ka0s/dsame3_simple/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
@@ -13,66 +13,68 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Communications :: Ham Radio
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dsame3
-Python EAS SAME Alert Message Decoder
+Python EAS SAME Alert Message Decoder, simplified
 
-**dsame3** is a program to decode [EAS](http://en.wikipedia.org/wiki/Emergency_Alert_System)/[SAME](http://en.wikipedia.org/wiki/Specific_Area_Message_Encoding) (Emergency Alert System/Specific Area Message Encoding) alert messages. These messages are primarily used by the National Weather Service for weather-related warnings. **dsame** will decode a demodulated message, filter by SAME ([US](http://www.nws.noaa.gov/nwr/coverage/county_coverage.html)/[CA](http://www.ec.gc.ca/meteo-weather/default.asp?lang=En&n=E5A4F19C-1)) and/or event code, provide readable text, or run an external program.
+**dsame3_simple** is a program to decode [EAS](http://en.wikipedia.org/wiki/Emergency_Alert_System)/[SAME](http://en.wikipedia.org/wiki/Specific_Area_Message_Encoding) (Emergency Alert System/Specific Area Message Encoding) alert messages. These messages are primarily used by the National Weather Service for weather-related warnings. **dsame** will decode a demodulated message, filter by SAME ([US](http://www.nws.noaa.gov/nwr/coverage/county_coverage.html)/[CA](http://www.ec.gc.ca/meteo-weather/default.asp?lang=En&n=E5A4F19C-1)) and/or event code, provide readable text, or run an external program.
 
 **DO NOT RELY ON THIS PROGRAM WHEN LOSS, DAMAGE, INJURY OR DEATH MAY OCCUR!**
 
-###NOTICE
+### NOTICE
 
 This program was originally written by [cuppa_joe](https://github.com/cuppa-joe/dsame), and was rewritten to include new updates and upgrade compatibility so others can modify the code without the headache of trying to work with Python 2.7. THIS IS NOT MY ORIGINAL CODE! I have modified it, and I will be updating it as necessary, since updates seem to have stopped on the original repository. 
 
-###Requirements
+Simplfied by [ars-ka0s](https://github.com/ars-ka0s) to remove several features such as transcription and recording that required specific libraries and OS support to make a pure python no dependency utility.
 
-* [Python](https://www.python.org/) 3.8+
+### Requirements
 
-###Installation
+* [Python](https://www.python.org/) 3.8+
 
-`pipx install dsame3_simple`
+### Installation
 
-Check [here](https://github.com/jamieden/dsame3/releases/latest) to download the latest release.
+`pip install dsame3_simple`
 
-###Command Line Options
+### Command Line Options
 
 ```
 usage: dsame3_simple [-h] [--msg MSG] [--same [SAME [SAME ...]]]
                      [--event [EVENT [EVENT ...]]] [--lang LANG]
                      [--loglevel {10,20,30,40,50}] [--version]
                      [--call CALL] [--command COMMAND]
 ```
-####Options
+#### Options
 
 Option            | Description                                                           | Example
 :-----------------|:----------------------------------------------------------------------|:----------------------
 `msg`             | Message to decode. Omit to read from standard input                   | `--msg "ZCZC-WXR-RWT-020103-020209-020091-020121-029047-029165-029095-029037+0030-1051700-KEAX/NWS"`
 `same`            | List of SAME codes to monitor                                         | `--same 029165 029095`
 `event`           | List of event codes to monitor                                        | `--event RWT TOR SVR`
 `loglevel`        | Set log level                                                         | `--loglevel 10`
 `call`            | Call an external program                                              | `--call alert.sh`
 `lang`            | Selects the language for the program**                                | `--lang EN`
 `command`         | External command line. Omit --call to send to standard output         | `--command "Event Code: {EEE}"`
 `wrap`            | Line length to wrap message (0 for no wrap)                           | `--wrap 80`
 
 ** The only available language options so far are English (EN) and Spanish (SP). The program defaults to English. 
 
-###Usage
+### Usage
+
+**dsame3_simple** can decode EAS messages from the command line, directly from the output of an external command, or by capturing the ouput of a shell script/batch file or external program. Use `msg` for single command line decoding. Without this option, standard input is used. Press `CTRL-C` to exit the program.
 
-**dsame3** can decode EAS messages from the command line, directly from the output of an external command, or by capturing the ouput of a shell script/batch file or external program. Use `msg` for single command line decoding. Without this option, standard input is used. Press `CTRL-C` to exit the program.
+The dsame3_simple.dsame.same_decode_string function can be used to decode programmatically as a library.
 
-###Filtering Alerts
+### Filtering Alerts
 
-There are two comands used to filter alerts. None, one or both can be specified. The `same` command is a list of SAME area codes ([United States](http://www.nws.noaa.gov/nwr/coverage/county_coverage.html)/[Canada](http://www.ec.gc.ca/meteo-weather/default.asp?lang=En&n=E5A4F19C-1)), and the `event` command is a list of event codes to monitor.
+There are two commands used to filter alerts. None, one or both can be specified. The `same` command is a list of SAME area codes ([United States](http://www.nws.noaa.gov/nwr/coverage/county_coverage.html)/[Canada](http://www.ec.gc.ca/meteo-weather/default.asp?lang=En&n=E5A4F19C-1)), and the `event` command is a list of event codes to monitor.
 
-####Event Codes
+#### Event Codes
 
 *This list includes current and proposed event codes.*
 
 Code| Description                  |Code| Description
 :--:|:-----------------------------|:--:|:-----------------------------
 ADR | Administrative Message       |AVA | Avalanche Watch
 AVW | Avalanche Warning            |BHW | Biological Hazard Warning
@@ -113,19 +115,19 @@
 WFW | Wild Fire Warning            |WSA | Winter Storm Watch
 WSW | Winter Storm Warning         |SQW | Snow Squall Warning*
 
 * Snow Squall Warnings are not conveyed to the EAS, however, it was added just in case/for futureproofing.
 
 An alert must match one of each specified alert type in order to be processed. If an alert type is omitted, any alert will match that type. In most cases, using only SAME codes to filter alerts will be the best option.
 
-###External Commands
+### External Commands
 
 The `call` option runs an external program, script/batch file for each alert.  The `command` option defines the command string sent to that program, script or batch file, or to standard output if the `call` option is omitted. The following variables can be used in command strings.
 
-####Command Variables
+#### Command Variables
 
 Variable        | Description                       | Example
 :---------------|:----------------------------------|:------------------
  {ORG}          | Organization code                 | WXR
  {EEE}          | Event code                        | RWT
  {PSSCCC}       | Geographical area (SAME) codes    | 020103-020209-020091-020121-029047-029165-029095-029037
  {TTTT}         | Purge time code                   | 0030
@@ -140,15 +142,15 @@
  {end}          | End time                          | 12:30 PM
  {length}       | Length of event                   | 30 minutes
  {seconds}      | Event length in seconds           | 1800 
  {date}         | Local date                        | 04/15/15 12:00:38
  {MESSAGE}      | Readable message                  | *(See sample text output below)*
 
 
-###Sample Commands
+### Sample Commands
 
 Decoding from a text file using standard input:
 
 `cat zczc.txt | dsame3_simple --same 029165`
 
 Call an external script with the event type and length:
 
@@ -158,20 +160,20 @@
 
 `dsame3_simple --msg "ZCZC-WXR-RWT-020103-020209-020091-020121-029047-029165-029095-029037+0030-1051700-KEAX/NWS" --text`
 
 Send an alert to a [Pushbullet](https://www.pushbullet.com) channel:
 
 `dsame3_simple --call pushbullet-channel.sh --command "{event}" "{MESSAGE}"`
 
-###Sample Text Output
+### Sample Text Output
 
 >The National Weather Service in Pleasant Hill, Missouri has issued a Required Weekly Test valid until 12:30 PM for the following counties in Kansas: Leavenworth, Wyandotte, Johnson, Miami, and for the following counties in Missouri: Clay, Platte, Jackson, Cass. (KEAX/NWS)
 
 
-###Known Issues
+### Known Issues
 
 * ~~SASMEX/SARMEX, a Mexican system for seismic alerts, is not implemented due to lack of documentation.~~ This issue has *HOPEFULLY* been resolved
 * ~~A correct and complete list of ICAO location codes used by the National Weather Service messages is not available.~~ This issue has *HOPEFULLY* been resolved
 * ~~Country detection may not be reliable for some locations with duplicate SAME codes.~~ This issue has *HOPEFULLY* been resolved
 * Date and time information may not be accurate when decoding old messages or messages from another time zone.
 * Multimon-ng will not decode the same alert in succession. This should only be an issue during testing and can be avoided by alternating test alerts.
```

