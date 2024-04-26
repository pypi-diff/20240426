# Comparing `tmp/gllogger-0.0.6.tar.gz` & `tmp/gllogger-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gllogger-0.0.6.tar", last modified: Fri Apr 26 11:39:23 2024, max compression
+gzip compressed data, was "gllogger-0.0.7.tar", last modified: Fri Apr 26 11:49:13 2024, max compression
```

## Comparing `gllogger-0.0.6.tar` & `gllogger-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:39:23.162022 gllogger-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-26 11:39:23.162022 gllogger-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-26 11:39:18.000000 gllogger-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-26 11:39:18.000000 gllogger-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:39:23.162022 gllogger-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:39:23.162022 gllogger-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:39:23.162022 gllogger-0.0.6/src/gllogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-26 11:39:23.000000 gllogger-0.0.6/src/gllogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 11:39:23.000000 gllogger-0.0.6/src/gllogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:39:23.000000 gllogger-0.0.6/src/gllogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 11:39:23.000000 gllogger-0.0.6/src/gllogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 11:39:23.000000 gllogger-0.0.6/src/gllogger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20134 2024-04-26 11:39:18.000000 gllogger-0.0.6/src/gllogger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:39:23.162022 gllogger-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 11:39:18.000000 gllogger-0.0.6/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:49:13.523367 gllogger-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-26 11:49:13.523367 gllogger-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-26 11:49:09.000000 gllogger-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-26 11:49:09.000000 gllogger-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 11:49:13.523367 gllogger-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:49:13.519367 gllogger-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:49:13.519367 gllogger-0.0.7/src/gllogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-26 11:49:13.000000 gllogger-0.0.7/src/gllogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 11:49:13.000000 gllogger-0.0.7/src/gllogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 11:49:13.000000 gllogger-0.0.7/src/gllogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 11:49:13.000000 gllogger-0.0.7/src/gllogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 11:49:13.000000 gllogger-0.0.7/src/gllogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20139 2024-04-26 11:49:09.000000 gllogger-0.0.7/src/gllogger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 11:49:13.519367 gllogger-0.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 11:49:09.000000 gllogger-0.0.7/test/test.py
```

### Comparing `gllogger-0.0.6/PKG-INFO` & `gllogger-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: gllogger
-Version: 0.0.6
+Version: 0.0.7
 Summary: gllogger
 Author-email: calm51 <calm51@protonmail.com>
-Project-URL: Homepage, https://github.com/calm510/gllogger
-Project-URL: Issues, https://github.com/calm510/gllogger/issues
+Project-URL: Homepage, https://github.com/calm51/gllogger
+Project-URL: Issues, https://github.com/calm51/gllogger/issues
 Keywords: logger,global logger,logger hook,easy logger
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: better_exceptions
 
+> pip install gllogger
 ```python3
 # NOTE: You should import gllogger before executing any other code.
 from gllogger import gL
 
+gL.setLoggerClass(__name__)
 gL.setGlobalLevel(logging.DEBUG)
-if gL.getLogger(__name__).name == "__main__":
-    gL.setLoggerClass()
 
 ...
 ```
 
 ```python3
 # You can log into the console,
 gL.getLogger(__name__).init(gL.OT_console)
```

