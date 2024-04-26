# Comparing `tmp/samples-filter-0.0.4.tar.gz` & `tmp/samples-filter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samples-filter-0.0.4.tar", last modified: Wed Apr 17 15:46:56 2024, max compression
+gzip compressed data, was "samples-filter-0.1.4.tar", last modified: Fri Apr 26 12:21:43 2024, max compression
```

## Comparing `samples-filter-0.0.4.tar` & `samples-filter-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 15:46:56.717473 samples-filter-0.0.4/
--rw-r--r--   0 r         (1000) r         (1001)     1087 2024-04-17 15:46:41.000000 samples-filter-0.0.4/LICENSE.txt
--rw-rw-r--   0 r         (1000) r         (1001)     4339 2024-04-17 15:46:56.717473 samples-filter-0.0.4/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1001)     3636 2024-04-17 15:46:41.000000 samples-filter-0.0.4/README.md
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 15:46:56.713473 samples-filter-0.0.4/objects/
--rw-r--r--   0 r         (1000) r         (1001)     1261 2024-04-17 15:46:41.000000 samples-filter-0.0.4/objects/__init__.py
--rw-r--r--   0 r         (1000) r         (1001)     1434 2024-04-17 15:46:41.000000 samples-filter-0.0.4/objects/__main__.py
--rw-r--r--   0 r         (1000) r         (1001)     2778 2024-04-17 15:46:41.000000 samples-filter-0.0.4/objects/cli.py
--rw-r--r--   0 r         (1000) r         (1001)     2376 2024-04-17 15:46:41.000000 samples-filter-0.0.4/objects/input.py
--rw-r--r--   0 r         (1000) r         (1001)     1337 2024-04-17 15:46:41.000000 samples-filter-0.0.4/objects/pre_filter.py
--rw-r--r--   0 r         (1000) r         (1001)     1889 2024-04-17 15:46:41.000000 samples-filter-0.0.4/objects/readme.py
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 15:46:56.717473 samples-filter-0.0.4/samples_filter.egg-info/
--rw-rw-r--   0 r         (1000) r         (1001)     4339 2024-04-17 15:46:56.000000 samples-filter-0.0.4/samples_filter.egg-info/PKG-INFO
--rw-rw-r--   0 r         (1000) r         (1001)      372 2024-04-17 15:46:56.000000 samples-filter-0.0.4/samples_filter.egg-info/SOURCES.txt
--rw-rw-r--   0 r         (1000) r         (1001)        1 2024-04-17 15:46:56.000000 samples-filter-0.0.4/samples_filter.egg-info/dependency_links.txt
--rw-rw-r--   0 r         (1000) r         (1001)       58 2024-04-17 15:46:56.000000 samples-filter-0.0.4/samples_filter.egg-info/entry_points.txt
--rw-rw-r--   0 r         (1000) r         (1001)        6 2024-04-17 15:46:56.000000 samples-filter-0.0.4/samples_filter.egg-info/requires.txt
--rw-rw-r--   0 r         (1000) r         (1001)        8 2024-04-17 15:46:56.000000 samples-filter-0.0.4/samples_filter.egg-info/top_level.txt
--rw-rw-r--   0 r         (1000) r         (1001)       38 2024-04-17 15:46:56.721473 samples-filter-0.0.4/setup.cfg
--rw-r--r--   0 r         (1000) r         (1001)     2521 2024-04-17 15:46:41.000000 samples-filter-0.0.4/setup.py
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-26 12:21:43.757009 samples-filter-0.1.4/
+-rw-r--r--   0 r         (1000) r         (1001)     1087 2024-04-26 12:16:28.000000 samples-filter-0.1.4/LICENSE.txt
+-rw-rw-r--   0 r         (1000) r         (1001)    11367 2024-04-26 12:21:43.757009 samples-filter-0.1.4/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1001)    10664 2024-04-26 12:16:28.000000 samples-filter-0.1.4/README.md
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-26 12:21:43.753009 samples-filter-0.1.4/objects/
+-rw-r--r--   0 r         (1000) r         (1001)     1261 2024-04-26 12:16:28.000000 samples-filter-0.1.4/objects/__init__.py
+-rw-r--r--   0 r         (1000) r         (1001)     1434 2024-04-26 12:16:28.000000 samples-filter-0.1.4/objects/__main__.py
+-rw-r--r--   0 r         (1000) r         (1001)     2736 2024-04-26 12:16:28.000000 samples-filter-0.1.4/objects/cli.py
+-rw-r--r--   0 r         (1000) r         (1001)     2757 2024-04-26 12:16:28.000000 samples-filter-0.1.4/objects/dataset.py
+-rw-r--r--   0 r         (1000) r         (1001)     1479 2024-04-26 12:16:28.000000 samples-filter-0.1.4/objects/feed.py
+-rw-r--r--   0 r         (1000) r         (1001)     3280 2024-04-26 12:16:28.000000 samples-filter-0.1.4/objects/filter_pipe.py
+-rw-r--r--   0 r         (1000) r         (1001)     2980 2024-04-26 12:16:28.000000 samples-filter-0.1.4/objects/input.py
+-rw-r--r--   0 r         (1000) r         (1001)     1433 2024-04-26 12:16:28.000000 samples-filter-0.1.4/objects/pre_filter.py
+-rw-r--r--   0 r         (1000) r         (1001)     1586 2024-04-26 12:16:28.000000 samples-filter-0.1.4/objects/readme.py
+-rw-r--r--   0 r         (1000) r         (1001)     1416 2024-04-26 12:16:28.000000 samples-filter-0.1.4/objects/text_prediction.py
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-26 12:21:43.757009 samples-filter-0.1.4/samples_filter.egg-info/
+-rw-rw-r--   0 r         (1000) r         (1001)    11367 2024-04-26 12:21:43.000000 samples-filter-0.1.4/samples_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 r         (1000) r         (1001)      457 2024-04-26 12:21:43.000000 samples-filter-0.1.4/samples_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 r         (1000) r         (1001)        1 2024-04-26 12:21:43.000000 samples-filter-0.1.4/samples_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       58 2024-04-26 12:21:43.000000 samples-filter-0.1.4/samples_filter.egg-info/entry_points.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       22 2024-04-26 12:21:43.000000 samples-filter-0.1.4/samples_filter.egg-info/requires.txt
+-rw-rw-r--   0 r         (1000) r         (1001)        8 2024-04-26 12:21:43.000000 samples-filter-0.1.4/samples_filter.egg-info/top_level.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       38 2024-04-26 12:21:43.757009 samples-filter-0.1.4/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1001)     2548 2024-04-26 12:16:28.000000 samples-filter-0.1.4/setup.py
```

### Comparing `samples-filter-0.0.4/LICENSE.txt` & `samples-filter-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `samples-filter-0.0.4/objects/__init__.py` & `samples-filter-0.1.4/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.0.4/objects/__main__.py` & `samples-filter-0.1.4/objects/__main__.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.0.4/objects/cli.py` & `samples-filter-0.1.4/objects/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -68,107 +68,104 @@
 00000430: 5741 5245 204f 5220 5448 4520 5553 4520  WARE OR THE USE 
 00000440: 4f52 204f 5448 4552 2044 4541 4c49 4e47  OR OTHER DEALING
 00000450: 5320 494e 2054 4845 0a23 2053 4f46 5457  S IN THE.# SOFTW
 00000460: 4152 452e 0a0a 2222 220a 436c 6920 7275  ARE...""".Cli ru
 00000470: 6e6e 6572 2e0a 2222 220a 6672 6f6d 2074  nner..""".from t
 00000480: 7970 696e 6720 696d 706f 7274 204f 7074  yping import Opt
 00000490: 696f 6e61 6c0a 0a69 6d70 6f72 7420 7479  ional..import ty
-000004a0: 7065 720a 0a66 726f 6d20 6f62 6a65 6374  per..from object
-000004b0: 7320 696d 706f 7274 204e 414d 452c 2056  s import NAME, V
-000004c0: 4552 5349 4f4e 0a66 726f 6d20 2e70 7265  ERSION.from .pre
-000004d0: 5f66 696c 7465 7220 696d 706f 7274 2050  _filter import P
-000004e0: 7265 4669 6c74 6572 0a66 726f 6d20 2e69  reFilter.from .i
-000004f0: 6e70 7574 2069 6d70 6f72 7420 496e 7075  nput import Inpu
-00000500: 740a 0a61 7070 203d 2074 7970 6572 2e54  t..app = typer.T
-00000510: 7970 6572 2829 0a0a 0a64 6566 205f 7665  yper()...def _ve
-00000520: 7273 696f 6e5f 6361 6c6c 6261 636b 2876  rsion_callback(v
-00000530: 616c 7565 3a20 626f 6f6c 2920 2d3e 204e  alue: bool) -> N
-00000540: 6f6e 653a 0a20 2020 2069 6620 7661 6c75  one:.    if valu
-00000550: 653a 0a20 2020 2020 2020 2074 7970 6572  e:.        typer
-00000560: 2e65 6368 6f28 6622 7b56 4552 5349 4f4e  .echo(f"{VERSION
-00000570: 7d22 290a 2020 2020 2020 2020 7261 6973  }").        rais
-00000580: 6520 7479 7065 722e 4578 6974 2829 0a0a  e typer.Exit()..
-00000590: 0a40 6170 702e 636f 6d6d 616e 6428 290a  .@app.command().
-000005a0: 6465 6620 6669 6c74 6572 280a 2020 2020  def filter(.    
-000005b0: 2020 2020 7265 706f 7369 746f 7269 6573      repositories
-000005c0: 3a20 7374 7220 3d20 7479 7065 722e 4f70  : str = typer.Op
-000005d0: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
-000005e0: 2020 2e2e 2e2c 2022 2d2d 7265 706f 7369    ..., "--reposi
-000005f0: 746f 7269 6573 222c 2068 656c 703d 2250  tories", help="P
-00000600: 6174 6820 746f 2074 6865 2072 6570 6f73  ath to the repos
-00000610: 6974 6f72 6965 7320 4353 5620 6669 6c65  itories CSV file
-00000620: 2e22 0a20 2020 2020 2020 2029 2c0a 2020  .".        ),.  
-00000630: 2020 2020 2020 6f75 743a 2073 7472 203d        out: str =
-00000640: 2074 7970 6572 2e4f 7074 696f 6e28 0a20   typer.Option(. 
-00000650: 2020 2020 2020 2020 2020 202e 2e2e 2c20             ..., 
-00000660: 222d 2d6f 7574 222c 2068 656c 703d 2250  "--out", help="P
-00000670: 6174 6820 746f 2074 6865 206f 7574 7075  ath to the outpu
-00000680: 7420 4353 5620 6669 6c65 2e22 0a20 2020  t CSV file.".   
-00000690: 2020 2020 2029 0a29 3a0a 2020 2020 2222       ).):.    ""
-000006a0: 220a 2020 2020 4669 6c74 6572 2072 6570  ".    Filter rep
-000006b0: 6f73 6974 6f72 6965 732e 0a20 2020 2022  ositories..    "
-000006c0: 2222 0a20 2020 2074 7970 6572 2e65 6368  "".    typer.ech
-000006d0: 6f28 6622 4669 6c74 6572 696e 6720 7b72  o(f"Filtering {r
-000006e0: 6570 6f73 6974 6f72 6965 737d 2e2e 2e22  epositories}..."
-000006f0: 290a 2020 2020 2320 4074 6f64 6f20 2331  ).    # @todo #1
-00000700: 303a 3435 6d69 6e20 4669 6c74 6572 2074  0:45min Filter t
-00000710: 6865 2072 6570 6f73 6974 6f72 6965 7320  he repositories 
-00000720: 7573 696e 6720 6765 6e65 7261 6c2d 6c69  using general-li
-00000730: 6b65 2069 6e74 6572 6661 6365 2e0a 2020  ke interface..  
-00000740: 2020 2320 2057 6520 7368 6f75 6c64 2065    #  We should e
-00000750: 7865 6375 7465 2066 696c 7465 7269 6e67  xecute filtering
-00000760: 2068 6572 6520 7573 696e 6720 736f 6d65   here using some
-00000770: 2067 656e 6572 616c 2069 6e74 6572 6661   general interfa
-00000780: 6365 2c20 736f 0a20 2020 2023 2020 6974  ce, so.    #  it
-00000790: 2077 6f75 6c64 2065 6173 7920 746f 2075   would easy to u
-000007a0: 7365 2065 6974 6865 7220 4c4c 4d20 6f72  se either LLM or
-000007b0: 204d 4c20 6669 6c74 6572 732e 0a20 2020   ML filters..   
-000007c0: 2023 2040 746f 646f 2023 3139 3a34 3520   # @todo #19:45 
-000007d0: 496d 706c 656d 656e 7420 6368 6169 6e20  Implement chain 
-000007e0: 6f66 2063 7376 2074 7261 6e73 666f 726d  of csv transform
-000007f0: 6174 696f 6e2e 0a20 2020 2023 2020 5765  ation..    #  We
-00000800: 2073 686f 756c 6420 696d 706c 656d 656e   should implemen
-00000810: 7420 6120 7472 616e 7366 6f72 6d61 7469  t a transformati
-00000820: 6f6e 2063 6861 696e 206f 6620 6373 7620  on chain of csv 
-00000830: 6669 6c65 732e 0a20 2020 2023 2020 466f  files..    #  Fo
-00000840: 7220 6e6f 7720 7765 2061 7265 206a 7573  r now we are jus
-00000850: 7420 6164 6469 6e67 2073 6570 6172 6174  t adding separat
-00000860: 6520 6f62 6a65 6374 7320 746f 2074 6869  e objects to thi
-00000870: 7320 7363 7269 7074 2e0a 2020 2020 2320  s script..    # 
-00000880: 204c 6574 2773 2063 7265 6174 6520 6120   Let's create a 
-00000890: 636c 6173 7320 286c 6574 2773 2063 616c  class (let's cal
-000008a0: 6c20 6974 2060 7472 6169 6e60 206f 7220  l it `train` or 
-000008b0: 6070 6970 656c 696e 6560 2920 7468 6174  `pipeline`) that
-000008c0: 2077 6f75 6c64 0a20 2020 2023 2020 6578   would.    #  ex
-000008d0: 6563 7574 6520 616c 6c20 7472 616e 7366  ecute all transf
-000008e0: 6f72 6d61 7469 6f6e 206f 6e65 2062 7920  ormation one by 
-000008f0: 6f6e 652e 0a20 2020 2050 7265 4669 6c74  one..    PreFilt
-00000900: 6572 286f 7574 292e 7072 6570 6172 6528  er(out).prepare(
-00000910: 290a 2020 2020 496e 7075 7428 7265 706f  ).    Input(repo
-00000920: 7369 746f 7269 6573 292e 636f 7079 2829  sitories).copy()
-00000930: 0a20 2020 2074 7970 6572 2e65 6368 6f28  .    typer.echo(
-00000940: 6622 4669 6c74 6572 696e 6720 636f 6d70  f"Filtering comp
-00000950: 6c65 7465 642e 2053 6176 696e 6720 6f75  leted. Saving ou
-00000960: 7470 7574 2074 6f20 7b6f 7574 7d2e 2e2e  tput to {out}...
-00000970: 2229 0a0a 0a23 2052 756e 2069 742e 0a40  ")...# Run it..@
-00000980: 6170 702e 6361 6c6c 6261 636b 2829 0a64  app.callback().d
-00000990: 6566 206d 6169 6e28 0a20 2020 2020 2020  ef main(.       
-000009a0: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-000009b0: 6c65 3d75 6e75 7365 642d 6172 6775 6d65  le=unused-argume
-000009c0: 6e74 0a20 2020 2020 2020 2076 6572 7369  nt.        versi
-000009d0: 6f6e 3a20 4f70 7469 6f6e 616c 5b62 6f6f  on: Optional[boo
-000009e0: 6c5d 203d 2074 7970 6572 2e4f 7074 696f  l] = typer.Optio
-000009f0: 6e28 0a20 2020 2020 2020 2020 2020 204e  n(.            N
-00000a00: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00000a10: 2022 2d2d 7665 7273 696f 6e22 2c0a 2020   "--version",.  
-00000a20: 2020 2020 2020 2020 2020 6865 6c70 3d22            help="
-00000a30: 5368 6f77 2074 6865 2061 7070 6c69 6361  Show the applica
-00000a40: 7469 6f6e 2773 2076 6572 7369 6f6e 2061  tion's version a
-00000a50: 6e64 2065 7869 742e 222c 0a20 2020 2020  nd exit.",.     
-00000a60: 2020 2020 2020 2063 616c 6c62 6163 6b3d         callback=
-00000a70: 5f76 6572 7369 6f6e 5f63 616c 6c62 6163  _version_callbac
-00000a80: 6b2c 0a20 2020 2020 2020 2020 2020 2069  k,.            i
-00000a90: 735f 6561 6765 723d 5472 7565 2c0a 2020  s_eager=True,.  
-00000aa0: 2020 2020 2020 290a 2920 2d3e 204e 6f6e        ).) -> Non
-00000ab0: 653a 0a20 2020 2066 2222 220a 2020 2020  e:.    f""".    
-00000ac0: 7b4e 414d 457d 0a20 2020 2022 2222 0a20  {NAME}.    """. 
-00000ad0: 2020 2072 6574 7572 6e0a                    return.
+000004a0: 7065 720a 0a66 726f 6d20 2e66 696c 7465  per..from .filte
+000004b0: 725f 7069 7065 2069 6d70 6f72 7420 4669  r_pipe import Fi
+000004c0: 6c74 6572 5069 7065 0a66 726f 6d20 6d6f  lterPipe.from mo
+000004d0: 6465 6c2e 7072 6564 6963 746f 7220 696d  del.predictor im
+000004e0: 706f 7274 2050 7265 6469 6374 6f72 0a66  port Predictor.f
+000004f0: 726f 6d20 2e64 6174 6173 6574 2069 6d70  rom .dataset imp
+00000500: 6f72 7420 4461 7461 7365 740a 6672 6f6d  ort Dataset.from
+00000510: 206f 626a 6563 7473 2069 6d70 6f72 7420   objects import 
+00000520: 4e41 4d45 2c20 5645 5253 494f 4e0a 6672  NAME, VERSION.fr
+00000530: 6f6d 202e 7072 655f 6669 6c74 6572 2069  om .pre_filter i
+00000540: 6d70 6f72 7420 5072 6546 696c 7465 720a  mport PreFilter.
+00000550: 6672 6f6d 202e 696e 7075 7420 696d 706f  from .input impo
+00000560: 7274 2049 6e70 7574 0a0a 6170 7020 3d20  rt Input..app = 
+00000570: 7479 7065 722e 5479 7065 7228 290a 0a0a  typer.Typer()...
+00000580: 6465 6620 5f76 6572 7369 6f6e 5f63 616c  def _version_cal
+00000590: 6c62 6163 6b28 7661 6c75 653a 2062 6f6f  lback(value: boo
+000005a0: 6c29 202d 3e20 4e6f 6e65 3a0a 2020 2020  l) -> None:.    
+000005b0: 6966 2076 616c 7565 3a0a 2020 2020 2020  if value:.      
+000005c0: 2020 7479 7065 722e 6563 686f 2866 227b    typer.echo(f"{
+000005d0: 5645 5253 494f 4e7d 2229 0a20 2020 2020  VERSION}").     
+000005e0: 2020 2072 6169 7365 2074 7970 6572 2e45     raise typer.E
+000005f0: 7869 7428 290a 0a0a 4061 7070 2e63 6f6d  xit()...@app.com
+00000600: 6d61 6e64 2829 0a64 6566 2066 696c 7465  mand().def filte
+00000610: 7228 0a20 2020 2020 2020 2072 6570 6f73  r(.        repos
+00000620: 6974 6f72 6965 733a 2073 7472 203d 2074  itories: str = t
+00000630: 7970 6572 2e4f 7074 696f 6e28 0a20 2020  yper.Option(.   
+00000640: 2020 2020 2020 2020 202e 2e2e 2c20 222d           ..., "-
+00000650: 2d72 6570 6f73 6974 6f72 6965 7322 2c20  -repositories", 
+00000660: 6865 6c70 3d22 5061 7468 2074 6f20 7468  help="Path to th
+00000670: 6520 696e 7075 7420 7265 706f 7369 746f  e input reposito
+00000680: 7269 6573 2043 5356 2066 696c 652e 220a  ries CSV file.".
+00000690: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+000006a0: 2020 206f 7574 3a20 7374 7220 3d20 7479     out: str = ty
+000006b0: 7065 722e 4f70 7469 6f6e 280a 2020 2020  per.Option(.    
+000006c0: 2020 2020 2020 2020 2e2e 2e2c 2022 2d2d          ..., "--
+000006d0: 6f75 7422 2c20 6865 6c70 3d22 5061 7468  out", help="Path
+000006e0: 2074 6f20 7468 6520 6f75 7470 7574 2043   to the output C
+000006f0: 5356 2066 696c 652e 220a 2020 2020 2020  SV file.".      
+00000700: 2020 290a 293a 0a20 2020 2022 2222 0a20    ).):.    """. 
+00000710: 2020 2046 696c 7465 7220 7265 706f 7369     Filter reposi
+00000720: 746f 7269 6573 2e0a 2020 2020 2222 220a  tories..    """.
+00000730: 2020 2020 2320 4074 6f64 6f20 2331 383a      # @todo #18:
+00000740: 3330 6d69 6e20 4669 6e64 2065 6666 6563  30min Find effec
+00000750: 7469 7665 2077 6179 2066 6f72 2070 726f  tive way for pro
+00000760: 6365 7373 696e 6720 7265 6164 6d65 2e0a  cessing readme..
+00000770: 2020 2020 2320 2046 6f72 206e 6f77 2077      #  For now w
+00000780: 6520 6172 6520 6e6f 7420 7072 6f63 6573  e are not proces
+00000790: 7369 6e67 2072 6561 646d 6520 6265 6361  sing readme beca
+000007a0: 7573 6520 6f66 0a20 2020 2023 2020 3c61  use of.    #  <a
+000007b0: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+000007c0: 6974 6875 622e 636f 6d2f 6831 616c 6578  ithub.com/h1alex
+000007d0: 6265 6c2f 7361 6d70 6c65 732d 6669 6c74  bel/samples-filt
+000007e0: 6572 2f69 7373 7565 732f 3339 223e 7468  er/issues/39">th
+000007f0: 6973 3c2f 613e 2e0a 2020 2020 2320 2057  is</a>..    #  W
+00000800: 6520 6e65 6564 2074 6f20 6669 6e64 2061  e need to find a
+00000810: 6374 7561 6c20 7761 7920 746f 2070 726f  ctual way to pro
+00000820: 6365 7373 2072 6561 646d 6520 746f 6f20  cess readme too 
+00000830: 7369 6e63 6520 6974 2063 616e 2062 6520  since it can be 
+00000840: 6372 7563 6961 6c0a 2020 2020 2320 2064  crucial.    #  d
+00000850: 6174 6120 6173 206d 6f64 656c 2069 6e70  ata as model inp
+00000860: 7574 2e20 4c65 7427 7320 7374 7564 7920  ut. Let's study 
+00000870: 7061 7065 7273 2c20 6f75 746c 696e 6564  papers, outlined
+00000880: 0a20 2020 2023 2020 3c61 2068 7265 663d  .    #  <a href=
+00000890: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000008a0: 636f 6d2f 7965 676f 7232 3536 2f63 616d  com/yegor256/cam
+000008b0: 2f69 7373 7565 732f 3232 3723 6973 7375  /issues/227#issu
+000008c0: 652d 3232 3030 3038 3035 3539 223e 6865  e-2200080559">he
+000008d0: 7265 3c2f 613e 0a20 2020 2023 2020 6669  re</a>.    #  fi
+000008e0: 7273 742c 2072 6574 6869 6e6b 2069 7420  rst, rethink it 
+000008f0: 616e 6420 7472 7920 746f 2069 6d70 6c65  and try to imple
+00000900: 6d65 6e74 2068 6572 652e 0a20 2020 2046  ment here..    F
+00000910: 696c 7465 7250 6970 6528 7265 706f 7369  ilterPipe(reposi
+00000920: 746f 7269 6573 2c20 6f75 742c 2050 7265  tories, out, Pre
+00000930: 6469 6374 6f72 2829 2c20 7479 7065 7229  dictor(), typer)
+00000940: 2e61 7070 6c79 2829 0a0a 0a23 2052 756e  .apply()...# Run
+00000950: 2069 742e 0a40 6170 702e 6361 6c6c 6261   it..@app.callba
+00000960: 636b 2829 0a64 6566 206d 6169 6e28 0a20  ck().def main(. 
+00000970: 2020 2020 2020 2023 2070 796c 696e 743a         # pylint:
+00000980: 2064 6973 6162 6c65 3d75 6e75 7365 642d   disable=unused-
+00000990: 6172 6775 6d65 6e74 0a20 2020 2020 2020  argument.       
+000009a0: 2076 6572 7369 6f6e 3a20 4f70 7469 6f6e   version: Option
+000009b0: 616c 5b62 6f6f 6c5d 203d 2074 7970 6572  al[bool] = typer
+000009c0: 2e4f 7074 696f 6e28 0a20 2020 2020 2020  .Option(.       
+000009d0: 2020 2020 204e 6f6e 652c 0a20 2020 2020       None,.     
+000009e0: 2020 2020 2020 2022 2d2d 7665 7273 696f         "--versio
+000009f0: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
+00000a00: 6865 6c70 3d22 5368 6f77 2074 6865 2061  help="Show the a
+00000a10: 7070 6c69 6361 7469 6f6e 2773 2076 6572  pplication's ver
+00000a20: 7369 6f6e 2061 6e64 2065 7869 742e 222c  sion and exit.",
+00000a30: 0a20 2020 2020 2020 2020 2020 2063 616c  .            cal
+00000a40: 6c62 6163 6b3d 5f76 6572 7369 6f6e 5f63  lback=_version_c
+00000a50: 616c 6c62 6163 6b2c 0a20 2020 2020 2020  allback,.       
+00000a60: 2020 2020 2069 735f 6561 6765 723d 5472       is_eager=Tr
+00000a70: 7565 2c0a 2020 2020 2020 2020 290a 2920  ue,.        ).) 
+00000a80: 2d3e 204e 6f6e 653a 0a20 2020 2066 2222  -> None:.    f""
+00000a90: 220a 2020 2020 7b4e 414d 457d 0a20 2020  ".    {NAME}.   
+00000aa0: 2022 2222 0a20 2020 2072 6574 7572 6e0a   """.    return.
```

