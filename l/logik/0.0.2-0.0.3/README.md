# Comparing `tmp/logik-0.0.2.tar.gz` & `tmp/logik-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logik-0.0.2.tar", last modified: Wed Apr  3 13:57:40 2024, max compression
+gzip compressed data, was "logik-0.0.3.tar", last modified: Fri Apr 26 14:22:51 2024, max compression
```

## Comparing `logik-0.0.2.tar` & `logik-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:40.665618 logik-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-03 13:57:31.000000 logik-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-03 13:57:40.665618 logik-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-03 13:57:31.000000 logik-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:40.661618 logik-0.0.2/logik/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 13:57:31.000000 logik-0.0.2/logik/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:40.661618 logik-0.0.2/logik/flows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:31.000000 logik-0.0.2/logik/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-03 13:57:31.000000 logik-0.0.2/logik/flows/logik_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:40.661618 logik-0.0.2/logik/fpgas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:31.000000 logik-0.0.2/logik/fpgas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 13:57:31.000000 logik-0.0.2/logik/fpgas/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-04-03 13:57:31.000000 logik-0.0.2/logik/fpgas/logik_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:40.661618 logik-0.0.2/logik/targets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:31.000000 logik-0.0.2/logik/targets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-03 13:57:31.000000 logik-0.0.2/logik/targets/logik_target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:40.661618 logik-0.0.2/logik/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:31.000000 logik-0.0.2/logik/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:40.661618 logik-0.0.2/logik/templates/logik_demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:31.000000 logik-0.0.2/logik/templates/logik_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-03 13:57:31.000000 logik-0.0.2/logik/templates/logik_demo/umi_pin_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:40.661618 logik-0.0.2/logik/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:31.000000 logik-0.0.2/logik/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:40.661618 logik-0.0.2/logik/tools/fasm_to_bitstream/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:31.000000 logik-0.0.2/logik/tools/fasm_to_bitstream/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      939 2024-04-03 13:57:31.000000 logik-0.0.2/logik/tools/fasm_to_bitstream/bitstream_bin_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-03 13:57:31.000000 logik-0.0.2/logik/tools/fasm_to_bitstream/bitstream_finish.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10960 2024-04-03 13:57:31.000000 logik-0.0.2/logik/tools/fasm_to_bitstream/fasm_to_bitstream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:40.665618 logik-0.0.2/logik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-03 13:57:40.000000 logik-0.0.2/logik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-03 13:57:40.000000 logik-0.0.2/logik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:57:40.000000 logik-0.0.2/logik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-03 13:57:40.000000 logik-0.0.2/logik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 13:57:40.000000 logik-0.0.2/logik.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 13:57:31.000000 logik-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:57:40.665618 logik-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:51.468989 logik-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-26 14:22:44.000000 logik-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-26 14:22:51.468989 logik-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-26 14:22:44.000000 logik-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:51.464989 logik-0.0.3/logik/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 14:22:44.000000 logik-0.0.3/logik/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:51.464989 logik-0.0.3/logik/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:44.000000 logik-0.0.3/logik/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-26 14:22:44.000000 logik-0.0.3/logik/flows/logik_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:51.464989 logik-0.0.3/logik/fpgas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:44.000000 logik-0.0.3/logik/fpgas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-26 14:22:44.000000 logik-0.0.3/logik/fpgas/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-04-26 14:22:44.000000 logik-0.0.3/logik/fpgas/logik_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:51.464989 logik-0.0.3/logik/targets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:44.000000 logik-0.0.3/logik/targets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-26 14:22:44.000000 logik-0.0.3/logik/targets/logik_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:51.464989 logik-0.0.3/logik/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:44.000000 logik-0.0.3/logik/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:51.464989 logik-0.0.3/logik/templates/logik_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:44.000000 logik-0.0.3/logik/templates/logik_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-26 14:22:44.000000 logik-0.0.3/logik/templates/logik_demo/umi_pin_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:51.464989 logik-0.0.3/logik/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:44.000000 logik-0.0.3/logik/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:51.464989 logik-0.0.3/logik/tools/fasm_to_bitstream/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:44.000000 logik-0.0.3/logik/tools/fasm_to_bitstream/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      939 2024-04-26 14:22:44.000000 logik-0.0.3/logik/tools/fasm_to_bitstream/bitstream_bin_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-26 14:22:44.000000 logik-0.0.3/logik/tools/fasm_to_bitstream/bitstream_finish.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10960 2024-04-26 14:22:44.000000 logik-0.0.3/logik/tools/fasm_to_bitstream/fasm_to_bitstream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:22:51.464989 logik-0.0.3/logik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-26 14:22:51.000000 logik-0.0.3/logik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-26 14:22:51.000000 logik-0.0.3/logik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:22:51.000000 logik-0.0.3/logik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-26 14:22:51.000000 logik-0.0.3/logik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 14:22:51.000000 logik-0.0.3/logik.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-26 14:22:44.000000 logik-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:22:51.468989 logik-0.0.3/setup.cfg
```

### Comparing `logik-0.0.2/LICENSE` & `logik-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logik-0.0.2/PKG-INFO` & `logik-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logik
-Version: 0.0.2
+Version: 0.0.3
 Summary: Logik is a light weight FPGA tool chain based on mature open source technologies.
 Author: Zero ASIC
 License: MIT License
         
         Copyright (c) 2024 Zero ASIC Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -12,75 +12,68 @@
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/zeroasiccorp/logik
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: siliconcompiler==0.21.7
+Requires-Dist: siliconcompiler>=0.21.7
 Provides-Extra: test
 Requires-Dist: pytest==8.1.1; extra == "test"
 Requires-Dist: pytest-timeout==2.3.1; extra == "test"
 Requires-Dist: flake8==7.0.0; extra == "test"
 Provides-Extra: docs