### Comparing `gllogger-0.0.6/README.md` & `gllogger-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,85 +1,84 @@
-00000000: 6060 6070 7974 686f 6e33 0a23 204e 4f54  ```python3.# NOT
-00000010: 453a 2059 6f75 2073 686f 756c 6420 696d  E: You should im
-00000020: 706f 7274 2067 6c6c 6f67 6765 7220 6265  port gllogger be
-00000030: 666f 7265 2065 7865 6375 7469 6e67 2061  fore executing a
-00000040: 6e79 206f 7468 6572 2063 6f64 652e 0a66  ny other code..f
-00000050: 726f 6d20 676c 6c6f 6767 6572 2069 6d70  rom gllogger imp
-00000060: 6f72 7420 674c 0a0a 674c 2e73 6574 476c  ort gL..gL.setGl
-00000070: 6f62 616c 4c65 7665 6c28 6c6f 6767 696e  obalLevel(loggin
-00000080: 672e 4445 4255 4729 0a69 6620 674c 2e67  g.DEBUG).if gL.g
-00000090: 6574 4c6f 6767 6572 285f 5f6e 616d 655f  etLogger(__name_
-000000a0: 5f29 2e6e 616d 6520 3d3d 2022 5f5f 6d61  _).name == "__ma
-000000b0: 696e 5f5f 223a 0a20 2020 2067 4c2e 7365  in__":.    gL.se
-000000c0: 744c 6f67 6765 7243 6c61 7373 2829 0a0a  tLoggerClass()..
-000000d0: 2e2e 2e0a 6060 600a 0a60 6060 7079 7468  ....```..```pyth
-000000e0: 6f6e 330a 2320 596f 7520 6361 6e20 6c6f  on3.# You can lo
-000000f0: 6720 696e 746f 2074 6865 2063 6f6e 736f  g into the conso
-00000100: 6c65 2c0a 674c 2e67 6574 4c6f 6767 6572  le,.gL.getLogger
-00000110: 285f 5f6e 616d 655f 5f29 2e69 6e69 7428  (__name__).init(
-00000120: 674c 2e4f 545f 636f 6e73 6f6c 6529 0a0a  gL.OT_console)..
-00000130: 2320 6f72 2079 6f75 2063 616e 2070 6173  # or you can pas
-00000140: 7320 6c6f 6773 2069 6e74 6f20 6120 6675  s logs into a fu
-00000150: 6e63 7469 6f6e 2c0a 6465 6620 674c 5f66  nction,.def gL_f
-00000160: 756e 6374 696f 6e28 7465 7874 293a 0a20  unction(text):. 
-00000170: 2020 2070 7269 6e74 2874 6578 7429 0a67     print(text).g
-00000180: 4c2e 7365 7446 756e 6374 696f 6e28 674c  L.setFunction(gL
-00000190: 5f66 756e 6374 696f 6e29 0a67 4c2e 6765  _function).gL.ge
-000001a0: 744c 6f67 6765 7228 5f5f 6e61 6d65 5f5f  tLogger(__name__
-000001b0: 292e 696e 6974 2867 4c2e 4f54 5f66 756e  ).init(gL.OT_fun
-000001c0: 6374 696f 6e29 0a0a 2320 6f72 2079 6f75  ction)..# or you
-000001d0: 2063 616e 2077 7269 7465 206c 6f67 7320   can write logs 
-000001e0: 746f 2066 696c 6573 2e0a 696d 706f 7274  to files..import
-000001f0: 206f 730a 674c 2e73 6574 4c6f 6744 6972   os.gL.setLogDir
-00000200: 286f 732e 7061 7468 2e6a 6f69 6e28 6f73  (os.path.join(os
-00000210: 2e67 6574 6377 6428 292c 2022 6c6f 6722  .getcwd(), "log"
-00000220: 2c20 2929 0a67 4c2e 6765 744c 6f67 6765  , )).gL.getLogge
-00000230: 7228 5f5f 6e61 6d65 5f5f 292e 696e 6974  r(__name__).init
-00000240: 2867 4c2e 4f54 5f6c 6f67 6769 6e67 290a  (gL.OT_logging).
-00000250: 0a0a 2320 5468 656e 2c20 7573 6520 7468  ..# Then, use th
-00000260: 6520 666f 6c6c 6f77 696e 6720 6675 6e63  e following func
-00000270: 7469 6f6e 2061 6e79 7768 6572 6520 746f  tion anywhere to
-00000280: 206c 6f67 2e0a 674c 2e64 6562 7567 7328   log..gL.debugs(
-00000290: 2261 222c 2031 2c20 5472 7565 2c20 290a  "a", 1, True, ).
-000002a0: 674c 2e69 6e66 6f73 2829 0a67 4c2e 7761  gL.infos().gL.wa
-000002b0: 726e 7328 290a 674c 2e65 7272 6f72 7328  rns().gL.errors(
-000002c0: 290a 0a22 2222 0a5b 4445 4255 4720 3030  )..""".[DEBUG 00
-000002d0: 3a30 303a 3030 206d 6169 6e5b 3135 5d2e  :00:00 main[15].
-000002e0: 3c6d 6f64 756c 653e 5d20 6120 3120 5472  <module>] a 1 Tr
-000002f0: 7565 0a22 2222 0a0a 6060 600a 0a60 6060  ue."""..```..```
-00000300: 7079 7468 6f6e 330a 2320 596f 7520 6361  python3.# You ca
-00000310: 6e20 7573 6520 2767 4c28 4578 6365 7074  n use 'gL(Except
-00000320: 696f 6e29 2720 746f 2065 6e61 626c 6520  ion)' to enable 
-00000330: 6c6f 6767 696e 6720 6f66 2063 6f6d 706c  logging of compl
-00000340: 6574 6520 6578 6365 7074 696f 6e20 7472  ete exception tr
-00000350: 6163 6562 6163 6b73 2c0a 2320 616e 6420  acebacks,.# and 
-00000360: 6966 2079 6f75 2068 6176 6520 2762 6574  if you have 'bet
-00000370: 7465 725f 6578 6365 7074 696f 6e73 2720  ter_exceptions' 
-00000380: 696e 7374 616c 6c65 642c 2074 6865 2074  installed, the t
-00000390: 7261 6365 6261 636b 7320 7769 6c6c 2062  racebacks will b
-000003a0: 6520 6576 656e 206d 6f72 6520 6465 7461  e even more deta
-000003b0: 696c 6564 2e0a 2320 2420 7069 7020 696e  iled..# $ pip in
-000003c0: 7374 616c 6c20 6265 7474 6572 5f65 7863  stall better_exc
-000003d0: 6570 7469 6f6e 730a 0a74 7279 3a0a 2020  eptions..try:.  
-000003e0: 2020 6465 6620 6628 612c 2062 293a 0a20    def f(a, b):. 
-000003f0: 2020 2020 2020 2072 6574 7572 6e20 6120         return a 
-00000400: 2f20 620a 2020 2020 6628 312c 2030 290a  / b.    f(1, 0).
-00000410: 6578 6365 7074 205a 6572 6f44 6976 6973  except ZeroDivis
-00000420: 696f 6e45 7272 6f72 2061 7320 653a 0a20  ionError as e:. 
-00000430: 2020 2067 4c2e 7761 726e 7328 674c 2865     gL.warns(gL(e
-00000440: 2929 0a0a 2222 220a 5b57 4152 4e49 4e47  ))..""".[WARNING
-00000450: 2030 303a 3030 3a30 3020 6d61 696e 5b31   00:00:00 main[1
-00000460: 305d 2e3c 6d6f 6475 6c65 3e5d 2054 7261  0].<module>] Tra
-00000470: 6365 6261 636b 2028 6d6f 7374 2072 6563  ceback (most rec
-00000480: 656e 7420 6361 6c6c 206c 6173 7429 3a0a  ent call last):.
-00000490: 2020 4669 6c65 2022 2f74 6d70 2f6d 6169    File "/tmp/mai
-000004a0: 6e2e 7079 222c 206c 696e 6520 382c 2069  n.py", line 8, i
-000004b0: 6e20 3c6d 6f64 756c 653e 0a20 2020 2066  n <module>.    f
-000004c0: 2831 2c20 3029 0a20 2020 20e2 9494 203c  (1, 0).    ... <
-000004d0: 6675 6e63 7469 6f6e 2066 2061 7420 3078  function f at 0x
-000004e0: 3034 4532 3634 4138 3e0a 2020 4669 6c65  04E264A8>.  File
-000004f0: 2022 2f74 6d70 2f6d 6169 6e2e 7079 222c   "/tmp/main.py",
-00000500: 206c 696e 6520 362c 2069 6e20 660a 2020   line 6, in f.  
-00000510: 2020 7265 7475 726e 2061 202f 2062 0a20    return a / b. 
-00000520: 2020 2020 2020 2020 2020 e294 8220 2020            ...   
-00000530: e294 9420 300a 2020 2020 2020 2020 2020  ... 0.          
-00000540: 20e2 9494 2031 0a22 2222 0a0a 6060 600a   ... 1."""..```.
+00000000: 3e20 7069 7020 696e 7374 616c 6c20 676c  > pip install gl
+00000010: 6c6f 6767 6572 0a60 6060 7079 7468 6f6e  logger.```python
+00000020: 330a 2320 4e4f 5445 3a20 596f 7520 7368  3.# NOTE: You sh
+00000030: 6f75 6c64 2069 6d70 6f72 7420 676c 6c6f  ould import gllo
+00000040: 6767 6572 2062 6566 6f72 6520 6578 6563  gger before exec
+00000050: 7574 696e 6720 616e 7920 6f74 6865 7220  uting any other 
+00000060: 636f 6465 2e0a 6672 6f6d 2067 6c6c 6f67  code..from gllog
+00000070: 6765 7220 696d 706f 7274 2067 4c0a 0a67  ger import gL..g
+00000080: 4c2e 7365 744c 6f67 6765 7243 6c61 7373  L.setLoggerClass
+00000090: 285f 5f6e 616d 655f 5f29 0a67 4c2e 7365  (__name__).gL.se
+000000a0: 7447 6c6f 6261 6c4c 6576 656c 286c 6f67  tGlobalLevel(log
+000000b0: 6769 6e67 2e44 4542 5547 290a 0a2e 2e2e  ging.DEBUG).....
+000000c0: 0a60 6060 0a0a 6060 6070 7974 686f 6e33  .```..```python3
+000000d0: 0a23 2059 6f75 2063 616e 206c 6f67 2069  .# You can log i
+000000e0: 6e74 6f20 7468 6520 636f 6e73 6f6c 652c  nto the console,
+000000f0: 0a67 4c2e 6765 744c 6f67 6765 7228 5f5f  .gL.getLogger(__
+00000100: 6e61 6d65 5f5f 292e 696e 6974 2867 4c2e  name__).init(gL.
+00000110: 4f54 5f63 6f6e 736f 6c65 290a 0a23 206f  OT_console)..# o
+00000120: 7220 796f 7520 6361 6e20 7061 7373 206c  r you can pass l
+00000130: 6f67 7320 696e 746f 2061 2066 756e 6374  ogs into a funct
+00000140: 696f 6e2c 0a64 6566 2067 4c5f 6675 6e63  ion,.def gL_func
+00000150: 7469 6f6e 2874 6578 7429 3a0a 2020 2020  tion(text):.    
+00000160: 7072 696e 7428 7465 7874 290a 674c 2e73  print(text).gL.s
+00000170: 6574 4675 6e63 7469 6f6e 2867 4c5f 6675  etFunction(gL_fu
+00000180: 6e63 7469 6f6e 290a 674c 2e67 6574 4c6f  nction).gL.getLo
+00000190: 6767 6572 285f 5f6e 616d 655f 5f29 2e69  gger(__name__).i
+000001a0: 6e69 7428 674c 2e4f 545f 6675 6e63 7469  nit(gL.OT_functi
+000001b0: 6f6e 290a 0a23 206f 7220 796f 7520 6361  on)..# or you ca
+000001c0: 6e20 7772 6974 6520 6c6f 6773 2074 6f20  n write logs to 
+000001d0: 6669 6c65 732e 0a69 6d70 6f72 7420 6f73  files..import os
+000001e0: 0a67 4c2e 7365 744c 6f67 4469 7228 6f73  .gL.setLogDir(os
+000001f0: 2e70 6174 682e 6a6f 696e 286f 732e 6765  .path.join(os.ge
+00000200: 7463 7764 2829 2c20 226c 6f67 222c 2029  tcwd(), "log", )
+00000210: 290a 674c 2e67 6574 4c6f 6767 6572 285f  ).gL.getLogger(_
+00000220: 5f6e 616d 655f 5f29 2e69 6e69 7428 674c  _name__).init(gL
+00000230: 2e4f 545f 6c6f 6767 696e 6729 0a0a 0a23  .OT_logging)...#
+00000240: 2054 6865 6e2c 2075 7365 2074 6865 2066   Then, use the f
+00000250: 6f6c 6c6f 7769 6e67 2066 756e 6374 696f  ollowing functio
+00000260: 6e20 616e 7977 6865 7265 2074 6f20 6c6f  n anywhere to lo
+00000270: 672e 0a67 4c2e 6465 6275 6773 2822 6122  g..gL.debugs("a"
+00000280: 2c20 312c 2054 7275 652c 2029 0a67 4c2e  , 1, True, ).gL.
+00000290: 696e 666f 7328 290a 674c 2e77 6172 6e73  infos().gL.warns
+000002a0: 2829 0a67 4c2e 6572 726f 7273 2829 0a0a  ().gL.errors()..
+000002b0: 2222 220a 5b44 4542 5547 2030 303a 3030  """.[DEBUG 00:00
+000002c0: 3a30 3020 6d61 696e 5b31 355d 2e3c 6d6f  :00 main[15].<mo
+000002d0: 6475 6c65 3e5d 2061 2031 2054 7275 650a  dule>] a 1 True.
+000002e0: 2222 220a 0a60 6060 0a0a 6060 6070 7974  """..```..```pyt
+000002f0: 686f 6e33 0a23 2059 6f75 2063 616e 2075  hon3.# You can u
+00000300: 7365 2027 674c 2845 7863 6570 7469 6f6e  se 'gL(Exception
+00000310: 2927 2074 6f20 656e 6162 6c65 206c 6f67  )' to enable log
+00000320: 6769 6e67 206f 6620 636f 6d70 6c65 7465  ging of complete
+00000330: 2065 7863 6570 7469 6f6e 2074 7261 6365   exception trace
+00000340: 6261 636b 732c 0a23 2061 6e64 2069 6620  backs,.# and if 
+00000350: 796f 7520 6861 7665 2027 6265 7474 6572  you have 'better
+00000360: 5f65 7863 6570 7469 6f6e 7327 2069 6e73  _exceptions' ins
+00000370: 7461 6c6c 6564 2c20 7468 6520 7472 6163  talled, the trac
+00000380: 6562 6163 6b73 2077 696c 6c20 6265 2065  ebacks will be e
+00000390: 7665 6e20 6d6f 7265 2064 6574 6169 6c65  ven more detaile
+000003a0: 642e 0a23 2024 2070 6970 2069 6e73 7461  d..# $ pip insta
+000003b0: 6c6c 2062 6574 7465 725f 6578 6365 7074  ll better_except
+000003c0: 696f 6e73 0a0a 7472 793a 0a20 2020 2064  ions..try:.    d
+000003d0: 6566 2066 2861 2c20 6229 3a0a 2020 2020  ef f(a, b):.    
+000003e0: 2020 2020 7265 7475 726e 2061 202f 2062      return a / b
+000003f0: 0a20 2020 2066 2831 2c20 3029 0a65 7863  .    f(1, 0).exc
+00000400: 6570 7420 5a65 726f 4469 7669 7369 6f6e  ept ZeroDivision
+00000410: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
+00000420: 674c 2e77 6172 6e73 2867 4c28 6529 290a  gL.warns(gL(e)).
+00000430: 0a22 2222 0a5b 5741 524e 494e 4720 3030  .""".[WARNING 00
+00000440: 3a30 303a 3030 206d 6169 6e5b 3130 5d2e  :00:00 main[10].
+00000450: 3c6d 6f64 756c 653e 5d20 5472 6163 6562  <module>] Traceb
+00000460: 6163 6b20 286d 6f73 7420 7265 6365 6e74  ack (most recent
+00000470: 2063 616c 6c20 6c61 7374 293a 0a20 2046   call last):.  F
+00000480: 696c 6520 222f 746d 702f 6d61 696e 2e70  ile "/tmp/main.p
+00000490: 7922 2c20 6c69 6e65 2038 2c20 696e 203c  y", line 8, in <
+000004a0: 6d6f 6475 6c65 3e0a 2020 2020 6628 312c  module>.    f(1,
+000004b0: 2030 290a 2020 2020 e294 9420 3c66 756e   0).    ... <fun
+000004c0: 6374 696f 6e20 6620 6174 2030 7830 3445  ction f at 0x04E
+000004d0: 3236 3441 383e 0a20 2046 696c 6520 222f  264A8>.  File "/
+000004e0: 746d 702f 6d61 696e 2e70 7922 2c20 6c69  tmp/main.py", li
+000004f0: 6e65 2036 2c20 696e 2066 0a20 2020 2072  ne 6, in f.    r
+00000500: 6574 7572 6e20 6120 2f20 620a 2020 2020  eturn a / b.    
+00000510: 2020 2020 2020 20e2 9482 2020 20e2 9494         ...   ...
+00000520: 2030 0a20 2020 2020 2020 2020 2020 e294   0.           ..
+00000530: 9420 310a 2222 220a 0a60 6060 0a         . 1."""..```.
```

### Comparing `gllogger-0.0.6/src/gllogger.egg-info/PKG-INFO` & `gllogger-0.0.7/src/gllogger.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: gllogger
-Version: 0.0.6
+Version: 0.0.7
 Summary: gllogger
 Author-email: calm51 <calm51@protonmail.com>
