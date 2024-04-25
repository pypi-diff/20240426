# Comparing `tmp/pysros-24.3.1.tar.gz` & `tmp/pysros-24.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysros-24.3.1.tar", last modified: Fri Mar 15 21:34:56 2024, max compression
+gzip compressed data, was "pysros-24.3.2.tar", last modified: Thu Apr 25 22:53:16 2024, max compression
```

## Comparing `pysros-24.3.1.tar` & `pysros-24.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:34:56.686829 pysros-24.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-03-15 21:34:52.000000 pysros-24.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-03-15 21:34:56.686829 pysros-24.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-03-15 21:34:52.000000 pysros-24.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:34:56.686829 pysros-24.3.1/pysros/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    63422 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/management.py
--rw-r--r--   0 runner    (1001) docker     (127)    20797 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    32703 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/model_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/model_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)    26212 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/pprint.py
--rw-r--r--   0 runner    (1001) docker     (127)    64049 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/request_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    41970 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/yang_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:34:56.686829 pysros-24.3.1/pysros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-03-15 21:34:56.000000 pysros-24.3.1/pysros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-15 21:34:56.000000 pysros-24.3.1/pysros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 21:34:56.000000 pysros-24.3.1/pysros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-15 21:34:56.000000 pysros-24.3.1/pysros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-15 21:34:56.000000 pysros-24.3.1/pysros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 21:34:56.686829 pysros-24.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-15 21:34:52.000000 pysros-24.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:16.540159 pysros-24.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-04-25 22:53:12.000000 pysros-24.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-25 22:53:16.540159 pysros-24.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-25 22:53:12.000000 pysros-24.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:16.536159 pysros-24.3.2/pysros/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63422 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20797 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32703 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/model_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/model_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26212 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64049 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/request_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41970 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-25 22:53:12.000000 pysros-24.3.2/pysros/yang_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 22:53:16.540159 pysros-24.3.2/pysros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-25 22:53:16.000000 pysros-24.3.2/pysros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-25 22:53:16.000000 pysros-24.3.2/pysros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 22:53:16.000000 pysros-24.3.2/pysros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 22:53:16.000000 pysros-24.3.2/pysros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 22:53:16.000000 pysros-24.3.2/pysros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 22:53:16.540159 pysros-24.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-25 22:53:12.000000 pysros-24.3.2/setup.py
```

### Comparing `pysros-24.3.1/LICENSE.md` & `pysros-24.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysros-24.3.1/PKG-INFO` & `pysros-24.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysros
-Version: 24.3.1
+Version: 24.3.2
 Summary: Python for the Nokia Service Router Operating Systems (pySROS)
 Home-page: https://www.nokia.com
 Author: Nokia
 Author-email: 
 License: Copyright 2021-2024 Nokia.  License available in the LICENSE.md file.
 Project-URL: Documentation, https://network.developer.nokia.com/static/sr/learn/pysros/latest/
 Project-URL: Source, https://github.com/nokia/pysros
@@ -45,15 +45,15 @@
     - With NETCONF enabled and accessible by an authorized user (to execute applications
     remotely)
 - A Python 3 interpreter of version 3.10 or newer when using the pySROS library to
   execute applications remotely
 
 ## License ##
 
-Copyright 2021-2023 Nokia.
+Copyright 2021-2024 Nokia.
 
 The license is located [here](LICENSE.md).
 
 ## Reporting issues ##
 
 Issues, suggestions, and enhancements are welcome.  Please use the Nokia support
 process.  Issues raised in GitHub may be considered for inclusion into the project
```

### Comparing `pysros-24.3.1/README.md` & `pysros-24.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     - With NETCONF enabled and accessible by an authorized user (to execute applications
     remotely)
 - A Python 3 interpreter of version 3.10 or newer when using the pySROS library to
   execute applications remotely
 
 ## License ##
 
-Copyright 2021-2023 Nokia.
+Copyright 2021-2024 Nokia.
 
 The license is located [here](LICENSE.md).
 
 ## Reporting issues ##
 
 Issues, suggestions, and enhancements are welcome.  Please use the Nokia support
 process.  Issues raised in GitHub may be considered for inclusion into the project
