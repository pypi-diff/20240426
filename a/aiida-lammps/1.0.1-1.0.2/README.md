# Comparing `tmp/aiida_lammps-1.0.1.tar.gz` & `tmp/aiida_lammps-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_lammps-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_lammps-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_lammps-1.0.1.tar` & `aiida_lammps-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      598 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0     3553 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      504 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/.gitignore
--rw-r--r--   0        0        0      459 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      208 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/.readthedocs.yml
--rw-r--r--   0        0        0     2556 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1087 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/LICENSE
--rw-r--r--   0        0        0     4534 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/README.md
--rw-r--r--   0        0        0       61 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/__init__.py
--rw-r--r--   0        0        0        0 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/calculations/__init__.py
--rw-r--r--   0        0        0    19975 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/calculations/base.py
--rw-r--r--   0        0        0     5858 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/calculations/raw.py
--rw-r--r--   0        0        0        0 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/data/__init__.py
--rw-r--r--   0        0        0    24293 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/data/lammps_potentials.json
--rw-r--r--   0        0        0    27957 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/data/potential.py
--rw-r--r--   0        0        0    10384 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/data/trajectory.py
--rw-r--r--   0        0        0        0 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/parsers/__init__.py
--rw-r--r--   0        0        0    10506 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/parsers/base.py
--rw-r--r--   0        0        0    37639 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/parsers/inputfile.py
--rw-r--r--   0        0        0      366 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/parsers/parse_raw/__init__.py
--rw-r--r--   0        0        0     1174 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/parsers/parse_raw/final_data.py
--rw-r--r--   0        0        0     5044 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/parsers/parse_raw/lammps_output.py
--rw-r--r--   0        0        0     6115 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/parsers/parse_raw/trajectory.py
--rw-r--r--   0        0        0     2064 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/parsers/raw.py
--rw-r--r--   0        0        0     6352 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/parsers/utils.py
--rw-r--r--   0        0        0    14021 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/parsers/variables_types.json
--rw-r--r--   0        0        0      657 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/utils.py
--rw-r--r--   0        0        0      139 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/validation/__init__.py
--rw-r--r--   0        0        0        0 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/validation/schemas/__init__.py
--rw-r--r--   0        0        0    41904 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/validation/schemas/lammps_schema.json
--rw-r--r--   0        0        0      635 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/validation/utils.py
--rw-r--r--   0        0        0        0 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/workflows/__init__.py
--rw-r--r--   0        0        0    12231 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/workflows/base.py
--rw-r--r--   0        0        0     7361 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/workflows/md.py
--rw-r--r--   0        0        0    19052 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/aiida_lammps/workflows/relax.py
--rw-r--r--   0        0        0      162 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/codecov.yml
--rw-r--r--   0        0        0    36362 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/conftest.py
--rw-r--r--   0        0        0      685 2023-11-28 17:18:27.868253 aiida_lammps-1.0.1/docker-compose.yml
--rw-r--r--   0        0        0   744450 2023-11-28 17:18:27.876253 aiida_lammps-1.0.1/examples/Fe_2.eam.fs
--rw-r--r--   0        0        0     7932 2023-11-28 17:18:27.876253 aiida_lammps-1.0.1/examples/calculations/launch_lammps_md.py
--rw-r--r--   0        0        0     7978 2023-11-28 17:18:27.876253 aiida_lammps-1.0.1/examples/calculations/launch_lammps_minimize.py
--rw-r--r--   0        0        0    10328 2023-11-28 17:18:27.876253 aiida_lammps-1.0.1/examples/launch_lammps_base_restart_file.py
--rw-r--r--   0        0        0    10328 2023-11-28 17:18:27.876253 aiida_lammps-1.0.1/examples/launch_lammps_base_restart_folder.py
--rw-r--r--   0        0        0     3155 2023-11-28 17:18:27.876253 aiida_lammps-1.0.1/examples/launch_lammps_base_script.py
--rw-r--r--   0        0        0     1949 2023-11-28 17:18:27.876253 aiida_lammps-1.0.1/examples/launch_lammps_raw_script.py
--rw-r--r--   0        0        0     3827 2023-11-28 17:18:27.876253 aiida_lammps-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6499 1970-01-01 00:00:00.000000 aiida_lammps-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      598 2024-04-26 15:08:32.565932 aiida_lammps-1.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     3726 2024-04-26 15:08:32.565932 aiida_lammps-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      504 2024-04-26 15:08:32.565932 aiida_lammps-1.0.2/.gitignore
+-rw-r--r--   0        0        0      459 2024-04-26 15:08:32.565932 aiida_lammps-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      208 2024-04-26 15:08:32.565932 aiida_lammps-1.0.2/.readthedocs.yml
+-rw-r--r--   0        0        0     2943 2024-04-26 15:08:32.565932 aiida_lammps-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1087 2024-04-26 15:08:32.565932 aiida_lammps-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4534 2024-04-26 15:08:32.565932 aiida_lammps-1.0.2/README.md
+-rw-r--r--   0        0        0      162 2024-04-26 15:08:32.565932 aiida_lammps-1.0.2/codecov.yml
+-rw-r--r--   0        0        0    37775 2024-04-26 15:08:32.565932 aiida_lammps-1.0.2/conftest.py
+-rw-r--r--   0        0        0      685 2024-04-26 15:08:32.565932 aiida_lammps-1.0.2/docker-compose.yml
+-rw-r--r--   0        0        0   744450 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/examples/Fe_2.eam.fs
+-rw-r--r--   0        0        0     7931 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/examples/calculations/launch_lammps_md.py
+-rw-r--r--   0        0        0     7977 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/examples/calculations/launch_lammps_minimize.py
+-rw-r--r--   0        0        0    10327 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/examples/launch_lammps_base_restart_file.py
+-rw-r--r--   0        0        0    10327 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/examples/launch_lammps_base_restart_folder.py
+-rw-r--r--   0        0        0     3155 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/examples/launch_lammps_base_script.py
+-rw-r--r--   0        0        0     1949 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/examples/launch_lammps_raw_script.py
+-rw-r--r--   0        0        0     4087 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/src/aiida_lammps/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/src/aiida_lammps/calculations/__init__.py
+-rw-r--r--   0        0        0    19969 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/src/aiida_lammps/calculations/base.py
+-rw-r--r--   0        0        0     5858 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/src/aiida_lammps/calculations/raw.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/src/aiida_lammps/data/__init__.py
+-rw-r--r--   0        0        0    24293 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/src/aiida_lammps/data/lammps_potentials.json
+-rw-r--r--   0        0        0    27945 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/src/aiida_lammps/data/potential.py
+-rw-r--r--   0        0        0    10384 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/src/aiida_lammps/data/trajectory.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:08:32.569932 aiida_lammps-1.0.2/src/aiida_lammps/parsers/__init__.py
+-rw-r--r--   0        0        0    10536 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/parsers/base.py
+-rw-r--r--   0        0        0    38548 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/parsers/inputfile.py
+-rw-r--r--   0        0        0      366 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/parsers/parse_raw/__init__.py
+-rw-r--r--   0        0        0     1174 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/parsers/parse_raw/final_data.py
+-rw-r--r--   0        0        0     5044 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/parsers/parse_raw/lammps_output.py
+-rw-r--r--   0        0        0     6115 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/parsers/parse_raw/trajectory.py
+-rw-r--r--   0        0        0     2064 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/parsers/raw.py
+-rw-r--r--   0        0        0     6427 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/parsers/utils.py
+-rw-r--r--   0        0        0    14024 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/parsers/variables_types.json
+-rw-r--r--   0        0        0      657 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/utils.py
+-rw-r--r--   0        0        0      139 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/validation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/validation/schemas/__init__.py
+-rw-r--r--   0        0        0    43491 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/validation/schemas/lammps_schema.json
+-rw-r--r--   0        0        0      635 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/validation/utils.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/workflows/__init__.py
+-rw-r--r--   0        0        0    12231 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/workflows/base.py
+-rw-r--r--   0        0        0     7361 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/workflows/md.py
+-rw-r--r--   0        0        0    19052 2024-04-26 15:08:32.573932 aiida_lammps-1.0.2/src/aiida_lammps/workflows/relax.py
+-rw-r--r--   0        0        0     6632 1970-01-01 00:00:00.000000 aiida_lammps-1.0.2/PKG-INFO
```

### Comparing `aiida_lammps-1.0.1/.github/dependabot.yml` & `aiida_lammps-1.0.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/.github/workflows/ci.yml` & `aiida_lammps-1.0.2/.github/workflows/ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -10,41 +10,45 @@
 jobs:
 
   pre-commit:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v4.1.1