-Project-URL: Homepage, https://github.com/calm510/gllogger
-Project-URL: Issues, https://github.com/calm510/gllogger/issues
+Project-URL: Homepage, https://github.com/calm51/gllogger
+Project-URL: Issues, https://github.com/calm51/gllogger/issues
 Keywords: logger,global logger,logger hook,easy logger
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: better_exceptions
 
+> pip install gllogger
 ```python3
 # NOTE: You should import gllogger before executing any other code.
 from gllogger import gL
 
+gL.setLoggerClass(__name__)
 gL.setGlobalLevel(logging.DEBUG)
-if gL.getLogger(__name__).name == "__main__":
-    gL.setLoggerClass()
 
 ...
 ```
 
 ```python3
 # You can log into the console,
 gL.getLogger(__name__).init(gL.OT_console)
```

### Comparing `gllogger-0.0.6/src/gllogger.py` & `gllogger-0.0.7/src/gllogger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 from gllogger import gL
 
+gL.setLoggerClass(__name__)
 gL.setGlobalLevel(logging.DEBUG)
-if gL.getLogger(__name__).name == "__main__":
-    gL.setLoggerClass()
 
 gL.getLogger(__name__).init(gL.OT_console)
 
 def gL_function(text):
     print(text)
 gL.setFunction(gL_function)
 gL.getLogger(__name__).init(gL.OT_function)
@@ -370,18 +369,19 @@
     @staticmethod
     def setGlobalLevel(level):
         return logging.getLogger().setLevel(level)
 
     _had_setLoggerClass = False
 
     @staticmethod
-    def setLoggerClass():
-        GlobalLogger._had_setLoggerClass = True
-        logging.setLoggerClass(GlobalLogger)
-        logging.setLoggerClass = lambda *args, **kwargs: GlobalLogger._instance.warns(args, kwargs)
+    def setLoggerClass(name):
+        if name == "__main__":
+            GlobalLogger._had_setLoggerClass = True
+            logging.setLoggerClass(GlobalLogger)
+            logging.setLoggerClass = lambda *args, **kwargs: GlobalLogger._instance.warns(args, kwargs)
         return
 
     @staticmethod
     def loggers():
         # [print(i) for i in gL.loggers()]
         for logger_name in logging.Logger.manager.loggerDict:
             yield logging.getLogger(logger_name)
```

