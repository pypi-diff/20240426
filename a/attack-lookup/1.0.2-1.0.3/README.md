# Comparing `tmp/attack-lookup-1.0.2.tar.gz` & `tmp/attack_lookup-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attack-lookup-1.0.2.tar", last modified: Tue May 10 21:14:06 2022, max compression
+gzip compressed data, was "attack_lookup-1.0.3.tar", last modified: Thu Apr 25 22:29:06 2024, max compression
```

## Comparing `attack-lookup-1.0.2.tar` & `attack_lookup-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zander     (501) staff       (20)        0 2022-05-10 21:14:06.192259 attack-lookup-1.0.2/
--rw-r--r--   0 zander     (501) staff       (20)     1070 2021-11-25 19:56:18.000000 attack-lookup-1.0.2/LICENSE
--rw-r--r--   0 zander     (501) staff       (20)       35 2021-11-25 19:56:18.000000 attack-lookup-1.0.2/MANIFEST.in
--rw-r--r--   0 zander     (501) staff       (20)     6150 2022-05-10 21:14:06.192101 attack-lookup-1.0.2/PKG-INFO
--rw-r--r--   0 zander     (501) staff       (20)     4857 2022-05-10 21:10:11.000000 attack-lookup-1.0.2/README.md
-drwxr-xr-x   0 zander     (501) staff       (20)        0 2022-05-10 21:14:06.163956 attack-lookup-1.0.2/attack_lookup/
--rw-r--r--   0 zander     (501) staff       (20)       34 2021-11-25 19:56:18.000000 attack-lookup-1.0.2/attack_lookup/__init__.py
--rw-r--r--   0 zander     (501) staff       (20)     3856 2021-11-26 16:13:58.000000 attack-lookup-1.0.2/attack_lookup/__main__.py
-drwxr-xr-x   0 zander     (501) staff       (20)        0 2022-05-10 21:14:06.162609 attack-lookup-1.0.2/attack_lookup/data/
-drwxr-xr-x   0 zander     (501) staff       (20)        0 2022-05-10 21:14:06.189223 attack-lookup-1.0.2/attack_lookup/data/v10.1/
--rw-r--r--   0 zander     (501) staff       (20) 22729202 2021-11-25 19:56:18.000000 attack-lookup-1.0.2/attack_lookup/data/v10.1/enterprise-attack.json
--rw-r--r--   0 zander     (501) staff       (20)  1052465 2021-11-25 19:56:18.000000 attack-lookup-1.0.2/attack_lookup/data/v10.1/ics-attack.json
--rw-r--r--   0 zander     (501) staff       (20)  1845007 2021-11-25 19:56:18.000000 attack-lookup-1.0.2/attack_lookup/data/v10.1/mobile-attack.json
--rw-r--r--   0 zander     (501) staff       (20)     4850 2022-05-10 21:10:11.000000 attack-lookup-1.0.2/attack_lookup/mapping.py
-drwxr-xr-x   0 zander     (501) staff       (20)        0 2022-05-10 21:14:06.164787 attack-lookup-1.0.2/attack_lookup.egg-info/
--rw-r--r--   0 zander     (501) staff       (20)     6150 2022-05-10 21:14:06.000000 attack-lookup-1.0.2/attack_lookup.egg-info/PKG-INFO
--rw-r--r--   0 zander     (501) staff       (20)      472 2022-05-10 21:14:06.000000 attack-lookup-1.0.2/attack_lookup.egg-info/SOURCES.txt
--rw-r--r--   0 zander     (501) staff       (20)        1 2022-05-10 21:14:06.000000 attack-lookup-1.0.2/attack_lookup.egg-info/dependency_links.txt
--rw-r--r--   0 zander     (501) staff       (20)       63 2022-05-10 21:14:06.000000 attack-lookup-1.0.2/attack_lookup.egg-info/entry_points.txt
--rw-r--r--   0 zander     (501) staff       (20)       30 2022-05-10 21:14:06.000000 attack-lookup-1.0.2/attack_lookup.egg-info/requires.txt
--rw-r--r--   0 zander     (501) staff       (20)       14 2022-05-10 21:14:06.000000 attack-lookup-1.0.2/attack_lookup.egg-info/top_level.txt
--rw-r--r--   0 zander     (501) staff       (20)       38 2022-05-10 21:14:06.192312 attack-lookup-1.0.2/setup.cfg
--rw-r--r--   0 zander     (501) staff       (20)     1057 2022-05-10 21:12:25.000000 attack-lookup-1.0.2/setup.py
+drwxr-xr-x   0 geech     (1000) geech     (1000)        0 2024-04-25 22:29:06.777675 attack_lookup-1.0.3/
+-rw-r--r--   0 geech     (1000) geech     (1000)     1070 2024-04-25 22:15:29.000000 attack_lookup-1.0.3/LICENSE
+-rw-r--r--   0 geech     (1000) geech     (1000)       35 2024-04-25 22:15:29.000000 attack_lookup-1.0.3/MANIFEST.in
+-rw-r--r--   0 geech     (1000) geech     (1000)     5248 2024-04-25 22:29:06.777675 attack_lookup-1.0.3/PKG-INFO
+-rw-r--r--   0 geech     (1000) geech     (1000)     4853 2024-04-25 22:24:39.000000 attack_lookup-1.0.3/README.md
+drwxr-xr-x   0 geech     (1000) geech     (1000)        0 2024-04-25 22:29:06.731008 attack_lookup-1.0.3/attack_lookup/
+-rw-r--r--   0 geech     (1000) geech     (1000)       34 2024-04-25 22:15:29.000000 attack_lookup-1.0.3/attack_lookup/__init__.py
+-rw-r--r--   0 geech     (1000) geech     (1000)     3854 2024-04-25 22:18:20.000000 attack_lookup-1.0.3/attack_lookup/__main__.py
+drwxr-xr-x   0 geech     (1000) geech     (1000)        0 2024-04-25 22:29:06.727674 attack_lookup-1.0.3/attack_lookup/data/
+drwxr-xr-x   0 geech     (1000) geech     (1000)        0 2024-04-25 22:29:06.771008 attack_lookup-1.0.3/attack_lookup/data/v15/
+-rw-r--r--   0 geech     (1000) geech     (1000) 26585200 2024-04-25 22:17:04.000000 attack_lookup-1.0.3/attack_lookup/data/v15/enterprise-attack.json
+-rw-r--r--   0 geech     (1000) geech     (1000)  1859133 2024-04-25 22:17:23.000000 attack_lookup-1.0.3/attack_lookup/data/v15/ics-attack.json
+-rw-r--r--   0 geech     (1000) geech     (1000)  2493231 2024-04-25 22:17:42.000000 attack_lookup-1.0.3/attack_lookup/data/v15/mobile-attack.json
+-rw-r--r--   0 geech     (1000) geech     (1000)     4848 2024-04-25 22:22:11.000000 attack_lookup-1.0.3/attack_lookup/mapping.py
+drwxr-xr-x   0 geech     (1000) geech     (1000)        0 2024-04-25 22:29:06.774341 attack_lookup-1.0.3/attack_lookup.egg-info/
+-rw-r--r--   0 geech     (1000) geech     (1000)     5248 2024-04-25 22:29:06.000000 attack_lookup-1.0.3/attack_lookup.egg-info/PKG-INFO
+-rw-r--r--   0 geech     (1000) geech     (1000)      466 2024-04-25 22:29:06.000000 attack_lookup-1.0.3/attack_lookup.egg-info/SOURCES.txt
+-rw-r--r--   0 geech     (1000) geech     (1000)        1 2024-04-25 22:29:06.000000 attack_lookup-1.0.3/attack_lookup.egg-info/dependency_links.txt
+-rw-r--r--   0 geech     (1000) geech     (1000)       62 2024-04-25 22:29:06.000000 attack_lookup-1.0.3/attack_lookup.egg-info/entry_points.txt
+-rw-r--r--   0 geech     (1000) geech     (1000)       33 2024-04-25 22:29:06.000000 attack_lookup-1.0.3/attack_lookup.egg-info/requires.txt
+-rw-r--r--   0 geech     (1000) geech     (1000)       14 2024-04-25 22:29:06.000000 attack_lookup-1.0.3/attack_lookup.egg-info/top_level.txt
+-rw-r--r--   0 geech     (1000) geech     (1000)       38 2024-04-25 22:29:06.777675 attack_lookup-1.0.3/setup.cfg
+-rw-r--r--   0 geech     (1000) geech     (1000)     1057 2024-04-25 22:18:05.000000 attack_lookup-1.0.3/setup.py
```

### Comparing `attack-lookup-1.0.2/LICENSE` & `attack_lookup-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `attack-lookup-1.0.2/PKG-INFO` & `attack_lookup-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,134 +1,136 @@
 Metadata-Version: 2.1
 Name: attack-lookup
-Version: 1.0.2
+Version: 1.0.3
 Summary: MITRE ATT&CK Lookup Tool
 Home-page: https://github.com/curated-intel/attack-lookup
 Author: Zander Work
 Author-email: pypi@zanderwork.com
 License: MIT
-Description:                                                                                
-                                                                                        
-                                       %%%%%#########%%%%%                              
-                                ###%%%%##                 &%%%                          
-                           (#####%%          /.. .,,,,&      .%%                        
-                       //((###            . ...**//((... ,     %%                       
-                   ***//((               (..***//((...*#,,,     %%                      
-               *******                  #(#./((((#......,%#(     %                      
-                *****                   @%##....#%%%%%,,%#((     %                      
-                  ****//                 %%%%,,%%%%%%%**/((     #                       
-                     *//((#*               %%,%%%%%##((((      %                        
-                        ((####%               ,((((((/                                  
-                           #####%%#,                                         **         
-                               ##%%%#####                              //**             
-                                    %%%%#########%.          ######((/                  
-                                           %%%%%#%%%%%%%%%#####                         
-                                           
-                                          by Curated Intelligence   
-        
-        # MITRE ATT&CK Lookup Tool
-        
-        [![PyPi license](https://badgen.net/pypi/license/attack-lookup/)](https://pypi.org/project/attack-lookup/) [![PyPi version](https://badgen.net/pypi/v/attack-lookup/)](https://pypi.org/project/attack-lookup/)
-        
-        `attack-lookup` is a tool that lets you easily check what Tactic, Technique, or Sub-technique ID maps to what name, and vice versa. It can be used interactively, for batch processing, or in your own tooling. 
-        
-        ## Installation
-        
-        `attack-lookup` can be installed from PyPI:
-        
-        ```
-        $ pip install attack-lookup
-        ```
-        
-        It can also be installed manually:
-        
-        ```
-        $ git clone https://github.com/curated-intel/attack-lookup.git
-        $ cd attack-lookup
-        $ python setup.py install --user
-        ```
-        
-        ## Usage
-        
-        ```
-        $ attack-lookup --help
-        usage: attack-lookup [-h] [-v VERSION] [-m {enterprise,ics,mobile}] [-O] [-i INPUT] [-o OUTPUT] [--output-mode {results,csv}]
-        
-        MITRE ATT&CK Lookup Tool
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -v VERSION, --version VERSION
-                                ATT&CK matrix version to use (default: v10.1)
-          -m {enterprise,ics,mobile}, --matrix {enterprise,ics,mobile}
-                                ATT&CK matrix to use (default: enterprise)
-          -O, --offline         Run in offline mode (default: False)
-          -i INPUT, --input INPUT
-                                Path to input file (one lookup value per line) (default: None)
-          -o OUTPUT, --output OUTPUT
-                                Path to output file (default: -)
-          --output-mode {results,csv}
-                                Mode for output file ("result" only has the lookup results, "csv" outputs a CSV with the lookup and result values (default: results)
-        ```
-        
-        By default, `attack-lookup` uses the latest version of the Enterprise matrix. When running in Online mode, `attack-lookup` pulls the latest matrix from MITRE's GitHub [repo](https://github.com/mitre/cti). When running in Offline mode, it can use any matrix available in `attack_lookup/data`.
-        
-        You can use `attack-lookup` in interactive or batch mode:
-        
-        ```
-        $ attack-lookup
-        (loading latest enterprise matrix...done)
-        Running attack-lookup in interactive mode, exit with (q)uit. Enter one or more values to lookup, separated by a comma.
-        ATT&CK> T1539
-        Steal Web Session Cookie
-        ATT&CK>
-        ```
-        
-        For batch mode, specify an input file, and optionally an output file/mode. By default, output will go to `stdout`.
-        ```
-        $ attack-lookup -i test
-        (loading latest enterprise matrix...done)
-        Collection
-        T1133
-        Peripheral Device Discovery
-        
-        $ attack-lookup -i test --output-mode=csv
-        (loading latest enterprise matrix...done)
-        TA0009,Collection
-        External Remote Services,T1133
-        T1120,Peripheral Device Discovery
-        
-        $ attack-lookup -i test --output-mode=csv -o out_file
-        (loading latest enterprise matrix...done)
-        Wrote output data to out_file
-        ```
-        
-        If multiple mappings exist (e.g., "Domains"), `attack-lookup` will provide all possible values:
-        ```
-        ATT&CK> Domains
-        Multiple possible values: T1583.001, T1584.001
-        ```
-        
-        ## API
-        
-        You can also use `attack-lookup` in your own scripts.
-        
-        ```py
-        from attack_lookup import AttackMapping
-        
-        # version is ignored when running online FYSA
-        mapping = AttackMapping(matrix="enterprise", version="v10.1", offline=False)
-        
-        # load the data
-        # this can take ~10sec
-        if not mapping.load_data():
-            print("failed to load data")
-        else:
-            mapping.lookup("T1574") # returns "Hijack Execution Flow"
-        ```
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests<3,>=2.22.0
+Requires-Dist: stix2==3.0.1
+
+                                                                               
+                                                                                
+                               %%%%%#########%%%%%                              
+                        ###%%%%##                 &%%%                          
+                   (#####%%          /.. .,,,,&      .%%                        
+               //((###            . ...**//((... ,     %%                       
+           ***//((               (..***//((...*#,,,     %%                      
+       *******                  #(#./((((#......,%#(     %                      
+        *****                   @%##....#%%%%%,,%#((     %                      
+          ****//                 %%%%,,%%%%%%%**/((     #                       
+             *//((#*               %%,%%%%%##((((      %                        
+                ((####%               ,((((((/                                  
+                   #####%%#,                                         **         
+                       ##%%%#####                              //**             
+                            %%%%#########%.          ######((/                  
+                                   %%%%%#%%%%%%%%%#####                         
+                                   
+                                  by Curated Intelligence   
+
+# MITRE ATT&CK Lookup Tool
+
+[![PyPi license](https://badgen.net/pypi/license/attack-lookup/)](https://pypi.org/project/attack-lookup/) [![PyPi version](https://badgen.net/pypi/v/attack-lookup/)](https://pypi.org/project/attack-lookup/)
+
+`attack-lookup` is a tool that lets you easily check what Tactic, Technique, or Sub-technique ID maps to what name, and vice versa. It can be used interactively, for batch processing, or in your own tooling. 
+
+## Installation
+
+`attack-lookup` can be installed from PyPI:
+
+```
+$ pip install attack-lookup
+```
+
+It can also be installed manually:
+
+```
+$ git clone https://github.com/curated-intel/attack-lookup.git
+$ cd attack-lookup
+$ python setup.py install --user
+```
+
+## Usage
+
+```
+$ attack-lookup --help
+usage: attack-lookup [-h] [-v VERSION] [-m {enterprise,ics,mobile}] [-O] [-i INPUT] [-o OUTPUT] [--output-mode {results,csv}]
+
+MITRE ATT&CK Lookup Tool
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -v VERSION, --version VERSION
+                        ATT&CK matrix version to use (default: v15)
+  -m {enterprise,ics,mobile}, --matrix {enterprise,ics,mobile}
+                        ATT&CK matrix to use (default: enterprise)
+  -O, --offline         Run in offline mode (default: False)
+  -i INPUT, --input INPUT
+                        Path to input file (one lookup value per line) (default: None)
+  -o OUTPUT, --output OUTPUT
+                        Path to output file (default: -)
+  --output-mode {results,csv}
+                        Mode for output file ("result" only has the lookup results, "csv" outputs a CSV with the lookup and result values (default: results)
+```
+
+By default, `attack-lookup` uses the latest version of the Enterprise matrix. When running in Online mode, `attack-lookup` pulls the latest matrix from MITRE's GitHub [repo](https://github.com/mitre/cti). When running in Offline mode, it can use any matrix available in `attack_lookup/data`.
+
+You can use `attack-lookup` in interactive or batch mode:
+
+```
+$ attack-lookup
+(loading latest enterprise matrix...done)
+Running attack-lookup in interactive mode, exit with (q)uit. Enter one or more values to lookup, separated by a comma.
+ATT&CK> T1539
+Steal Web Session Cookie
+ATT&CK>
+```
+
+For batch mode, specify an input file, and optionally an output file/mode. By default, output will go to `stdout`.
+```
+$ attack-lookup -i test
+(loading latest enterprise matrix...done)
+Collection
+T1133
+Peripheral Device Discovery
+
+$ attack-lookup -i test --output-mode=csv
+(loading latest enterprise matrix...done)
+TA0009,Collection
+External Remote Services,T1133
+T1120,Peripheral Device Discovery
+
+$ attack-lookup -i test --output-mode=csv -o out_file
+(loading latest enterprise matrix...done)
+Wrote output data to out_file
+```
+
+If multiple mappings exist (e.g., "Domains"), `attack-lookup` will provide all possible values:
+```
+ATT&CK> Domains
+Multiple possible values: T1583.001, T1584.001
+```
+
+## API
+
+You can also use `attack-lookup` in your own scripts.
+
+```py
+from attack_lookup import AttackMapping
+
+# version is ignored when running online FYSA
+mapping = AttackMapping(matrix="enterprise", version="v15", offline=False)
+
+# load the data
+# this can take ~10sec
+if not mapping.load_data():
+    print("failed to load data")
+else:
+    mapping.lookup("T1574") # returns "Hijack Execution Flow"
+```
```

### Comparing `attack-lookup-1.0.2/README.md` & `attack_lookup-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 usage: attack-lookup [-h] [-v VERSION] [-m {enterprise,ics,mobile}] [-O] [-i INPUT] [-o OUTPUT] [--output-mode {results,csv}]
 
 MITRE ATT&CK Lookup Tool
 
 optional arguments:
   -h, --help            show this help message and exit
   -v VERSION, --version VERSION
-                        ATT&CK matrix version to use (default: v10.1)
+                        ATT&CK matrix version to use (default: v15)
   -m {enterprise,ics,mobile}, --matrix {enterprise,ics,mobile}
                         ATT&CK matrix to use (default: enterprise)
   -O, --offline         Run in offline mode (default: False)
   -i INPUT, --input INPUT
                         Path to input file (one lookup value per line) (default: None)
   -o OUTPUT, --output OUTPUT
                         Path to output file (default: -)
@@ -104,15 +104,15 @@
 
 You can also use `attack-lookup` in your own scripts.
 
 ```py
 from attack_lookup import AttackMapping
 
 # version is ignored when running online FYSA
-mapping = AttackMapping(matrix="enterprise", version="v10.1", offline=False)
+mapping = AttackMapping(matrix="enterprise", version="v15", offline=False)
 
 # load the data
 # this can take ~10sec
 if not mapping.load_data():
     print("failed to load data")
 else:
     mapping.lookup("T1574") # returns "Hijack Execution Flow"
```

### Comparing `attack-lookup-1.0.2/attack_lookup/__main__.py` & `attack_lookup-1.0.3/attack_lookup/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 
 from .mapping import AttackMapping
 
 def parse_args():
     args = argparse.ArgumentParser(prog="attack-lookup", description="MITRE ATT&CK Lookup Tool", formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    args.add_argument("-v", "--version", default="v10.1", help="ATT&CK matrix version to use")
+    args.add_argument("-v", "--version", default="v15", help="ATT&CK matrix version to use")
     args.add_argument("-m", "--matrix", choices=["enterprise", "ics", "mobile"], default="enterprise", help="ATT&CK matrix to use")
     args.add_argument("-O", "--offline", action="store_true", help="Run in offline mode")
 
     args.add_argument("-i", "--input", help="Path to input file (one lookup value per line)")
     args.add_argument("-o", "--output", default="-", help="Path to output file")
     args.add_argument("--output-mode", choices=["results", "csv"], default="results", help="Mode for output file (\"result\" only has the lookup results, \"csv\" outputs a CSV with the lookup and result values")
```

### Comparing `attack-lookup-1.0.2/attack_lookup/mapping.py` & `attack_lookup-1.0.3/attack_lookup/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import requests
 from stix2 import MemoryStore
 from stix2.datastore.filters import Filter
 
 class AttackMapping:
     valid_matrices = ["enterprise", "ics", "mobile"]
 
-    def __init__(self, matrix: str = "enterprise", version: str = "v10.1", offline: bool = False):
+    def __init__(self, matrix: str = "enterprise", version: str = "v15", offline: bool = False):
         if matrix not in AttackMapping.valid_matrices:
             raise ValueError(f"Invalid matrix specified. Valid matrices are: [{', '.join(AttackMapping.valid_matrices)}]")
 
         self.matrix = matrix
 
         if version[0] != "v":
             version = "v" + version
```

### Comparing `attack-lookup-1.0.2/attack_lookup.egg-info/PKG-INFO` & `attack_lookup-1.0.3/attack_lookup.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,134 +1,136 @@
 Metadata-Version: 2.1
 Name: attack-lookup
-Version: 1.0.2
+Version: 1.0.3
 Summary: MITRE ATT&CK Lookup Tool
 Home-page: https://github.com/curated-intel/attack-lookup
 Author: Zander Work
 Author-email: pypi@zanderwork.com
 License: MIT
-Description:                                                                                
-                                                                                        
-                                       %%%%%#########%%%%%                              
-                                ###%%%%##                 &%%%                          
-                           (#####%%          /.. .,,,,&      .%%                        
-                       //((###            . ...**//((... ,     %%                       
-                   ***//((               (..***//((...*#,,,     %%                      
-               *******                  #(#./((((#......,%#(     %                      
-                *****                   @%##....#%%%%%,,%#((     %                      
-                  ****//                 %%%%,,%%%%%%%**/((     #                       
-                     *//((#*               %%,%%%%%##((((      %                        
-                        ((####%               ,((((((/                                  
-                           #####%%#,                                         **         
-                               ##%%%#####                              //**             
-                                    %%%%#########%.          ######((/                  
-                                           %%%%%#%%%%%%%%%#####                         
-                                           
-                                          by Curated Intelligence   
-        
-        # MITRE ATT&CK Lookup Tool
-        
-        [![PyPi license](https://badgen.net/pypi/license/attack-lookup/)](https://pypi.org/project/attack-lookup/) [![PyPi version](https://badgen.net/pypi/v/attack-lookup/)](https://pypi.org/project/attack-lookup/)
-        
-        `attack-lookup` is a tool that lets you easily check what Tactic, Technique, or Sub-technique ID maps to what name, and vice versa. It can be used interactively, for batch processing, or in your own tooling. 
-        
-        ## Installation
-        
-        `attack-lookup` can be installed from PyPI:
-        
-        ```
-        $ pip install attack-lookup
-        ```
-        
-        It can also be installed manually:
-        
-        ```
-        $ git clone https://github.com/curated-intel/attack-lookup.git
-        $ cd attack-lookup
-        $ python setup.py install --user
-        ```
-        
-        ## Usage
-        
-        ```
-        $ attack-lookup --help
-        usage: attack-lookup [-h] [-v VERSION] [-m {enterprise,ics,mobile}] [-O] [-i INPUT] [-o OUTPUT] [--output-mode {results,csv}]
-        
-        MITRE ATT&CK Lookup Tool
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -v VERSION, --version VERSION
-                                ATT&CK matrix version to use (default: v10.1)
-          -m {enterprise,ics,mobile}, --matrix {enterprise,ics,mobile}
-                                ATT&CK matrix to use (default: enterprise)
-          -O, --offline         Run in offline mode (default: False)
-          -i INPUT, --input INPUT
-                                Path to input file (one lookup value per line) (default: None)
-          -o OUTPUT, --output OUTPUT
-                                Path to output file (default: -)
-          --output-mode {results,csv}
-                                Mode for output file ("result" only has the lookup results, "csv" outputs a CSV with the lookup and result values (default: results)
-        ```
-        
-        By default, `attack-lookup` uses the latest version of the Enterprise matrix. When running in Online mode, `attack-lookup` pulls the latest matrix from MITRE's GitHub [repo](https://github.com/mitre/cti). When running in Offline mode, it can use any matrix available in `attack_lookup/data`.
-        
-        You can use `attack-lookup` in interactive or batch mode:
-        
-        ```
-        $ attack-lookup
-        (loading latest enterprise matrix...done)
-        Running attack-lookup in interactive mode, exit with (q)uit. Enter one or more values to lookup, separated by a comma.
-        ATT&CK> T1539
-        Steal Web Session Cookie
-        ATT&CK>
-        ```
-        
-        For batch mode, specify an input file, and optionally an output file/mode. By default, output will go to `stdout`.
-        ```
-        $ attack-lookup -i test
-        (loading latest enterprise matrix...done)
-        Collection
-        T1133
-        Peripheral Device Discovery
-        
-        $ attack-lookup -i test --output-mode=csv
-        (loading latest enterprise matrix...done)
-        TA0009,Collection
-        External Remote Services,T1133
-        T1120,Peripheral Device Discovery
-        
-        $ attack-lookup -i test --output-mode=csv -o out_file
-        (loading latest enterprise matrix...done)
-        Wrote output data to out_file
-        ```
-        
-        If multiple mappings exist (e.g., "Domains"), `attack-lookup` will provide all possible values:
-        ```
-        ATT&CK> Domains
-        Multiple possible values: T1583.001, T1584.001
-        ```
-        
-        ## API
-        
-        You can also use `attack-lookup` in your own scripts.
-        
-        ```py
-        from attack_lookup import AttackMapping
-        
-        # version is ignored when running online FYSA
-        mapping = AttackMapping(matrix="enterprise", version="v10.1", offline=False)
-        
-        # load the data
-        # this can take ~10sec
-        if not mapping.load_data():
-            print("failed to load data")
-        else:
-            mapping.lookup("T1574") # returns "Hijack Execution Flow"
-        ```
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests<3,>=2.22.0
+Requires-Dist: stix2==3.0.1
+
+                                                                               
+                                                                                
+                               %%%%%#########%%%%%                              
+                        ###%%%%##                 &%%%                          
+                   (#####%%          /.. .,,,,&      .%%                        
+               //((###            . ...**//((... ,     %%                       
+           ***//((               (..***//((...*#,,,     %%                      
+       *******                  #(#./((((#......,%#(     %                      
+        *****                   @%##....#%%%%%,,%#((     %                      
+          ****//                 %%%%,,%%%%%%%**/((     #                       
+             *//((#*               %%,%%%%%##((((      %                        
+                ((####%               ,((((((/                                  
+                   #####%%#,                                         **         
+                       ##%%%#####                              //**             
+                            %%%%#########%.          ######((/                  
+                                   %%%%%#%%%%%%%%%#####                         
+                                   
+                                  by Curated Intelligence   
+
+# MITRE ATT&CK Lookup Tool
+
+[![PyPi license](https://badgen.net/pypi/license/attack-lookup/)](https://pypi.org/project/attack-lookup/) [![PyPi version](https://badgen.net/pypi/v/attack-lookup/)](https://pypi.org/project/attack-lookup/)
+
+`attack-lookup` is a tool that lets you easily check what Tactic, Technique, or Sub-technique ID maps to what name, and vice versa. It can be used interactively, for batch processing, or in your own tooling. 
+
+## Installation
+
+`attack-lookup` can be installed from PyPI:
+
+```
+$ pip install attack-lookup
+```
+
+It can also be installed manually:
+
+```
+$ git clone https://github.com/curated-intel/attack-lookup.git
+$ cd attack-lookup
+$ python setup.py install --user
+```
+
+## Usage
+
+```
+$ attack-lookup --help
+usage: attack-lookup [-h] [-v VERSION] [-m {enterprise,ics,mobile}] [-O] [-i INPUT] [-o OUTPUT] [--output-mode {results,csv}]
+
+MITRE ATT&CK Lookup Tool
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -v VERSION, --version VERSION
+                        ATT&CK matrix version to use (default: v15)
+  -m {enterprise,ics,mobile}, --matrix {enterprise,ics,mobile}
+                        ATT&CK matrix to use (default: enterprise)
+  -O, --offline         Run in offline mode (default: False)
+  -i INPUT, --input INPUT
+                        Path to input file (one lookup value per line) (default: None)
+  -o OUTPUT, --output OUTPUT
+                        Path to output file (default: -)
+  --output-mode {results,csv}
+                        Mode for output file ("result" only has the lookup results, "csv" outputs a CSV with the lookup and result values (default: results)
+```
+
+By default, `attack-lookup` uses the latest version of the Enterprise matrix. When running in Online mode, `attack-lookup` pulls the latest matrix from MITRE's GitHub [repo](https://github.com/mitre/cti). When running in Offline mode, it can use any matrix available in `attack_lookup/data`.
+
+You can use `attack-lookup` in interactive or batch mode:
+
+```
+$ attack-lookup
+(loading latest enterprise matrix...done)
+Running attack-lookup in interactive mode, exit with (q)uit. Enter one or more values to lookup, separated by a comma.
+ATT&CK> T1539
+Steal Web Session Cookie
+ATT&CK>
+```
+
+For batch mode, specify an input file, and optionally an output file/mode. By default, output will go to `stdout`.
+```
+$ attack-lookup -i test
+(loading latest enterprise matrix...done)
+Collection
+T1133
+Peripheral Device Discovery
+
+$ attack-lookup -i test --output-mode=csv
+(loading latest enterprise matrix...done)
+TA0009,Collection
+External Remote Services,T1133
+T1120,Peripheral Device Discovery
+
+$ attack-lookup -i test --output-mode=csv -o out_file
+(loading latest enterprise matrix...done)
+Wrote output data to out_file
+```
+
+If multiple mappings exist (e.g., "Domains"), `attack-lookup` will provide all possible values:
+```
+ATT&CK> Domains
+Multiple possible values: T1583.001, T1584.001
+```
+
+## API
+
+You can also use `attack-lookup` in your own scripts.
+
+```py
+from attack_lookup import AttackMapping
+
+# version is ignored when running online FYSA
+mapping = AttackMapping(matrix="enterprise", version="v15", offline=False)
+
+# load the data
+# this can take ~10sec
+if not mapping.load_data():
+    print("failed to load data")
+else:
+    mapping.lookup("T1574") # returns "Hijack Execution Flow"
+```
```

### Comparing `attack-lookup-1.0.2/setup.py` & `attack_lookup-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     deps = [x.strip() for x in f.readlines()]
 
 with open(base_dir / "README.md", "r") as f:
     readme = f.read()
 
 setup(
     name="attack-lookup",
-    version="1.0.2",
+    version="1.0.3",
     description="MITRE ATT&CK Lookup Tool",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/curated-intel/attack-lookup",
     author="Zander Work",
     author_email="pypi@zanderwork.com",
     license="MIT",
```