-    - name: Set up Python 3.8
-      uses: actions/setup-python@v4
-      with:
-        python-version: "3.8"
-    - uses: pre-commit/action@v3.0.0
+      - uses: actions/checkout@v3.3.0
+      - name: Set up Python
+        uses: actions/setup-python@v4.5.0
+        with:
+          python-version: "3.9"
+      - name: Make sure virtualevn>20 is installed, which will yield newer pip and possibility to pin pip version.
+        run: pip install "virtualenv>20"
+      - name: Install Tox
+        run: pip install tox
+      - name: Run pre-commit in Tox
+        run: tox -e pre-commit
+
 
   tests:
 
     name: pytest (Python ${{ matrix.python-version }}, LAMMPS ${{ matrix.lammps-version }})
 
     timeout-minutes: 30
 
     strategy:
       fail-fast: false
       matrix:
         include:
-          - python-version: "3.8"
-            lammps-version: "2020.03.03"
-          - python-version: "3.8"
-            lammps-version: "2020.12.24"
           - python-version: "3.9"
             lammps-version: "2020.12.24"
           - python-version: "3.9"
-            lammps-version: "2020.03.03"
+            lammps-version: "2022.06.23"
           - python-version: "3.10"
-            lammps-version: "2021.09.29"
+            lammps-version: "2022.06.23"
+          - python-version: "3.11"
+            lammps-version: "2022.06.23"
 
     runs-on: ubuntu-latest
 
     services:
       postgres:
         image: postgres:12
         env:
@@ -83,18 +87,18 @@
       - name: Make sure virtualevn>20 is installed, which will yield newer pip and possibility to pin pip version.
         run: pip install "virtualenv>20"
       - name: Install Tox
         run: pip install tox
 
       - name: Run pytest
         run: |
-          tox -e ${{ matrix.python-version }}-aiida_lammps -- tests/ --cov=./aiida_lammps --cov-append --cov-report=xml --cov-report=term-missing
+          tox -e ${{ matrix.python-version }}-aiida_lammps -- tests/ --cov=aiida_lammps --cov-append --cov-report=xml --cov-report=term-missing
 
       - name: Upload to Codecov
-        if: matrix.python-version == 3.8
+        if: matrix.python-version == 3.10
         uses: codecov/codecov-action@v3
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           name: pytests-lammps
           flags: pytests
           fail_ci_if_error: true
 
@@ -120,15 +124,15 @@
     needs: [pre-commit, tests]
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags')
     runs-on: ubuntu-latest
     steps:
       - name: Checkout source
         uses: actions/checkout@v4.1.1
       - name: Set up Python 3.8
-        uses: actions/setup-python@v4.5.0
+        uses: actions/setup-python@v5
         with:
           python-version: "3.8"
       - name: install flit
         run: |
           pip install flit~=3.4
       - name: Build and publish
         run: |
```

### Comparing `aiida_lammps-1.0.1/CHANGELOG.md` & `aiida_lammps-1.0.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## v1.0.2 2024-04-26
+
+- Fixing an issue in which some LAMMPS vectorial properties were not working properly.
+- Changed how the formatting of the dump command is done to prevent issues from vectorial quantities with undetermined size.
+- Added the capability to override the dimension and boundary commands in LAMMPS.
+- Pinning the version of jsonschema to avoid issues with python>=3.9.
+
 ## v1.0.1 2023-11-28
 
 Minor internal improvements to the code base
 
 ## v1.0.0 2023-11-28
 
 ⬆️ Support for aiida-core >= 2.0.0
```

### Comparing `aiida_lammps-1.0.1/LICENSE` & `aiida_lammps-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/README.md` & `aiida_lammps-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/aiida_lammps/calculations/base.py` & `aiida_lammps-1.0.2/src/aiida_lammps/calculations/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The plugin will take the input parameters validate them against a schema
 and then use them to generate the ``LAMMPS`` input file. The input file
 is generated depending on the parameters provided, the type of potential,
 the input structure and whether or not a restart file is provided.
 """
 import os
-from typing import ClassVar, Dict, Union
+from typing import ClassVar, Union
 
 from aiida import orm
 from aiida.common import datastructures
 from aiida.engine import CalcJob
 
 from aiida_lammps.data.potential import LammpsPotentialData
 from aiida_lammps.data.trajectory import LammpsTrajectory
@@ -26,15 +26,15 @@
 
     The plugin will take the input parameters validate them against a schema
     and then use them to generate the ``LAMMPS`` input file. The input file
     is generated depending on the parameters provided, the type of potential,
     the input structure and whether or not a restart file is provided.
     """
 