-Requires-Dist: Sphinx==7.2.6; extra == "docs"
+Requires-Dist: Sphinx==7.3.7; extra == "docs"
 Requires-Dist: sphinx-rtd-theme==2.0.0; extra == "docs"
 Requires-Dist: autodocsumm==0.2.12; extra == "docs"
 
-![image info](images/logik_logo_with_text.png)
+![Logik](https://raw.githubusercontent.com/zeroasiccorp/logik/main/images/logik_logo_with_text.png)
 
 [![Regression](https://github.com/zeroasiccorp/logik/actions/workflows/regression.yml/badge.svg)](https://github.com/zeroasiccorp/logik/actions/workflows/regression.yml)
 [![Lint](https://github.com/zeroasiccorp/logik/actions/workflows/lint.yml/badge.svg)](https://github.com/zeroasiccorp/logik/actions/workflows/lint.yml)
 
 -----------------------------------------------------------------------------------
 
-Logik is a light weight FPGA tool chain based on mature open source technologies, including:
+Logik is an open source FPGA toolchain that fully automates converting RTL to bits, including synthesis, placement, routing, bitstream generation, and analysis. Users enter design sources, constraints, and compile options through a simple [SiliconCompiler](https://github.com/siliconcompiler/siliconcompiler/) Python API. Once setup is complete, automated compilation can be initiated with a single line run command.
 
-* [Silicon Compiler](https://github.com/siliconcompiler/siliconcompiler): Hardware compiler framework
-* [Yosys](https://github.com/YosysHQ/yosys): Logic synthesis
-* [VPR](https://github.com/verilog-to-routing/vtr-verilog-to-routing): FPGA place and route
-* [GHDL](https://ghdl.github.io/ghdl/): VHDL parser
-* [Surelog](https://github.com/chipsalliance/Surelog): SystemVerilog parser
-* [FASM](https://github.com/chipsalliance/fasm): FPGA assembly parser and generator
+![logik_flow](https://raw.githubusercontent.com/zeroasiccorp/logik/main/images/logik_flow.svg)
 
-Design sources, constraints, and compile configuration is specified by the user through a simple Python interface. Compilation is managed by the SiliconCompiler framework. Logik supports most of the features you would expect in a commercial proprietary FPGA tool chain.
+Logik supports most of the features you would expect in a commercial proprietary FPGA tool chain.
 
 | Feature                  | Status |
 |--------------------------|--------|
 | Design languages         | Verilog, SystemVerilog, VHDL
 | ALU synthesis            | Supported
 | RAM synthesis            | Supported
 | Timing constraints (SDC) | Supported
 | Pin Constraints (PCF)    | Supported
 | Bitstream generation     | Supported
 | IP management            | Supported
 | Remote compilation       | Supported
 | Multi-clock designs      | In progress
 | FPGA devices             | ZA
 
-![image info](images/logik_flow.svg)
-
 ## Getting Started
 
 The Logik project is available through PyPi and can be installed using pip. If you want to run locally on your machine, you will need to [install all of the pre-requisites](#installation) or launch the [Logik Docker image](#running-docker).
 
 ```sh
 python -m pip install --upgrade logik
 ```
 
-The following example illustrate some essential Logik features. For complete documentation of all options available, see the [SiliconCompiler project](https://github.com/siliconcompiler/siliconcompiler/blob/main/README.md). 
+The following example illustrate some essential Logik features. For complete documentation of all options available, see the [SiliconCompiler project](https://github.com/siliconcompiler/siliconcompiler/blob/main/README.md).
 
 ```python
 from siliconcompiler import Chip
 from logik.targets import logik_target
 
 def hello_adder():
 
     # Create compilation object
-    chip = Chip('adder')                                  
+    chip = Chip('adder')
 
     # Specify design sources
     chip.input('adder.v')
 
     # Specify pin constraints
     chip.input('adder.pcf')
 
@@ -88,15 +81,15 @@
     chip.set('option', 'quiet', True)
     chip.set('option', 'remote', True)
 
     # Select target fpga
     chip.set('fpga', 'partname', 'logik_demo')
 
     # Load target settings
-    chip.load_target(logik_target)                        
+    chip.load_target(logik_target)
 
     # Run compiler
     chip.run()
 
     # Display compiler results
     chip.summary()
 
@@ -125,15 +118,24 @@
 
 Logik is available as wheel packages on PyPI for macOS, Windows and Linux platforms. For a Python 3.8-3.12 environment, just use pip to install.
 
 ```sh
 python -m pip install --upgrade logik
 ```
 
-Running natively on your local machine will require a number of prerequisite tools (Yosys, Surelog, VPR). Automated Ubuntu based install scripts are included for convenience within the SiliconCompiler project. Detailed instructions for installing all tools can be found in the [SiliconCompiler Installation Guide](https://docs.siliconcompiler.com/en/stable/user_guide/installation.html#external-tools).
+Running natively on your local machine will require installing a number of prerequisites:
+
+* [Silicon Compiler](https://github.com/siliconcompiler/siliconcompiler): Hardware compiler framework
+* [Yosys](https://github.com/YosysHQ/yosys): Logic synthesis
+* [VPR](https://github.com/verilog-to-routing/vtr-verilog-to-routing): FPGA place and route
+* [GHDL](https://ghdl.github.io/ghdl/): VHDL parser
+* [Surelog](https://github.com/chipsalliance/Surelog): SystemVerilog parser
+* [FASM](https://github.com/chipsalliance/fasm): FPGA assembly parser and generator
+
+Automated Ubuntu based install scripts are included for convenience within the SiliconCompiler project. Detailed instructions for installing all tools can be found in the [SiliconCompiler Installation Guide](https://docs.siliconcompiler.com/en/stable/user_guide/installation.html#external-tools).
 
 
 ## Running Docker
 
 A [Docker image](https://github.com/siliconcompiler/siliconcompiler/pkgs/container/sc_runner) is provided for users who wish to avoid the installation of the pre-requisite tools. The following command starts a new container from that image and maps the local directory `sc_work` to the path `/sc_work` in the container.
 
 ```sh
```

### Comparing `logik-0.0.2/README.md` & `logik-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,51 @@
-![image info](images/logik_logo_with_text.png)
+![Logik](https://raw.githubusercontent.com/zeroasiccorp/logik/main/images/logik_logo_with_text.png)
 
 [![Regression](https://github.com/zeroasiccorp/logik/actions/workflows/regression.yml/badge.svg)](https://github.com/zeroasiccorp/logik/actions/workflows/regression.yml)
 [![Lint](https://github.com/zeroasiccorp/logik/actions/workflows/lint.yml/badge.svg)](https://github.com/zeroasiccorp/logik/actions/workflows/lint.yml)
 
 -----------------------------------------------------------------------------------
 
-Logik is a light weight FPGA tool chain based on mature open source technologies, including:
+Logik is an open source FPGA toolchain that fully automates converting RTL to bits, including synthesis, placement, routing, bitstream generation, and analysis. Users enter design sources, constraints, and compile options through a simple [SiliconCompiler](https://github.com/siliconcompiler/siliconcompiler/) Python API. Once setup is complete, automated compilation can be initiated with a single line run command.
 
-* [Silicon Compiler](https://github.com/siliconcompiler/siliconcompiler): Hardware compiler framework
-* [Yosys](https://github.com/YosysHQ/yosys): Logic synthesis
-* [VPR](https://github.com/verilog-to-routing/vtr-verilog-to-routing): FPGA place and route
-* [GHDL](https://ghdl.github.io/ghdl/): VHDL parser
-* [Surelog](https://github.com/chipsalliance/Surelog): SystemVerilog parser
-* [FASM](https://github.com/chipsalliance/fasm): FPGA assembly parser and generator
+![logik_flow](https://raw.githubusercontent.com/zeroasiccorp/logik/main/images/logik_flow.svg)
 
-Design sources, constraints, and compile configuration is specified by the user through a simple Python interface. Compilation is managed by the SiliconCompiler framework. Logik supports most of the features you would expect in a commercial proprietary FPGA tool chain.
+Logik supports most of the features you would expect in a commercial proprietary FPGA tool chain.
 
 | Feature                  | Status |
 |--------------------------|--------|
 | Design languages         | Verilog, SystemVerilog, VHDL
 | ALU synthesis            | Supported
 | RAM synthesis            | Supported
 | Timing constraints (SDC) | Supported
 | Pin Constraints (PCF)    | Supported
 | Bitstream generation     | Supported
 | IP management            | Supported
 | Remote compilation       | Supported
 | Multi-clock designs      | In progress
 | FPGA devices             | ZA
 
-![image info](images/logik_flow.svg)
-
 ## Getting Started
 
 The Logik project is available through PyPi and can be installed using pip. If you want to run locally on your machine, you will need to [install all of the pre-requisites](#installation) or launch the [Logik Docker image](#running-docker).
 
 ```sh
 python -m pip install --upgrade logik
 ```
 
-The following example illustrate some essential Logik features. For complete documentation of all options available, see the [SiliconCompiler project](https://github.com/siliconcompiler/siliconcompiler/blob/main/README.md). 
+The following example illustrate some essential Logik features. For complete documentation of all options available, see the [SiliconCompiler project](https://github.com/siliconcompiler/siliconcompiler/blob/main/README.md).
 
 ```python
 from siliconcompiler import Chip
 from logik.targets import logik_target
 
 def hello_adder():
 
     # Create compilation object
-    chip = Chip('adder')                                  
+    chip = Chip('adder')
 
     # Specify design sources
     chip.input('adder.v')
 
     # Specify pin constraints
     chip.input('adder.pcf')
 
@@ -60,15 +53,15 @@
     chip.set('option', 'quiet', True)
     chip.set('option', 'remote', True)
 
     # Select target fpga
     chip.set('fpga', 'partname', 'logik_demo')
 
     # Load target settings
-    chip.load_target(logik_target)                        
+    chip.load_target(logik_target)
 
     # Run compiler
     chip.run()
 
     # Display compiler results
     chip.summary()
 
@@ -97,15 +90,24 @@
 
 Logik is available as wheel packages on PyPI for macOS, Windows and Linux platforms. For a Python 3.8-3.12 environment, just use pip to install.
 
 ```sh
 python -m pip install --upgrade logik
 ```
 
-Running natively on your local machine will require a number of prerequisite tools (Yosys, Surelog, VPR). Automated Ubuntu based install scripts are included for convenience within the SiliconCompiler project. Detailed instructions for installing all tools can be found in the [SiliconCompiler Installation Guide](https://docs.siliconcompiler.com/en/stable/user_guide/installation.html#external-tools).
+Running natively on your local machine will require installing a number of prerequisites:
+
+* [Silicon Compiler](https://github.com/siliconcompiler/siliconcompiler): Hardware compiler framework
+* [Yosys](https://github.com/YosysHQ/yosys): Logic synthesis
+* [VPR](https://github.com/verilog-to-routing/vtr-verilog-to-routing): FPGA place and route
+* [GHDL](https://ghdl.github.io/ghdl/): VHDL parser
+* [Surelog](https://github.com/chipsalliance/Surelog): SystemVerilog parser
+* [FASM](https://github.com/chipsalliance/fasm): FPGA assembly parser and generator
+
+Automated Ubuntu based install scripts are included for convenience within the SiliconCompiler project. Detailed instructions for installing all tools can be found in the [SiliconCompiler Installation Guide](https://docs.siliconcompiler.com/en/stable/user_guide/installation.html#external-tools).
 
 
 ## Running Docker
 
 A [Docker image](https://github.com/siliconcompiler/siliconcompiler/pkgs/container/sc_runner) is provided for users who wish to avoid the installation of the pre-requisite tools. The following command starts a new container from that image and maps the local directory `sc_work` to the path `/sc_work` in the container.
 
 ```sh
```

### Comparing `logik-0.0.2/logik/flows/logik_flow.py` & `logik-0.0.3/logik/flows/logik_flow.py`

 * *Files identical despite different names*

### Comparing `logik-0.0.2/logik/fpgas/_common.py` & `logik-0.0.3/logik/fpgas/_common.py`

 * *Files identical despite different names*

### Comparing `logik-0.0.2/logik/fpgas/logik_demo.py` & `logik-0.0.3/logik/fpgas/logik_demo.py`

 * *Files identical despite different names*

### Comparing `logik-0.0.2/logik/targets/logik_target.py` & `logik-0.0.3/logik/targets/logik_target.py`

 * *Files identical despite different names*

### Comparing `logik-0.0.2/logik/templates/logik_demo/umi_pin_constraints.py` & `logik-0.0.3/logik/templates/logik_demo/umi_pin_constraints.py`

 * *Files identical despite different names*

### Comparing `logik-0.0.2/logik/tools/fasm_to_bitstream/bitstream_bin_convert.py` & `logik-0.0.3/logik/tools/fasm_to_bitstream/bitstream_bin_convert.py`

 * *Files identical despite different names*

### Comparing `logik-0.0.2/logik/tools/fasm_to_bitstream/bitstream_finish.py` & `logik-0.0.3/logik/tools/fasm_to_bitstream/bitstream_finish.py`

 * *Files identical despite different names*

### Comparing `logik-0.0.2/logik/tools/fasm_to_bitstream/fasm_to_bitstream.py` & `logik-0.0.3/logik/tools/fasm_to_bitstream/fasm_to_bitstream.py`

 * *Files identical despite different names*

### Comparing `logik-0.0.2/logik.egg-info/PKG-INFO` & `logik-0.0.3/logik.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logik
-Version: 0.0.2
+Version: 0.0.3
 Summary: Logik is a light weight FPGA tool chain based on mature open source technologies.
 Author: Zero ASIC
 License: MIT License
         
         Copyright (c) 2024 Zero ASIC Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -12,75 +12,68 @@
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 Project-URL: Homepage, https://github.com/zeroasiccorp/logik
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: siliconcompiler==0.21.7
+Requires-Dist: siliconcompiler>=0.21.7
 Provides-Extra: test
 Requires-Dist: pytest==8.1.1; extra == "test"
 Requires-Dist: pytest-timeout==2.3.1; extra == "test"
 Requires-Dist: flake8==7.0.0; extra == "test"
 Provides-Extra: docs
-Requires-Dist: Sphinx==7.2.6; extra == "docs"
+Requires-Dist: Sphinx==7.3.7; extra == "docs"
 Requires-Dist: sphinx-rtd-theme==2.0.0; extra == "docs"
 Requires-Dist: autodocsumm==0.2.12; extra == "docs"
 
-![image info](images/logik_logo_with_text.png)
+![Logik](https://raw.githubusercontent.com/zeroasiccorp/logik/main/images/logik_logo_with_text.png)
 
 [![Regression](https://github.com/zeroasiccorp/logik/actions/workflows/regression.yml/badge.svg)](https://github.com/zeroasiccorp/logik/actions/workflows/regression.yml)
 [![Lint](https://github.com/zeroasiccorp/logik/actions/workflows/lint.yml/badge.svg)](https://github.com/zeroasiccorp/logik/actions/workflows/lint.yml)
 
 -----------------------------------------------------------------------------------
 
-Logik is a light weight FPGA tool chain based on mature open source technologies, including:
+Logik is an open source FPGA toolchain that fully automates converting RTL to bits, including synthesis, placement, routing, bitstream generation, and analysis. Users enter design sources, constraints, and compile options through a simple [SiliconCompiler](https://github.com/siliconcompiler/siliconcompiler/) Python API. Once setup is complete, automated compilation can be initiated with a single line run command.
 
-* [Silicon Compiler](https://github.com/siliconcompiler/siliconcompiler): Hardware compiler framework
-* [Yosys](https://github.com/YosysHQ/yosys): Logic synthesis
-* [VPR](https://github.com/verilog-to-routing/vtr-verilog-to-routing): FPGA place and route
-* [GHDL](https://ghdl.github.io/ghdl/): VHDL parser
-* [Surelog](https://github.com/chipsalliance/Surelog): SystemVerilog parser
-* [FASM](https://github.com/chipsalliance/fasm): FPGA assembly parser and generator
+![logik_flow](https://raw.githubusercontent.com/zeroasiccorp/logik/main/images/logik_flow.svg)
 
-Design sources, constraints, and compile configuration is specified by the user through a simple Python interface. Compilation is managed by the SiliconCompiler framework. Logik supports most of the features you would expect in a commercial proprietary FPGA tool chain.
+Logik supports most of the features you would expect in a commercial proprietary FPGA tool chain.
 
 | Feature                  | Status |
 |--------------------------|--------|
 | Design languages         | Verilog, SystemVerilog, VHDL
 | ALU synthesis            | Supported
 | RAM synthesis            | Supported
 | Timing constraints (SDC) | Supported
 | Pin Constraints (PCF)    | Supported
 | Bitstream generation     | Supported
 | IP management            | Supported
 | Remote compilation       | Supported
 | Multi-clock designs      | In progress
 | FPGA devices             | ZA
 
-![image info](images/logik_flow.svg)
-
 ## Getting Started
 
 The Logik project is available through PyPi and can be installed using pip. If you want to run locally on your machine, you will need to [install all of the pre-requisites](#installation) or launch the [Logik Docker image](#running-docker).
 
 ```sh
 python -m pip install --upgrade logik
 ```
 
-The following example illustrate some essential Logik features. For complete documentation of all options available, see the [SiliconCompiler project](https://github.com/siliconcompiler/siliconcompiler/blob/main/README.md). 
+The following example illustrate some essential Logik features. For complete documentation of all options available, see the [SiliconCompiler project](https://github.com/siliconcompiler/siliconcompiler/blob/main/README.md).
 
 ```python
 from siliconcompiler import Chip
 from logik.targets import logik_target
 
 def hello_adder():
 
     # Create compilation object
-    chip = Chip('adder')                                  
+    chip = Chip('adder')
 
     # Specify design sources
     chip.input('adder.v')
 
     # Specify pin constraints
     chip.input('adder.pcf')
 
@@ -88,15 +81,15 @@
     chip.set('option', 'quiet', True)
     chip.set('option', 'remote', True)
 
     # Select target fpga
     chip.set('fpga', 'partname', 'logik_demo')
 
     # Load target settings
-    chip.load_target(logik_target)                        
+    chip.load_target(logik_target)
 
     # Run compiler
     chip.run()
 
     # Display compiler results
     chip.summary()
 
@@ -125,15 +118,24 @@
 
 Logik is available as wheel packages on PyPI for macOS, Windows and Linux platforms. For a Python 3.8-3.12 environment, just use pip to install.
 
 ```sh
 python -m pip install --upgrade logik
 ```
 
-Running natively on your local machine will require a number of prerequisite tools (Yosys, Surelog, VPR). Automated Ubuntu based install scripts are included for convenience within the SiliconCompiler project. Detailed instructions for installing all tools can be found in the [SiliconCompiler Installation Guide](https://docs.siliconcompiler.com/en/stable/user_guide/installation.html#external-tools).
+Running natively on your local machine will require installing a number of prerequisites:
+
+* [Silicon Compiler](https://github.com/siliconcompiler/siliconcompiler): Hardware compiler framework
+* [Yosys](https://github.com/YosysHQ/yosys): Logic synthesis
+* [VPR](https://github.com/verilog-to-routing/vtr-verilog-to-routing): FPGA place and route
+* [GHDL](https://ghdl.github.io/ghdl/): VHDL parser
+* [Surelog](https://github.com/chipsalliance/Surelog): SystemVerilog parser
+* [FASM](https://github.com/chipsalliance/fasm): FPGA assembly parser and generator
+
+Automated Ubuntu based install scripts are included for convenience within the SiliconCompiler project. Detailed instructions for installing all tools can be found in the [SiliconCompiler Installation Guide](https://docs.siliconcompiler.com/en/stable/user_guide/installation.html#external-tools).
 
 
 ## Running Docker
 
 A [Docker image](https://github.com/siliconcompiler/siliconcompiler/pkgs/container/sc_runner) is provided for users who wish to avoid the installation of the pre-requisite tools. The following command starts a new container from that image and maps the local directory `sc_work` to the path `/sc_work` in the container.
 
 ```sh
```

### Comparing `logik-0.0.2/logik.egg-info/SOURCES.txt` & `logik-0.0.3/logik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logik-0.0.2/pyproject.toml` & `logik-0.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 name = "logik"
 authors = [{name = "Zero ASIC"}]
 description = "Logik is a light weight FPGA tool chain based on mature open source technologies."
 readme = "README.md"
 urls = {Homepage = "https://github.com/zeroasiccorp/logik"}
 requires-python = ">= 3.8"
 dependencies = [
-    "siliconcompiler == 0.21.7",
+    "siliconcompiler >= 0.21.7",
 ]
 license = {file = "LICENSE"}
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "logik.__version__"}
 
 [project.optional-dependencies]
 test = [
     "pytest == 8.1.1",
     "pytest-timeout == 2.3.1",
     "flake8 == 7.0.0"
 ]
 docs = [
-    "Sphinx == 7.2.6",
+    "Sphinx == 7.3.7",
     "sphinx-rtd-theme == 2.0.0",
     "autodocsumm == 0.2.12"
 ]
 
 [tool.setuptools]
 include-package-data = true
```

