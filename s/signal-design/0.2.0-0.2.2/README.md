# Comparing `tmp/signal_design-0.2.0.tar.gz` & `tmp/signal_design-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal_design-0.2.0.tar", max compression
+gzip compressed data, was "signal_design-0.2.2.tar", max compression
```

## Comparing `signal_design-0.2.0.tar` & `signal_design-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1066 2024-02-29 13:30:57.335013 signal_design-0.2.0/LICENSE
--rw-r--r--   0        0        0     3074 2024-02-29 13:30:57.335013 signal_design-0.2.0/README.md
--rw-r--r--   0        0        0     2087 2024-02-29 13:31:32.830477 signal_design-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      226 2024-02-29 13:31:32.826477 signal_design-0.2.0/signal_design/__init__.py
--rw-r--r--   0        0        0     5464 2024-02-29 13:30:57.343013 signal_design-0.2.0/signal_design/axis.py
--rw-r--r--   0        0        0      946 2024-02-29 13:30:57.343013 signal_design-0.2.0/signal_design/core.py
--rw-r--r--   0        0        0    14901 2024-02-29 13:30:57.343013 signal_design-0.2.0/signal_design/default_methods.py
--rw-r--r--   0        0        0      648 2024-02-29 13:30:57.343013 signal_design-0.2.0/signal_design/exc.py
--rw-r--r--   0        0        0      707 2024-02-29 13:30:57.343013 signal_design-0.2.0/signal_design/help_types.py
--rw-r--r--   0        0        0    16210 2024-02-29 13:30:57.343013 signal_design-0.2.0/signal_design/relation.py
--rw-r--r--   0        0        0    10771 2024-02-29 13:30:57.343013 signal_design-0.2.0/signal_design/signal.py
--rw-r--r--   0        0        0    10960 2024-02-29 13:30:57.343013 signal_design-0.2.0/signal_design/spectrum.py
--rw-r--r--   0        0        0     4179 1970-01-01 00:00:00.000000 signal_design-0.2.0/setup.py
--rw-r--r--   0        0        0     4275 1970-01-01 00:00:00.000000 signal_design-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-26 07:18:35.129489 signal_design-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3074 2024-04-26 07:18:35.129489 signal_design-0.2.2/README.md
+-rw-r--r--   0        0        0     2087 2024-04-26 07:19:12.269346 signal_design-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      226 2024-04-26 07:19:12.269346 signal_design-0.2.2/signal_design/__init__.py
+-rw-r--r--   0        0        0     5464 2024-04-26 07:18:35.133489 signal_design-0.2.2/signal_design/axis.py
+-rw-r--r--   0        0        0      946 2024-04-26 07:18:35.133489 signal_design-0.2.2/signal_design/core.py
+-rw-r--r--   0        0        0    14901 2024-04-26 07:18:35.133489 signal_design-0.2.2/signal_design/default_methods.py
+-rw-r--r--   0        0        0      648 2024-04-26 07:18:35.133489 signal_design-0.2.2/signal_design/exc.py
+-rw-r--r--   0        0        0      707 2024-04-26 07:18:35.133489 signal_design-0.2.2/signal_design/help_types.py
+-rw-r--r--   0        0        0    16210 2024-04-26 07:18:35.133489 signal_design-0.2.2/signal_design/relation.py
+-rw-r--r--   0        0        0    10771 2024-04-26 07:18:35.133489 signal_design-0.2.2/signal_design/signal.py
+-rw-r--r--   0        0        0    10960 2024-04-26 07:18:35.133489 signal_design-0.2.2/signal_design/spectrum.py
+-rw-r--r--   0        0        0     4179 1970-01-01 00:00:00.000000 signal_design-0.2.2/setup.py
+-rw-r--r--   0        0        0     4275 1970-01-01 00:00:00.000000 signal_design-0.2.2/PKG-INFO
```

### Comparing `signal_design-0.2.0/LICENSE` & `signal_design-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `signal_design-0.2.0/README.md` & `signal_design-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `signal_design-0.2.0/pyproject.toml` & `signal_design-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "signal-design"
-version = "0.2.0"
+version = "0.2.2"
 description = "The project for creation and analysis signals."
 authors = ["Omnivanitate <serebraykov.vs@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Omnivanitate/signal-design"
 documentation = "https://signal-design.readthedocs.io"
 packages = [{include = "signal_design"}]
```

### Comparing `signal_design-0.2.0/signal_design/axis.py` & `signal_design-0.2.2/signal_design/axis.py`

 * *Files identical despite different names*

### Comparing `signal_design-0.2.0/signal_design/core.py` & `signal_design-0.2.2/signal_design/core.py`

 * *Files identical despite different names*

### Comparing `signal_design-0.2.0/signal_design/default_methods.py` & `signal_design-0.2.2/signal_design/default_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -483,15 +483,15 @@
         size = None
     elif isinstance(time, int):
         size = time
     else:
         size = time.size
 
     if frequency.start < 0.:
-        amplitude = np.fft.rfft(spectrum, size)
+        amplitude = np.fft.ifft(spectrum, size)
     else:
         amplitude = np.fft.irfft(spectrum, size)
         
 
     if time is None or isinstance(time, int):
 
         if size is None:
```

### Comparing `signal_design-0.2.0/signal_design/exc.py` & `signal_design-0.2.2/signal_design/exc.py`

 * *Files identical despite different names*

### Comparing `signal_design-0.2.0/signal_design/help_types.py` & `signal_design-0.2.2/signal_design/help_types.py`

 * *Files identical despite different names*

### Comparing `signal_design-0.2.0/signal_design/relation.py` & `signal_design-0.2.2/signal_design/relation.py`

 * *Files identical despite different names*

### Comparing `signal_design-0.2.0/signal_design/signal.py` & `signal_design-0.2.2/signal_design/signal.py`

 * *Files identical despite different names*

### Comparing `signal_design-0.2.0/signal_design/spectrum.py` & `signal_design-0.2.2/signal_design/spectrum.py`

 * *Files identical despite different names*

### Comparing `signal_design-0.2.0/setup.py` & `signal_design-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 extras_require = \
 {':python_version >= "3.6" and python_version < "3.8"': ['numpy<=1.19',
                                                          'scipy>=1.2,<1.8'],
  ':python_version >= "3.8"': ['numpy>1.19', 'scipy>=1.8']}
 
 setup_kwargs = {
     'name': 'signal-design',
-    'version': '0.2.0',
+    'version': '0.2.2',
     'description': 'The project for creation and analysis signals.',
     'long_description': '# signal-design\n\nSimple way to create signals.\n\n## The project is intended for designing signals.\n\nThe package is intended to create and develop signals of\nvarying complexity.\n\nThe project can be used both for educational and work purposes.\n\nIt is convenient to use [`Jupyter Lab`](https://jupyter.org/) or\n[`Jupyter Notebook`](https://jupyter.org/) to speed up the development\nof signals, to compare their parameters with other signals,\nand to visualize them.\n\nThe project is designed so that you can easily change the creation of\nsignals.\n\nIn addition, documentation consist tutorial how to work with library\nand examples of ready-made signals. You can write own signal creation.\n\n# Installation\n\nTo install use:\n\n```bash\n$ pip install signal-design\n```\n\nor using `poetry`\n\n```bash\n$ poetry add signal-design\n```\n\nAlso you can clone or load project from [GitHub](https://github.com/Omnivanitate/signal-design),\nand install requirement packages using the\n\n```bash\n$ pip install -r requirements/build.txt\n```\n\nor if you want develop, use\n\n```bash\n$ pip install -r requirements/dev.txt\n\n```\n\nor\n\n```bash\n$ poetry install\n```\n\nor coping pieces of code and create your own.\n\n## Usage\n\nThe project is a library. Working with it is the same as with\nother third-part libraries of the python language.  \nAn example of how to include the library is described\n[here](https://docs.python.org/3/tutorial/modules.html).\n\nThe library consists sub-modules:\n\n- `signal_design.core` - contains basic classes `MathOperation` and `RelationProtocol`.\n- `signal_design.exc` - contains exceptions.\n- `signal_design.axis` - contains class `Axis`\n- `signal_design.relation` - contains class `Relation`\n- `signal_design.signal` - contains class `Signal`\n- `signal_design.spectrum` - contains class `Spectrum`\n- `signal_design.default_methods` - contains default methods for class above.\n\nFor convenient base classes:\n`Axis`, `Relation`, `Signal`, `Spectrum` - can be imported from\nthe `signal_design` module.\n\nFor example:\n\n```python\nfrom signal_design import Signal\n```\n\n### Quick start. Simple work flow.\n\nBelow is a simple example of creating a signal and visualizing it.\nA more extended description of the work of the library in the documentation.\nOther examples are contained in the documentation contains in _Tutorial_\nsection.\n\nFor the following code [`Matplotlib`](https://matplotlib.org/) need be used\nto visualize a result of work. But `Matplotlib` can be replaced with another\nlibrary that you use.\n\n```python\nimport numpy as np\nimport matplotlib.pyplot as plt\n\nfrom signal_design import Axis, Signal\n\ntime = Axis.get_using_end(start=0., end=10., sample=0.01)\namplitude = np.sin(2*np.pi*time.array)\nsignal = Signal(time, amplitude)\n\nplt.plot(*signal.get_data())\nplt.xlabel(\'Time, s\')\nplt.ylabel(\'Amplitude\')\nplt.title(\'Sin 1Hz\')\n```\n\nResult:\n\n![signal_with_matplotlib](https://raw.githubusercontent.com/Omnivanitate/signal-design/main/docs/assets/sin_func.png "Sin function.")\n\n## Credits\n\n`signal-design` was created with  \n[`numpy`](https://numpy.org/)  \n[`scipy`](https://scipy.org/)\n',
     'author': 'Omnivanitate',
     'author_email': 'serebraykov.vs@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Omnivanitate/signal-design',
```

### Comparing `signal_design-0.2.0/PKG-INFO` & `signal_design-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-design
-Version: 0.2.0
+Version: 0.2.2
 Summary: The project for creation and analysis signals.
 Home-page: https://github.com/Omnivanitate/signal-design
 License: MIT
 Author: Omnivanitate
 Author-email: serebraykov.vs@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