-    _DEFAULT_VARIABLES: ClassVar[Dict[str, str]] = {
+    _DEFAULT_VARIABLES: ClassVar[dict[str, str]] = {
         "input_filename": "input.in",
         "structure_filename": "structure.dat",
         "output_filename": "lammps.out",
         "logfile_filename": "log.lammps",
         "variables_filename": "aiida_lammps.yaml",
         "trajectory_filename": "aiida_lammps.trajectory.dump",
         "restart_filename": "lammps.restart",
```

### Comparing `aiida_lammps-1.0.1/aiida_lammps/calculations/raw.py` & `aiida_lammps-1.0.2/src/aiida_lammps/calculations/raw.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/aiida_lammps/data/lammps_potentials.json` & `aiida_lammps-1.0.2/src/aiida_lammps/data/lammps_potentials.json`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/aiida_lammps/data/potential.py` & `aiida_lammps-1.0.2/src/aiida_lammps/data/potential.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import datetime
 
 # pylint: disable=arguments-differ, too-many-public-methods
 import io
 import json
 import os
 import pathlib
-from typing import Any, BinaryIO, ClassVar, Dict, List, Optional, Union
+from typing import Any, BinaryIO, ClassVar, Optional, Union
 import warnings
 
 from aiida import orm, plugins
 from aiida.common.constants import elements
 from aiida.common.exceptions import StoringNotAllowed
 from aiida.common.files import md5_from_filelike
 
@@ -43,15 +43,15 @@
     :rtype: str
     """
     if not isinstance(data, str):
         raise TypeError(f'"{data}" is not of type str')
     return data
 
 
-def _validate_string_list(data: Union[str, List[str]]) -> List[str]:
+def _validate_string_list(data: Union[str, list[str]]) -> list[str]:
     """
     Validate the a list of strings
 
     :param data: string or list of strings
     :type data: Union[str, List[str]]
     :raises TypeError: raise if the data is not of type str or list
     :raises TypeError: raise if an entry in the list is not fo type str
@@ -82,15 +82,15 @@
     if isinstance(data, (float, str)):
         data = int(str(data).strip())
     if isinstance(data, datetime.datetime):
         data = data.year
     return data
 
 
-def _validate_sources(data: Union[dict, List[dict]]) -> List[dict]:
+def _validate_sources(data: Union[dict, list[dict]]) -> list[dict]:
     """
     Validate the sources for the potential.
 
     This checks whether the entry is a dictionary that can be used to describe
     the citation for a potential.
 
     :param data: citation data for a potential
@@ -160,15 +160,15 @@
     _key_md5 = "md5"
 
     _schema_file = os.path.join(
         os.path.dirname(os.path.abspath(__file__)),
         "lammps_potentials.json",
     )
 
-    _extra_keys: ClassVar[Dict[str, Any]] = {
+    _extra_keys: ClassVar[dict[str, Any]] = {
         "title": {"validator": _validate_string},
         "developer": {"validator": _validate_string_list},
         "publication_year": {"validator": _validate_datetime},
         "content_origin": {"validator": _validate_string},
         "content_other_locations": {"validator": _validate_string_list},
         "data_method": {
             "values": ["experiment", "computation", "unknown"],
```

### Comparing `aiida_lammps-1.0.1/aiida_lammps/data/trajectory.py` & `aiida_lammps-1.0.2/src/aiida_lammps/data/trajectory.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/aiida_lammps/parsers/base.py` & `aiida_lammps-1.0.2/src/aiida_lammps/parsers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 It takes care of parsing the lammps.out file, the trajectory file and the
 yaml file with the final value of the variables printed in the ``thermo_style``.
 """
 import glob
 import os
 import time
-from typing import Union
+from typing import Any, Union
 
 from aiida import orm
 from aiida.common import exceptions
 from aiida.parsers.parser import Parser
 import numpy as np
 
 from aiida_lammps.data.trajectory import LammpsTrajectory
@@ -174,16 +174,16 @@
         ):
             self.check_convergence(global_data=global_data)
 
         return None
 
     def parse_restartfile(
         self,
-        parameters: dict,
-        list_of_files: list,
+        parameters: dict[str, Any],
+        list_of_files: list[str],
         temp_folder: Union[os.PathLike, str, None],
     ) -> str:
         """
         Parse the restartfile generated by ``LAMMPS`` and store it as a node in the database.
 
         ``LAMMPS`` can produce several restartfiles, where some are written
         during the simulation at regular intervals, and another that is
@@ -245,16 +245,16 @@
                 latest_file = os.path.basename(restartfiles[np.array(_files).argmax()])
                 restart_filename = latest_file
                 with open(os.path.join(temp_folder, latest_file), mode="rb") as handle:
                     restart_file = orm.SinglefileData(handle)
                 self.out("restartfile", restart_file)
         return restart_filename
 
-    def check_convergence(self, global_data: dict):
-        """Check for the convergence of the calculaiton in the case of a minimization run"""
+    def check_convergence(self, global_data: dict[str, Any]):
+        """Check for the convergence of the calculation in the case of a minimization run"""
         _etol = global_data.get("minimization", {}).get(
             "energy_relative_difference", None
         )
         _ftol = global_data.get("minimization", {}).get("force_two_norm", None)
         _stop_criterion = global_data.get("minimization", {}).get(
             "stop_criterion", None
         )
```

### Comparing `aiida_lammps-1.0.1/aiida_lammps/parsers/inputfile.py` & `aiida_lammps-1.0.2/src/aiida_lammps/parsers/inputfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,30 @@
 blocks will be responsible for printing and/or generate the data that needs to
 be set in the LAMMPS file in accordance to the user defined parameters.
 
 Certain blocks are conditionally called, e.g. if no fixes are specified the
 fixes block is never called, on the other hand the control block is always
 called since it is necessary for the functioning of LAMMPS.
 """
+
 from builtins import ValueError
 import json
 import os
 import re
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
 from aiida import orm
 import numpy as np
 
 from aiida_lammps.data.potential import LammpsPotentialData
 from aiida_lammps.parsers.utils import flatten, generate_header
 
 
 def generate_input_file(
-    parameters: dict,
+    parameters: dict[str, Any],
     potential: LammpsPotentialData,
     structure: orm.StructureData,
     trajectory_filename: str = "aiida_lammps.trajectory.dump",
     restart_filename: str = "lammps.restart",
     potential_filename: str = "potential.dat",
     structure_filename: str = "structure.dat",
     variables_filename: str = "aiida_lammps.yaml",
@@ -169,15 +170,15 @@
         + run_block
         + final_block
         + restart_block["final"]
     )
     return input_file
 
 
-def write_control_block(parameters_control: dict) -> str:
+def write_control_block(parameters_control: dict[str, Any]) -> str:
     """
     Generate the input block with global control options.
 
     This takes the general options that affect the entire simulation, these
     are then used (or their default values) to generate the control block.
 
     :param parameters_control: dictionary with the basic control parameters
@@ -210,15 +211,15 @@
     control_block += generate_header("End of the Control information")
     return control_block
 
 
 def write_potential_block(
     potential: LammpsPotentialData,
     structure: orm.StructureData,
-    parameters_potential: dict,
+    parameters_potential: dict[str, Any],
     potential_file: str,
 ) -> str:
     """
     Generate the input block with potential options.
 
     This will take into consideration the type of potential, as well as other
     parameters which affect the usage of the potential (such as neighbor information)
@@ -267,54 +268,63 @@
             f' {join_keywords(parameters_potential["neighbor_modify"])}\n'
         )
     potential_block += generate_header("End of Potential information")
     return potential_block
 
 
 def write_structure_block(
-    parameters_structure: dict,
+    parameters_structure: dict[str, Any],
     structure: orm.StructureData,
     structure_filename: str,
-) -> Union[str, list]:
+) -> tuple[str, list[str]]:
     """
     Generate the input block with the structure options.
 
     Takes the AiiDA StructureData as well as as a series of user defined
     parameters to generate the structure related input block.
     This is also responsible of defining the distinct groups that can then
     be used for different compute and/or fixes operations.
 
     :param parameters_structure: set of user defined parameters relating to the
         structure.
-    :type parameters_structure: dict
+    :type parameters_structure: Dict[str, Any]
     :param structure: structure that will be studied
     :type structure: orm.StructureData
     :param structure_filename: name of the file where the structure will be
         written so that LAMMPS can read it
     :type structure_filename: str
     :return: block with the structural information and list of groups present
-    :rtype: Union[str, list]
+    :rtype: Tuple[str, List[str]]
     """
 
-    group_names = []
+    group_names: list[str] = []
 
-    kind_name_id_map = {}
+    kind_name_id_map: dict[str, int] = {}
     for site in structure.sites:
         if site.kind_name not in kind_name_id_map:
             kind_name_id_map[site.kind_name] = len(kind_name_id_map) + 1
 
     structure_block = generate_header("Start of the Structure information")
     structure_block += f'box tilt {parameters_structure.get("box_tilt", "small")}\n'
 
-    structure_block += f'dimension {structure.get_dimensionality()["dim"]}\n'
-    structure_block += "boundary "
-    for _bound in ["pbc1", "pbc2", "pbc3"]:
-        structure_block += f'{"p" if structure.base.attributes.all[_bound] else "f"} '
-    structure_block += "\n"
+    # Set the dimensions of the structure
+    if "dimension" in parameters_structure:
+        structure_block += f"dimension {parameters_structure['dimension']}\n"
+    else:
+        structure_block += f"dimension {structure.get_dimensionality()['dim']}\n"
+
+    # Set the boundary conditions of the structure
+    if "boundary" in parameters_structure:
+        structure_block += f"boundary {' '.join(parameters_structure['boundary'])} \n"
+    else:
+        structure_block += f"boundary {' '.join(['p' if entry else 'f' for entry in structure.pbc])} \n"
+
+    # Set the atom style for the structure
     structure_block += f'atom_style {parameters_structure["atom_style"]}\n'
+    # Write the command to read the structure from a file
     structure_block += f"read_data {structure_filename}\n"
     # Set the groups which will be used for the calculations
     if "groups" in parameters_structure:
         for _group in parameters_structure["groups"]:
             # Check if the given type name corresponds to the ones assigned to the atom types
             if "type" in _group["args"]:
                 _subset = _group["args"][_group["args"].index("type") + 1 :]
@@ -327,15 +337,15 @@
             )
             # Store the name of the group for later usage
             group_names.append(_group["name"])
     structure_block += generate_header("End of the Structure information")
     return structure_block, group_names
 
 
-def write_minimize_block(parameters_minimize: dict) -> str:
+def write_minimize_block(parameters_minimize: dict[str, Union[str, float, int]]) -> str:
     """
     Generate the input block with the minimization options.
 
     If the user wishes to do a minimization calculation the parameters will be passed
     to this routine and the necessary block for the input file will be generated.
 
     .. note:: this mode is mutually exclusive with the md mode.
@@ -353,15 +363,15 @@
     minimize_block += f' {parameters_minimize.get("max_iterations", 1000)}'
     minimize_block += f' {parameters_minimize.get("max_evaluations", 1000)}\n'
     minimize_block += generate_header("End of the Minimization information")
 
     return minimize_block
 
 
-def write_md_block(parameters_md: dict) -> str:
+def write_md_block(parameters_md: dict[str, Any]) -> str:
     """
     Generate the input block with the MD options.
 
     If the user wishes to perform an MD run this will take the user defined
     parameters and set them in a LAMMPS compliant form.
 
     .. note:: For MD to function an integrator must be provided, this is done
@@ -402,15 +412,15 @@
     md_block += f'run {parameters_md.get("max_number_steps", 100)}\n'
     md_block += generate_header("End of the MD information")
 
     return md_block
 
 
 def write_final_variables_block(
-    fixed_thermo: list,
+    fixed_thermo: list[str],
     final_file: str = "aiida_lammps.yaml",
 ) -> str:
     """
     Generate the block to print the final values of the compute variables.
 
     This takes all the global computes and other thermo values evaluated in
     the simulation and appends them to a final yaml file for recovery.
@@ -441,15 +451,15 @@
     variables_block += generate_header(
         "End of the Printing Final Variables information"
     )
 
     return variables_block
 
 
-def generate_velocity_string(parameters_velocity: dict) -> str:
+def generate_velocity_string(parameters_velocity: list[dict[str, Any]]) -> str:
     """
     Generate the velocity string for the MD block.
 
     This takes the different possible velocity settings and generate a string
     which is LAMMPS compatible.
 
     :param parameters_velocity: dictionary with the velocity parameters
@@ -460,15 +470,15 @@
     options = ""
     for entry in parameters_velocity:
         _options = generate_velocity_options(entry)
         if "create" in entry:
             options += f'velocity {entry.get("group", "all")} create'
             options += f' {entry["create"].get("temp")}'
             options += (
-                f' {entry["create"].get("seed", np.random.randint(1e4))} {_options}\n'
+                f' {entry["create"].get("seed", np.random.randint(10000))} {_options}\n'
             )
         if "set" in entry:
             options += f'velocity {entry.get("group", "all")} set'
             options += f' {entry["set"].get("vx", "NULL")}'
             options += f' {entry["set"].get("vy", "NULL")}'
             options += f' {entry["set"].get("vz", "NULL")} {_options}\n'
         if "scale" in entry:
@@ -483,15 +493,15 @@
             )
         if "zero" in entry:
             options += f'velocity {entry.get("group", "all")} zero'
             options += f' {entry["zero"]} {_options}\n'
     return options
 
 
-def generate_velocity_options(options_velocity: dict) -> str:
+def generate_velocity_options(options_velocity: dict[str, Any]) -> str:
     """
     Generate the options string for every velocity.
 
     Independent of the way in which one specifies the velocity there are several
     options that are global, this functions allows them to be setup.
 
     :param options_velocity: dictionary with the velocity parameters
@@ -506,15 +516,15 @@
         if _option in options_velocity:
             velocity_option += f" {_option} {options_velocity[_option]} "
     return velocity_option
 
 
 def generate_integration_options(
     style: str,
-    integration_parameters: dict,
+    integration_parameters: dict[str, Any],
 ) -> str:
     """
     Create a string with the integration options.
 
     This will check that the appropriate options are setup for each of the
     supported integrators. These will be appended to a string which is then
     passed to each of the integrators.
@@ -597,44 +607,47 @@
     options = ""
 
     # Set the options that depend on the temperature
     if style in temperature_dependent:
         for _option in temperature_options:
             if _option in integration_parameters:
                 _value = integration_parameters.get(_option)
-                _value = [str(val) for val in _value]
-                options += f' {_option} {" ".join(_value) if isinstance(_value, list) else _value} '
+                if _value:
+                    _value = [str(val) for val in _value]
+                    options += f' {_option} {" ".join(_value) if isinstance(_value, list) else _value} '
     # Set the options that depend on the pressure
     if style in pressure_dependent:
         for _option in pressure_options:
             if _option in integration_parameters:
                 _value = integration_parameters.get(_option)
-                _value = [str(val) for val in _value]
-                options += f' {_option} {" ".join(_value) if isinstance(_value, list) else _value} '
+                if _value:
+                    _value = [str(val) for val in _value]
+                    options += f' {_option} {" ".join(_value) if isinstance(_value, list) else _value} '
     # Set the options that depend on the 'uef' parameters
     if style in uef_dependent:
         for _option in uef_options:
             if _option in integration_parameters:
                 _value = integration_parameters.get(_option)
-                _value = [str(val) for val in _value]
-                options += f' {_option} {" ".join(_value) if isinstance(_value, list) else _value} '
+                if _value:
+                    _value = [str(val) for val in _value]
+                    options += f' {_option} {" ".join(_value) if isinstance(_value, list) else _value} '
     # Set the options that depend on the 'nve/limit' parameters
     if style in ["nve/limit"]:
         options += f' {integration_parameters.get("xmax", 0.1)} '
     # Set the options that depend on the 'langevin' parameters
     if style in ["nve/dotc/langevin"]:
         options += f' {integration_parameters.get("temp")}'
         options += f' {integration_parameters.get("seed")}'
         options += f' angmom {integration_parameters.get("angmom")}'
     return options
 
 
 def write_fix_block(
-    parameters_fix: dict,
-    group_names: Optional[list] = None,
+    parameters_fix: dict[str, Any],
+    group_names: Optional[list[str]] = None,
 ) -> str:
     """
     Generate the input block with the fix options.
 
     This takes the user defined fixes and generates a block where each one of
     them is defined. They can be applied to different groups which can be
     selected by the user and are checked to exist with the previously defined groups
@@ -669,16 +682,16 @@
             fix_block += f"fix {generate_id_tag(key, _group)} {_group} {key} "
             fix_block += f'{join_keywords(entry["type"])}\n'
     fix_block += generate_header("End of the Fix information")
     return fix_block
 
 
 def write_compute_block(
-    parameters_compute: dict,
-    group_names: Optional[list] = None,
+    parameters_compute: dict[str, Any],
+    group_names: Optional[list[str]] = None,
 ) -> str:
     """
     Generate the input block with the compute options.
 
     This takes the user defined computes and generates a block where each one of
     them is defined. They can be applied to different groups which can be
     selected by the user and are checked to exist with the previously defined groups
@@ -705,19 +718,19 @@
             compute_block += f"compute {generate_id_tag(key, _group)} {_group} {key} "
             compute_block += f'{join_keywords(entry["type"])}\n'
     compute_block += generate_header("End of the Compute information")
     return compute_block
 
 
 def write_dump_block(
-    parameters_dump: dict,
+    parameters_dump: dict[str, Any],
     trajectory_filename: str,
     atom_style: str,
-    parameters_compute: Optional[dict] = None,
-    kind_symbols: Optional[list] = None,
+    kind_symbols: list[str],
+    parameters_compute: Optional[dict[str, Any]] = None,
 ) -> str:
     """Generate the block with dumps commands.
 
     This will check for any compute and/or fix that generates atom dependent data
     and will make sure that it is written to file in a controllable manner, so that
     they can be easily parsed afterwards.
 
@@ -738,50 +751,51 @@
     )
 
     with open(_file) as handler:
         _compute_variables = json.load(handler)["computes"]
 
     computes_list = []
 
-    for key, value in parameters_compute.items():
-        for entry in value:
-            _locality = _compute_variables[key]["locality"]
-            _printable = _compute_variables[key]["printable"]
-
-            if _locality == "local" and _printable:
-                computes_list.append(
-                    generate_printing_string(
-                        name=key,
-                        group=entry["group"],
-                        calculation_type="compute",
+    if parameters_compute:
+        for key, value in parameters_compute.items():
+            for entry in value:
+                _locality = _compute_variables[key]["locality"]
+                _printable = _compute_variables[key]["printable"]
+
+                if _locality == "local" and _printable:
+                    computes_list.append(
+                        generate_printing_string(
+                            name=key,
+                            group=entry["group"],
+                            calculation_type="compute",
+                        )
                     )
-                )
 
     num_double = len(list(flatten([compute.split() for compute in computes_list])))
     num_double += 3
     if atom_style == "charge":
         num_double += 1
     dump_block = generate_header("Start of the Dump information")
     dump_block += f'dump aiida all custom {parameters_dump.get("dump_rate", 10)} '
     dump_block += f"{trajectory_filename} id type element x y z "
     dump_block += f'{"q " if atom_style=="charge" else ""}'
     dump_block += f'{" ".join(computes_list)}\n'
     dump_block += "dump_modify aiida sort id\n"
     dump_block += f'dump_modify aiida element {" ".join(kind_symbols)}\n'
-    dump_block += "dump_modify aiida format line "
-    dump_block += f'"%6d %4d %4s {" ".join(["%16.10f"]*num_double)}"\n'
+    dump_block += "dump_modify aiida format int ' %d ' \n"
+    dump_block += "dump_modify aiida format float ' %16.10e ' \n"
     dump_block += generate_header("End of the Dump information")
 
     return dump_block
 
 
 def write_thermo_block(
-    parameters_thermo: dict,
-    parameters_compute: Optional[dict] = None,
-) -> Union[str, list]:
+    parameters_thermo: dict[str, Any],
+    parameters_compute: Optional[dict[str, Any]] = None,
+) -> tuple[str, list[str]]:
     """Generate the block with the thermo command.
 
     This will take all the global computes which were generated during the calculation
     plus the 'common' thermodynamic parameters set by LAMMPS and set them so that
     they are printed to the LAMMPS output file.
 
     :param parameters_thermo: user defined parameters to control the output data.
@@ -800,27 +814,28 @@
     )
 
     with open(_file) as handler:
         _compute_variables = json.load(handler)["computes"]
 
     computes_list = []
 
-    for key, value in parameters_compute.items():
-        for entry in value:
-            _locality = _compute_variables[key]["locality"]
-            _printable = _compute_variables[key]["printable"]
-
-            if _locality == "global" and _printable:
-                computes_list.append(
-                    generate_printing_string(
-                        name=key,
-                        group=entry["group"],
-                        calculation_type="compute",
+    if parameters_compute:
+        for key, value in parameters_compute.items():
+            for entry in value:
+                _locality = _compute_variables[key]["locality"]
+                _printable = _compute_variables[key]["printable"]
+
+                if _locality == "global" and _printable:
+                    computes_list.append(
+                        generate_printing_string(
+                            name=key,
+                            group=entry["group"],
+                            calculation_type="compute",
+                        )
                     )
-                )
 
     computes_printing = parameters_thermo.get("thermo_printing", None)
 
     if computes_printing is None or not computes_printing:
         fixed_thermo = ["step", "temp", "epair", "emol", "etotal", "press"]
     else:
         fixed_thermo = [key for key, value in computes_printing.items() if value]
@@ -844,16 +859,16 @@
         flatten([compute.split() for compute in computes_list])
     )
 
     return thermo_block, printing_variables
 
 
 def write_restart_block(
-    parameters_restart: dict, restart_filename: str, max_number_steps: int
-) -> dict:
+    parameters_restart: dict[str, Any], restart_filename: str, max_number_steps: int
+) -> dict[str, Any]:
     """Generate the block to write the restart file.
 
     :param parameters_restart: set of parameters controlling the printing of the restartfile
     :type parameters_restart: dict
     :param restart_filename: Name of the LAMMPS restart file
     :type restart_filename: str
     :param max_number_steps: maximum number of steps in the simulation
@@ -962,15 +977,15 @@
 
     if _type == "array":
         _string.append(f"{prefactor}_{generate_id_tag(name, group)}")
 
     return " ".join(_string)
 
 
-def generate_id_tag(name: Optional[str] = None, group: Optional[str] = None) -> str:
+def generate_id_tag(name: str, group: str) -> str:
     """Generate an id tag for fixes and/or computes.
 
     To standardize the naming of computes and/or fixes and to ensure that one
     can programmatically recreate them their name will consist of the name of the fix/compute
     with the group at which is applied appended plus the aiida keyword. Of this
     way one can always regenerate these tags by knowing which fix/computes
     were asked of the calculation.
@@ -982,15 +997,15 @@
     :return: if tag for the compute/fix
     :rtype: str
     """
 
     return f"{name.replace('/','_')}_{group}_aiida"
 
 
-def join_keywords(value: list) -> str:
+def join_keywords(value: list[Any]) -> str:
     """
     Generate a string for the compute/fix options.
 
     Depending on the desired fix/compute several options might need to be passed
     to it to dictate its behavior. Having the user pass these options as a single string
     is a bad idea, instead it is simple if the user passes them as a list, where key,value
     pairs dictionaries can be present and or single entries. These items will be
@@ -1001,13 +1016,15 @@
     :type value: list
     :return: LAMMPS compliant string with the fix/compute options
     :rtype: str
     """
 
     return " ".join(
         [
-            f"{entry['keyword']} {entry['value']}"
-            if isinstance(entry, dict)
-            else f"{entry}"
+            (
+                f"{entry['keyword']} {entry['value']}"
+                if isinstance(entry, dict)
+                else f"{entry}"
+            )
             for entry in value
         ]
     )
```

### Comparing `aiida_lammps-1.0.1/aiida_lammps/parsers/parse_raw/final_data.py` & `aiida_lammps-1.0.2/src/aiida_lammps/parsers/parse_raw/final_data.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/aiida_lammps/parsers/parse_raw/lammps_output.py` & `aiida_lammps-1.0.2/src/aiida_lammps/parsers/parse_raw/lammps_output.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/aiida_lammps/parsers/parse_raw/trajectory.py` & `aiida_lammps-1.0.2/src/aiida_lammps/parsers/parse_raw/trajectory.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/aiida_lammps/parsers/raw.py` & `aiida_lammps-1.0.2/src/aiida_lammps/parsers/raw.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/aiida_lammps/parsers/utils.py` & `aiida_lammps-1.0.2/src/aiida_lammps/parsers/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Utility functions for the handling of the input files"""
+
 from collections.abc import Iterable
 from typing import Optional, Union
 
+from aiida import orm
 import numpy as np
 
 
 def _transform_cell(cell) -> Union[np.array, np.array]:
     """Transform the cell to an orientation, compatible with LAMMPS
 
     LAMMPS requires the simulation cell to be in the format of a
@@ -30,17 +32,17 @@
     new_cell = np.dot(inversion, new_cell.T).T
     transform = np.dot(transform, inversion.T).T
 
     return new_cell, transform
 
 
 def generate_lammps_structure(
-    structure,
+    structure: orm.StructureData,
     atom_style: str = "atomic",
-    charge_dict: Optional[dict] = None,
+    charge_dict: Optional[dict[str, float]] = None,
     round_dp: Optional[float] = None,
     docstring: str = "generated by aiida_lammps",
 ) -> Union[str, np.array]:
     """Creation of the structure file content.
 
     As allowing the users to create their lattices using LAMMPS' would be too
     complex, one must ensure that the aiida StructureData is written to file in
@@ -150,30 +152,30 @@
     for element in full_list:
         if isinstance(element, Iterable) and not isinstance(element, (str, bytes)):
             yield from flatten(element)
         else:
             yield element
 
 
-def convert_to_str(value):
+def convert_to_str(value) -> str:
     """convert True/False to yes/no and all values to strings"""
     if isinstance(value, bool):
         if value:
             return "yes"
         return "no"
     return str(value)
 
 
-def _convert_values(value):
+def _convert_values(value) -> str:
     if isinstance(value, (tuple, list)):
         return " ".join([convert_to_str(v) for v in value])
     return convert_to_str(value)
 
 
-def join_keywords(dct, ignore=None):
+def join_keywords(dct, ignore=None) -> str:
     """join a dict of {keyword: value, ...} into a string 'keyword value ...'
 
     value can be a single value or a list/tuple of values
     """
     ignore = ignore if ignore else []
     return " ".join(
         [
```

### Comparing `aiida_lammps-1.0.1/aiida_lammps/parsers/variables_types.json` & `aiida_lammps-1.0.2/src/aiida_lammps/parsers/variables_types.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993708053691275%*

 * *Differences: {"'computes'": "{'property/atom': {'type': 'vector'}, 'property/chunk': {'type': 'vector'}, "*

 * *               "'property/local': {'type': 'vector'}}"}*

```diff
@@ -474,27 +474,27 @@
             "size": 0,
             "type": "scalar"
         },
         "property/atom": {
             "locality": "local",
             "printable": true,
             "size": 0,
-            "type": "array"
+            "type": "vector"
         },
         "property/chunk": {
             "locality": "global",
             "printable": false,
             "size": 0,
-            "type": "array"
+            "type": "vector"
         },
         "property/local": {
             "locality": "global",
             "printable": true,
             "size": 0,
-            "type": "array"
+            "type": "vector"
         },
         "ptm/atom": {
             "locality": "local",
             "printable": true,
             "size": 0,
             "type": "scalar"
         },
```

### Comparing `aiida_lammps-1.0.1/aiida_lammps/utils.py` & `aiida_lammps-1.0.2/src/aiida_lammps/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/aiida_lammps/validation/schemas/lammps_schema.json` & `aiida_lammps-1.0.2/src/aiida_lammps/validation/schemas/lammps_schema.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333333%*

 * *Differences: {"'structure'": "{'properties': {'dimension': OrderedDict([('type', 'integer'), ('propertyNames', "*

 * *                "OrderedDict([('enum', [2, 3])]))]), 'boundary': OrderedDict([('type', 'array'), "*

 * *                "('minItems', 3), ('maxItems', 3), ('items', [OrderedDict([('description', "*

 * *                "'boundary conditions along the a-direction'), ('type', 'string'), ('enum', ['p', "*

 * *                "'f', 's', 'm', 'pp', 'pf', 'ps', 'pm', 'fp', 'ff', 'fs', 'fm', 'sp', 'sf', 'ss', "*

 * *                "'sm […]*

```diff
@@ -1145,22 +1145,72 @@
                         "tri",
                         "template",
                         "hybrid"
                     ]
                 },
                 "type": "string"
             },
+            "boundary": {
+                "items": [
+                    {
+                        "description": "boundary conditions along the a-direction",
+                        "enum": [
+                            "p",
+                            "f",
+                            "s",
+                            "m",
+                            "pp",
+                            "pf",
+                            "ps",
+                            "pm",
+                            "fp",
+                            "ff",
+                            "fs",
+                            "fm",
+                            "sp",
+                            "sf",
+                            "ss",
+                            "sm",
+                            "mp",
+                            "mf",
+                            "ms",
+                            "mm"
+                        ],
+                        "type": "string"
+                    },
+                    {
+                        "description": "boundary conditions along the b-direction",
+                        "type": "string"
+                    },
+                    {
+                        "description": "boundary conditions along the c-direction",
+                        "type": "string"
+                    }
+                ],
+                "maxItems": 3,
+                "minItems": 3,
+                "type": "array"
+            },
             "box_tilt": {
                 "propertyNames": {
                     "enum": [
                         "small",
                         "large"
                     ]
                 },
                 "type": "string"
+            },
+            "dimension": {
+                "propertyNames": {
+                    "enum": [
+                        2,
+                        3
+                    ]
+                },
+                "type": "integer"
             }
         },
         "type": "object"
     },
     "then": {
         "properties": {
             "fix": {
```

### Comparing `aiida_lammps-1.0.1/aiida_lammps/validation/utils.py` & `aiida_lammps-1.0.2/src/aiida_lammps/validation/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/aiida_lammps/workflows/base.py` & `aiida_lammps-1.0.2/src/aiida_lammps/workflows/base.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/aiida_lammps/workflows/md.py` & `aiida_lammps-1.0.2/src/aiida_lammps/workflows/md.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/aiida_lammps/workflows/relax.py` & `aiida_lammps-1.0.2/src/aiida_lammps/workflows/relax.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/conftest.py` & `aiida_lammps-1.0.2/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """
 initialise a test database and profile
 """
+
 # pylint: disable=redefined-outer-name
 from __future__ import annotations
 
 from collections.abc import Mapping
 from contextlib import suppress
 import os
 import pathlib
 import shutil
 import tempfile
 from typing import Any
 
 from aiida import orm
 from aiida.common import AttributeDict, CalcInfo, LinkType, exceptions
-from aiida.engine import CalcJob
+from aiida.engine import Process
 from aiida.engine.utils import instantiate_process
 from aiida.manage.manager import get_manager
 from aiida.plugins import WorkflowFactory
 from aiida.plugins.entry_point import format_entry_point_string
+from aiida_lammps.calculations.base import LammpsBaseCalculation
+from aiida_lammps.data.potential import LammpsPotentialData
+from aiida_lammps.data.trajectory import LammpsTrajectory
 import numpy as np
 import pytest
 import yaml
 
-from aiida_lammps.calculations.base import LammpsBaseCalculation
-from aiida_lammps.data.potential import LammpsPotentialData
-from aiida_lammps.data.trajectory import LammpsTrajectory
 from tests.utils import TEST_DIR, AiidaTestApp
 
 pytest_plugins = ["aiida.manage.tests.pytest_fixtures"]
 
 
 def pytest_addoption(parser):
     """Define pytest command-line."""
@@ -65,14 +66,20 @@
     return [
         f'LAMMPS Executable: {shutil.which(config.getoption("lammps_exec") or "lammps")}',
         f'LAMMPS Work Directory: {config.getoption("lammps_workdir") or "<TEMP>"}',
     ]
 
 
 @pytest.fixture
+def structure_parameters() -> AttributeDict:
+    parameteters = AttributeDict({"dimension": 2, "boundary": ["p", "p", "f"]})
+    return parameteters
+
+
+@pytest.fixture
 def filepath_tests() -> pathlib.Path:
     """Return the path to the tests folder."""
     return pathlib.Path(__file__).resolve().parent / "tests"
 
 
 @pytest.fixture
 def fixture_localhost(aiida_localhost):
@@ -115,14 +122,23 @@
     parameters.control.units = "metal"
     parameters.control.timestep = 1e-5
     parameters.compute = {
         "pe/atom": [{"type": [{"keyword": " ", "value": " "}], "group": "all"}],
         "ke/atom": [{"type": [{"keyword": " ", "value": " "}], "group": "all"}],
         "stress/atom": [{"type": ["NULL"], "group": "all"}],
         "pressure": [{"type": ["thermo_temp"], "group": "all"}],
+        "property/atom": [
+            {
+                "type": [
+                    {"keyword": " ", "value": "fx"},
+                    {"keyword": " ", "value": "fy"},
+                ],
+                "group": "all",
+            }
+        ],
     }
 
     parameters.minimize = {
         "style": "cg",
         "energy_tolerance": 1e-5,
         "force_tolerance": 1e-5,
         "max_evaluations": 5000,
@@ -167,14 +183,23 @@
     parameters.control.timestep = 1e-5
     parameters.compute = {
         "pe/atom": [{"type": [{"keyword": " ", "value": " "}], "group": "all"}],
         "ke/atom": [{"type": [{"keyword": " ", "value": " "}], "group": "all"}],
         "stress/atom": [{"type": ["NULL"], "group": "all"}],
         "pressure": [{"type": ["thermo_temp"], "group": "all"}],
         "ke": [{"type": [{"keyword": " ", "value": " "}], "group": "test"}],
+        "property/atom": [
+            {
+                "type": [
+                    {"keyword": " ", "value": "fx"},
+                    {"keyword": " ", "value": "fy"},
+                ],
+                "group": "all",
+            }
+        ],
     }
 
     parameters.minimize = {
         "style": "cg",
         "energy_tolerance": 1e-5,
         "force_tolerance": 1e-5,
     }
@@ -214,14 +239,23 @@
     parameters.control.units = "metal"
     parameters.control.timestep = 1e-5
     parameters.compute = {
         "pe/atom": [{"type": [{"keyword": " ", "value": " "}], "group": "all"}],
         "ke/atom": [{"type": [{"keyword": " ", "value": " "}], "group": "all"}],
         "stress/atom": [{"type": ["NULL"], "group": "all"}],
         "pressure": [{"type": ["thermo_temp"], "group": "all"}],
+        "property/atom": [
+            {
+                "type": [
+                    {"keyword": " ", "value": "fx"},
+                    {"keyword": " ", "value": "fy"},
+                ],
+                "group": "all",
+            }
+        ],
     }
     parameters.md = {
         "integration": {
             "style": "nve",
         },
         "max_number_steps": 5000,
     }
@@ -258,14 +292,23 @@
     parameters.control.units = "metal"
     parameters.control.timestep = 1e-5
     parameters.compute = {
         "pe/atom": [{"type": [{"keyword": " ", "value": " "}], "group": "all"}],
         "ke/atom": [{"type": [{"keyword": " ", "value": " "}], "group": "all"}],
         "stress/atom": [{"type": ["NULL"], "group": "all"}],
         "pressure": [{"type": ["thermo_temp"], "group": "all"}],
+        "property/atom": [
+            {
+                "type": [
+                    {"keyword": " ", "value": "fx"},
+                    {"keyword": " ", "value": "fy"},
+                ],
+                "group": "all",
+            }
+        ],
     }
     parameters.md = {
         "integration": {
             "style": "nvt",
             "constraints": {
                 "temp": [400, 400, 100],
             },
@@ -305,14 +348,23 @@
     parameters.control.units = "metal"
     parameters.control.timestep = 1e-5
     parameters.compute = {
         "pe/atom": [{"type": [{"keyword": " ", "value": " "}], "group": "all"}],
         "ke/atom": [{"type": [{"keyword": " ", "value": " "}], "group": "all"}],
         "stress/atom": [{"type": ["NULL"], "group": "all"}],
         "pressure": [{"type": ["thermo_temp"], "group": "all"}],
+        "property/atom": [
+            {
+                "type": [
+                    {"keyword": " ", "value": "fx"},
+                    {"keyword": " ", "value": "fy"},
+                ],
+                "group": "all",
+            }
+        ],
     }
     parameters.md = {
         "integration": {
             "style": "npt",
             "constraints": {
                 "temp": [400, 400, 100],
                 "iso": [0.0, 0.0, 1000.0],
@@ -561,15 +613,15 @@
     as well as the ``CalcInfo`` instance that it returned.
     """
 
     def factory(
         entry_point_name: str,
         inputs: dict[str, Any] | None = None,
         return_process: bool = False,
-    ) -> tuple[pathlib.Path, CalcInfo] | CalcJob:
+    ) -> tuple[pathlib.Path, CalcInfo] | Process:
         """Create a :class:`aiida.engine.CalcJob` instance with the given inputs.
 
         :param entry_point_name: The entry point name of the calculation job plugin to run.
         :param inputs: The dictionary of inputs for the calculation job.
         :param return_process: Flag, if ``True``, return the constructed ``CalcJob`` instance instead of the tuple of
             the temporary folder and ``CalcInfo`` instance.
         """
