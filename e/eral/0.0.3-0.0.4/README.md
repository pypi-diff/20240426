# Comparing `tmp/eral-0.0.3.tar.gz` & `tmp/eral-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eral-0.0.3.tar", last modified: Fri Apr 26 11:02:01 2024, max compression
+gzip compressed data, was "eral-0.0.4.tar", last modified: Fri Apr 26 11:14:01 2024, max compression
```

## Comparing `eral-0.0.3.tar` & `eral-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 11:02:01.449059 eral-0.0.3/
--rw-rw-rw-   0        0        0     3355 2024-04-26 11:02:01.446059 eral-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2556 2024-04-26 10:09:06.000000 eral-0.0.3/README.md
--rw-rw-rw-   0        0        0      793 2024-04-26 11:01:13.000000 eral-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 11:02:01.450059 eral-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-26 11:02:01.358059 eral-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 11:02:01.403058 eral-0.0.3/src/eral/
--rw-rw-rw-   0        0        0        0 2023-10-25 13:21:15.000000 eral-0.0.3/src/eral/__init__.py
--rw-rw-rw-   0        0        0     9222 2024-04-12 09:13:29.000000 eral-0.0.3/src/eral/alignment_prototyping_functions.py
--rw-rw-rw-   0        0        0     8236 2024-04-10 12:02:33.000000 eral-0.0.3/src/eral/eral.py
--rw-rw-rw-   0        0        0     4313 2024-04-10 11:36:54.000000 eral-0.0.3/src/eral/eral_score.py
--rw-rw-rw-   0        0        0     7492 2024-04-10 12:12:14.000000 eral-0.0.3/src/eral/time_series_alignment.py
--rw-rw-rw-   0        0        0     1957 2024-02-18 16:15:48.000000 eral-0.0.3/src/eral/time_series_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-26 11:02:01.443059 eral-0.0.3/src/eral.egg-info/
--rw-rw-rw-   0        0        0     3355 2024-04-26 11:02:01.000000 eral-0.0.3/src/eral.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-04-26 11:02:01.000000 eral-0.0.3/src/eral.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 11:02:01.000000 eral-0.0.3/src/eral.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      177 2024-04-26 11:02:01.000000 eral-0.0.3/src/eral.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-26 11:02:01.000000 eral-0.0.3/src/eral.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 11:14:01.289258 eral-0.0.4/
+-rw-rw-rw-   0        0        0     3230 2024-04-26 11:14:01.286258 eral-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2439 2024-04-26 11:12:07.000000 eral-0.0.4/README package.md
+-rw-rw-rw-   0        0        0     2617 2024-04-26 11:13:20.000000 eral-0.0.4/README.md
+-rw-rw-rw-   0        0        0      801 2024-04-26 11:13:45.000000 eral-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 11:14:01.289258 eral-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 11:14:01.231445 eral-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 11:14:01.257353 eral-0.0.4/src/eral/
+-rw-rw-rw-   0        0        0        0 2023-10-25 13:21:15.000000 eral-0.0.4/src/eral/__init__.py
+-rw-rw-rw-   0        0        0     9222 2024-04-12 09:13:29.000000 eral-0.0.4/src/eral/alignment_prototyping_functions.py
+-rw-rw-rw-   0        0        0     8236 2024-04-10 12:02:33.000000 eral-0.0.4/src/eral/eral.py
+-rw-rw-rw-   0        0        0     4313 2024-04-10 11:36:54.000000 eral-0.0.4/src/eral/eral_score.py
+-rw-rw-rw-   0        0        0     7492 2024-04-10 12:12:14.000000 eral-0.0.4/src/eral/time_series_alignment.py
+-rw-rw-rw-   0        0        0     1957 2024-02-18 16:15:48.000000 eral-0.0.4/src/eral/time_series_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-26 11:14:01.284335 eral-0.0.4/src/eral.egg-info/
+-rw-rw-rw-   0        0        0     3230 2024-04-26 11:14:01.000000 eral-0.0.4/src/eral.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-04-26 11:14:01.000000 eral-0.0.4/src/eral.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 11:14:01.000000 eral-0.0.4/src/eral.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      177 2024-04-26 11:14:01.000000 eral-0.0.4/src/eral.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-26 11:14:01.000000 eral-0.0.4/src/eral.egg-info/top_level.txt
```

### Comparing `eral-0.0.3/PKG-INFO` & `eral-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eral
-Version: 0.0.3
+Version: 0.0.4
 Summary: Implementation of ERAL algorithm (Stržinar et al., 2024)
 Author-email: Žiga Stržinar <ziga.strzinar@ijs.si>
 Project-URL: Homepage, https://repo.ijs.si/zstrzinar/eral
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -23,64 +23,56 @@
 
 ## Introduction
 The ERAL (Error In Alignment) algorithm is a state-of-the-art method designed for time series alignment and averaging.
 The method obtains the average time series (the prototype) from a set of time series (a class).
 
 ## Installation
 