```

### Comparing `pysros-24.3.1/pysros/errors.py` & `pysros-24.3.2/pysros/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 from .exceptions import (ActionTerminatedIncompleteError, InternalError,
                          InvalidPathError, JsonDecodeError,
                          ModelProcessingError, SrosConfigConflictError,
                          SrosMgmtError, XmlDecodeError, make_exception)
 
 __doc__ = """This module contains error definitions for pySROS.
```

### Comparing `pysros-24.3.1/pysros/exceptions.py` & `pysros-24.3.2/pysros/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 __all__ = (
     "SrosMgmtError", "InvalidPathError", "ModelProcessingError",
     "InternalError", "SrosConfigConflictError",
     "ActionTerminatedIncompleteError", "JsonDecodeError", "XmlDecodeError",
 )
```

### Comparing `pysros-24.3.1/pysros/identifier.py` & `pysros-24.3.2/pysros/identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 import re
 
 from .errors import *
 from .errors import make_exception
 from .singleton import _Singleton
```

### Comparing `pysros-24.3.1/pysros/management.py` & `pysros-24.3.2/pysros/management.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 import base64
 import contextlib
 import datetime
 import hashlib
 import os.path
 import pathlib
```

### Comparing `pysros-24.3.1/pysros/model.py` & `pysros-24.3.2/pysros/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 import copy
 import locale
 import sys
 from enum import Enum, IntEnum, IntFlag
 from typing import List, Optional
```

### Comparing `pysros-24.3.1/pysros/model_builder.py` & `pysros-24.3.2/pysros/model_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 import copy
 from collections import defaultdict
 from itertools import chain
 from typing import DefaultDict, Dict, Optional, Set, Union
 
 from .errors import *
```

### Comparing `pysros-24.3.1/pysros/model_path.py` & `pysros-24.3.2/pysros/model_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 from typing import Iterable
 
 from .identifier import Identifier
 
 
 class ModelPath:
```

### Comparing `pysros-24.3.1/pysros/model_walker.py` & `pysros-24.3.2/pysros/model_walker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 import contextlib
 import copy
 import json
 from enum import Enum, auto
 from typing import List, Optional, Union
```

### Comparing `pysros-24.3.1/pysros/pprint.py` & `pysros-24.3.2/pysros/pprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 from .errors import *
 from .errors import make_exception
 from .wrappers import *
 
 __all__ = (
     "TreePrinter", "printTree", "Column", "Padding", "Table", "KeyValueTable",
```

### Comparing `pysros-24.3.1/pysros/request_data.py` & `pysros-24.3.2/pysros/request_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 import copy
 import json
 import pprint
 import itertools
 from abc import ABC, abstractmethod
 from collections import OrderedDict
```

### Comparing `pysros-24.3.1/pysros/singleton.py` & `pysros-24.3.2/pysros/singleton.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 class _Singleton(type):
     _instances = {}
 
     def __new__(cls, *args, **kwargs):
         res = super(_Singleton, cls).__new__(cls, *args, **kwargs)
         res.__copy__ = lambda self: self
```

### Comparing `pysros-24.3.1/pysros/tokenizer.py` & `pysros-24.3.2/pysros/tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 import collections
 import re
 
 from .errors import *
 from .errors import make_exception
```

### Comparing `pysros-24.3.1/pysros/wrappers.py` & `pysros-24.3.2/pysros/wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 import operator
 import collections
 
 from abc import abstractmethod
 from io import StringIO
 from functools import total_ordering
```

### Comparing `pysros-24.3.1/pysros/yang_type.py` & `pysros-24.3.2/pysros/yang_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021-2023 Nokia
+# Copyright 2021-2024 Nokia
 
 import base64
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from typing import (Any, Dict, Iterable, List, Mapping, NamedTuple, Optional,
                     Set, Tuple, Union)
```

### Comparing `pysros-24.3.1/pysros.egg-info/PKG-INFO` & `pysros-24.3.2/pysros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysros
-Version: 24.3.1
+Version: 24.3.2
 Summary: Python for the Nokia Service Router Operating Systems (pySROS)
 Home-page: https://www.nokia.com
 Author: Nokia
 Author-email: 
 License: Copyright 2021-2024 Nokia.  License available in the LICENSE.md file.
 Project-URL: Documentation, https://network.developer.nokia.com/static/sr/learn/pysros/latest/
 Project-URL: Source, https://github.com/nokia/pysros
@@ -45,15 +45,15 @@
     - With NETCONF enabled and accessible by an authorized user (to execute applications
     remotely)
 - A Python 3 interpreter of version 3.10 or newer when using the pySROS library to
   execute applications remotely
 
 ## License ##
 
-Copyright 2021-2023 Nokia.
+Copyright 2021-2024 Nokia.
 
 The license is located [here](LICENSE.md).
 
 ## Reporting issues ##
 
 Issues, suggestions, and enhancements are welcome.  Please use the Nokia support
 process.  Issues raised in GitHub may be considered for inclusion into the project
```

### Comparing `pysros-24.3.1/setup.py` & `pysros-24.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pysros',
-    version='24.3.1',
+    version='24.3.2',
     packages=['pysros'],
     url='https://www.nokia.com',
     license='Copyright 2021-2024 Nokia.  License available in the LICENSE.md file.',
     author='Nokia',
     author_email='',
     description='Python for the Nokia Service Router Operating Systems (pySROS)',
     project_urls={
```