```

### Comparing `aiida_lammps-1.0.1/docker-compose.yml` & `aiida_lammps-1.0.2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/examples/Fe_2.eam.fs` & `aiida_lammps-1.0.2/examples/Fe_2.eam.fs`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/examples/calculations/launch_lammps_md.py` & `aiida_lammps-1.0.2/examples/calculations/launch_lammps_md.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Sets up an example for the calculation of bcc Fe using ``aiida-lammps``.
 """
 from aiida import orm
 from aiida.common.extendeddicts import AttributeDict
 from aiida.engine import run_get_node
 from aiida.plugins import CalculationFactory
-import numpy as np
-
 from aiida_lammps.data.potential import LammpsPotentialData
+import numpy as np
 
 
 def generate_structure() -> orm.StructureData:
     """
     Generates the structure for the calculation.
 
     It will create a bcc structure in a cubic lattice.
```

### Comparing `aiida_lammps-1.0.1/examples/calculations/launch_lammps_minimize.py` & `aiida_lammps-1.0.2/examples/calculations/launch_lammps_minimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Sets up an example for the calculation of bcc Fe using ``aiida-lammps``.
 """
 from aiida import orm
 from aiida.common.extendeddicts import AttributeDict
 from aiida.engine import run_get_node
 from aiida.plugins import CalculationFactory
-import numpy as np
-
 from aiida_lammps.data.potential import LammpsPotentialData
+import numpy as np
 
 
 def generate_structure() -> orm.StructureData:
     """
     Generates the structure for the calculation.
 
     It will create a bcc structure in a cubic lattice.
