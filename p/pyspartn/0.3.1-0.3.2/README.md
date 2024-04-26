# Comparing `tmp/pyspartn-0.3.1.tar.gz` & `tmp/pyspartn-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspartn-0.3.1.tar", last modified: Tue Apr 23 07:50:12 2024, max compression
+gzip compressed data, was "pyspartn-0.3.2.tar", last modified: Fri Apr 26 07:21:43 2024, max compression
```

## Comparing `pyspartn-0.3.1.tar` & `pyspartn-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-23 07:50:12.238873 pyspartn-0.3.1/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2024-04-20 10:34:35.000000 pyspartn-0.3.1/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2024-04-20 10:34:35.000000 pyspartn-0.3.1/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    19547 2024-04-23 07:50:12.238520 pyspartn-0.3.1/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    15955 2024-04-23 07:49:44.000000 pyspartn-0.3.1/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2446 2024-04-23 07:49:44.000000 pyspartn-0.3.1/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2024-04-23 07:50:12.238931 pyspartn-0.3.1/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-23 07:50:12.233755 pyspartn-0.3.1/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-23 07:50:12.236023 pyspartn-0.3.1/src/pyspartn/
--rw-r--r--   0 steve      (501) staff       (20)      598 2024-04-20 10:34:35.000000 pyspartn-0.3.1/src/pyspartn/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      162 2024-04-23 07:49:44.000000 pyspartn-0.3.1/src/pyspartn/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      671 2024-04-20 10:34:35.000000 pyspartn-0.3.1/src/pyspartn/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)     2441 2024-04-20 10:34:35.000000 pyspartn-0.3.1/src/pyspartn/socket_stream.py
--rw-r--r--   0 steve      (501) staff       (20)     7808 2024-04-20 10:34:35.000000 pyspartn-0.3.1/src/pyspartn/spartnhelpers.py
--rw-r--r--   0 steve      (501) staff       (20)    18609 2024-04-23 07:49:44.000000 pyspartn-0.3.1/src/pyspartn/spartnmessage.py
--rw-r--r--   0 steve      (501) staff       (20)    10066 2024-04-20 10:34:35.000000 pyspartn-0.3.1/src/pyspartn/spartnreader.py
--rw-r--r--   0 steve      (501) staff       (20)      222 2024-04-20 10:34:35.000000 pyspartn-0.3.1/src/pyspartn/spartntables.py
--rw-r--r--   0 steve      (501) staff       (20)     8507 2024-04-23 07:49:44.000000 pyspartn-0.3.1/src/pyspartn/spartntypes_core.py
--rw-r--r--   0 steve      (501) staff       (20)    23851 2024-04-23 07:49:44.000000 pyspartn-0.3.1/src/pyspartn/spartntypes_get.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-23 07:50:12.237658 pyspartn-0.3.1/src/pyspartn.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    19547 2024-04-23 07:50:12.000000 pyspartn-0.3.1/src/pyspartn.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      576 2024-04-23 07:50:12.000000 pyspartn-0.3.1/src/pyspartn.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2024-04-23 07:50:12.000000 pyspartn-0.3.1/src/pyspartn.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      134 2024-04-23 07:50:12.000000 pyspartn-0.3.1/src/pyspartn.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        9 2024-04-23 07:50:12.000000 pyspartn-0.3.1/src/pyspartn.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-23 07:50:12.237370 pyspartn-0.3.1/tests/
--rw-r--r--   0 steve      (501) staff       (20)     4043 2024-04-20 10:34:35.000000 pyspartn-0.3.1/tests/test_socket.py
--rw-r--r--   0 steve      (501) staff       (20)     6172 2024-04-20 10:34:35.000000 pyspartn-0.3.1/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)   102476 2024-04-23 07:49:44.000000 pyspartn-0.3.1/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 07:21:43.611648 pyspartn-0.3.2/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2024-04-25 22:03:47.000000 pyspartn-0.3.2/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2024-04-25 22:03:47.000000 pyspartn-0.3.2/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    22910 2024-04-26 07:21:43.611349 pyspartn-0.3.2/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    19358 2024-04-26 07:17:19.000000 pyspartn-0.3.2/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2446 2024-04-26 07:17:19.000000 pyspartn-0.3.2/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2024-04-26 07:21:43.611705 pyspartn-0.3.2/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 07:21:43.606999 pyspartn-0.3.2/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 07:21:43.609070 pyspartn-0.3.2/src/pyspartn/
+-rw-r--r--   0 steve      (501) staff       (20)      598 2024-04-25 22:03:47.000000 pyspartn-0.3.2/src/pyspartn/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      162 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      671 2024-04-25 22:03:47.000000 pyspartn-0.3.2/src/pyspartn/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     2441 2024-04-25 22:03:47.000000 pyspartn-0.3.2/src/pyspartn/socket_stream.py
+-rw-r--r--   0 steve      (501) staff       (20)     8202 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/spartnhelpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    18848 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/spartnmessage.py
+-rw-r--r--   0 steve      (501) staff       (20)    11757 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/spartnreader.py
+-rw-r--r--   0 steve      (501) staff       (20)     4010 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/spartntables.py
+-rw-r--r--   0 steve      (501) staff       (20)     9339 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/spartntypes_core.py
+-rw-r--r--   0 steve      (501) staff       (20)    25523 2024-04-26 07:17:19.000000 pyspartn-0.3.2/src/pyspartn/spartntypes_get.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 07:21:43.610545 pyspartn-0.3.2/src/pyspartn.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    22910 2024-04-26 07:21:43.000000 pyspartn-0.3.2/src/pyspartn.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      576 2024-04-26 07:21:43.000000 pyspartn-0.3.2/src/pyspartn.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2024-04-26 07:21:43.000000 pyspartn-0.3.2/src/pyspartn.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      134 2024-04-26 07:21:43.000000 pyspartn-0.3.2/src/pyspartn.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)        9 2024-04-26 07:21:43.000000 pyspartn-0.3.2/src/pyspartn.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-04-26 07:21:43.610253 pyspartn-0.3.2/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     4043 2024-04-25 22:03:47.000000 pyspartn-0.3.2/tests/test_socket.py
+-rw-r--r--   0 steve      (501) staff       (20)     8457 2024-04-26 07:17:19.000000 pyspartn-0.3.2/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)   137741 2024-04-26 07:17:19.000000 pyspartn-0.3.2/tests/test_stream.py
```

### Comparing `pyspartn-0.3.1/LICENSE` & `pyspartn-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.1/PKG-INFO` & `pyspartn-0.3.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.3.1
+Version: 0.3.2
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -77,14 +77,15 @@
 [Current Status](#currentstatus) |
 [Installation](#installation) |
 [Reading](#reading) |
 [Parsing](#parsing) |
 [Generating](#generating) |
 [Serializing](#serializing) |
 [Examples](#examples) |
+[Troubleshooting](#troubleshooting) |
 [Graphical Client](#gui) |
 [Author & License](#author)
 
 `pyspartn` is an original Python 3 parser for the SPARTN &copy; GPS/GNSS protocol. SPARTN is an open-source GPS/GNSS [differential correction or DGPS](https://en.wikipedia.org/wiki/Differential_GPS) protocol published by u-blox:
 
 [SPARTN Protocol](https://www.spartnformat.org/download/) (available in the public domain).
 © 2021 u-blox AG. All rights reserved.
@@ -109,19 +110,15 @@
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyspartn)
 
 The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
 
-The `SPARTNMessage` class implements decrypt and decode algorithms for OCB, HPAC and GAD message types:
- - GAD payload decryption and decode is fully tested and functional, which confirms that the global decryption mechanism and parsing algorithms are essentially correct.
- - HPAC and OCB payload decodes appear to be working OK, but results have not yet been fully validated and some individual attributes may be incorrect.
-
-*For the time being, a temporary override has been implemented in `spartnmessage.py` to suppress the `decode` flag for those payload types that cannot yet be successfully decoded. Testing contributions welcome*.
+The `SPARTNMessage` class implements optional decrypt and decode algorithms for OCB, HPAC and GAD message types (*BPAC, EAS & PROP message types are rarely used and not currently implemented*). Test coverage is currently limited by available SPARTN test data sources - additional testing contributions are welcome.
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyspartn](https://www.semuconsulting.com/pyspartn).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided. For general queries and advice, please use the [Discussion](https://github.com/semuconsulting/pyspartn/discussions) Forum.
 
@@ -178,25 +175,25 @@
 class pyspartn.spartnreader.SPARTNReader(stream, **kwargs)
 ```
 
 You can create a `SPARTNReader` object by calling the constructor with an active stream object. 
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
 or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
-Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator.
+Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator. See examples below.
 
 Example -  Serial input:
 ```python
 >>> from serial import Serial
 >>> from pyspartn import SPARTNReader
 >>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
 >>>spr = SPARTNReader(stream)
 >>> (raw_data, parsed_data) = spr.read()
 >>> print(parsed_data)
-
+...
 ```
 
 Example - File input (using iterator).
 ```python
 >>> from pyspartn import SPARTNReader
 >>> stream = open('spartndata.log', 'rb')
 >>> spr = SPARTNReader(stream)
@@ -208,63 +205,93 @@
 ```python
 >>> import socket
 >>> from pyspartn import SPARTNReader
 >>> stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
 >>> stream.connect(("localhost", 50007))
 >>> spr = SPARTNReader(stream)
 >>> for (raw_data, parsed_data) in spr: print(parsed_data)
+...
+```
+
+#### Encrypted Payloads
+
+Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now()`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
+
+The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need amending every 4 weeks.
+
+Example -  Real time serial input with decryption:
+```python
+>>> from serial import Serial
+>>> from pyspartn import SPARTNReader
+>>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
+>>>spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
+>>> (raw_data, parsed_data) = spr.read()
+>>> print(parsed_data)
+...
+```
+
+Example - Historical file input with decryption.
+```python
+>>> from datetime import datetime
+>>> from pyspartn import SPARTNReader
+>>> stream = open('spartndata.log', 'rb')
+>>> spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255))
+>>> for (raw_data, parsed_data) in spr: print(parsed_data)
+...
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
-You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. The optional `decode` keyword argument signifies whether to decrypt and decode the full payload (default = `False`). If `decode` is set to `True` and the message is encrypted (`eaf=1`), you *must* provide the following arguments:
-- `key` - the SPARTN decryption key valid at the time the message was originally created, as provided by your SPARTN service (normally 32 hexadecimal characters). 
-- `basedate` - a nominal datetime or 32-bit gnssTimeTag value, needed to convert an ambiguous 16-bit gnssTimeTag value to its unambiguous 32-bit equivalent. This is used by the decryption routine to determine the cryptographic Initialisation Vector (IV). If you're parsing messages in real time, this can default to `datetime.now()`. If you're parsing data from an older message stream, you will need to use the datetime the stream was originally created (*to the nearest half day*), or a 32-bit gnssTimeTag value from the same stream. See examples below.
+You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. If the message payload is encrypted (`eaf=1`), a decryption `key` and `basedate` must be provided. See examples below.
 
 **NB:** Once instantiated, a `SPARTNMMessage` object is immutable.
 
-Example - without payload decryption:
+Example - without payload decryption or decoding:
 
 ```python
 >>> from pyspartn import SPARTNReader
->>> msg = SPARTNReader.parse(b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad", decode=False)
+>>> transport = b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
+>>> msg = SPARTNReader.parse(transport, decode=0)
 >>> print(msg)
-<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
+<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
-Example - with payload decryption (requires key and, for messages where timeTagtype = 0, a nominal basedate for IV calculation):
+Example - with payload decryption and decoding (requires key and, for messages where `timeTagtype=0`, a nominal basedate):
 
 ```python
->>> from pyspartn import SPARTNReader
 >>> from datetime import datetime
->>> msg = SPARTNReader.parse(b'\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80', decode=True, key="6b30302427df05b4d98911ebff3a4d95", basedate=datetime(2023,6,27,22,3,0))
+>>> from pyspartn import SPARTNReader
+>>> transport = b'\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80'
+>>> msg = SPARTNReader.parse(transport, decode=1, key="6b30302427df05b4d98911ebff3a4d95", basedate=datetime(2023,6,27,22,3,0))
                                                                                
 >>> print(msg)
-<SPARTN(SPARTN-1X-GAD, msgType=2, nData=50, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=32580, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=6182016, SF005=37, SF068=1, SF069=0, SF030=7, SF031_01=32, SF032_01=1332, SF033_01=1987, SF034_01=6, SF035_01=2, SF036_01=5, SF037_01=22, SF031_02=33, SF032_02=1332, SF033_02=2033, SF034_02=6, SF035_02=3, SF036_02=5, SF037_02=16, SF031_03=34, SF032_03=1301, SF033_03=1921, SF034_03=2, SF035_03=6, SF036_03=18, SF037_03=10, SF031_04=35, SF032_04=1297, SF033_04=1987, SF034_04=3, SF035_04=3, SF036_04=12, SF037_04=22, SF031_05=36, SF032_05=1448, SF033_05=1768, SF034_05=6, SF035_05=2, SF036_05=5, SF037_05=30, SF031_06=37, SF032_06=1391, SF033_06=1745, SF034_06=4, SF035_06=7, SF036_06=7, SF037_06=10, SF031_07=38, SF032_07=1360, SF033_07=1906, SF034_07=3, SF035_07=2, SF036_07=8, SF037_07=22)>
+<SPARTN(SPARTN-1X-GAD, msgType=2, nData=50, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=32580, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=6182016, SF005=37, SF068=1, SF069=0, SF030=7, SF031_01=32, SF032_01=43.20000000000002, SF033_01=18.700000000000017, SF034_01=6, SF035_01=2, SF036_01=0.6, SF037_01=2.3000000000000003, SF031_02=33, SF032_02=43.20000000000002, SF033_02=23.30000000000001, SF034_02=6, SF035_02=3, SF036_02=0.6, SF037_02=1.7000000000000002, SF031_03=34, SF032_03=40.099999999999994, SF033_03=12.100000000000023, SF034_03=2, SF035_03=6, SF036_03=1.9000000000000001, SF037_03=1.1, SF031_04=35, SF032_04=39.70000000000002, SF033_04=18.700000000000017, SF034_04=3, SF035_04=3, SF036_04=1.3000000000000003, SF037_04=2.3000000000000003, SF031_05=36, SF032_05=54.80000000000001, SF033_05=-3.1999999999999886, SF034_05=6, SF035_05=2, SF036_05=0.6, SF037_05=3.1, SF031_06=37, SF032_06=49.099999999999994, SF033_06=-5.5, SF034_06=4, SF035_06=7, SF036_06=0.8, SF037_06=1.1, SF031_07=38, SF032_07=46.0, SF033_07=10.600000000000023, SF034_07=3, SF035_07=2, SF036_07=0.9, SF037_07=2.3000000000000003, SF031_08=39, SF032_08=46.0, SF033_08=1.8000000000000114, SF034_08=7, SF035_08=2, SF036_08=0.7000000000000001, SF037_08=2.3000000000000003)>
 ```
 
-
 The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity'. SPARTN data fields are denoted `SFnnn` - use the `datadesc()` helper method to obtain a more user-friendly text description of the data field.
 
 ```python
+>>> from datetime import datetime
 >>> from pyspartn import SPARTNReader, datadesc
->>> msg = SPARTNReader.parse(b'\x73\x03\x35\xec\x08\xc7\xd4\x20\x70\x5b\x1f\xc ... \x1e\xbe\x18\x43\x2d\x57\xe7\xa7', decode=True, key="00112233445566778899aabbccddeeff")
+>>> msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255))
 >>> print(msg)
-<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=619, eaf=1, crcType=2, frameCrc=12, msgSubtype=0, timeTagtype=1, gnssTimeTag=419070990, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=5760935, SF005=508, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=127, SF044_01=1, SF048_01=213, SF049a_01=257, SF049b_01=253, SF054_01=1, SatBitmaskLen_01=0, SF011_01=70263185, SF055_01_01=6, SF056_01_01=1, SF060_01_01=8944, ... SF061b_09_08=8287)>
+     <SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, ..., SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>
 >>> msg.identity
 'SPARTN-1X-HPAC-GPS'
 >>> msg.gnssTimeTag
-419070990
->>> msg.SF005
-508
-datadesc("SF005")
-'Solution issue of update (SIOU)'
+451165680
+>>> datadesc("SF005"), msg.SF005
+('Solution issue of update (SIOU)', 152)
+>>> datadesc("SF061a"), msg.SF061a_10_05
+('Large ionosphere coefficient C01', -0.27200000000000557)
 ```
 
+Enumerations for coded values can be found in [spartntables.py](https://github.com/semuconsulting/pyspartn/blob/main/src/pyspartn/spartntables.py).
+
 The `payload` attribute always contains the raw payload as bytes.
 
 ---
 ## <a name="generating">Generating</a>
 
 ```
 class pyspartn.spartnmessage.SPARTNMessage(**kwargs)
@@ -275,34 +302,34 @@
 
 Example:
 
 ```python
 >>> from pyspartn import SPARTNMessage
 >>> msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
 >>> print(msg)
-<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
+<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
 ---
 ## <a name="serializing">Serializing</a>
 
 The `SPARTNMessage` class implements a `serialize()` method to convert a `SPARTNMMessage` object to a bytes array suitable for writing to an output stream.
 
-e.g. to create and send a `1005` message type:
+e.g. to create and send a SPARTN-1X-OCB-GPS message type:
 
 ```python
 >>> from serial import Serial
->>> serialOut = Serial('COM7', 38400, timeout=5)
+>>> serialOut = Serial('/dev/ttyACM1', 38400, timeout=5)
 >>> from pyspartn import SPARTNMessage
 >>> msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
 >>> print(msg)
-<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
+<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 >>> output = msg.serialize()
 >>> output
-b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
+b's\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad'
 >>> serialOut.write(output)
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
@@ -313,14 +340,27 @@
 SPARTN NTRIP service e.g. u-blox Thingstream PointPerfect NTRIP.
 1. `spartn_decrypt.py` - illustrates how to read, decrypt and decode a binary SPARTN log file (e.g. from the `spartn_mqtt_client.py` or `spartn_ntrip_client.py` examples above).
 1. `rxmpmp_extract_spartn.py` - ilustrates how to extract individual SPARTN messages from the accumulated UBX-RXM-PMP data output by an NEO-D9S L-band correction receiver.
 1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from the binary SPARTN messages output by the `rxmpmp_extract_spartn.py` above.
 1. `gad_plot.py` - illustrates how to extract geographic area definitions from a series of SPARTN-GAD-1X messages - the output file from the example above can be used as an input. This example also serves to illustrate how to decrypt SPARTN messages.
 
 ---
+## <a name="troubleshooting">Troubleshooting</a>
+
+1. `SPARTNTypeError` or `SPARTNParseError` when parsing encrypted messages with 16-bit gnssTimetags (`timeTagtype=0`), e.g. GAD or some OCB messages:
+
+   ```
+   pyspartn.exceptions.SPARTNTypeError: Error processing attribute 'group' in message type SPARTN-1X-GAD
+   ```
+
+   This is almost certainly due to an invalid decryption key and/or basedate. Remember that keys are only valid for a 4 week period, and basedates are valid for no more than half a day. Note also that different GNSS constellations use different UTC datums e.g. GLONASS timestamps are based on UTC+3. Check with your SPARTN service provider for the latest decryption key(s), and check the provenence date of your SPARTN datasource.
+
+1. Checking for successful decryption. `SPARTNMessage` objects implement a protected attribute `_padding`, which represents the number of redundant bits added to the payload content in order to byte-align the payload with the number of bytes specified in the transport layer payload length attribute `nData`. If the payload has been successfully decrypted and decoded, the value of `_padding` should always be between 0 and 8. Checking `0 <= msg._padding <= 8` provides an informal (_but not necessarily definitive_) check of successful decryption and decoding (see, for example, [spartn_decrypt.py](https://github.com/semuconsulting/pyspartn/blob/main/examples/spartn_decrypt.py)).
+
+---
 ## <a name="gui">Graphical Client</a>
 
 A python/tkinter graphical GPS client which supports NMEA, UBX, RTCM3 and SPARTN protocols is available at: 
 
 [https://github.com/semuconsulting/PyGPSClient](https://github.com/semuconsulting/PyGPSClient)
 
 ---
```

### Comparing `pyspartn-0.3.1/README.md` & `pyspartn-0.3.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [Current Status](#currentstatus) |
 [Installation](#installation) |
 [Reading](#reading) |
 [Parsing](#parsing) |
 [Generating](#generating) |
 [Serializing](#serializing) |
 [Examples](#examples) |
+[Troubleshooting](#troubleshooting) |
 [Graphical Client](#gui) |
 [Author & License](#author)
 
 `pyspartn` is an original Python 3 parser for the SPARTN &copy; GPS/GNSS protocol. SPARTN is an open-source GPS/GNSS [differential correction or DGPS](https://en.wikipedia.org/wiki/Differential_GPS) protocol published by u-blox:
 
 [SPARTN Protocol](https://www.spartnformat.org/download/) (available in the public domain).
 © 2021 u-blox AG. All rights reserved.
@@ -35,19 +36,15 @@
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyspartn)
 
 The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
 
-The `SPARTNMessage` class implements decrypt and decode algorithms for OCB, HPAC and GAD message types:
- - GAD payload decryption and decode is fully tested and functional, which confirms that the global decryption mechanism and parsing algorithms are essentially correct.
- - HPAC and OCB payload decodes appear to be working OK, but results have not yet been fully validated and some individual attributes may be incorrect.
-
-*For the time being, a temporary override has been implemented in `spartnmessage.py` to suppress the `decode` flag for those payload types that cannot yet be successfully decoded. Testing contributions welcome*.
+The `SPARTNMessage` class implements optional decrypt and decode algorithms for OCB, HPAC and GAD message types (*BPAC, EAS & PROP message types are rarely used and not currently implemented*). Test coverage is currently limited by available SPARTN test data sources - additional testing contributions are welcome.
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyspartn](https://www.semuconsulting.com/pyspartn).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided. For general queries and advice, please use the [Discussion](https://github.com/semuconsulting/pyspartn/discussions) Forum.
 
@@ -104,25 +101,25 @@
 class pyspartn.spartnreader.SPARTNReader(stream, **kwargs)
 ```
 
 You can create a `SPARTNReader` object by calling the constructor with an active stream object. 
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
 or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
-Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator.
+Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator. See examples below.
 
 Example -  Serial input:
 ```python
 >>> from serial import Serial
 >>> from pyspartn import SPARTNReader
 >>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
 >>>spr = SPARTNReader(stream)
 >>> (raw_data, parsed_data) = spr.read()
 >>> print(parsed_data)
-
+...
 ```
 
 Example - File input (using iterator).
 ```python
 >>> from pyspartn import SPARTNReader
 >>> stream = open('spartndata.log', 'rb')
 >>> spr = SPARTNReader(stream)
@@ -134,63 +131,93 @@
 ```python
 >>> import socket
 >>> from pyspartn import SPARTNReader
 >>> stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
 >>> stream.connect(("localhost", 50007))
 >>> spr = SPARTNReader(stream)
 >>> for (raw_data, parsed_data) in spr: print(parsed_data)
+...
+```
+
+#### Encrypted Payloads
+
+Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now()`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
+
+The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need amending every 4 weeks.
+
+Example -  Real time serial input with decryption:
+```python
+>>> from serial import Serial
+>>> from pyspartn import SPARTNReader
+>>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
+>>>spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
+>>> (raw_data, parsed_data) = spr.read()
+>>> print(parsed_data)
+...
+```
+
+Example - Historical file input with decryption.
+```python
+>>> from datetime import datetime
+>>> from pyspartn import SPARTNReader
+>>> stream = open('spartndata.log', 'rb')
+>>> spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255))
+>>> for (raw_data, parsed_data) in spr: print(parsed_data)
+...
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
-You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. The optional `decode` keyword argument signifies whether to decrypt and decode the full payload (default = `False`). If `decode` is set to `True` and the message is encrypted (`eaf=1`), you *must* provide the following arguments:
-- `key` - the SPARTN decryption key valid at the time the message was originally created, as provided by your SPARTN service (normally 32 hexadecimal characters). 
-- `basedate` - a nominal datetime or 32-bit gnssTimeTag value, needed to convert an ambiguous 16-bit gnssTimeTag value to its unambiguous 32-bit equivalent. This is used by the decryption routine to determine the cryptographic Initialisation Vector (IV). If you're parsing messages in real time, this can default to `datetime.now()`. If you're parsing data from an older message stream, you will need to use the datetime the stream was originally created (*to the nearest half day*), or a 32-bit gnssTimeTag value from the same stream. See examples below.
+You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. If the message payload is encrypted (`eaf=1`), a decryption `key` and `basedate` must be provided. See examples below.
 
 **NB:** Once instantiated, a `SPARTNMMessage` object is immutable.
 
-Example - without payload decryption:
+Example - without payload decryption or decoding:
 
 ```python
 >>> from pyspartn import SPARTNReader
->>> msg = SPARTNReader.parse(b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad", decode=False)
+>>> transport = b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
+>>> msg = SPARTNReader.parse(transport, decode=0)
 >>> print(msg)
-<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
+<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
-Example - with payload decryption (requires key and, for messages where timeTagtype = 0, a nominal basedate for IV calculation):
+Example - with payload decryption and decoding (requires key and, for messages where `timeTagtype=0`, a nominal basedate):
 
 ```python
->>> from pyspartn import SPARTNReader
 >>> from datetime import datetime
->>> msg = SPARTNReader.parse(b'\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80', decode=True, key="6b30302427df05b4d98911ebff3a4d95", basedate=datetime(2023,6,27,22,3,0))
+>>> from pyspartn import SPARTNReader
+>>> transport = b'\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80'
+>>> msg = SPARTNReader.parse(transport, decode=1, key="6b30302427df05b4d98911ebff3a4d95", basedate=datetime(2023,6,27,22,3,0))
                                                                                
 >>> print(msg)
-<SPARTN(SPARTN-1X-GAD, msgType=2, nData=50, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=32580, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=6182016, SF005=37, SF068=1, SF069=0, SF030=7, SF031_01=32, SF032_01=1332, SF033_01=1987, SF034_01=6, SF035_01=2, SF036_01=5, SF037_01=22, SF031_02=33, SF032_02=1332, SF033_02=2033, SF034_02=6, SF035_02=3, SF036_02=5, SF037_02=16, SF031_03=34, SF032_03=1301, SF033_03=1921, SF034_03=2, SF035_03=6, SF036_03=18, SF037_03=10, SF031_04=35, SF032_04=1297, SF033_04=1987, SF034_04=3, SF035_04=3, SF036_04=12, SF037_04=22, SF031_05=36, SF032_05=1448, SF033_05=1768, SF034_05=6, SF035_05=2, SF036_05=5, SF037_05=30, SF031_06=37, SF032_06=1391, SF033_06=1745, SF034_06=4, SF035_06=7, SF036_06=7, SF037_06=10, SF031_07=38, SF032_07=1360, SF033_07=1906, SF034_07=3, SF035_07=2, SF036_07=8, SF037_07=22)>
+<SPARTN(SPARTN-1X-GAD, msgType=2, nData=50, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=32580, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=6182016, SF005=37, SF068=1, SF069=0, SF030=7, SF031_01=32, SF032_01=43.20000000000002, SF033_01=18.700000000000017, SF034_01=6, SF035_01=2, SF036_01=0.6, SF037_01=2.3000000000000003, SF031_02=33, SF032_02=43.20000000000002, SF033_02=23.30000000000001, SF034_02=6, SF035_02=3, SF036_02=0.6, SF037_02=1.7000000000000002, SF031_03=34, SF032_03=40.099999999999994, SF033_03=12.100000000000023, SF034_03=2, SF035_03=6, SF036_03=1.9000000000000001, SF037_03=1.1, SF031_04=35, SF032_04=39.70000000000002, SF033_04=18.700000000000017, SF034_04=3, SF035_04=3, SF036_04=1.3000000000000003, SF037_04=2.3000000000000003, SF031_05=36, SF032_05=54.80000000000001, SF033_05=-3.1999999999999886, SF034_05=6, SF035_05=2, SF036_05=0.6, SF037_05=3.1, SF031_06=37, SF032_06=49.099999999999994, SF033_06=-5.5, SF034_06=4, SF035_06=7, SF036_06=0.8, SF037_06=1.1, SF031_07=38, SF032_07=46.0, SF033_07=10.600000000000023, SF034_07=3, SF035_07=2, SF036_07=0.9, SF037_07=2.3000000000000003, SF031_08=39, SF032_08=46.0, SF033_08=1.8000000000000114, SF034_08=7, SF035_08=2, SF036_08=0.7000000000000001, SF037_08=2.3000000000000003)>
 ```
 
-
 The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity'. SPARTN data fields are denoted `SFnnn` - use the `datadesc()` helper method to obtain a more user-friendly text description of the data field.
 
 ```python
+>>> from datetime import datetime
 >>> from pyspartn import SPARTNReader, datadesc
->>> msg = SPARTNReader.parse(b'\x73\x03\x35\xec\x08\xc7\xd4\x20\x70\x5b\x1f\xc ... \x1e\xbe\x18\x43\x2d\x57\xe7\xa7', decode=True, key="00112233445566778899aabbccddeeff")
+>>> msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255))
 >>> print(msg)
-<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=619, eaf=1, crcType=2, frameCrc=12, msgSubtype=0, timeTagtype=1, gnssTimeTag=419070990, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=5760935, SF005=508, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=127, SF044_01=1, SF048_01=213, SF049a_01=257, SF049b_01=253, SF054_01=1, SatBitmaskLen_01=0, SF011_01=70263185, SF055_01_01=6, SF056_01_01=1, SF060_01_01=8944, ... SF061b_09_08=8287)>
+     <SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, ..., SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>
 >>> msg.identity
 'SPARTN-1X-HPAC-GPS'
 >>> msg.gnssTimeTag
-419070990
->>> msg.SF005
-508
-datadesc("SF005")
-'Solution issue of update (SIOU)'
+451165680
+>>> datadesc("SF005"), msg.SF005
+('Solution issue of update (SIOU)', 152)
+>>> datadesc("SF061a"), msg.SF061a_10_05
+('Large ionosphere coefficient C01', -0.27200000000000557)
 ```
 
+Enumerations for coded values can be found in [spartntables.py](https://github.com/semuconsulting/pyspartn/blob/main/src/pyspartn/spartntables.py).
+
 The `payload` attribute always contains the raw payload as bytes.
 
 ---
 ## <a name="generating">Generating</a>
 
 ```
 class pyspartn.spartnmessage.SPARTNMessage(**kwargs)
@@ -201,34 +228,34 @@
 
 Example:
 
 ```python
 >>> from pyspartn import SPARTNMessage
 >>> msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
 >>> print(msg)
-<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
+<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
 ---
 ## <a name="serializing">Serializing</a>
 
 The `SPARTNMessage` class implements a `serialize()` method to convert a `SPARTNMMessage` object to a bytes array suitable for writing to an output stream.
 
-e.g. to create and send a `1005` message type:
+e.g. to create and send a SPARTN-1X-OCB-GPS message type:
 
 ```python
 >>> from serial import Serial
->>> serialOut = Serial('COM7', 38400, timeout=5)
+>>> serialOut = Serial('/dev/ttyACM1', 38400, timeout=5)
 >>> from pyspartn import SPARTNMessage
 >>> msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
 >>> print(msg)
-<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
+<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 >>> output = msg.serialize()
 >>> output
-b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
+b's\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad'
 >>> serialOut.write(output)
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
@@ -239,14 +266,27 @@
 SPARTN NTRIP service e.g. u-blox Thingstream PointPerfect NTRIP.
 1. `spartn_decrypt.py` - illustrates how to read, decrypt and decode a binary SPARTN log file (e.g. from the `spartn_mqtt_client.py` or `spartn_ntrip_client.py` examples above).
 1. `rxmpmp_extract_spartn.py` - ilustrates how to extract individual SPARTN messages from the accumulated UBX-RXM-PMP data output by an NEO-D9S L-band correction receiver.
 1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from the binary SPARTN messages output by the `rxmpmp_extract_spartn.py` above.
 1. `gad_plot.py` - illustrates how to extract geographic area definitions from a series of SPARTN-GAD-1X messages - the output file from the example above can be used as an input. This example also serves to illustrate how to decrypt SPARTN messages.
 
 ---
+## <a name="troubleshooting">Troubleshooting</a>
+
+1. `SPARTNTypeError` or `SPARTNParseError` when parsing encrypted messages with 16-bit gnssTimetags (`timeTagtype=0`), e.g. GAD or some OCB messages:
+
+   ```
+   pyspartn.exceptions.SPARTNTypeError: Error processing attribute 'group' in message type SPARTN-1X-GAD
+   ```
+
+   This is almost certainly due to an invalid decryption key and/or basedate. Remember that keys are only valid for a 4 week period, and basedates are valid for no more than half a day. Note also that different GNSS constellations use different UTC datums e.g. GLONASS timestamps are based on UTC+3. Check with your SPARTN service provider for the latest decryption key(s), and check the provenence date of your SPARTN datasource.
+
+1. Checking for successful decryption. `SPARTNMessage` objects implement a protected attribute `_padding`, which represents the number of redundant bits added to the payload content in order to byte-align the payload with the number of bytes specified in the transport layer payload length attribute `nData`. If the payload has been successfully decrypted and decoded, the value of `_padding` should always be between 0 and 8. Checking `0 <= msg._padding <= 8` provides an informal (_but not necessarily definitive_) check of successful decryption and decoding (see, for example, [spartn_decrypt.py](https://github.com/semuconsulting/pyspartn/blob/main/examples/spartn_decrypt.py)).
+
+---
 ## <a name="gui">Graphical Client</a>
 
 A python/tkinter graphical GPS client which supports NMEA, UBX, RTCM3 and SPARTN protocols is available at: 
 
 [https://github.com/semuconsulting/PyGPSClient](https://github.com/semuconsulting/PyGPSClient)
 
 ---
```

### Comparing `pyspartn-0.3.1/pyproject.toml` & `pyspartn-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "pyspartn"
 authors = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 maintainers = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 description = "SPARTN protocol parser"
-version = "0.3.1"
+version = "0.3.2"
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Environment :: MacOS X",
```

### Comparing `pyspartn-0.3.1/src/pyspartn/__init__.py` & `pyspartn-0.3.2/src/pyspartn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.1/src/pyspartn/exceptions.py` & `pyspartn-0.3.2/src/pyspartn/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.1/src/pyspartn/socket_stream.py` & `pyspartn-0.3.2/src/pyspartn/socket_stream.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.1/src/pyspartn/spartnhelpers.py` & `pyspartn-0.3.2/src/pyspartn/spartnhelpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,28 +12,15 @@
 # pylint: disable=invalid-name
 
 from datetime import datetime, timedelta
 
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
 from pyspartn.exceptions import SPARTNMessageError
-from pyspartn.spartntypes_core import SPARTN_DATA_FIELDS, TIMEBASE
-
-
-def datadesc(datafield: str) -> str:
-    """
-    Get description of data field.
-
-    :param str datafield: datafield e.g. 'SF054'
-    :return: datafield description e.g. "Ionosphere equation type"
-    :rtype: str
-    """
-
-    (_, _, desc) = SPARTN_DATA_FIELDS[datafield[0:5]]
-    return desc
+from pyspartn.spartntypes_core import FL, IN, SPARTN_DATA_FIELDS, TIMEBASE
 
 
 def att2idx(att: str) -> int:
     """
     Get integer index corresponding to grouped attribute.
     e.g. SF019_04 -> 4; SF019_23 -> 23
 
@@ -60,33 +47,61 @@
 
     try:
         return att[: att.rindex("_")]
     except ValueError:
         return att
 
 
-def bitsval(bitfield: bytes, position: int, length: int) -> int:
+def datadesc(datafield: str) -> str:
+    """
+    Get description of data field.
+
+    :param str datafield: datafield e.g. 'SF054'
+    :return: datafield description e.g. "Ionosphere equation type"
+    :rtype: str
+    """
+
+    info = SPARTN_DATA_FIELDS[att2name(datafield)]
+    return info[-1]
+
+
+def bitsval(
+    bitfield: bytes,
+    position: int,
+    length: int,
+    typ: str = IN,
+    res: float = 1.0,
+    rngmin: float = 0.0,
+) -> int:
     """
     Get unisgned integer value of masked bits in bytes.
 
     :param bytes bitfield: bytes
     :param int position: position in bitfield, from leftmost bit
-    :param int length: length of masked bits
+    :param int length: length of field in bits
+    :param str typ: field type (i.e. Integer, Bitmask, Float)
+    :param float res: field resolution (i.e. scaling factor)
+    :param float rngmin: field range minimum value
     :return: value
     :rtype: int
     :raises: SPARTNMessageError if end of bitfield
     """
 
     lbb = len(bitfield) * 8
     if position + length > lbb:
         raise SPARTNMessageError(
             f"Attribute size {length} exceeds remaining payload length {lbb - position}"
         )
 
-    return int.from_bytes(bitfield, "big") >> (lbb - position - length) & 2**length - 1
+    intval = (
+        int.from_bytes(bitfield, "big") >> (lbb - position - length) & 2**length - 1
+    )
+    if typ == FL:  # float
+        return enc2float(intval, res, rngmin)
+    return intval
 
 
 def crc_poly(
     data: int, n: int, poly: int, crc: int = 0, ref_out: bool = False, xor_out: int = 0
 ) -> int:
     """
     Configurable CRC algorithm.
@@ -259,15 +274,15 @@
     secs = timetag16
     if basedate.hour >= 12:
         secs += 43200
     time16 = base16 + timedelta(seconds=secs)
     return date2timetag(time16)
 
 
-def enc2float(value: int, res: float, rngmin: float) -> float:
+def enc2float(value: int, res: float, rngmin: float = 0) -> float:
     """
     Convert encoded floating point value to float.
 
     SPARTN protocol stores floating point numbers in
     encoded integer format.
 
     :param int value: encoded value
```

### Comparing `pyspartn-0.3.1/src/pyspartn/spartnmessage.py` & `pyspartn-0.3.2/src/pyspartn/spartnmessage.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     decrypt,
     escapeall,
     timetag2date,
     valid_crc,
 )
 from pyspartn.spartntypes_core import (
     CBBMLEN,
+    FL,
     NB,
     PBBMLEN,
     SPARTN_DATA_FIELDS,
     SPARTN_MSGIDS,
     SPARTN_PRE,
     STBMLEN,
     VALCRC,
@@ -51,25 +52,23 @@
     def __init__(
         self,
         transport: bytes = None,
         validate: int = VALCRC,
         decode: bool = False,
         key: str = None,
         basedate: object = None,
-        scaling: bool = False,
     ):
         """
         Constructor.
 
         :param bytes transport: SPARTN message transport (None)
         :param bool validate: validate CRC (True)
         :param bool decode: decrypt and decode payloads (False)
         :param str key: decryption key as hexadecimal string (None)
         :param object basedate: basedate as datetime or 32-bit gnssTimeTag as integer (now)
-        :param bool scaling: apply attribute scaling factors (False)
         :raises: ParameterError if invalid parameters
         """
         # pylint: disable=too-many-arguments
 
         # object is mutable during initialisation only
         super().__setattr__("_immutable", False)
 
@@ -78,15 +77,14 @@
             raise SPARTNMessageError("Transport must be provided")
 
         self._preamble = bitsval(self._transport, 0, 8)
         if self._preamble != SPARTN_PRE:  # not SPARTN
             raise SPARTNParseError(f"Unknown message preamble {self._preamble}")
 
         self._validate = validate
-        self._scaling = scaling
         self._decode = decode
         self._padding = 0
         basedate = datetime.now() if basedate is None else basedate
         if isinstance(basedate, int):  # 32-bit gnssTimeTag
             self._basedate = timetag2date(basedate)
         else:  # datetime
             self._basedate = basedate
@@ -309,15 +307,15 @@
                 numr, nestlevel = numr.split("+")
                 for i in range(int(nestlevel)):
                     numr += f"_{index[i]:02d}"
             if numr[0:3] == NB:  # repeats = num bits set
                 rng = bin(getattr(self, numr[3:])).count("1")
             else:
                 rng = getattr(self, numr)  # repeats = attribute value
-                if numr == "SF030":
+                if numr in ("SF030", "SF071"):
                     rng += 1
 
         # recursively process each group attribute,
         # incrementing the payload offset and index as we go
         for i in range(rng):
             index[-1] = i + 1
             for key1 in gdict:
@@ -331,15 +329,15 @@
         self,
         att: object,
         offset: int,
         key: str,
         index: list,
     ) -> int:
         """
-        Set individual attribute value, applying scaling where appropriate.
+        Set individual attribute value.
 
         :param str att: attribute type string e.g. 'INT008'
         :param int offset: payload offset in bits
         :param str key: attribute keyword
         :param list index: repeating group index array
         :return: offset
         :rtype: int
@@ -349,22 +347,27 @@
         # if attribute is part of a (nested) repeating group, suffix name with index
         keyr = key
         for i in index:  # one index for each nested level
             if i > 0:
                 keyr += f"_{i:02d}"
 
         # get value of required number of bits at current payload offset
-        # (attribute length, resolution, description)
-        attlen, res, _ = SPARTN_DATA_FIELDS[key]
+        # (attribute length, resolution, minimum, description)
+        attinfo = SPARTN_DATA_FIELDS[key]
+        attlen = attinfo[0]
+        atttyp = attinfo[1]  # IN, EN, BM, FL
         if isinstance(attlen, str):  # variable length attribute
             attlen = self._getvarlen(key, index)
-        if not self._scaling:
-            res = 0
         try:
-            val = bitsval(self._payload, offset, attlen)
+            if atttyp == FL:
+                res = attinfo[2]  # resolution (i.e. scaling factor)
+                rngmin = attinfo[3]  # range minimum
+                val = bitsval(self._payload, offset, attlen, atttyp, res, rngmin)
+            else:
+                val = bitsval(self._payload, offset, attlen, atttyp)
         except SPARTNMessageError as err:
             # print(self)
             raise err
 
         setattr(self, keyr, val)
 
         offset += attlen
@@ -439,15 +442,17 @@
             elif key == "SF105":  # Galileo code bias mask
                 attl = [8, 15][sflen]
             elif key == "SF106":  # BDS code bias mask
                 attl = [8, 15][sflen]
             elif key == "SF107":  # QZSS code bias mask
                 attl = [6, 11][sflen]
         elif key == "SF079":  # Grid node present mask
-            pass  # TODO used by BPAC, not yet implemented
+            attl = (getattr(self, f"SF075{sfx}") + 1) * (
+                getattr(self, f"SF076{sfx}") + 1
+            )  # TODO used by BPAC, not yet tested
         elif key == "SF088":  # Cryptographic Key,
             attl = self.SF087
         elif key == "SF092":  # Computed Authentication Data (CAD),
             attl = self.SF091
 
         return attl
```

### Comparing `pyspartn-0.3.1/src/pyspartn/spartnreader.py` & `pyspartn-0.3.2/src/pyspartn/spartnreader.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,37 +15,57 @@
 | preamble  | framestart | payload     |  payload    | embedded   |   crc     |
 |           |            | descriptor  |             | auth data  |           |
 +===========+============+=============+=============+============+===========+
 | 8 bits    |  24 bits   | 32-64 bits  | 8-8192 bits | 0-512 bits | 8-32 bits |
 | 0x73 's'  |            |             |             |            |           |
 +-----------+------------+-------------+-------------+------------+-----------+
 
+NB Use of gnssTimeTag for message decryption:
+
+The SPARTN protocol requires a key and basedate to calculate the Initialisation
+Vector (IV) for encrypted messages (eaf=1). The key is provided by the 
+SPARTN service provider. The basedate is derived in one of two ways:
+1. For messages with unambiguous 32-bit gnssTimeTag values (timeTagtype = 1),
+the basedate is the gnssTimeTag. No other information is needed.
+2. For messages with ambiguous 16-bit gnssTimeTag values (timeTagtype = 0),
+the basedate can be derived from a 32-bit gnssTimeTag for the same message
+subtype (GPS, GLO, etc.) from the same datastream, or provided as an external
+parameter. SPARTNReader will accumulate any 32-bit gnssTimeTag in the incoming
+datastream for use in decryption.
+
+
 Created on 10 Feb 2023
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2023
 :license: BSD 3-Clause
 """
 
 # pylint: disable=invalid-name too-many-instance-attributes
 
-from datetime import datetime
+from datetime import datetime, timedelta
 from os import getenv
 from socket import socket
 
 from pyspartn.exceptions import (
     ParameterError,
     SPARTNMessageError,
     SPARTNParseError,
     SPARTNTypeError,
 )
 from pyspartn.socket_stream import SocketStream
 from pyspartn.spartnhelpers import bitsval, timetag2date, valid_crc
 from pyspartn.spartnmessage import SPARTNMessage
-from pyspartn.spartntypes_core import ERRLOG, ERRRAISE, SPARTN_PREB, VALCRC
+from pyspartn.spartntypes_core import (
+    ERRLOG,
+    ERRRAISE,
+    SPARTN_PREB,
+    TIMETAGSHIFT,
+    VALCRC,
+)
 
 
 class SPARTNReader:
     """
     SPARTNReader class.
     """
 
@@ -80,14 +100,16 @@
             self._stream = datastream
         self.key = getenv("MQTTKEY", None) if key is None else key
         self._validate = validate
         self._quitonerror = quitonerror
         self._errorhandler = errorhandler
         self._decode = decode
         self._key = key
+        # accumlated array of 32-bit gnssTimeTag from datastream
+        self._timetags = {}
         basedate = datetime.now() if basedate is None else basedate
         if isinstance(basedate, int):  # 32-bit gnssTimeTag
             self._basedate = timetag2date(basedate)
         else:  # datetime
             self._basedate = basedate
         self._basedate = (
             datetime.now() if basedate is None else basedate
@@ -168,20 +190,24 @@
         # msgType = bitsval(framestart, 0, 7)
         nData = bitsval(framestart, 7, 10)
         eaf = bitsval(framestart, 17, 1)
         crcType = bitsval(framestart, 18, 2)
         # frameCrc = bitsval(framestart, 20, 4)
 
         payDesc = self._read_bytes(4)
-        # msgSubtype = bitsval(payDesc, 0, 4)
+        # msgSubtype denotes constellation - GPS, GLO, GAL, etc.
+        msgSubtype = bitsval(payDesc, 0, 4)
         timeTagtype = bitsval(payDesc, 4, 1)
         if timeTagtype:
             payDesc += self._read_bytes(2)
         gtlen = 32 if timeTagtype else 16
-        # gnssTimeTag = bitsval(payDesc, 5, gtlen)
+        gnssTimeTag = bitsval(payDesc, 5, gtlen)
+        # store 32-bit timetag for this subtype for later use in decryption
+        if timeTagtype == 1:
+            self._timetags[msgSubtype] = gnssTimeTag
         # solutionId = bitsval(payDesc, gtlen + 5, 7)
         # solutionProcId = bitsval(payDesc, gtlen + 12, 4)
         authInd = 0
         if eaf:
             payDesc += self._read_bytes(2)
             # encryptionId = bitsval(payDesc, gtlen + 16, 4)
             # encryptionSeq = bitsval(payDesc, gtlen + 20, 6)
@@ -209,20 +235,32 @@
         # validate CRC
         core = framestart + payDesc + payload + embAuth
         raw_data = preamble + core + crcb
         if self._validate & VALCRC:
             if not valid_crc(core, crc, crcType):
                 raise SPARTNParseError(f"Invalid CRC {crc}")
 
+        # use 32-bit timetag for this subtype from datastream if available,
+        # otherwise use value provided in arguments adjusted for UTC and leap second shift
+        if isinstance(self._basedate, int):  # 32-bit gnssTimetag
+            basedate = self._timetags.get(
+                msgSubtype,
+                self._basedate + TIMETAGSHIFT.get(msgSubtype, 0),
+            )
+        else:  # datetime
+            basedate = self._timetags.get(
+                msgSubtype,
+                self._basedate + timedelta(seconds=TIMETAGSHIFT.get(msgSubtype, 0)),
+            )
         parsed_data = self.parse(
             raw_data,
             validate=self._validate,
             decode=self._decode,
             key=self._key,
-            basedate=self._basedate,
+            basedate=basedate,
         )
         return (raw_data, parsed_data)
 
     def _read_bytes(self, size: int) -> bytes:
         """
         Read a specified number of bytes from stream.
```

### Comparing `pyspartn-0.3.1/src/pyspartn/spartntypes_core.py` & `pyspartn-0.3.2/src/pyspartn/spartntypes_core.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,20 +19,36 @@
 ERRIGNORE = 0
 VALNONE = 0
 VALCRC = 1
 VALMSGID = 2
 SPARTN_PRE = 0x73
 SPARTN_PREB = b"s"
 
+# Attribute types
+IN = "IN"  # integer
+EN = "EN"  # enumeration
+BM = "BM"  # bitmask
+FL = "FL"  # float
+
 # Transient attribute names used to store variable bitmask length flags
 NB = "NB_"
 STBMLEN = "SatBitmaskLen"
 PBBMLEN = "PhaseBiasBitmaskLen"
 CBBMLEN = "CodeBiasBitmaskLen"
 
+# UTC + leap second basedate shift for different constellations
+# relative to GPS (UTC + 18 leap seconds); valid as from 2017/1/1
+TIMETAGSHIFT = {
+    0: 0,  # GPS
+    1: 10782,  # GLO = GPS + 3600 * 3 - 18
+    2: 0,  # GAL = GPS
+    3: -14,  # BEI = GPS - 14
+    4: 0,  # QZS = GPS
+}
+
 # SPARTN message types
 SPARTN_MSGIDS = {
     0: "SPARTN-1X-OCB",  # Orbit, Clock, Bias
     (0, 0): "SPARTN-1X-OCB-GPS",
     (0, 1): "SPARTN-1X-OCB-GLO",
     (0, 2): "SPARTN-1X-OCB-GAL",
     (0, 3): "SPARTN-1X-OCB-BEI",
@@ -53,125 +69,126 @@
     120: "SPARTN_1X-PROP",  # Proprietary messages
     (120, 0): "SPARTN-1X-PROP-TEST",
     (120, 1): "SPARTN-1X-PROP-UBLOX",
     (120, 2): "SPARTN-1X-PROP-SWIFT",
 }
 
 # Datafields used in message definitions
-# key: (length in bits, resolution, description)
+# key (IN, BM, EN): (length in bits, type, resolution or n/a, description)
+# key (FL): (length in bits, type, resolution, range minimum, description)
 SPARTN_DATA_FIELDS = {
-    "SF005": (9, "1", "Solution issue of update (SIOU)"),
-    "SF008": (1, "n/a", "Yaw present flag"),
-    "SF009": (1, "1", "Satellite reference datum"),
-    "SF010": (1, "n/a", "End of OCB set (EOS)"),
-    STBMLEN: (2, "n/a", "Length of satellite bitmask"),
-    "SF011": ("34 to 66", "Bitmask", "GPS Satellite mask"),
-    "SF012": ("26 to 65", "Bitmask", "GLONASS Satellite mask"),
-    "SF013": (1, "n/a", "Do not use (DNU)"),
-    "SF014O": (1, "Bitmask", "Orbit data present flag"),
-    "SF014C": (1, "Bitmask", "Clock data present flag"),
-    "SF014B": (1, "Bitmask", "Bias data present flag"),
-    "SF015": (3, "n/a", "Continuity indicator"),
-    "SF016": (2, "n/a", "GPS ephemeris type"),
-    "SF017": (2, "n/a", "GLO ephemeris type"),
-    "SF018": (8, "1", "GPS IODE"),
-    "SF019": (7, "1", "GLO IODE"),
-    "SF020R": (14, "0.002 m", "Satellite radial corrections"),
-    "SF020A": (14, "0.002 m", "Satellite along-track corrections"),
-    "SF020C": (14, "0.002 m", "Satellite cross-track corrections"),
-    "SF020CK": (14, "0.002 m", "Satellite clock corrections"),
-    "SF020PB": (14, "0.002 m", "Phase bias correction"),
-    "SF021": (6, "6°", "Satellite yaw"),
-    "SF022": (3, "n/a", "IODE continuity"),
-    "SF023": (1, "n/a", "Fix flag"),
-    "SF024": (3, "n/a", "User range error (URE)"),
-    PBBMLEN: (1, "n/a", "Length of phase bias bitmask"),
-    "SF025": ("7 or 12", "bitmask", "GPS phase bias mask"),
-    "SF026": ("6 or 10", "bitmask", "GLONASS phase bias mask"),
-    CBBMLEN: (1, "n/a", "Length of code bias bitmask"),
-    "SF027": ("7 or 12", "bitmask", "GPS code bias mask"),
-    "SF028": ("6 or 10", "bitmask", "GLONASS code bias mask"),
-    "SF029": (11, "0.02 m", "Code bias correction"),
-    "SF030": (5, "1", "Area Count"),  # NB: area count = SF030 + 1
-    "SF031": (8, "1", "Area ID"),
-    "SF032": (11, "0.1 degrees", "Area reference latitude"),
-    "SF033": (12, "0.1 degrees", "Area reference longitude"),
-    "SF034": (3, "1", "Area latitude grid node count"),
-    "SF035": (3, "1", "Area longitude grid node count"),
-    "SF036": (5, "0.1 degrees", "Area latitude grid node spacing"),
-    "SF037": (5, "0.1 degrees", "Area longitude grid node spacing"),
-    "SF039": (7, "1", "Number of grid points present"),
-    "SF040": (2, "1", "Poly/Grid block present indicator"),
-    "SF040T": (2, "1", "Troposphere Poly/Grid block present indicator"),
-    "SF040I": (2, "1", "Ionoshere Poly/Grid block present indicator"),
-    "SF041": (3, "1", "Troposphere equation type"),
-    "SF042": (3, "1", "Troposphere quality"),
-    "SF043": (8, "0.004 m", "Area average vertical hydrostatic delay"),
-    "SF044": (1, "1", "Troposphere polynomial coefficient size indicator"),
-    "SF045": (7, "0.004 m", "Small troposphere coefficient T00"),
-    "SF046a": (7, "0.001 m / degree", "Small troposphere coefficient T01"),
-    "SF046b": (7, "0.001 m / degree", "Small troposphere coefficient T10"),
-    "SF047": (9, "0.0002 m /degree2", "Small troposphere coefficient T11"),
-    "SF048": (9, "0.004 m", "Large troposphere coefficient T00"),
-    "SF049a": (9, "0.001 m / degree", "Large troposphere coefficient T01"),
-    "SF049b": (9, "0.001 m / degree", "Large troposphere coefficient T10"),
-    "SF050": (11, "0.0002 m / degree2", "Large troposphere coefficient T11"),
-    "SF051": (1, "1", "Troposphere residual field size"),
-    "SF052": (6, "0.004 m", "Small troposphere residual zenith delay"),
-    "SF053": (8, "0.004 m", "Large troposphere residual zenith delay"),
-    "SF054": (3, "1", "Ionosphere equation type"),
-    "SF055": (4, "1", "Ionosphere quality"),
-    "SF056": (1, "1", "Ionosphere polynomial coefficient size indicator"),
-    "SF057": (12, "0.04 TECU", "Small ionosphere coefficient C00"),
-    "SF058a": (12, "0.008 TECU / degree", "Small ionosphere coefficient C01"),
-    "SF058b": (12, "0.008 TECU / degree", "Small ionosphere coefficient C10"),
-    "SF059": (13, "0.002 TECU / degree2 ", "Small ionosphere coefficient C11"),
-    "SF060": (14, "0.04 TECU", "Large ionosphere coefficient C00"),
-    "SF061a": (14, "0.008 TECU / degree", "Large ionosphere coefficient C01"),
-    "SF061b": (14, "0.008 TECU / degree", "Large ionosphere coefficient C10"),
-    "SF062": (15, "0.002 TECU / degree2", "Large ionosphere coefficient C11"),
-    "SF063": (2, "1", "Ionosphere residual field size"),
-    "SF064": (4, "0.04 TECU", "Small ionosphere residual slant delay"),
-    "SF065": (7, "0.04 TECU", "Medium ionosphere residual slant delay"),
-    "SF066": (10, "0.04 TECU", "Large ionosphere residual slant delay"),
-    "SF067": (14, "0.04 TECU", "Extra-large ionosphere residual slant delay"),
-    "SF068": (4, "1", "Area Issue of Update (AIOU)"),
-    "SF069": (1, "N/A", "Reserved"),
-    "SF070": (2, "1", "Ionosphere shell height"),
-    "SF071": (2, "1", "BPAC area count"),
-    "SF072": (2, "1", "BPAC area ID"),
-    "SF073": (8, "1.0 degrees", "BPAC area reference latitude"),
-    "SF074": (9, "1.0 degrees", "BPAC area reference longitude"),
-    "SF075": (4, "1", "BPAC area latitude grid node count"),
-    "SF076": (4, "1", "BPAC area longitude grid node count"),
-    "SF077": (2, "1", "BPAC area latitude grid node spacing "),
-    "SF078": (2, "1", "BPAC area longitude grid node spacing "),
-    "SF079": ("N", "Bitmask", "Grid node present mask"),
-    "SF080": (12, "0.25 TECU", "Area average VTEC"),
-    "SF081": (1, "1", "VTEC size indicator"),
-    "SF082": (7, "0.25 TECU", "Small VTEC residual "),
-    "SF083": (11, "0.25 TECU", "Large VTEC residual "),
-    "SF084": (20, "1", "Customer Key ID"),
-    "SF085": (4, "1", "Encryption Type"),
-    "SF086": (6, "1", "Week of Applicability"),
-    "SF087": (4, "1", "Key length"),
-    "SF088": ("Key length (SF087)", "1", "Cryptographic Key"),
-    "SF089": (5, "1", "Count of Message IDs"),
-    "SF090": (4, "1", "Group Authentication Type"),
-    "SF091": (4, "1", "Computed Authentication Data (CAD) Length"),
-    "SF092": ("CAD length (SF091)", "1", "Computed Authentication Data (CAD)"),
-    "SF093": ("38 to 66", "Bitmask", "Galileo satellite mask"),
-    "SF094": ("39 to 66", "Bitmask", "BDS satellite mask"),
-    "SF095": ("12 to 66", "Bitmask", "QZSS satellite mask"),
-    "SF096": (3, "n/a", "Galileo ephemeris type"),
-    "SF097": (4, "n/a", "BDS ephemeris type"),
-    "SF098": (3, "n/a", "QZSS ephemeris type"),
-    "SF099": (10, "1", "Galileo IODnav"),
-    "SF100": (8, "1", "BDS IODE/IODC"),
-    "SF101": (8, "1", "QZSS IODE"),
-    "SF102": ("9 or 16", "Bitmask", "Galileo phase bias mask"),
-    "SF103": ("9 or 16", "Bitmask", "BDS phase bias mask"),
-    "SF104": ("7 or 12", "Bitmask", "QZSS phase bias mask"),
-    "SF105": ("9 or 16", "Bitmask", "Galileo code bias mask"),
-    "SF106": ("9 or 16", "Bitmask", "BDS code bias mask"),
-    "SF107": ("7 or 12", "Bitmask", "QZSS code bias mask"),
+    "SF005": (9, IN, 1, "Solution issue of update (SIOU)"),
+    "SF008": (1, EN, "n/a", "Yaw present flag"),
+    "SF009": (1, IN, 1, "Satellite reference datum"),
+    "SF010": (1, IN, "n/a", "End of OCB set (EOS)"),
+    STBMLEN: (2, IN, "n/a", "Length of satellite bitmask"),
+    "SF011": ("34 to 66", BM, "Bitmask", "GPS Satellite mask"),
+    "SF012": ("26 to 65", BM, "Bitmask", "GLONASS Satellite mask"),
+    "SF013": (1, IN, "n/a", "Do not use (DNU)"),
+    "SF014O": (1, BM, "Bitmask", "Orbit data present flag"),
+    "SF014C": (1, BM, "Bitmask", "Clock data present flag"),
+    "SF014B": (1, BM, "Bitmask", "Bias data present flag"),
+    "SF015": (3, IN, "n/a", "Continuity indicator"),
+    "SF016": (2, EN, "n/a", "GPS ephemeris type"),
+    "SF017": (2, EN, "n/a", "GLO ephemeris type"),
+    "SF018": (8, IN, 1, "GPS IODE"),
+    "SF019": (7, IN, 1, "GLO IODE"),
+    "SF020R": (14, FL, 0.002, -16.382, "Satellite radial corrections"),
+    "SF020A": (14, FL, 0.002, -16.382, "Satellite along-track corrections"),
+    "SF020C": (14, FL, 0.002, -16.382, "Satellite cross-track corrections"),
+    "SF020CK": (14, FL, 0.002, -16.382, "Satellite clock corrections"),
+    "SF020PB": (14, FL, 0.002, -16.382, "Phase bias correction"),
+    "SF021": (6, FL, 6, 0, "Satellite yaw"),
+    "SF022": (3, IN, "n/a", "IODE continuity"),
+    "SF023": (1, EN, "n/a", "Fix flag"),
+    "SF024": (3, IN, "n/a", "User range error (URE)"),
+    PBBMLEN: (1, IN, "n/a", "Length of phase bias bitmask"),
+    "SF025": ("7 or 12", BM, "bitmask", "GPS phase bias mask"),
+    "SF026": ("6 or 10", BM, "bitmask", "GLONASS phase bias mask"),
+    CBBMLEN: (1, IN, "n/a", "Length of code bias bitmask"),
+    "SF027": ("7 or 12", BM, "bitmask", "GPS code bias mask"),
+    "SF028": ("6 or 10", BM, "bitmask", "GLONASS code bias mask"),
+    "SF029": (11, FL, 0.02, -20.46, "Code bias correction"),
+    "SF030": (5, IN, 1, "Area Count"),  # NB: area count = SF030 + 1
+    "SF031": (8, IN, 1, "Area ID"),
+    "SF032": (11, FL, 0.1, -90, "Area reference latitude"),
+    "SF033": (12, FL, 0.1, -180, "Area reference longitude"),
+    "SF034": (3, IN, 1, "Area latitude grid node count"),
+    "SF035": (3, IN, 1, "Area longitude grid node count"),
+    "SF036": (5, FL, 0.1, 0.1, "Area latitude grid node spacing"),
+    "SF037": (5, FL, 0.1, 0.1, "Area longitude grid node spacing"),
+    "SF039": (7, IN, 1, "Number of grid points present"),
+    "SF040": (2, IN, 1, "Poly/Grid block present indicator"),
+    "SF040T": (2, IN, 1, "Troposphere Poly/Grid block present indicator"),
+    "SF040I": (2, IN, 1, "Ionoshere Poly/Grid block present indicator"),
+    "SF041": (3, EN, 1, "Troposphere equation type"),
+    "SF042": (3, IN, 1, "Troposphere quality"),
+    "SF043": (8, FL, 0.004, -0.508, "Area average vertical hydrostatic delay"),
+    "SF044": (1, IN, 1, "Troposphere polynomial coefficient size indicator"),
+    "SF045": (7, FL, 0.004, -0.252, "Small troposphere coefficient T00"),
+    "SF046a": (7, FL, 0.001, -0.063, "Small troposphere coefficient T01"),
+    "SF046b": (7, FL, 0.001, -0.063, "Small troposphere coefficient T10"),
+    "SF047": (9, FL, 0.0002, -0.0510, "Small troposphere coefficient T11"),
+    "SF048": (9, FL, 0.004, -1.020, "Large troposphere coefficient T00"),
+    "SF049a": (9, FL, 0.001, -0.255, "Large troposphere coefficient T01"),
+    "SF049b": (9, FL, 0.001, -0.255, "Large troposphere coefficient T10"),
+    "SF050": (11, FL, 0.0002, -0.2046, "Large troposphere coefficient T11"),
+    "SF051": (1, IN, 1, "Troposphere residual field size"),
+    "SF052": (6, FL, 0.004, -0.124, "Small troposphere residual zenith delay"),
+    "SF053": (8, FL, 0.004, -0.508, "Large troposphere residual zenith delay"),
+    "SF054": (3, EN, 1, "Ionosphere equation type"),
+    "SF055": (4, IN, 1, "Ionosphere quality"),
+    "SF056": (1, IN, 1, "Ionosphere polynomial coefficient size indicator"),
+    "SF057": (12, FL, 0.04, -81.88, "Small ionosphere coefficient C00"),
+    "SF058a": (12, FL, 0.008, -16.376, "Small ionosphere coefficient C01"),
+    "SF058b": (12, FL, 0.008, -16.376, "Small ionosphere coefficient C10"),
+    "SF059": (13, FL, 0.002, -8.190, "Small ionosphere coefficient C11"),
+    "SF060": (14, FL, 0.04, -327.64, "Large ionosphere coefficient C00"),
+    "SF061a": (14, FL, 0.008, -65.528, "Large ionosphere coefficient C01"),
+    "SF061b": (14, FL, 0.008, -65.528, "Large ionosphere coefficient C10"),
+    "SF062": (15, FL, 0.002, -32.766, "Large ionosphere coefficient C11"),
+    "SF063": (2, IN, 1, "Ionosphere residual field size"),
+    "SF064": (4, FL, 0.04, -0.28, "Small ionosphere residual slant delay"),
+    "SF065": (7, FL, 0.04, -2.52, "Medium ionosphere residual slant delay"),
+    "SF066": (10, FL, 0.04, -20.44, "Large ionosphere residual slant delay"),
+    "SF067": (14, FL, 0.04, -327.64, "Extra-large ionosphere residual slant delay"),
+    "SF068": (4, IN, 1, "Area Issue of Update (AIOU)"),
+    "SF069": (1, IN, "n/a", "Reserved"),
+    "SF070": (2, IN, 1, "Ionosphere shell height"),
+    "SF071": (2, IN, 1, "BPAC area count"),
+    "SF072": (2, IN, 1, "BPAC area ID"),
+    "SF073": (8, FL, 1.0, -85.0, "BPAC area reference latitude"),
+    "SF074": (9, FL, 1.0, -180.0, "BPAC area reference longitude"),
+    "SF075": (4, IN, 1, "BPAC area latitude grid node count"),
+    "SF076": (4, IN, 1, "BPAC area longitude grid node count"),
+    "SF077": (2, IN, 1, "BPAC area latitude grid node spacing "),
+    "SF078": (2, IN, 1, "BPAC area longitude grid node spacing "),
+    "SF079": ("N", BM, "Bitmask", "Grid node present mask"),
+    "SF080": (12, FL, 0.25, -511.75, "Area average VTEC"),
+    "SF081": (1, IN, 1, "VTEC size indicator"),
+    "SF082": (7, FL, 0.25, -15.75, "Small VTEC residual "),
+    "SF083": (11, FL, 0.25, -255.75, "Large VTEC residual "),
+    "SF084": (20, IN, 1, "Customer Key ID"),
+    "SF085": (4, EN, 1, "Encryption Type"),
+    "SF086": (6, IN, 1, "Week of Applicability"),
+    "SF087": (4, IN, 1, "Key length"),
+    "SF088": ("Key length (SF087)", IN, "1", "Cryptographic Key"),
+    "SF089": (5, IN, 1, "Count of Message IDs"),
+    "SF090": (4, EN, 1, "Group Authentication Type"),
+    "SF091": (4, IN, 1, "Computed Authentication Data (CAD) Length"),
+    "SF092": ("CAD length (SF091)", IN, 1, "Computed Authentication Data (CAD)"),
+    "SF093": ("38 to 66", BM, "Bitmask", "Galileo satellite mask"),
+    "SF094": ("39 to 66", BM, "Bitmask", "BDS satellite mask"),
+    "SF095": ("12 to 66", BM, "Bitmask", "QZSS satellite mask"),
+    "SF096": (3, EN, "n/a", "Galileo ephemeris type"),
+    "SF097": (4, EN, "n/a", "BDS ephemeris type"),
+    "SF098": (3, EN, "n/a", "QZSS ephemeris type"),
+    "SF099": (10, IN, 1, "Galileo IODnav"),
+    "SF100": (8, IN, 1, "BDS IODE/IODC"),
+    "SF101": (8, IN, 1, "QZSS IODE"),
+    "SF102": ("9 or 16", BM, "Bitmask", "Galileo phase bias mask"),
+    "SF103": ("9 or 16", BM, "Bitmask", "BDS phase bias mask"),
+    "SF104": ("7 or 12", BM, "Bitmask", "QZSS phase bias mask"),
+    "SF105": ("9 or 16", BM, "Bitmask", "Galileo code bias mask"),
+    "SF106": ("9 or 16", BM, "Bitmask", "BDS code bias mask"),
+    "SF107": ("7 or 12", BM, "Bitmask", "QZSS code bias mask"),
 }
```

### Comparing `pyspartn-0.3.1/src/pyspartn/spartntypes_get.py` & `pyspartn-0.3.2/src/pyspartn/spartntypes_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -599,17 +599,55 @@
                 "SF035": "Area longitude grid node count",
                 "SF036": "Area latitude grid node spacing",
                 "SF037": "Area longitude grid node spacing",
             },
         ),
     },
     # ********************************************************************
-    # BPAC
+    # BPAC TODO not yet tested - no available test data source
     # ********************************************************************
-    "SPARTN-1X-BPAC": {},  # TODO
+    "SPARTN-1X-BPAC": {
+        "SF005": "Solution issue of updated (SIOU)",
+        "SF069": "Reserved",
+        "SF070": "Ionosphere shell height",
+        "SF071": "BPAC area count",  # NB: N - 1
+        "groupBPAC": (  # repeating group * (SF071 + 1)
+            "SF071",
+            {
+                "SF072": "BPAC area ID",
+                "SF073": "BPAC area reference latitude",
+                "SF074": "BPAC area reference longitude",
+                "SF075": "BPAC area latitude grid node count",  # NB: N - 1
+                "SF076": "BPAC area longitude grid node count",  # NB: N - 1
+                "SF077": "BPAC area latitude grid node spacing",
+                "SF078": "BPAC area longitude grid node spacing",
+                "SF080": "Average area VTEC",
+                "SF079": "Grid node present mask",  # len = (SF075 + 1) * (SF076 + 1)
+                "groupVTEC": (
+                    NB + "SF079+1",  # repeating group
+                    {
+                        "SF055": "VTEC quality",
+                        "SF081": "VTEC size indicator",
+                        "optSF081-0": (
+                            ("SF081+2", 0),  # if SF081 = 0
+                            {
+                                "SF082": "Small VTEC residual",
+                            },
+                        ),
+                        "optSF081-1": (
+                            ("SF081+2", 1),  # if SF081 = 1
+                            {
+                                "SF083": "Large VTEC residual",
+                            },
+                        ),
+                    },
+                ),
+            },
+        ),
+    },
     # ********************************************************************
     # EAS-DYN
     # ********************************************************************
     "SPARTN-1X-EAS-DYN": {},  # TODO
     # ********************************************************************
     # EAS-GRP deprecated
     # ********************************************************************
```

### Comparing `pyspartn-0.3.1/src/pyspartn.egg-info/PKG-INFO` & `pyspartn-0.3.2/src/pyspartn.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspartn
-Version: 0.3.1
+Version: 0.3.2
 Summary: SPARTN protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2023, SEMU Consulting
         All rights reserved.
@@ -77,14 +77,15 @@
 [Current Status](#currentstatus) |
 [Installation](#installation) |
 [Reading](#reading) |
 [Parsing](#parsing) |
 [Generating](#generating) |
 [Serializing](#serializing) |
 [Examples](#examples) |
+[Troubleshooting](#troubleshooting) |
 [Graphical Client](#gui) |
 [Author & License](#author)
 
 `pyspartn` is an original Python 3 parser for the SPARTN &copy; GPS/GNSS protocol. SPARTN is an open-source GPS/GNSS [differential correction or DGPS](https://en.wikipedia.org/wiki/Differential_GPS) protocol published by u-blox:
 
 [SPARTN Protocol](https://www.spartnformat.org/download/) (available in the public domain).
 © 2021 u-blox AG. All rights reserved.
@@ -109,19 +110,15 @@
 ![Release Date](https://img.shields.io/github/release-date-pre/semuconsulting/pyspartn)
 ![Last Commit](https://img.shields.io/github/last-commit/semuconsulting/pyspartn)
 ![Contributors](https://img.shields.io/github/contributors/semuconsulting/pyspartn.svg)
 ![Open Issues](https://img.shields.io/github/issues-raw/semuconsulting/pyspartn)
 
 The `SPARTNReader` class is fully functional and is capable of parsing individual SPARTN transport-layer messages from a binary data stream containing *solely* SPARTN data, with their associated metadata (message type/subtype, payload length, encryption parameters, etc.).
 
-The `SPARTNMessage` class implements decrypt and decode algorithms for OCB, HPAC and GAD message types:
- - GAD payload decryption and decode is fully tested and functional, which confirms that the global decryption mechanism and parsing algorithms are essentially correct.
- - HPAC and OCB payload decodes appear to be working OK, but results have not yet been fully validated and some individual attributes may be incorrect.
-
-*For the time being, a temporary override has been implemented in `spartnmessage.py` to suppress the `decode` flag for those payload types that cannot yet be successfully decoded. Testing contributions welcome*.
+The `SPARTNMessage` class implements optional decrypt and decode algorithms for OCB, HPAC and GAD message types (*BPAC, EAS & PROP message types are rarely used and not currently implemented*). Test coverage is currently limited by available SPARTN test data sources - additional testing contributions are welcome.
 
 Sphinx API Documentation in HTML format is available at [https://www.semuconsulting.com/pyspartn](https://www.semuconsulting.com/pyspartn).
 
 Contributions welcome - please refer to [CONTRIBUTING.MD](https://github.com/semuconsulting/pyspartn/blob/master/CONTRIBUTING.md).
 
 [Bug reports](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/bug_report.md) and [Feature requests](https://github.com/semuconsulting/pyspartn/blob/master/.github/ISSUE_TEMPLATE/feature_request.md) - please use the templates provided. For general queries and advice, please use the [Discussion](https://github.com/semuconsulting/pyspartn/discussions) Forum.
 
@@ -178,25 +175,25 @@
 class pyspartn.spartnreader.SPARTNReader(stream, **kwargs)
 ```
 
 You can create a `SPARTNReader` object by calling the constructor with an active stream object. 
 The stream object can be any data stream which supports a `read(n) -> bytes` method (e.g. File or Serial, with 
 or without a buffer wrapper). `pyspartn` implements an internal `SocketStream` class to allow sockets to be read in the same way as other streams (see example below).
 
-Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator.
+Individual SPARTN messages can then be read using the `SPARTNReader.read()` function, which returns both the raw binary data (as bytes) and the parsed data (as a `SPARTNMessage`, via the `parse()` method). The function is thread-safe in so far as the incoming data stream object is thread-safe. `SPARTNReader` also implements an iterator. See examples below.
 
 Example -  Serial input:
 ```python
 >>> from serial import Serial
 >>> from pyspartn import SPARTNReader
 >>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
 >>>spr = SPARTNReader(stream)
 >>> (raw_data, parsed_data) = spr.read()
 >>> print(parsed_data)
-
+...
 ```
 
 Example - File input (using iterator).
 ```python
 >>> from pyspartn import SPARTNReader
 >>> stream = open('spartndata.log', 'rb')
 >>> spr = SPARTNReader(stream)
@@ -208,63 +205,93 @@
 ```python
 >>> import socket
 >>> from pyspartn import SPARTNReader
 >>> stream = socket.socket(socket.AF_INET, socket.SOCK_STREAM):
 >>> stream.connect(("localhost", 50007))
 >>> spr = SPARTNReader(stream)
 >>> for (raw_data, parsed_data) in spr: print(parsed_data)
+...
+```
+
+#### Encrypted Payloads
+
+Some proprietary SPARTN message sources (e.g. Thingstream PointPerfect © MQTT) use encrypted payloads (`eaf=1`). In order to decrypt and decode these payloads, the user must set `decode=1` and provide a valid decryption `key`. Keys are typically 32-character hexadecimal strings valid for a 4 week period. If the datastream contains messages with ambiguous 16-bit gnssTimetags (`timeTagtype=0`) - which generally includes all GAD messages and some OCB messages - a nominal `basedate` is also required, representing the date on which the datastream was originally created to the nearest half day. If you're parsing data in real time, this can be left at the default `datetime.now()`. If you're parsing historical data, you will need to provide a basedate representing the date on which the datastream was originally created to the nearest half day. See examples below.
+
+The current decryption key can also be set via environment variable `MQTTKEY`, but bear in mind this will need amending every 4 weeks.
+
+Example -  Real time serial input with decryption:
+```python
+>>> from serial import Serial
+>>> from pyspartn import SPARTNReader
+>>> stream = Serial('/dev/tty.usbmodem14101', 9600, timeout=3)
+>>>spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc")
+>>> (raw_data, parsed_data) = spr.read()
+>>> print(parsed_data)
+...
+```
+
+Example - Historical file input with decryption.
+```python
+>>> from datetime import datetime
+>>> from pyspartn import SPARTNReader
+>>> stream = open('spartndata.log', 'rb')
+>>> spr = SPARTNReader(stream, decode=1, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2023, 4, 18, 20, 48, 29, 977255))
+>>> for (raw_data, parsed_data) in spr: print(parsed_data)
+...
 ```
 
 ---
 ## <a name="parsing">Parsing</a>
 
-You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. The optional `decode` keyword argument signifies whether to decrypt and decode the full payload (default = `False`). If `decode` is set to `True` and the message is encrypted (`eaf=1`), you *must* provide the following arguments:
-- `key` - the SPARTN decryption key valid at the time the message was originally created, as provided by your SPARTN service (normally 32 hexadecimal characters). 
-- `basedate` - a nominal datetime or 32-bit gnssTimeTag value, needed to convert an ambiguous 16-bit gnssTimeTag value to its unambiguous 32-bit equivalent. This is used by the decryption routine to determine the cryptographic Initialisation Vector (IV). If you're parsing messages in real time, this can default to `datetime.now()`. If you're parsing data from an older message stream, you will need to use the datetime the stream was originally created (*to the nearest half day*), or a 32-bit gnssTimeTag value from the same stream. See examples below.
+You can parse individual SPARTN messages using the static `SPARTNReader.parse(data)` function, which takes a bytes array containing a binary SPARTN message and returns a `SPARTNMessage` object. If the message payload is encrypted (`eaf=1`), a decryption `key` and `basedate` must be provided. See examples below.
 
 **NB:** Once instantiated, a `SPARTNMMessage` object is immutable.
 
-Example - without payload decryption:
+Example - without payload decryption or decoding:
 
 ```python
 >>> from pyspartn import SPARTNReader
->>> msg = SPARTNReader.parse(b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad", decode=False)
+>>> transport = b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
+>>> msg = SPARTNReader.parse(transport, decode=0)
 >>> print(msg)
-<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
+<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
-Example - with payload decryption (requires key and, for messages where timeTagtype = 0, a nominal basedate for IV calculation):
+Example - with payload decryption and decoding (requires key and, for messages where `timeTagtype=0`, a nominal basedate):
 
 ```python
->>> from pyspartn import SPARTNReader
 >>> from datetime import datetime
->>> msg = SPARTNReader.parse(b'\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80', decode=True, key="6b30302427df05b4d98911ebff3a4d95", basedate=datetime(2023,6,27,22,3,0))
+>>> from pyspartn import SPARTNReader
+>>> transport = b'\x73\x04\x19\x62\x03\xfa\x20\x5b\x1f\xc8\x31\x0b\x03\xd3\xa4\xb1\xdb\x79\x21\xcb\x5c\x27\x12\xa7\xa8\xc2\x52\xfd\x4a\xfb\x1a\x96\x3b\x64\x2a\x4e\xcd\x86\xbb\x31\x7c\x61\xde\xf5\xdb\x3d\xa3\x2c\x65\xd5\x05\x9f\x1c\xd9\x96\x47\x3b\xca\x13\x5e\x5e\x54\x80'
+>>> msg = SPARTNReader.parse(transport, decode=1, key="6b30302427df05b4d98911ebff3a4d95", basedate=datetime(2023,6,27,22,3,0))
                                                                                
 >>> print(msg)
-<SPARTN(SPARTN-1X-GAD, msgType=2, nData=50, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=32580, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=6182016, SF005=37, SF068=1, SF069=0, SF030=7, SF031_01=32, SF032_01=1332, SF033_01=1987, SF034_01=6, SF035_01=2, SF036_01=5, SF037_01=22, SF031_02=33, SF032_02=1332, SF033_02=2033, SF034_02=6, SF035_02=3, SF036_02=5, SF037_02=16, SF031_03=34, SF032_03=1301, SF033_03=1921, SF034_03=2, SF035_03=6, SF036_03=18, SF037_03=10, SF031_04=35, SF032_04=1297, SF033_04=1987, SF034_04=3, SF035_04=3, SF036_04=12, SF037_04=22, SF031_05=36, SF032_05=1448, SF033_05=1768, SF034_05=6, SF035_05=2, SF036_05=5, SF037_05=30, SF031_06=37, SF032_06=1391, SF033_06=1745, SF034_06=4, SF035_06=7, SF036_06=7, SF037_06=10, SF031_07=38, SF032_07=1360, SF033_07=1906, SF034_07=3, SF035_07=2, SF036_07=8, SF037_07=22)>
+<SPARTN(SPARTN-1X-GAD, msgType=2, nData=50, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=32580, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=6182016, SF005=37, SF068=1, SF069=0, SF030=7, SF031_01=32, SF032_01=43.20000000000002, SF033_01=18.700000000000017, SF034_01=6, SF035_01=2, SF036_01=0.6, SF037_01=2.3000000000000003, SF031_02=33, SF032_02=43.20000000000002, SF033_02=23.30000000000001, SF034_02=6, SF035_02=3, SF036_02=0.6, SF037_02=1.7000000000000002, SF031_03=34, SF032_03=40.099999999999994, SF033_03=12.100000000000023, SF034_03=2, SF035_03=6, SF036_03=1.9000000000000001, SF037_03=1.1, SF031_04=35, SF032_04=39.70000000000002, SF033_04=18.700000000000017, SF034_04=3, SF035_04=3, SF036_04=1.3000000000000003, SF037_04=2.3000000000000003, SF031_05=36, SF032_05=54.80000000000001, SF033_05=-3.1999999999999886, SF034_05=6, SF035_05=2, SF036_05=0.6, SF037_05=3.1, SF031_06=37, SF032_06=49.099999999999994, SF033_06=-5.5, SF034_06=4, SF035_06=7, SF036_06=0.8, SF037_06=1.1, SF031_07=38, SF032_07=46.0, SF033_07=10.600000000000023, SF034_07=3, SF035_07=2, SF036_07=0.9, SF037_07=2.3000000000000003, SF031_08=39, SF032_08=46.0, SF033_08=1.8000000000000114, SF034_08=7, SF035_08=2, SF036_08=0.7000000000000001, SF037_08=2.3000000000000003)>
 ```
 
-
 The `SPARTNMessage` object exposes different public attributes depending on its message type or 'identity'. SPARTN data fields are denoted `SFnnn` - use the `datadesc()` helper method to obtain a more user-friendly text description of the data field.
 
 ```python
+>>> from datetime import datetime
 >>> from pyspartn import SPARTNReader, datadesc
->>> msg = SPARTNReader.parse(b'\x73\x03\x35\xec\x08\xc7\xd4\x20\x70\x5b\x1f\xc ... \x1e\xbe\x18\x43\x2d\x57\xe7\xa7', decode=True, key="00112233445566778899aabbccddeeff")
+>>> msg = SPARTNReader.parse(b"s\x02\xf7\xeb\x08\xd7!\xef\x80[\x17\x88\xc2?\x0f\x ... \xc4#fFy\xb9\xd5", decode=True, key="930d847b779b126863c8b3b2766ae7cc", basedate=datetime(2024, 4, 18, 20, 48, 29, 977255))
 >>> print(msg)
-<SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=619, eaf=1, crcType=2, frameCrc=12, msgSubtype=0, timeTagtype=1, gnssTimeTag=419070990, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=63, authInd=1, embAuthLen=0, crc=5760935, SF005=508, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=2, SF043_01=127, SF044_01=1, SF048_01=213, SF049a_01=257, SF049b_01=253, SF054_01=1, SatBitmaskLen_01=0, SF011_01=70263185, SF055_01_01=6, SF056_01_01=1, SF060_01_01=8944, ... SF061b_09_08=8287)>
+     <SPARTN(SPARTN-1X-HPAC-GPS, msgType=1, nData=495, eaf=1, crcType=2, frameCrc=11, msgSubtype=0, timeTagtype=1, gnssTimeTag=451165680, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=30, authInd=1, embAuthLen=0, crc=7977429, SF005=152, SF068=1, SF069=0, SF030=9, SF031_01=0, SF039_01=0, SF040T_01=1, SF040I_01=1, SF041_01=1, SF042_01=1, SF043_01=0.0, SF044_01=1, SF048_01=-0.21199999999999997, SF049a_01=0.0, SF049b_01=0.0010000000000000009, SF054_01=1, SatBitmaskLen_01=0, SF011_01=880836738, SF055_01_01=1, SF056_01_01=1, SF060_01_01=-11.120000000000005, ..., SF061a_10_05=-0.27200000000000557, SF061b_10_05=0.1839999999999975, SF055_10_06=2, SF056_10_06=1, SF060_10_06=7.640000000000043, SF061a_10_06=-1.3840000000000003, SF061b_10_06=-0.7920000000000016)>
 >>> msg.identity
 'SPARTN-1X-HPAC-GPS'
 >>> msg.gnssTimeTag
-419070990
->>> msg.SF005
-508
-datadesc("SF005")
-'Solution issue of update (SIOU)'
+451165680
+>>> datadesc("SF005"), msg.SF005
+('Solution issue of update (SIOU)', 152)
+>>> datadesc("SF061a"), msg.SF061a_10_05
+('Large ionosphere coefficient C01', -0.27200000000000557)
 ```
 
+Enumerations for coded values can be found in [spartntables.py](https://github.com/semuconsulting/pyspartn/blob/main/src/pyspartn/spartntables.py).
+
 The `payload` attribute always contains the raw payload as bytes.
 
 ---
 ## <a name="generating">Generating</a>
 
 ```
 class pyspartn.spartnmessage.SPARTNMessage(**kwargs)
@@ -275,34 +302,34 @@
 
 Example:
 
 ```python
 >>> from pyspartn import SPARTNMessage
 >>> msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
 >>> print(msg)
-<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
+<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 ```
 
 ---
 ## <a name="serializing">Serializing</a>
 
 The `SPARTNMessage` class implements a `serialize()` method to convert a `SPARTNMMessage` object to a bytes array suitable for writing to an output stream.
 
-e.g. to create and send a `1005` message type:
+e.g. to create and send a SPARTN-1X-OCB-GPS message type:
 
 ```python
 >>> from serial import Serial
->>> serialOut = Serial('COM7', 38400, timeout=5)
+>>> serialOut = Serial('/dev/ttyACM1', 38400, timeout=5)
 >>> from pyspartn import SPARTNMessage
 >>> msg = SPARTNMessage(transport=b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad")
 >>> print(msg)
-<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, msgSubtype=0, nData=37, eaf=1, crcType=2, frameCrc=2, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11)>
+<SPARTN(SPARTN-1X-OCB-GPS, msgType=0, nData=37, eaf=1, crcType=2, frameCrc=2, msgSubtype=0, timeTagtype=0, gnssTimeTag=3970, solutionId=5, solutionProcId=11, encryptionId=1, encryptionSeq=9, authInd=1, embAuthLen=0, crc=7627181, )>
 >>> output = msg.serialize()
 >>> output
-b"s\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad"
+b's\x00\x12\xe2\x00|\x10[\x12H\xf5\t\xa0\xb4+\x99\x02\x15\xe2\x05\x85\xb7\x83\xc5\xfd\x0f\xfe\xdf\x18\xbe\x7fv \xc3`\x82\x98\x10\x07\xdc\xeb\x82\x7f\xcf\xf8\x9e\xa3ta\xad'
 >>> serialOut.write(output)
 ```
 
 ---
 ## <a name="examples">Examples</a>
 
 The following examples are available in the /examples folder:
@@ -313,14 +340,27 @@
 SPARTN NTRIP service e.g. u-blox Thingstream PointPerfect NTRIP.
 1. `spartn_decrypt.py` - illustrates how to read, decrypt and decode a binary SPARTN log file (e.g. from the `spartn_mqtt_client.py` or `spartn_ntrip_client.py` examples above).
 1. `rxmpmp_extract_spartn.py` - ilustrates how to extract individual SPARTN messages from the accumulated UBX-RXM-PMP data output by an NEO-D9S L-band correction receiver.
 1. `spartnparser.py` - illustrates how to parse SPARTN transport layer data from the binary SPARTN messages output by the `rxmpmp_extract_spartn.py` above.
 1. `gad_plot.py` - illustrates how to extract geographic area definitions from a series of SPARTN-GAD-1X messages - the output file from the example above can be used as an input. This example also serves to illustrate how to decrypt SPARTN messages.
 
 ---
+## <a name="troubleshooting">Troubleshooting</a>
+
+1. `SPARTNTypeError` or `SPARTNParseError` when parsing encrypted messages with 16-bit gnssTimetags (`timeTagtype=0`), e.g. GAD or some OCB messages:
+
+   ```
+   pyspartn.exceptions.SPARTNTypeError: Error processing attribute 'group' in message type SPARTN-1X-GAD
+   ```
+
+   This is almost certainly due to an invalid decryption key and/or basedate. Remember that keys are only valid for a 4 week period, and basedates are valid for no more than half a day. Note also that different GNSS constellations use different UTC datums e.g. GLONASS timestamps are based on UTC+3. Check with your SPARTN service provider for the latest decryption key(s), and check the provenence date of your SPARTN datasource.
+
+1. Checking for successful decryption. `SPARTNMessage` objects implement a protected attribute `_padding`, which represents the number of redundant bits added to the payload content in order to byte-align the payload with the number of bytes specified in the transport layer payload length attribute `nData`. If the payload has been successfully decrypted and decoded, the value of `_padding` should always be between 0 and 8. Checking `0 <= msg._padding <= 8` provides an informal (_but not necessarily definitive_) check of successful decryption and decoding (see, for example, [spartn_decrypt.py](https://github.com/semuconsulting/pyspartn/blob/main/examples/spartn_decrypt.py)).
+
+---
 ## <a name="gui">Graphical Client</a>
 
 A python/tkinter graphical GPS client which supports NMEA, UBX, RTCM3 and SPARTN protocols is available at: 
 
 [https://github.com/semuconsulting/PyGPSClient](https://github.com/semuconsulting/PyGPSClient)
 
 ---
```

### Comparing `pyspartn-0.3.1/src/pyspartn.egg-info/SOURCES.txt` & `pyspartn-0.3.2/src/pyspartn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.1/tests/test_socket.py` & `pyspartn-0.3.2/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyspartn-0.3.1/tests/test_static.py` & `pyspartn-0.3.2/tests/test_static.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,14 +23,46 @@
     decrypt,
     enc2float,
     encrypt,
     escapeall,
     timetag2date,
     valid_crc,
 )
+from pyspartn.spartntypes_core import SPARTN_DATA_FIELDS, FL
+from pyspartn.spartntables import (
+    SF015_ENUM,
+    SF022_ENUM,
+    SF024_ENUM,
+    SF042_ENUM,
+    SF044_ENUM,
+    SF051_ENUM,
+    SF055_ENUM,
+    SF056_ENUM,
+    SF063_ENUM,
+    SF070_ENUM,
+    SF077_ENUM,
+    SF078_ENUM,
+    SF081_ENUM,
+    SF085_ENUM,
+    SF087_ENUM,
+    SF090_ENUM,
+    SF091_ENUM,
+    SF093_ENUM,
+    SF094_ENUM,
+    SF095_ENUM,
+    SF096_ENUM,
+    SF097_ENUM,
+    SF098_ENUM,
+    SF102_ENUM,
+    SF103_ENUM,
+    SF104_ENUM,
+    SF105_ENUM,
+    SF106_ENUM,
+    SF107_ENUM,
+)
 
 
 class StaticTest(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
         dirname = os.path.dirname(__file__)
 
@@ -42,14 +74,24 @@
         EXPECTED_RESULT = [1, 8, 3, 15]
 
         bm = b"\x01\x08\x03\xf0\xff"
         for i, (ps, ln) in enumerate(bits):
             res = bitsval(bm, ps, ln)
             self.assertEqual(res, EXPECTED_RESULT[i])
 
+    def testbitsval2(self):
+        bits = [(7, 1), (8, 8), (22, 2), (24, 4)]
+        EXPECTED_RESULT = [-0.5, 3.0, 0.5, 6.5]
+
+        bm = b"\x01\x08\x03\xf0\xff"
+        for i, (ps, ln) in enumerate(bits):
+            res = bitsval(bm, ps, ln, "FL", 0.5, -1.0)
+            # print(res)
+            self.assertEqual(res, EXPECTED_RESULT[i])
+
     def testbitsvalerr(self):
         EXPECTED_ERROR = "Attribute size 16 exceeds remaining payload length 2"
         bm = b"\x01\x08\x03\xf0\xff"
         # print(f"Length bitfield = {len(bm) * 8}")
         with self.assertRaisesRegex(SPARTNMessageError, EXPECTED_ERROR):
             res = bitsval(bm, 38, 16)
 
@@ -160,14 +202,16 @@
             self.assertEqual(res, EXPECTED_RESULT[i])
 
     def testdatadesc(self):  # test datadesc
         res = datadesc("SF054")
         self.assertEqual(res, "Ionosphere equation type")
         res = datadesc("SF043_01")
         self.assertEqual(res, "Area average vertical hydrostatic delay")
+        res = datadesc("SF049a")
+        self.assertEqual(res, "Large troposphere coefficient T01")
 
     def testenc2float(self):  # test enc2float
         res = enc2float(1332, 0.1, -90)
         self.assertAlmostEqual(res, 43.20000000000002, 6)
         res = enc2float(2033, 0.1, -180)
         self.assertAlmostEqual(res, 23.30000000000001, 6)
 
@@ -175,11 +219,55 @@
         res = timetag2date(425595780)
         self.assertEqual(res, datetime(2023, 6, 27, 21, 3, 0))
 
     def testdate2timetag(self):  # test date2timetag
         res = date2timetag(datetime(2023, 6, 27, 21, 3, 0))
         self.assertEqual(res, 425595780)
 
+    def testdatafields(self):  # check float datafields are correctly configured
+        for _, value in SPARTN_DATA_FIELDS.items():
+            if value[1] == FL:
+                self.assertTrue(
+                    isinstance(value[3], (int, float))
+                    and isinstance(value[2], (int, float))
+                )
+
+    def testtables(self):  # sanity check on lookup tables
+        i = 0
+        for tbl in (
+            SF015_ENUM,
+            SF022_ENUM,
+            SF024_ENUM,
+            SF042_ENUM,
+            SF044_ENUM,
+            SF051_ENUM,
+            SF055_ENUM,
+            SF056_ENUM,
+            SF063_ENUM,
+            SF070_ENUM,
+            SF077_ENUM,
+            SF078_ENUM,
+            SF081_ENUM,
+            SF085_ENUM,
+            SF087_ENUM,
+            SF090_ENUM,
+            SF091_ENUM,
+            SF093_ENUM,
+            SF094_ENUM,
+            SF095_ENUM,
+            SF096_ENUM,
+            SF097_ENUM,
+            SF098_ENUM,
+            SF102_ENUM,
+            SF103_ENUM,
+            SF104_ENUM,
+            SF105_ENUM,
+            SF106_ENUM,
+            SF107_ENUM,
+        ):
+            i += len(tbl)
+        self.assertEqual(i, 141)
+
 
 if __name__ == "__main__":
     # import sys;sys.argv = ['', 'Test.testName']
     unittest.main()
```