-To use ERAL, please clone the git repository:
+To use ERAL, please install the package from pypi.org using pip:
 ```bash
-git clone https://repo.ijs.si/zstrzinar/eral.git
+pip install eral
 ```
 
-The repository contains a requirements file, ensure you have all the requirements
-```
-pip install -r requirements.txt
-```
-
-### pip package
-A pip package is being prepared and will be made available soon.
-
 ## Usage
 
 The main entry point for the end user is `obtain_prototype` method in `eral.eral`:
 
 ```py
-from src.eral.eral import obtain_prototype
+from eral.eral import obtain_prototype
 
 class_prototype = obtain_prototype(...)
 ```
 
 The function takes several arguments, most important are:
 - `class_segments`: a list of time series to be aligned and averaged
 - `prototyping_function`: determines how the average is computed, typically the function `get_new_prototype_variable_clipping` from `eral.alignment_prototyping_functions` can be used.
 - `exclustion_zone`: percentage of forbidden alignments (see [1])
 
 The basic function call is:
 
 ```py
 import numpy as np
-from src.eral.eral import obtain_prototype
-from src.eral.alignment_prototyping_functions import get_new_prototype_variable_clipping
+from eral.eral import obtain_prototype
+from eral.alignment_prototyping_functions import get_new_prototype_variable_clipping
 
 X: list[np.ndarray] = [...]  # Class data
 
 class_prototype = obtain_prototype(X,
                                    prototyping_function=get_new_prototype_variable_clipping,
                                    exclusion_zone=0.2)
 ```
 