```

### Comparing `aiida_lammps-1.0.1/examples/launch_lammps_base_restart_file.py` & `aiida_lammps-1.0.2/examples/launch_lammps_base_restart_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Sets up an example for the calculation of bcc Fe using ``aiida-lammps``.
 """
 from aiida import orm
 from aiida.common.extendeddicts import AttributeDict
 from aiida.engine import run_get_node
 from aiida.plugins import CalculationFactory
-import numpy as np
-
 from aiida_lammps.data.potential import LammpsPotentialData
+import numpy as np
 
 
 def generate_structure() -> orm.StructureData:
     """
     Generates the structure for the calculation.
 
     It will create a bcc structure in a cubic lattice.
```

### Comparing `aiida_lammps-1.0.1/examples/launch_lammps_base_restart_folder.py` & `aiida_lammps-1.0.2/examples/launch_lammps_base_restart_folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 Sets up an example for the calculation of bcc Fe using ``aiida-lammps``.
 """
 from aiida import orm
 from aiida.common.extendeddicts import AttributeDict
 from aiida.engine import run_get_node
 from aiida.plugins import CalculationFactory
-import numpy as np
-
 from aiida_lammps.data.potential import LammpsPotentialData
+import numpy as np
 
 
 def generate_structure() -> orm.StructureData:
     """
     Generates the structure for the calculation.
 
     It will create a bcc structure in a cubic lattice.