### Comparing `samples-filter-0.0.4/objects/input.py` & `samples-filter-0.1.4/objects/dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,43 +17,54 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
-Pipeline input.
+Dataset.
 """
 import csv
-from .readme import Readme
 
-class Input:
-    DESTINATION = "pipeline/input.csv"
 
-    def __init__(self, name):
-        self.name = name
+class Dataset:
+    DESTINATION = "pipeline/dataset.csv"
 
-    def copy(self):
-        # @todo #19:25min Prepare files in /pipeline directory.
-        #  We should create them before running actual processing.
-        #  For now we need to manually create files.
-        #  Don't forget to remove this puzzle.
-        with open(self.name, "r") as input, open(self.DESTINATION, "w", newline="") as pipe:
+    def __init__(self, where):
+        self.where = where
+
+    """
+    Formulate dataset.
+    """
+    def formulate(self):
+        with open(self.where, "r") as input, open(self.DESTINATION, "w", newline="") as pipe:
             reader = csv.DictReader(input)
             writer = csv.DictWriter(
                 pipe,
-                fieldnames=["full_name", "description", "topics", "readme"]
+                fieldnames=[
+                    "full_name",
+                    "description",
+                    "topics",
+                    "readme"
+                ]
             )
             writer.writeheader()
+            # @todo #34:60min CSV column 'readme' is too big to read with reader.
+            #  Column that contains readme in some cases is over the limit,
+            #  which is `131072`. It this problem causes exception and
+            #  terminates next row processing. Let's try to compress +
+            #  decompress readme when writing/reading it. Another option can
+            #  be to present the whole dataset in other format, for instance
+            #  JSON. Don't forget to remove this puzzle.
             for row in reader:
                 repo = row["full_name"]
                 description = row["description"]
                 topics = row["topics"]
-                readme = Readme(repo).asText()
+                readme = row["readme"]
                 out = {
                     "full_name": repo,
                     "description": description,
                     "topics": topics,
                     "readme": readme
                 }
                 writer.writerow(out)
-                print(f"Copied {repo} to {self.DESTINATION}")
+                print(f"Prepared dataset for {repo}")
```

### Comparing `samples-filter-0.0.4/objects/pre_filter.py` & `samples-filter-0.1.4/objects/pre_filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
 Prepares outputs before running filters.
 """
