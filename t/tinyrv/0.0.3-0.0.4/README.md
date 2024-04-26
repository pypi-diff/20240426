# Comparing `tmp/tinyrv-0.0.3.tar.gz` & `tmp/tinyrv-0.0.4.tar.gz`

## Comparing `tinyrv-0.0.3.tar` & `tinyrv-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0    16686 2020-02-02 00:00:00.000000 tinyrv-0.0.3/tinyrv.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinyrv-0.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tinyrv-0.0.3/LICENSE
--rw-r--r--   0        0        0     7785 2020-02-02 00:00:00.000000 tinyrv-0.0.3/README.md
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tinyrv-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 tinyrv-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    16686 2020-02-02 00:00:00.000000 tinyrv-0.0.4/tinyrv.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 tinyrv-0.0.4/tinyrv_opcodes/arg_lut.csv
+-rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 tinyrv-0.0.4/tinyrv_opcodes/constants.py
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 tinyrv-0.0.4/tinyrv_opcodes/csrs.csv
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 tinyrv-0.0.4/tinyrv_opcodes/csrs32.csv
+-rw-r--r--   0        0        0   236488 2020-02-02 00:00:00.000000 tinyrv-0.0.4/tinyrv_opcodes/instr_dict.yaml
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinyrv-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tinyrv-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7785 2020-02-02 00:00:00.000000 tinyrv-0.0.4/README.md
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tinyrv-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 tinyrv-0.0.4/PKG-INFO
```

### Comparing `tinyrv-0.0.3/tinyrv.py` & `tinyrv-0.0.4/tinyrv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import os, re, csv, struct, array, collections, struct, yaml, importlib.resources, pathlib
 
 try:
-    base = pathlib.Path('.') if pathlib.Path('tinyrv-opcodes').exists() else importlib.resources.files('tinyrv')
-    opcodes = yaml.safe_load(open(base / 'tinyrv-opcodes/instr_dict.yaml'))
+    base = pathlib.Path('.') if pathlib.Path('tinyrv_opcodes').exists() else importlib.resources.files('tinyrv')
+    opcodes = yaml.safe_load(open(base / 'tinyrv_opcodes/instr_dict.yaml'))
     for aname, op in opcodes.items(): op['name'] = aname
     mask_match = [(int(op['mask'], 16), int(op['match'], 16), op) for op in opcodes.values()]
     def dr(h,l): return list(range(h,l-1,-1))
-    arg_bits = dict((a, dr(int(h),int(l))) for a, h, l in csv.reader(open(base / 'tinyrv-opcodes/arg_lut.csv'), skipinitialspace=True))
-    for s in open(base / 'tinyrv-opcodes/constants.py').readlines():  # immediate scrambling from latex_mapping. Some better way?
+    arg_bits = dict((a, dr(int(h),int(l))) for a, h, l in csv.reader(open(base / 'tinyrv_opcodes/arg_lut.csv'), skipinitialspace=True))
+    for s in open(base / 'tinyrv_opcodes/constants.py').readlines():  # immediate scrambling from latex_mapping. Some better way?
         if m := re.match(r"latex_mapping\[['\"](.*?)['\"]\] = ['\"][^\[]*\[([^\]]*)\]['\"]", s):
             fbits = sum([(dr(*(int(i) for i in part.split(':'))) if ':' in part else [int(part)]) for part in m[2].split('$\\\\vert$')], [])
             locs = [-1] * (max(fbits)+1)
             for i, b in enumerate(fbits): locs[-b-1] = arg_bits[m[1]][i]
             arg_bits[m[1]] = [31] * (32-len(locs)) + locs if locs[0] == 31 else locs  # sign extension
-    csrs = dict((int(a, 16), n) for fn in ['tinyrv-opcodes/csrs.csv', 'tinyrv-opcodes/csrs32.csv'] for a, n in csv.reader(open(base / fn), skipinitialspace=True))
+    csrs = dict((int(a, 16), n) for fn in ['tinyrv_opcodes/csrs.csv', 'tinyrv_opcodes/csrs32.csv'] for a, n in csv.reader(open(base / fn), skipinitialspace=True))
     csrs_addrs = dict((n, a) for a, n in csrs.items())
     iregs = 'zero,ra,sp,gp,tp,t0,t1,t2,fp,s1,a0,a1,a2,a3,a4,a5,a6,a7,s2,s3,s4,s5,s6,s7,s8,s9,s10,s11,t3,t4,t5,t6'.split(',')
     st = 'sb,sh,sw,sd'.split(','); ldst = 'lb,lh,lw,ld,lbu,lhu,lwu'.split(',') + st
     fence_flags = ',w,r,rw,o,ow,or,orw,i,iw,ir,irw,io,iow,ior,iorw'.split(',')
     customs = {0b0001011: 'custom0', 0b0101011: 'custom1', 0b1011011: 'custom2', 0b1111011: 'custom3'}  # RISC-V spec ch. 34, table 70
 except Exception as e: raise Exception("Unable to load RISC-V specs. Do:\n"
-                                       "git clone https://github.com/riscv/riscv-opcodes.git tinyrv-opcodes\n"
-                                       "cd tinyrv-opcodes; make")
+                                       "git clone https://github.com/riscv/riscv-opcodes.git tinyrv_opcodes\n"
+                                       "cd tinyrv_opcodes; make")
 
 def xfmt(d, xlen): return f'{{:0{xlen//4}x}}'.format(d&((1<<xlen)-1))
 
 class rvop:
     def __init__(self, **kwargs): [setattr(self, k, v) for k, v in kwargs.items()]
     def arg_str(self):
         args = [None]*4