```

### Comparing `aiida_lammps-1.0.1/examples/launch_lammps_base_script.py` & `aiida_lammps-1.0.2/examples/launch_lammps_base_script.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/examples/launch_lammps_raw_script.py` & `aiida_lammps-1.0.2/examples/launch_lammps_raw_script.py`

 * *Files identical despite different names*

### Comparing `aiida_lammps-1.0.1/pyproject.toml` & `aiida_lammps-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,73 @@
 [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "aiida-lammps"
 dynamic = ["version", "description"]
-authors = [{name = "Chris Sewell", email = "chrisj_sewell@hotmail.com"}, {name = "Jonathan Chico", email = "jonathan.chico@sandvik.com"}]
+authors = [
+    { name = "Chris Sewell", email = "chrisj_sewell@hotmail.com" },
+    { name = "Jonathan Chico", email = "jonathan.chico@sandvik.com" },
+]
 readme = "README.md"
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Scientific/Engineering :: Physics",
-    "Framework :: AiiDA"
+    "Framework :: AiiDA",
 ]
 keywords = ["aiida", "workflows", "lammps"]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = [
-    "aiida-core[atomic_tools]>=2.0.0,<3.0.0",
+    "aiida-core[atomic_tools]~=2.3",
     "importlib_resources",
-    "jsonschema",
+    "jsonschema~=3.2.0",
     "numpy",
     "packaging",
-    "python-dateutil"
+    "python-dateutil",
 ]
 
 [project.urls]
 Documentation = "https://aiida-lammps.readthedocs.io"
 Source = "https://github.com/aiidaplugins/aiida-lammps"
 
 [project.optional-dependencies]
 tests = [
     'pgtest~=1.3',
     'pytest~=7.4',
     'pytest-regressions~=2.3',
     "pytest-cov",
     "coverage",
     "pytest-timeout",
-    "pytest-regressions"
+    "pytest-regressions",
 ]
 
 docs = [
     'sphinx~=6.2.1',
     'sphinx-copybutton~=0.5.2',
     'sphinx-book-theme~=1.0.1',
     'sphinx-click~=5.1.0',
-    'sphinx-design~=0.4.1',
+    'sphinx-design~=0.5.0',
     'sphinxcontrib-details-directive~=0.1.0',
     'sphinx-autoapi~=3.0',
     'myst_parser~=2.0.0',
-    "furo"
+    "furo",
 ]
 