+import os.path
+
+
 class PreFilter:
     def __init__(self, out):
         self.out = out
 
     def prepare(self):
+        if not os.path.exists("pipeline"):
+            os.makedirs("pipeline")
         with open(self.out, "w") as file:
             file.write("")
```

### Comparing `samples-filter-0.0.4/objects/readme.py` & `samples-filter-0.1.4/objects/readme.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,29 +19,22 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """
 GitHub Readme.
 """
-import base64
-
 import requests
 
-
 class Readme:
-    def __init__(self, repo):
+    def __init__(self, repo, branch):
         self.repo = repo
+        self.branch = branch
 
-    # @todo #19:45min Use raw.githubusercontent.com instead of api.github.com.
-    #  We should use static GitHub content hosting instead of their API
-    #  in order to prevent problems with rate limits.
-    #  Don't forget to remove this puzzle.
     def asText(self):
         response = requests.get(
-            f"https://api.github.com/repos/{self.repo}/readme",
-            headers={"Accept": "application/vnd.github.v3+json"}
+            f"https://raw.githubusercontent.com/{self.repo}/{self.branch}/README.md",
         )
         if response.status_code == 200:
-            return base64.b64decode(response.json()["content"]).decode("utf-8")
+            return response.text
         else:
-            print(f"Failed to fetch README for {self.repo}")
+            print(f"Failed to fetch README for {self.repo}@{self.branch}")
```

### Comparing `samples-filter-0.0.4/setup.py` & `samples-filter-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     long_description = f.read()
 
 setup(
     name='samples-filter',
     version=actual,
     packages=find_packages(),
     install_requires=[
-        'typer'
+        'typer',
+        'pyarrow==16.0.0'
     ],
     entry_points={
         'console_scripts': [
             'samples-filter=objects.__main__:main',
         ],
     },
     author='Aliaksei Bialiauski',
```