```

### Comparing `tinyrv-0.0.3/LICENSE` & `tinyrv-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyrv-0.0.3/README.md` & `tinyrv-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -142,18 +142,18 @@
 ## Dev Setup
 
 All code is in `tinyrv.py`.
 No dependencies, except [pyyaml](https://pypi.org/project/PyYAML/).
 However, tinyRV needs to load opcode specs from [riscv-opcodes](https://github.com/riscv/riscv-opcodes).
 Do this:
 ```sh
-git clone https://github.com/riscv/riscv-opcodes.git tinyrv-opcodes
-cd tinyrv-opcodes; make
+git clone https://github.com/riscv/riscv-opcodes.git tinyrv_opcodes
+cd tinyrv_opcodes; make
 ```
-The necessary opcode specs are also bundled in the PyPI package. If there is a `tinyrv-opcodes` in the current directory, tinyRV will try to use those instead of the packaged ones.
+The necessary opcode specs are also bundled in the PyPI package. If there is a `tinyrv_opcodes` in the current directory, tinyRV will try to use those instead of the packaged ones.
 
 ## Testing
 
 Need python (duh!) and [riscv-gnu-toolchain](https://github.com/riscv/riscv-gnu-toolchain). Tested on MacOS.
 
 Install [the RISC-V compatibility framework RISCOF](https://github.com/riscv-software-src/riscof):
 ```sh
```

### Comparing `tinyrv-0.0.3/pyproject.toml` & `tinyrv-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tinyrv"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Stefan Holst", email="mail@s-holst.de" },
 ]
 description = "A tiny RISC-V instruction set simulator"
 readme = "README.md"
 requires-python = ">=3.8"
 requires = ["pyyaml"]
@@ -21,23 +21,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.sdist]
 include = [
   "tinyrv.py",
-  "tinyrv-opcodes/instr_dict.yaml",
-  "tinyrv-opcodes/csrs.csv",
-  "tinyrv-opcodes/csrs32.csv",
-  "tinyrv-opcodes/arg_lut.csv",
-  "tinyrv-opcodes/constants.py",
+  "tinyrv_opcodes/instr_dict.yaml",
+  "tinyrv_opcodes/csrs.csv",
+  "tinyrv_opcodes/csrs32.csv",
+  "tinyrv_opcodes/arg_lut.csv",
+  "tinyrv_opcodes/constants.py",
 ]
 
 [tool.hatch.build.targets.wheel]
 include = [
   "tinyrv.py",
-  "tinyrv-opcodes/instr_dict.yaml",
-  "tinyrv-opcodes/csrs.csv",
-  "tinyrv-opcodes/csrs32.csv",
-  "tinyrv-opcodes/arg_lut.csv",
-  "tinyrv-opcodes/constants.py",
+  "tinyrv_opcodes/instr_dict.yaml",
+  "tinyrv_opcodes/csrs.csv",
+  "tinyrv_opcodes/csrs32.csv",
+  "tinyrv_opcodes/arg_lut.csv",
+  "tinyrv_opcodes/constants.py",
 ]
```

### Comparing `tinyrv-0.0.3/PKG-INFO` & `tinyrv-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tinyrv
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tiny RISC-V instruction set simulator
 Project-URL: Homepage, https://github.com/s-holst/tinyrv
 Project-URL: Issues, https://github.com/s-holst/tinyrv/issues
 Author-email: Stefan Holst <mail@s-holst.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -156,18 +156,18 @@
 ## Dev Setup
 
 All code is in `tinyrv.py`.
 No dependencies, except [pyyaml](https://pypi.org/project/PyYAML/).
 However, tinyRV needs to load opcode specs from [riscv-opcodes](https://github.com/riscv/riscv-opcodes).
 Do this:
 ```sh
-git clone https://github.com/riscv/riscv-opcodes.git tinyrv-opcodes
-cd tinyrv-opcodes; make
+git clone https://github.com/riscv/riscv-opcodes.git tinyrv_opcodes
+cd tinyrv_opcodes; make
 ```
-The necessary opcode specs are also bundled in the PyPI package. If there is a `tinyrv-opcodes` in the current directory, tinyRV will try to use those instead of the packaged ones.
+The necessary opcode specs are also bundled in the PyPI package. If there is a `tinyrv_opcodes` in the current directory, tinyRV will try to use those instead of the packaged ones.
 
 ## Testing
 
 Need python (duh!) and [riscv-gnu-toolchain](https://github.com/riscv/riscv-gnu-toolchain). Tested on MacOS.
 
 Install [the RISC-V compatibility framework RISCOF](https://github.com/riscv-software-src/riscof):
 ```sh
```