+pre-commit = ['pre-commit~=2.17']
+
 [project.entry-points."aiida.calculations"]
 "lammps.base" = "aiida_lammps.calculations.base:LammpsBaseCalculation"
 "lammps.raw" = "aiida_lammps.calculations.raw:LammpsRawCalculation"
 
 [project.entry-points."aiida.parsers"]
 "lammps.base" = "aiida_lammps.parsers.base:LammpsBaseParser"
 "lammps.raw" = "aiida_lammps.parsers.raw:LammpsRawParser"
@@ -75,49 +81,54 @@
 "lammps.relax" = "aiida_lammps.workflows.relax:LammpsRelaxWorkChain"
 "lammps.md" = "aiida_lammps.workflows.md:LammpsMDWorkChain"
 
 [tool.flit.module]
 name = "aiida_lammps"
 
 [tool.flit.sdist]
-exclude = [
-    "docs/",
-    "tests/",
-]
+exclude = ["docs/", "tests/"]
 
 [tool.coverage.run]
 # Configuration of [coverage.py](https://coverage.readthedocs.io)
 # reporting which lines of your plugin are covered by tests
-source=["aiida_lammps"]
+source = ["src"]
+
 
 [tool.ruff]
 extend-select = ["B0", "C4", "I", "ICN", "ISC", "N", "RUF", "SIM", "UP"]
 extend-ignore = ["B028", "ISC001"]
 
 [tool.ruff.lint.isort]
 force-sort-within-sections = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = pre-commit,{3.8,3.9,3.10}-aiida_lammps