-For full examples, please refer to the `examples/` directory.
+For full examples, please refer to the `examples/` directory at [our repository](https://repo.ijs.si/zstrzinar/eral).
 
 ## Examples
 
-The `examples/` directory contains Jupyter notebooks that illustrate different uses and capabilities of the ERAL algorithm. 
+The `examples/` directory at [our repository](https://repo.ijs.si/zstrzinar/eral) contains Jupyter notebooks that illustrate different uses and capabilities of the ERAL algorithm. 
 To run an example, navigate to the `examples/` directory and execute the desired notebook.
 
 - Notebook titled `01 ERAL demo` demonstrates the ERAL prototyping method using the Trace dataset from UCR Archive.
 - Notebook titled `02 ERAL demo on industrial data` downloads an industrial dataset from Mendeley Data, and calculates the prototypes for all classes.
 - Notebook titled `03 Comparison` compares ERAL to DBA, SSG and others, using implementations in `tslearn`
 
 
 ## References
-[1] Paper introducing ERAL
+[1] Paper introducing ERAL\
 [2] Stržinar, Žiga; Pregelj, Boštjan; Petrovčič, Janko; Škrjanc, Igor; Dolanc, Gregor (2024), “Pneumatic Pressure and Electrical Current Time Series in Manufacturing”, Mendeley Data, V2, doi: 10.17632/ypzswhhzh9.2, url: https://data.mendeley.com/datasets/ypzswhhzh9/2
```

### Comparing `eral-0.0.3/README.md` & `eral-0.0.4/README package.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,64 +2,56 @@
 
 ## Introduction
 The ERAL (Error In Alignment) algorithm is a state-of-the-art method designed for time series alignment and averaging.
 The method obtains the average time series (the prototype) from a set of time series (a class).
 
 ## Installation
 
-To use ERAL, please clone the git repository:
+To use ERAL, please install the package from pypi.org using pip:
 ```bash
-git clone https://repo.ijs.si/zstrzinar/eral.git
+pip install eral
 ```
 
-The repository contains a requirements file, ensure you have all the requirements
-```
-pip install -r requirements.txt
-```
-
-### pip package
-A pip package is being prepared and will be made available soon.
-
 ## Usage
 
 The main entry point for the end user is `obtain_prototype` method in `eral.eral`:
 
 ```py
-from src.eral.eral import obtain_prototype
+from eral.eral import obtain_prototype
 
 class_prototype = obtain_prototype(...)
 ```
 
 The function takes several arguments, most important are:
 - `class_segments`: a list of time series to be aligned and averaged
 - `prototyping_function`: determines how the average is computed, typically the function `get_new_prototype_variable_clipping` from `eral.alignment_prototyping_functions` can be used.
 - `exclustion_zone`: percentage of forbidden alignments (see [1])
 
 The basic function call is:
 
 ```py
 import numpy as np
-from src.eral.eral import obtain_prototype
-from src.eral.alignment_prototyping_functions import get_new_prototype_variable_clipping
+from eral.eral import obtain_prototype
+from eral.alignment_prototyping_functions import get_new_prototype_variable_clipping
 
 X: list[np.ndarray] = [...]  # Class data
 
 class_prototype = obtain_prototype(X,
                                    prototyping_function=get_new_prototype_variable_clipping,
                                    exclusion_zone=0.2)
 ```
 
-For full examples, please refer to the `examples/` directory.
+For full examples, please refer to the `examples/` directory at [our repository](https://repo.ijs.si/zstrzinar/eral).
 
 ## Examples
 
-The `examples/` directory contains Jupyter notebooks that illustrate different uses and capabilities of the ERAL algorithm. 
+The `examples/` directory at [our repository](https://repo.ijs.si/zstrzinar/eral) contains Jupyter notebooks that illustrate different uses and capabilities of the ERAL algorithm. 
 To run an example, navigate to the `examples/` directory and execute the desired notebook.
 
 - Notebook titled `01 ERAL demo` demonstrates the ERAL prototyping method using the Trace dataset from UCR Archive.
 - Notebook titled `02 ERAL demo on industrial data` downloads an industrial dataset from Mendeley Data, and calculates the prototypes for all classes.
 - Notebook titled `03 Comparison` compares ERAL to DBA, SSG and others, using implementations in `tslearn`
 
 
 ## References
-[1] Paper introducing ERAL
+[1] Paper introducing ERAL\
 [2] Stržinar, Žiga; Pregelj, Boštjan; Petrovčič, Janko; Škrjanc, Igor; Dolanc, Gregor (2024), “Pneumatic Pressure and Electrical Current Time Series in Manufacturing”, Mendeley Data, V2, doi: 10.17632/ypzswhhzh9.2, url: https://data.mendeley.com/datasets/ypzswhhzh9/2
```

### Comparing `eral-0.0.3/pyproject.toml` & `eral-0.0.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "eral"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Žiga Stržinar", email="ziga.strzinar@ijs.si" },
 ]
 description = "Implementation of ERAL algorithm (Stržinar et al., 2024)"
-readme = "README.md"
+readme = "README package.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "dtw-python>=1.3.0",
```

### Comparing `eral-0.0.3/src/eral/alignment_prototyping_functions.py` & `eral-0.0.4/src/eral/alignment_prototyping_functions.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.3/src/eral/eral.py` & `eral-0.0.4/src/eral/eral.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.3/src/eral/eral_score.py` & `eral-0.0.4/src/eral/eral_score.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.3/src/eral/time_series_alignment.py` & `eral-0.0.4/src/eral/time_series_alignment.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.3/src/eral/time_series_helpers.py` & `eral-0.0.4/src/eral/time_series_helpers.py`

 * *Files identical despite different names*

### Comparing `eral-0.0.3/src/eral.egg-info/PKG-INFO` & `eral-0.0.4/src/eral.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eral
-Version: 0.0.3
+Version: 0.0.4
 Summary: Implementation of ERAL algorithm (Stržinar et al., 2024)
 Author-email: Žiga Stržinar <ziga.strzinar@ijs.si>
 Project-URL: Homepage, https://repo.ijs.si/zstrzinar/eral
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
@@ -23,64 +23,56 @@
 
 ## Introduction
 The ERAL (Error In Alignment) algorithm is a state-of-the-art method designed for time series alignment and averaging.
 The method obtains the average time series (the prototype) from a set of time series (a class).
 
 ## Installation
 
-To use ERAL, please clone the git repository:
+To use ERAL, please install the package from pypi.org using pip:
 ```bash
-git clone https://repo.ijs.si/zstrzinar/eral.git
+pip install eral
 ```
 
-The repository contains a requirements file, ensure you have all the requirements
-```
-pip install -r requirements.txt
-```
-
-### pip package
-A pip package is being prepared and will be made available soon.
-
 ## Usage
 
 The main entry point for the end user is `obtain_prototype` method in `eral.eral`:
 
 ```py
-from src.eral.eral import obtain_prototype
+from eral.eral import obtain_prototype
 
 class_prototype = obtain_prototype(...)
 ```
 
 The function takes several arguments, most important are:
 - `class_segments`: a list of time series to be aligned and averaged
 - `prototyping_function`: determines how the average is computed, typically the function `get_new_prototype_variable_clipping` from `eral.alignment_prototyping_functions` can be used.
 - `exclustion_zone`: percentage of forbidden alignments (see [1])
 
 The basic function call is:
 
 ```py
 import numpy as np
-from src.eral.eral import obtain_prototype
-from src.eral.alignment_prototyping_functions import get_new_prototype_variable_clipping
+from eral.eral import obtain_prototype
+from eral.alignment_prototyping_functions import get_new_prototype_variable_clipping
 
 X: list[np.ndarray] = [...]  # Class data
 
 class_prototype = obtain_prototype(X,
                                    prototyping_function=get_new_prototype_variable_clipping,
                                    exclusion_zone=0.2)
 ```
 
-For full examples, please refer to the `examples/` directory.
+For full examples, please refer to the `examples/` directory at [our repository](https://repo.ijs.si/zstrzinar/eral).
 
 ## Examples
 
-The `examples/` directory contains Jupyter notebooks that illustrate different uses and capabilities of the ERAL algorithm. 
+The `examples/` directory at [our repository](https://repo.ijs.si/zstrzinar/eral) contains Jupyter notebooks that illustrate different uses and capabilities of the ERAL algorithm. 
 To run an example, navigate to the `examples/` directory and execute the desired notebook.
 
 - Notebook titled `01 ERAL demo` demonstrates the ERAL prototyping method using the Trace dataset from UCR Archive.
 - Notebook titled `02 ERAL demo on industrial data` downloads an industrial dataset from Mendeley Data, and calculates the prototypes for all classes.
 - Notebook titled `03 Comparison` compares ERAL to DBA, SSG and others, using implementations in `tslearn`
 
 
 ## References
-[1] Paper introducing ERAL
+[1] Paper introducing ERAL\
 [2] Stržinar, Žiga; Pregelj, Boštjan; Petrovčič, Janko; Škrjanc, Igor; Dolanc, Gregor (2024), “Pneumatic Pressure and Electrical Current Time Series in Manufacturing”, Mendeley Data, V2, doi: 10.17632/ypzswhhzh9.2, url: https://data.mendeley.com/datasets/ypzswhhzh9/2
```