+envlist = pre-commit,{3.9,3.10,3.11}-aiida_lammps
 requires = virtualenv >= 20
 isolated_build = True
 
 [testenv]
 setenv = AIIDA_PATH={toxworkdir}/.aiida
 allowlist_externals =
                     mkdir
                     rm
 commands =
 	 mkdir -p {toxworkdir}/.aiida
 	 pytest --lammps-exec lmp_serial {posargs}
 	 rm -r {toxworkdir}/.aiida
 extras = tests
 
+[testenv:pre-commit]
+allowlist_externals = bash
+commands = bash -ec 'pre-commit run --all-files || ( git diff; git status; exit 1; )'
+extras =
+       pre-commit
+       tests
+
 [testenv:docs-{clean,update}]
 extras = docs
 description =
     clean: Build the documentation (remove any existing build)
     update: Build the documentation (modify any existing build)
 passenv = RUN_APIDOC
 setenv =
```

### Comparing `aiida_lammps-1.0.1/PKG-INFO` & `aiida_lammps-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 Metadata-Version: 2.1
 Name: aiida-lammps
-Version: 1.0.1
+Version: 1.0.2
 Summary: AiiDA plugin for the LAMMPS code
 Keywords: aiida,workflows,lammps
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>, Jonathan Chico <jonathan.chico@sandvik.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Framework :: AiiDA
-Requires-Dist: aiida-core[atomic_tools]>=2.0.0,<3.0.0
+Requires-Dist: aiida-core[atomic_tools]~=2.3
 Requires-Dist: importlib_resources
-Requires-Dist: jsonschema
+Requires-Dist: jsonschema~=3.2.0
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: python-dateutil
 Requires-Dist: sphinx~=6.2.1 ; extra == "docs"
 Requires-Dist: sphinx-copybutton~=0.5.2 ; extra == "docs"
 Requires-Dist: sphinx-book-theme~=1.0.1 ; extra == "docs"
 Requires-Dist: sphinx-click~=5.1.0 ; extra == "docs"
-Requires-Dist: sphinx-design~=0.4.1 ; extra == "docs"
+Requires-Dist: sphinx-design~=0.5.0 ; extra == "docs"
 Requires-Dist: sphinxcontrib-details-directive~=0.1.0 ; extra == "docs"
 Requires-Dist: sphinx-autoapi~=3.0 ; extra == "docs"
 Requires-Dist: myst_parser~=2.0.0 ; extra == "docs"
 Requires-Dist: furo ; extra == "docs"
+Requires-Dist: pre-commit~=2.17 ; extra == "pre-commit"
 Requires-Dist: pgtest~=1.3 ; extra == "tests"
 Requires-Dist: pytest~=7.4 ; extra == "tests"
 Requires-Dist: pytest-regressions~=2.3 ; extra == "tests"
 Requires-Dist: pytest-cov ; extra == "tests"
 Requires-Dist: coverage ; extra == "tests"
 Requires-Dist: pytest-timeout ; extra == "tests"
 Requires-Dist: pytest-regressions ; extra == "tests"
 Project-URL: Documentation, https://aiida-lammps.readthedocs.io
 Project-URL: Source, https://github.com/aiidaplugins/aiida-lammps
 Provides-Extra: docs
+Provides-Extra: pre-commit
 Provides-Extra: tests
 
 [![CI Status](https://github.com/aiidaplugins/aiida-lammps/workflows/CI/badge.svg)](https://github.com/aiidaplugins/aiida-lammps)
 [![Coverage Status](https://codecov.io/gh/aiidaplugins/aiida-lammps/branch/master/graph/badge.svg)](https://codecov.io/gh/aiidaplugins/aiida-lammps)
 [![PyPI](https://img.shields.io/pypi/v/aiida-lammps.svg)](https://pypi.python.org/pypi/aiida-lammps/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Docs status](https://readthedocs.org/projects/aiida-lammps/badge)](http://aiida-lammps.readthedocs.io/)
```

