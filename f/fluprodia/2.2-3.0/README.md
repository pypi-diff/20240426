# Comparing `tmp/fluprodia-2.2.tar.gz` & `tmp/fluprodia-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluprodia-2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fluprodia-3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fluprodia-2.2.tar` & `fluprodia-3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1649 2023-12-04 07:14:52.003443 fluprodia-2.2/CHANGELOG.rst
--rw-r--r--   0        0        0     2210 2023-12-07 17:42:54.221123 fluprodia-2.2/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1111 2022-12-02 16:23:35.372137 fluprodia-2.2/LICENSE
--rw-r--r--   0        0        0     5098 2023-12-07 17:50:21.823631 fluprodia-2.2/README.rst
--rw-r--r--   0        0        0     4912 2023-12-07 17:28:01.436045 fluprodia-2.2/docs/README.rst
--rw-r--r--   0        0        0    29585 2023-12-07 14:17:42.348154 fluprodia-2.2/docs/_static/images/logo_fluprodia_small.svg
--rw-r--r--   0        0        0    29828 2023-12-07 15:13:58.835502 fluprodia-2.2/docs/_static/images/logo_fluprodia_small_darkmode.svg
--rw-r--r--   0        0        0       29 2022-12-02 16:23:35.372137 fluprodia-2.2/docs/authors.rst
--rw-r--r--   0        0        0       31 2022-12-02 16:23:35.372137 fluprodia-2.2/docs/changelog.rst
--rw-r--r--   0        0        0     3699 2023-12-07 15:05:54.136759 fluprodia-2.2/docs/conf.py
--rw-r--r--   0        0        0       34 2022-12-02 16:23:35.372137 fluprodia-2.2/docs/contributing.rst
--rw-r--r--   0        0        0      262 2023-12-07 17:27:46.148538 fluprodia-2.2/docs/index.rst
--rw-r--r--   0        0        0     2496 2023-12-07 17:26:35.831705 fluprodia-2.2/docs/installation.rst
--rw-r--r--   0        0        0   216190 2023-12-04 18:23:26.492658 fluprodia-2.2/docs/reference/_images/Ts_R290_isolines.svg
--rw-r--r--   0        0        0   212552 2023-12-04 18:23:27.021556 fluprodia-2.2/docs/reference/_images/Ts_R290_pressure_loss.svg
--rw-r--r--   0        0        0   125924 2023-12-04 18:23:14.901351 fluprodia-2.2/docs/reference/_images/Ts_diagram.svg
--rw-r--r--   0        0        0   126103 2023-12-07 17:43:37.844787 fluprodia-2.2/docs/reference/_images/Ts_diagram_H2O.svg
--rw-r--r--   0        0        0   128714 2023-12-04 18:23:34.815330 fluprodia-2.2/docs/reference/_images/Ts_diagram_states.svg
--rw-r--r--   0        0        0   108148 2023-12-04 18:23:23.933735 fluprodia-2.2/docs/reference/_images/logph_R290_full.svg
--rw-r--r--   0        0        0   140191 2023-12-04 18:23:25.801304 fluprodia-2.2/docs/reference/_images/logph_R290_isolines.svg
--rw-r--r--   0        0        0   152726 2023-12-04 18:23:24.464968 fluprodia-2.2/docs/reference/_images/logph_R290_zoomed.svg
--rw-r--r--   0        0        0   162597 2023-12-04 18:23:24.980806 fluprodia-2.2/docs/reference/_images/logph_R290_zoomed_temperature_labels.svg
--rw-r--r--   0        0        0   108148 2023-12-04 18:23:15.312340 fluprodia-2.2/docs/reference/_images/logph_diagram.svg
--rw-r--r--   0        0        0   147439 2023-12-07 17:43:37.040465 fluprodia-2.2/docs/reference/_images/logph_diagram_H2O.svg
--rw-r--r--   0        0        0   104299 2023-12-07 17:43:43.932762 fluprodia-2.2/docs/reference/_images/logph_diagram_R290.svg
--rw-r--r--   0        0        0    99930 2023-12-04 18:23:34.396119 fluprodia-2.2/docs/reference/_images/logph_diagram_states.svg
--rw-r--r--   0        0        0      122 2022-12-02 16:23:35.441359 fluprodia-2.2/docs/reference/index.rst
--rw-r--r--   0        0        0       77 2023-12-07 17:32:15.145820 fluprodia-2.2/docs/requirements.txt
--rw-r--r--   0        0        0    17549 2023-12-04 09:18:05.989379 fluprodia-2.2/docs/usage.rst
--rw-r--r--   0        0        0     2140 2023-12-07 17:50:42.974846 fluprodia-2.2/pyproject.toml
--rw-r--r--   0        0        0      116 2023-12-07 17:50:49.780444 fluprodia-2.2/src/fluprodia/__init__.py
--rw-r--r--   0        0        0    41007 2023-12-04 18:24:06.825404 fluprodia-2.2/src/fluprodia/fluid_property_diagram.py
--rw-r--r--   0        0        0       80 2022-12-02 16:23:35.441359 fluprodia-2.2/tests/test_fluprodia.py
--rw-r--r--   0        0        0     6497 1970-01-01 00:00:00.000000 fluprodia-2.2/PKG-INFO
+-rw-r--r--   0        0        0     1649 2023-12-04 07:14:52.003443 fluprodia-3.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     2210 2023-12-07 17:42:54.221123 fluprodia-3.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1111 2022-12-02 16:23:35.372137 fluprodia-3.0/LICENSE
+-rw-r--r--   0        0        0     5098 2023-12-07 17:50:21.823631 fluprodia-3.0/README.rst
+-rw-r--r--   0        0        0     4912 2024-04-26 18:04:02.394957 fluprodia-3.0/docs/README.rst
+-rw-r--r--   0        0        0    29585 2023-12-07 14:17:42.348154 fluprodia-3.0/docs/_static/images/logo_fluprodia_small.svg
+-rw-r--r--   0        0        0    29828 2023-12-07 15:13:58.835502 fluprodia-3.0/docs/_static/images/logo_fluprodia_small_darkmode.svg
+-rw-r--r--   0        0        0       29 2022-12-02 16:23:35.372137 fluprodia-3.0/docs/authors.rst
+-rw-r--r--   0        0        0       31 2022-12-02 16:23:35.372137 fluprodia-3.0/docs/changelog.rst
+-rw-r--r--   0        0        0     3699 2023-12-07 15:05:54.136759 fluprodia-3.0/docs/conf.py
+-rw-r--r--   0        0        0       34 2022-12-02 16:23:35.372137 fluprodia-3.0/docs/contributing.rst
+-rw-r--r--   0        0        0      262 2023-12-07 17:27:46.148538 fluprodia-3.0/docs/index.rst
+-rw-r--r--   0        0        0     2496 2023-12-07 17:26:35.831705 fluprodia-3.0/docs/installation.rst
+-rw-r--r--   0        0        0   216190 2023-12-04 18:23:26.492658 fluprodia-3.0/docs/reference/_images/Ts_R290_isolines.svg
+-rw-r--r--   0        0        0   212552 2023-12-04 18:23:27.021556 fluprodia-3.0/docs/reference/_images/Ts_R290_pressure_loss.svg
+-rw-r--r--   0        0        0   125924 2023-12-04 18:23:14.901351 fluprodia-3.0/docs/reference/_images/Ts_diagram.svg
+-rw-r--r--   0        0        0   126103 2023-12-07 17:43:37.844787 fluprodia-3.0/docs/reference/_images/Ts_diagram_H2O.svg
+-rw-r--r--   0        0        0   128714 2023-12-04 18:23:34.815330 fluprodia-3.0/docs/reference/_images/Ts_diagram_states.svg
+-rw-r--r--   0        0        0   108148 2023-12-04 18:23:23.933735 fluprodia-3.0/docs/reference/_images/logph_R290_full.svg
+-rw-r--r--   0        0        0   140191 2023-12-04 18:23:25.801304 fluprodia-3.0/docs/reference/_images/logph_R290_isolines.svg
+-rw-r--r--   0        0        0   152726 2023-12-04 18:23:24.464968 fluprodia-3.0/docs/reference/_images/logph_R290_zoomed.svg
+-rw-r--r--   0        0        0   162597 2023-12-04 18:23:24.980806 fluprodia-3.0/docs/reference/_images/logph_R290_zoomed_temperature_labels.svg
+-rw-r--r--   0        0        0   108148 2023-12-04 18:23:15.312340 fluprodia-3.0/docs/reference/_images/logph_diagram.svg
+-rw-r--r--   0        0        0   147439 2023-12-07 17:43:37.040465 fluprodia-3.0/docs/reference/_images/logph_diagram_H2O.svg
+-rw-r--r--   0        0        0   104299 2023-12-07 17:43:43.932762 fluprodia-3.0/docs/reference/_images/logph_diagram_R290.svg
+-rw-r--r--   0        0        0    99930 2023-12-04 18:23:34.396119 fluprodia-3.0/docs/reference/_images/logph_diagram_states.svg
+-rw-r--r--   0        0        0      122 2022-12-02 16:23:35.441359 fluprodia-3.0/docs/reference/index.rst
+-rw-r--r--   0        0        0       77 2023-12-07 17:32:15.145820 fluprodia-3.0/docs/requirements.txt
+-rw-r--r--   0        0        0    17737 2024-04-26 18:06:06.705823 fluprodia-3.0/docs/usage.rst
+-rw-r--r--   0        0        0     2073 2024-04-26 18:08:25.017418 fluprodia-3.0/pyproject.toml
+-rw-r--r--   0        0        0      196 2024-04-26 18:08:50.950992 fluprodia-3.0/src/fluprodia/__init__.py
+-rw-r--r--   0        0        0    42960 2024-04-26 18:06:35.273273 fluprodia-3.0/src/fluprodia/fluid_property_diagram.py
+-rw-r--r--   0        0        0       80 2022-12-02 16:23:35.441359 fluprodia-3.0/tests/test_fluprodia.py
+-rw-r--r--   0        0        0     6497 1970-01-01 00:00:00.000000 fluprodia-3.0/PKG-INFO
```

### Comparing `fluprodia-2.2/CHANGELOG.rst` & `fluprodia-3.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/CONTRIBUTING.rst` & `fluprodia-3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/LICENSE` & `fluprodia-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/README.rst` & `fluprodia-3.0/README.rst`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/README.rst` & `fluprodia-3.0/docs/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -80,28 +80,28 @@
 
     >>> fig, ax = plt.subplots(1, figsize=(8, 5))
     >>> diagram.draw_isolines(diagram_type='logph', fig=fig, ax=ax, x_min=0, x_max=3000, y_min=0.01, y_max=1000)
     >>> plt.tight_layout()
     >>> fig.savefig('logph_diagram_H2O.svg')
     >>> fig.savefig('logph_diagram_H2O.png', dpi=300)
 
-.. figure:: /reference/_images/logph_diagram_H2O.png
+.. figure:: /reference/_images/logph_diagram_H2O.svg
     :align: center
 
 Or, a Ts-diagram:
 
 .. code-block::
 
     >>> fig, ax = plt.subplots(1, figsize=(8, 5))
     >>> diagram.draw_isolines(diagram_type='Ts', fig=fig, ax=ax, x_min=0, x_max=8000, y_min=0, y_max=700)
     >>> plt.tight_layout()
     >>> fig.savefig('Ts_diagram_H2O.svg')
     >>> fig.savefig('Ts_diagram_H2O.png', dpi=300)
 
-.. figure:: /reference/_images/Ts_diagram_H2O.png
+.. figure:: /reference/_images/Ts_diagram_H2O.svg
     :align: center
 
 The fluids are available through CoolProp. To generate a diagram for a new fluid
 simply change the name. Isolines come with defaults as well.
 
 .. code-block:: python
 
@@ -110,15 +110,15 @@
     >>> diagram.calc_isolines()
     >>> fig, ax = plt.subplots(1, figsize=(8, 5))
     >>> diagram.draw_isolines(diagram_type='logph', fig=fig, ax=ax, x_min=0, x_max=800, y_min=1e-1, y_max=1e2)
     >>> plt.tight_layout()
     >>> fig.savefig('logph_diagram_R290.png', dpi=300)
     >>> fig.savefig('logph_diagram_R290.svg')
 
-.. figure:: /reference/_images/logph_diagram_R290.png
+.. figure:: /reference/_images/logph_diagram_R290.svg
     :align: center
 
 Documentation
 =============
 
 For further examples and usage please refer to the online documentation at
 https://fluprodia.readthedocs.io/.
```

### Comparing `fluprodia-2.2/docs/_static/images/logo_fluprodia_small.svg` & `fluprodia-3.0/docs/_static/images/logo_fluprodia_small.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/_static/images/logo_fluprodia_small_darkmode.svg` & `fluprodia-3.0/docs/_static/images/logo_fluprodia_small_darkmode.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/conf.py` & `fluprodia-3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/installation.rst` & `fluprodia-3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/Ts_R290_isolines.svg` & `fluprodia-3.0/docs/reference/_images/Ts_R290_isolines.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/Ts_R290_pressure_loss.svg` & `fluprodia-3.0/docs/reference/_images/Ts_R290_pressure_loss.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/Ts_diagram.svg` & `fluprodia-3.0/docs/reference/_images/Ts_diagram.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/Ts_diagram_H2O.svg` & `fluprodia-3.0/docs/reference/_images/Ts_diagram_H2O.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/Ts_diagram_states.svg` & `fluprodia-3.0/docs/reference/_images/Ts_diagram_states.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/logph_R290_full.svg` & `fluprodia-3.0/docs/reference/_images/logph_R290_full.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/logph_R290_isolines.svg` & `fluprodia-3.0/docs/reference/_images/logph_R290_isolines.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/logph_R290_zoomed.svg` & `fluprodia-3.0/docs/reference/_images/logph_R290_zoomed.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/logph_R290_zoomed_temperature_labels.svg` & `fluprodia-3.0/docs/reference/_images/logph_R290_zoomed_temperature_labels.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/logph_diagram.svg` & `fluprodia-3.0/docs/reference/_images/logph_diagram.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/logph_diagram_H2O.svg` & `fluprodia-3.0/docs/reference/_images/logph_diagram_H2O.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/logph_diagram_R290.svg` & `fluprodia-3.0/docs/reference/_images/logph_diagram_R290.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/reference/_images/logph_diagram_states.svg` & `fluprodia-3.0/docs/reference/_images/logph_diagram_states.svg`

 * *Files identical despite different names*

### Comparing `fluprodia-2.2/docs/usage.rst` & `fluprodia-3.0/docs/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -434,8 +434,16 @@
     >>> plt.tight_layout()
     >>> fig.savefig('Ts_diagram_states.svg')
 
 .. note::
 
     The values for plotting must be passed in the diagrams unit system.
 
+Export the underlying data
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+You can export the underlying data in :code:`json` format:
+
+.. code-block:: python
+
+    >>> diagram.to_json("diagram.json")
+
 .. [1] Witte, F.; Tuschy, I. (2020). TESPy: Thermal Engineering Systems in Python. Journal of Open Source Software, 5(49), 2178, https://doi.org/10.21105/joss.02178.
```

### Comparing `fluprodia-2.2/pyproject.toml` & `fluprodia-3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     "docs/",
     "tests/",
 ]
 exclude = ["docs/_build"]
 
 [project]
 name = "fluprodia"
-version = "2.2"
-description = "Create beautiful fluid property diagrams using CoolProp and matplotlib"
+dynamic = ["version", "description"]
 readme = "README.rst"
 authors = [
     {name = "Francesco Witte", email = "tespy@witte.sh"},
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Education",
```

### Comparing `fluprodia-2.2/src/fluprodia/fluid_property_diagram.py` & `fluprodia-3.0/src/fluprodia/fluid_property_diagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,24 @@
 This file is part of project fluprodia (github.com/fwitte/fluprodia). It's
 copyrighted by the contributors recorded in the version control history of the
 file, available from its original location
 src/fluprodia/fluid_property_diagram.py
 
 SPDX-License-Identifier: MIT
 """
+import json
+import os
 
 import CoolProp as CP
 import numpy as np
 
+from fluprodia import __version__
 
-def beautiful_unit_string(unit):
+
+def _beautiful_unit_string(unit):
     r"""Convert unit fractions to latex.
 
     Parameters
     ----------
     unit : str
         Value of unit for input, e.g. :code:`m^3/kg`.
 
@@ -31,15 +35,15 @@
         numerator = unit.split('/')[0]
         denominator = unit.split('/')[1]
         unit = '$\\frac{' + numerator + '}{' + denominator + '}$'
 
     return unit
 
 
-def isolines_log(val_min, val_max):
+def _isolines_log(val_min, val_max):
     """Generate default logarithmic isolines.
 
     Parameters
     ----------
     val_min : float
         Minimum value for isoline range.
 
@@ -146,14 +150,18 @@
     ...            'values': iso_h,
     ...            'style': {'linewidth': 2, 'color': '#ff0000'}
     ...         }, 'v': {'values': np.array([])}},
     ...     x_min=0, x_max=8, y_min=0, y_max=700
     ... )
     >>> plt.tight_layout()
     >>> fig.savefig('Ts_Diagramm.pdf')
+
+    It is also possible to export the data of a diagram:
+
+    >>> diagram.to_json("./tmp/water.json")
     """
 
     def __init__(self, fluid):
         u"""Create a FluidPropertyDiagram object.
 
         Parameters
         ----------
@@ -168,17 +176,19 @@
         """
         self.fluid = fluid
         self.state = CP.AbstractState('HEOS', self.fluid)
 
         self.converters = {}
         self.converters['p'] = {
             'Pa': 1, 'hPa': 1e2, 'mbar': 1e2, 'psi': 6894.7572931783,
-            'kPa': 1e3, 'bar': 1e5, 'MPa': 1e6}
+            'kPa': 1e3, 'bar': 1e5, 'MPa': 1e6
+        }
         self.converters['T'] = {
-            'K': [0, 1], '°C': [273.15, 1], '°F': [459.67, 5 / 9]}
+            'K': [0, 1], '°C': [273.15, 1], '°F': [459.67, 5 / 9]
+        }
         self.converters['s'] = {'J/kgK': 1, 'kJ/kgK': 1e3, 'MJ/kgK': 1e6}
         self.converters['h'] = {'J/kg': 1, 'kJ/kg': 1e3, 'MJ/kg': 1e6}
         self.converters['v'] = {'m^3/kg': 1, 'l/kg': 1e-3}
         self.converters['Q'] = {'-': 1, '%': 0.01}
 
         self.units = {
             'p': 'Pa',
@@ -227,49 +237,47 @@
                 'x_property': 'v',
                 'y_property': 'p',
                 'x_scale': 'log',
                 'y_scale': 'linear'
             }
         }
 
+        self._setup_functions_and_inputs()
+        self._setup_datastructures()
+        self._setup_isoline_defaults()
+        self._setup_default_line_layout()
+        self._setup_default_label_positioning()
+
+    def _setup_functions_and_inputs(self):
+        """Setup lookup tables for isoline functions and CoolProp inputs."""
         self.single_isoline_functions = {
-            'p': self.single_isobaric,
-            'v': self.single_isochoric,
-            'T': self.single_isothermal,
-            'h': self.single_isenthalpic,
-            's': self.single_isentropic
+            'p': self._single_isobaric,
+            'v': self._single_isochoric,
+            'T': self._single_isothermal,
+            'h': self._single_isenthalpic,
+            's': self._single_isentropic
         }
-
         self.CoolProp_inputs = {
             'p': CP.iP,
             'v': CP.iDmass,
             'T': CP.iT,
             'h': CP.iHmass,
             's': CP.iSmass
         }
 
-        self.x_min = None
-        self.x_max = None
-        self.y_min = None
-        self.y_max = None
-
-        self.set_unit_system()
-
+    def _setup_datastructures(self):
+        """Set up datastructures for all isolines."""
         self.pressure = {'isolines': np.array([])}
         self.entropy = {'isolines': np.array([])}
         self.temperature = {'isolines': np.array([])}
         self.enthalpy = {'isolines': np.array([])}
         self.volume = {'isolines': np.array([])}
         self.quality = {'isolines': np.array([])}
 
-        self.set_isoline_defaults()
-        self.default_line_layout()
-        self.default_label_positioning()
-
-    def default_line_layout(self):
+    def _setup_default_line_layout(self):
         """Definition of the default isoline layout."""
         self.pressure['style'] = {
             'linestyle': '-.',
             'color': '#363636',
             'linewidth': 0.5
         }
         self.volume['style'] = {
@@ -294,15 +302,15 @@
         }
         self.temperature['style'] = {
             'linestyle': '--',
             'color': '#363636',
             'linewidth': 0.5
         }
 
-    def default_label_positioning(self):
+    def _setup_default_label_positioning(self):
         """Definition of the default label positioning."""
         self.pressure['label_position'] = 0.85
         self.volume['label_position'] = 0.7
         self.quality['label_position'] = 0.225
         self.entropy['label_position'] = 0.95
         self.enthalpy['label_position'] = 0.85
         self.temperature['label_position'] = 0.95
@@ -337,15 +345,15 @@
                 obj['isolines'] = self.convert_to_SI(kwargs[key], key).round(8)
             else:
                 msg = (
                     'The specified isoline \'' + key + '\' is not available. '
                     'Choose from: ' + str(keys) + '.')
                 print(msg)
 
-    def set_isoline_defaults(self):
+    def _setup_isoline_defaults(self):
         """Calculate the default values for the isolines."""
         self.p_trip = self.state.trivial_keyed_output(CP.iP_triple)
         self.p_max = self.state.trivial_keyed_output(CP.iP_max)
         self.T_trip = self.state.trivial_keyed_output(CP.iT_triple)
         self.T_max = self.state.trivial_keyed_output(CP.iT_max)
 
         self.p_crit = self.state.trivial_keyed_output(CP.iP_critical)
@@ -384,17 +392,17 @@
 
         step = round(int(self.s_max - self.s_min) / 15, -1)
         self.entropy['isolines'] = np.arange(self.s_min, self.s_max, step).round(8)
 
         step = round(int(self.h_max - self.h_min) / 15, -1)
         self.enthalpy['isolines'] = np.arange(0, self.h_max, step).round(8)
 
-        self.pressure['isolines'] = isolines_log(
+        self.pressure['isolines'] = _isolines_log(
             self.p_trip + 1e-2, self.p_max).round(8)
-        self.volume['isolines'] = isolines_log(self.v_min, self.v_max).round(8)
+        self.volume['isolines'] = _isolines_log(self.v_min, self.v_max).round(8)
 
     def set_unit_system(self, **kwargs):
         u"""Set the unit system for the fluid properties.
 
         Parameters
         ----------
         p : str
@@ -422,21 +430,21 @@
             :code:`-, %`.
         """
         for key, value in kwargs.items():
             if value in self.converters[key].keys():
                 self.units[key] = value
             else:
                 msg = (
-                    'The unit ' + str(value) + ' is not available for the '
-                    'fluid property ' + self.properties[key] + '. Please '
-                    'choose from ' + ', '.join(self.converters[key].keys()) +
-                    '.')
+                    f'The unit {value} is not available for the  fluid '
+                    f'property {self.properties[key]} . Please choose from '
+                    f'{", ".join(self.converters[key].keys())}.'
+                )
                 raise ValueError(msg)
 
-    def draw_isoline_label(self, fig, ax, isoline, property, idx, x, y, x_min, x_max, y_min, y_max):
+    def _draw_isoline_label(self, fig, ax, isoline, property, idx, x, y, x_min, x_max, y_min, y_max):
         """Draw a label for an isoline.
 
         Parameters
         ----------
         isoline : float
             Value of the isoline.
 
@@ -487,66 +495,66 @@
                     height / (np.log(y_max) - np.log(y_min)))
             else:
                 y_scaled = (y[idx] - y[idx - 1]) * (
                     height / (y_max - y_min))
 
             alpha = np.arctan(y_scaled / x_scaled) / (2 * np.pi) * 360
 
-        unit = beautiful_unit_string(self.units[property])
+        unit = _beautiful_unit_string(self.units[property])
 
         txt = str(isoline) + ' ' + unit
         ax.text(
             x[idx], y[idx], txt, fontsize=5,
             rotation=alpha, va='center', ha='center',
             bbox=dict(facecolor='white', edgecolor='white', pad=0.0)
         )
 
     def calc_isolines(self):
         """Calculate all isolines."""
-        self.isobaric()
-        self.isochoric()
-        self.isoquality()
-        self.isenthalpic()
-        self.isothermal()
-        self.isentropic()
+        self._isobaric()
+        self._isochoric()
+        self._isoquality()
+        self._isenthalpic()
+        self._isothermal()
+        self._isentropic()
 
-    def isobaric(self):
+    def _isobaric(self):
         """Calculate an isoline of constant pressure."""
         isolines = self.pressure['isolines']
 
         iterator = 1 / np.append(
             np.geomspace(self.v_min, self.v_intermediate, 100, endpoint=False),
             np.geomspace(self.v_intermediate, self.v_max, 100))
 
         for p in isolines.round(8):
-            self.pressure[p] = self.single_isobaric(iterator, np.ones(len(iterator)) * p)
+            self.pressure[p] = self._single_isobaric(iterator, np.ones(len(iterator)) * p)
 
-    def isochoric(self):
+    def _isochoric(self):
         """Calculate an isoline of constant specific volume."""
         isolines = self.volume['isolines']
 
         iterator = np.append(
             np.geomspace(self.p_trip, self.p_crit * 0.8, 100, endpoint=False),
             np.geomspace(self.p_crit * 0.8, self.p_max, 100))
 
         for v in isolines.round(8):
-            self.volume[v] = self.single_isochoric(
+            self.volume[v] = self._single_isochoric(
                 iterator, np.ones(len(iterator)) * 1 / v)
 
-    def isothermal(self):
+    def _isothermal(self):
         """Calculate an isoline of constant temperature."""
         isolines = self.temperature['isolines']
 
         iterator = np.linspace(self.s_min, self.s_max, 200)
 
         for T in isolines.round(8):
-            self.temperature[T] = self.single_isothermal(
+            self.temperature[T] = self._single_isothermal(
                 iterator, np.ones(len(iterator)) * T)
 
-    def isoquality(self):
+    def _isoquality(self):
         """Calculate an isoline of constant vapor mass fraction."""
         isolines = self.quality['isolines']
 
         iterator = np.append(
             np.linspace(self.T_trip, self.T_crit * 0.97, 40, endpoint=False),
             np.linspace(self.T_crit * 0.97, self.T_crit, 40))
 
@@ -566,37 +574,63 @@
 
             self.quality[Q]['h'] = np.asarray(self.quality[Q]['h'])
             self.quality[Q]['p'] = np.asarray(self.quality[Q]['p'])
             self.quality[Q]['v'] = np.asarray(self.quality[Q]['v'])
             self.quality[Q]['s'] = np.asarray(self.quality[Q]['s'])
             self.quality[Q]['T'] = np.asarray(self.quality[Q]['T'])
 
-    def isenthalpic(self):
+    def _isenthalpic(self):
         """Calculate an isoline of constant specific enthalpy."""
         isolines = self.enthalpy['isolines']
 
         iterator = 1 / np.append(
             np.geomspace(self.v_min, self.v_intermediate, 100, endpoint=False),
-            np.geomspace(self.v_intermediate, self.v_max, 100))
+            np.geomspace(self.v_intermediate, self.v_max, 100)
+        )
 
         for h in isolines.round(8):
-            self.enthalpy[h] = self.single_isenthalpic(
-                    iterator, np.ones(len(iterator)) * h)
+            self.enthalpy[h] = self._single_isenthalpic(
+                iterator, np.ones(len(iterator)) * h
+            )
 
-    def isentropic(self):
+    def _isentropic(self):
         """Calculate an isoline of constant specific entropy."""
         isolines = self.entropy['isolines']
 
         iterator = 1 / np.append(
             np.geomspace(self.v_min, self.v_intermediate, 100, endpoint=False),
             np.geomspace(self.v_intermediate, self.v_max, 100))
 
         for s in isolines.round(8):
-            self.entropy[s] = self.single_isentropic(
-                        iterator, np.ones(len(iterator)) * s)
+            self.entropy[s] = self._single_isentropic(
+                iterator, np.ones(len(iterator)) * s
+            )
+
+    def to_json(self, path):
+        data = {
+            prop: {
+                f"{isoline}": {
+                    subprop: list(getattr(self, prop)[isoline][subprop].astype(float))
+                    for subprop in getattr(self, prop)[isoline]
+                } for isoline in getattr(self, prop)["isolines"]
+            } for prop in self.properties.values()
+        }
+
+        data["META"] = {
+            "fluid": self.fluid,
+            "CoolProp-version": CP.__version__,
+            "fluprodia-version": __version__
+        }
+
+        directory = os.path.dirname(path)
+        if directory != "" and not os.path.exists(directory):
+            os.makedirs(directory)
+
+        with open(path, "w", encoding="utf-8") as f:
+            f.write(json.dumps(data, indent=2))
 
     def calc_individual_isoline(
             self, isoline_property=None,
             isoline_value=None,
             isoline_value_end=None,
             starting_point_property=None, ending_point_property=None,
             starting_point_value=None, ending_point_value=None):
@@ -750,95 +784,94 @@
         else:
             isoline_vector = np.linspace(isoline_value, isoline_value_end, 100)
 
         datapoints = f(iterator, isoline_vector)
 
         for key in datapoints.keys():
             datapoints[key] = self.convert_from_SI(datapoints[key], key)
+
         return datapoints
 
-    def single_isobaric(self, iterator, p):
+    def _single_isobaric(self, iterator, p):
         """Calculate an isoline of constant pressure."""
         datapoints = {'h': [], 'T': [], 'v': [], 's': [], 'p': [], 'Q': []}
 
         if iterator[0] < iterator[-1]:
             rising = True
         else:
             rising = False
 
-        i = 0
-        for val in iterator:
+        for i, val in enumerate(iterator):
             try:
                 self.state.update(CP.DmassP_INPUTS, val, p[i])
                 datapoints['h'] += [self.state.hmass()]
                 datapoints['T'] += [self.state.T()]
                 datapoints['v'] += [1 / val]
                 datapoints['s'] += [self.state.smass()]
                 datapoints['p'] += [p[i]]
                 if p[i] < self.p_crit:
                     datapoints['Q'] += [self.state.Q()]
                 else:
                     datapoints['Q'] += [-1]
 
             except ValueError as e:
                 pass
-            i += 1
 
         for key in datapoints.keys():
             datapoints[key] = np.asarray(datapoints[key])
 
-        data = self.get_Q_crossings(datapoints, 'p', rising)
+        data = self._get_Q_crossings(datapoints, 'p', rising)
         if len(data) == 0:
             return datapoints
         else:
-            return self.insert_Q_crossings(datapoints, 'p', data)
+            return self._insert_Q_crossings(datapoints, 'p', data)
 
-    def single_isochoric(self, iterator, D):
+    def _single_isochoric(self, iterator, D):
         """Calculate an isoline of constant specific volume."""
         datapoints = {'h': [], 'T': [], 'v': [], 's': [], 'p': [], 'Q': []}
 
         if iterator[0] < iterator[-1]:
             rising = True
         else:
             rising = False
 
-        i = 0
-        for val in iterator:
+        for i, val in enumerate(iterator):
             try:
                 self.state.update(CP.DmassP_INPUTS, D[i], val)
                 datapoints['h'] += [self.state.hmass()]
                 datapoints['T'] += [self.state.T()]
                 datapoints['v'] += [1 / D[i]]
                 datapoints['s'] += [self.state.smass()]
                 datapoints['p'] += [val]
                 if val < self.p_crit:
                     datapoints['Q'] += [self.state.Q()]
                 else:
                     datapoints['Q'] += [-1]
             except ValueError:
                 pass
-            i += 1
 
         for key in datapoints.keys():
             datapoints[key] = np.asarray(datapoints[key])
 
-        data = self.get_Q_crossings(datapoints, 'v', rising)
-        return self.insert_Q_crossings(datapoints, 'v', data)
+        data = self._get_Q_crossings(datapoints, 'v', rising)
+        if len(data) == 0:
+            return datapoints
+        else:
+            return self._insert_Q_crossings(datapoints, 'v', data)
 
-    def single_isothermal(self, iterator, T):
+    def _single_isothermal(self, iterator, T):
         """Calculate an isoline of constant temperature."""
         datapoints = {'h': [], 'T': [], 'v': [], 's': [], 'p': [], 'Q': []}
 
         if iterator[0] < iterator[-1]:
             rising = True
         else:
             rising = False
 
-        i = 0
-        for val in iterator:
+        for i, val in enumerate(iterator):
             try:
                 self.state.update(CP.SmassT_INPUTS, val, T[i])
                 datapoints['T'] += [T[i]]
                 datapoints['p'] += [self.state.p()]
                 datapoints['v'] += [1 / self.state.rhomass()]
                 datapoints['s'] += [val]
                 datapoints['h'] += [self.state.hmass()]
@@ -846,78 +879,75 @@
                     datapoints['Q'] += [self.state.Q()]
                 else:
                     datapoints['Q'] += [-1]
             except ValueError:
                 # for some reason PropSI inputs are way more stable here
                 try:
                     p = CP.CoolProp.PropsSI(
-                        'P', 'T', T[i], 'S', val, self.fluid)
+                        'P', 'T', T[i], 'S', val, self.fluid
+                    )
                     self.state.update(CP.PSmass_INPUTS, val, p)
                     datapoints['T'] += [T[i]]
                     datapoints['p'] += [p]
                     datapoints['v'] += [1 / self.state.rhomass()]
                     datapoints['s'] += [val]
                     datapoints['h'] += [self.state.hmass()]
                 except ValueError:
                     pass
-            i += 1
 
         for key in datapoints.keys():
             datapoints[key] = np.asarray(datapoints[key])
 
-        data = self.get_Q_crossings(datapoints, 'T', rising)
-        return self.insert_Q_crossings(datapoints, 'T', data)
+        data = self._get_Q_crossings(datapoints, 'T', rising)
+        if len(data) == 0:
+            return datapoints
+        else:
+            return self._insert_Q_crossings(datapoints, 'T', data)
 
-    def single_isenthalpic(self, iterator, h):
+    def _single_isenthalpic(self, iterator, h):
         """Calculate an isoline of constant specific enthalpy."""
         datapoints = {'h': [], 'T': [], 'v': [], 's': [], 'p': []}
 
-        i = 0
-        for val in iterator:
+        for i, val in enumerate(iterator):
             try:
                 self.state.update(CP.DmassHmass_INPUTS, val, h[i])
                 datapoints['T'] += [self.state.T()]
                 datapoints['p'] += [self.state.p()]
                 datapoints['v'] += [1 / val]
                 datapoints['s'] += [self.state.smass()]
                 datapoints['h'] += [h[i]]
             except ValueError:
                 pass
 
-            i += 1
-
         for key in datapoints.keys():
             datapoints[key] = np.asarray(datapoints[key])
 
         return datapoints
 
-    def single_isentropic(self, iterator, s):
+    def _single_isentropic(self, iterator, s):
         """Calculate an isoline of constant specific entropy."""
         datapoints = {'h': [], 'T': [], 'v': [], 's': [], 'p': []}
 
-        i = 0
-        for val in iterator:
+        for i, val in enumerate(iterator):
             try:
                 self.state.update(CP.DmassSmass_INPUTS, val, s[i])
                 datapoints['T'] += [self.state.T()]
                 datapoints['p'] += [self.state.p()]
                 datapoints['v'] += [1 / val]
                 datapoints['s'] += [s[i]]
                 datapoints['h'] += [self.state.hmass()]
             except ValueError:
                 pass
 
-            i += 1
-
         for key in datapoints.keys():
             datapoints[key] = np.asarray(datapoints[key])
 
         return datapoints
 
-    def get_Q_crossings(self, datapoints, property, rising):
+    def _get_Q_crossings(self, datapoints, property, rising):
         """Return data of Q=0 or Q=1 crossings of specified line."""
         num_points = len(datapoints['Q'])
         distance_to_gas = 1 - datapoints['Q']
         distance_to_liq = datapoints['Q']
 
         idx_gas = np.argwhere(
             (distance_to_gas < distance_to_liq) &
@@ -956,25 +986,27 @@
                 Q2 = datapoints['Q'][idx_liq[pos] + next_point]
                 prop1 = datapoints[property][idx_liq[pos]]
                 prop2 = datapoints[property][idx_liq[pos] + next_point]
                 data[0] = prop1 + (0 - Q1) / (Q2 - Q1) * (prop2 - prop1)
 
         return data
 
-    def insert_Q_crossings(self, datapoints, property, data):
+    def _insert_Q_crossings(self, datapoints, property, data):
         """Insert data of Q=0 and Q=1 crossings into specified line."""
         rising = datapoints['s'][0] < datapoints['s'][-1]
         for Q, value in data.items():
             if property == 'v':
                 value = 1 / value
             try:
                 self.state.update(*CP.CoolProp.generate_update_pair(
-                    self.CoolProp_inputs[property], value, CP.iQ, Q))
+                    self.CoolProp_inputs[property], value, CP.iQ, Q)
+                )
             except ValueError:
                 continue
+
             s = self.state.smass()
 
             if rising:
                 position = np.searchsorted(datapoints['s'], s)
             else:
                 position = np.searchsorted(-datapoints['s'], -s)
 
@@ -991,63 +1023,76 @@
                         result = 1 / result
                     datapoints[prop] = np.insert(
                         datapoints[prop], position, result
                     )
 
         return datapoints
 
-    def draw_isolines(self, fig, ax, diagram_type, x_min, x_max, y_min, y_max, isoline_data={}):
-        """Draw the isolines of a specific diagram type.
+    def draw_isolines(self, fig, ax, diagram_type, x_min, x_max, y_min, y_max, isoline_data=None):
+        """_summary_
 
         Parameters
         ----------
+        fig : matplotlib.pyplot.figure
+            Figure to draw into
+
+        ax : matplotlib.pyplot.axes
+            Axes to draw into
+
         diagram_type : str
-            Which type of diagram should be drawn.
+            Name of the diagram
+
+        x_min : number
+            Minimum for x range
+
+        x_max : number
+            Maximum for x range
+
+        y_min : number
+            Minimum for y range
 
-        isoline_data : dict
-            Dictionary holding additional data on the isolines to be drawn.
-            These are
+        y_max : number
+            Maximum for y range
+
+        isoline_data : dict, optional
+            Dictionary holding additional data on the isolines to be drawn,
+            by default None. These are
 
             - the isoline values with key :code:`values` and
             - the isoline style with key :code:`style`.
 
             The islonline style is another dictionary holding keyword arguments
             of a :code:`matplotlib.lines.Line2D` object. See
             https://matplotlib.org/api/_as_gen/matplotlib.lines.Line2D.html#matplotlib.lines.Line2D
             for more information.
         """
-        if not isinstance(diagram_type, str):
-            msg = (
-                'The diagram_type must be specified as string. Available '
-                'inputs are: ' + str(self.supported_diagrams.keys()) + '.')
-            raise TypeError(msg)
-        elif diagram_type not in self.supported_diagrams.keys():
-            msg = (
-                'The specified diagram_type is not available. Available '
-                'inputs are: ' + str(self.supported_diagrams.keys()) + '.')
-            raise ValueError(msg)
+        if isoline_data is None:
+            isoline_data = {}
+
+        self._check_diagram_types(diagram_type)
+
+        x_scale = self.supported_diagrams[diagram_type]['x_scale']
+        y_scale = self.supported_diagrams[diagram_type]['y_scale']
+
+        x_property = self.supported_diagrams[diagram_type]['x_property']
+        y_property = self.supported_diagrams[diagram_type]['y_property']
 
         ax.clear()
 
         ax.set_ylim([y_min, y_max])
         ax.set_xlim([x_min, x_max])
 
-        x_property = self.supported_diagrams[diagram_type]['x_property']
-        y_property = self.supported_diagrams[diagram_type]['y_property']
-        x_scale = self.supported_diagrams[diagram_type]['x_scale']
-        y_scale = self.supported_diagrams[diagram_type]['y_scale']
         ax.set_xscale(x_scale)
         ax.set_yscale(y_scale)
 
-        self.x_label = (
-            x_property + ' in ' +
-            beautiful_unit_string(self.units[x_property]))
-        self.y_label = (
-            y_property + ' in ' +
-            beautiful_unit_string(self.units[y_property]))
+        x_label = f'{x_property} in {_beautiful_unit_string(self.units[x_property])}'
+        y_label = f'{y_property} in {_beautiful_unit_string(self.units[y_property])}'
+
+        ax.set_xlabel(x_label)
+        ax.set_ylabel(y_label)
 
         isolines = [
             x for x in self.properties.keys()
             if x not in [x_property, y_property]
         ]
 
         for isoline in isolines:
@@ -1060,25 +1105,28 @@
             if isoline in isoline_data.keys():
                 keys = isoline_data[isoline].keys()
                 if 'style' in keys:
                     data['style'].update(isoline_data[isoline]['style'])
 
                 if 'values' in keys:
                     isovalues = self.convert_to_SI(
-                        isoline_data[isoline]['values'], isoline)
+                        isoline_data[isoline]['values'], isoline
+                    )
 
                 if 'label_position' in keys:
                     data['label_position'] = (
-                        isoline_data[isoline]['label_position'])
+                        isoline_data[isoline]['label_position']
+                    )
 
             for isoval in isovalues.round(8):
                 if isoval not in data['isolines']:
                     msg = (
-                        'Could not find data for ' + property + ' isoline '
-                        'with value: ' + str(isoval) + '.')
+                        f'Could not find data for {property} isoline with '
+                        f'value: {isoval}.'
+                    )
                     continue
 
                 x = self.convert_from_SI(data[isoval][x_property], x_property)
                 y = self.convert_from_SI(data[isoval][y_property], y_property)
 
                 indices = np.intersect1d(
                     np.where((x >= x_min) & (x <= x_max)),
@@ -1103,32 +1151,48 @@
                 y = y[indices]
                 x = x[indices]
 
                 ax.plot(x, y, **data['style'])
 
                 isoval = self.convert_from_SI(isoval, isoline)
 
-                self.draw_isoline_label(
+                self._draw_isoline_label(
                     fig, ax,
                     isoval.round(8), isoline,
                     int(data['label_position'] * len(x)),
                     x, y, x_min, x_max, y_min, y_max
                 )
 
+    def _check_diagram_types(self, diagram_type):
+        if not isinstance(diagram_type, str):
+            msg = (
+                'The diagram_type must be specified as string. Available '
+                f'inputs are: {", ".join(self.supported_diagrams.keys())}.'
+            )
+            raise TypeError(msg)
+        elif diagram_type not in self.supported_diagrams.keys():
+            msg = (
+                'The specified diagram_type is not available. Available '
+                f'types are: {", ".join(self.supported_diagrams.keys())}.'
+            )
+            raise ValueError(msg)
+
     def convert_to_SI(self, value, property):
         """Convert a value to its SI value."""
         if property == 'T':
             return (
-                (value +
-                 self.converters[property][self.units[property]][0]) *
-                self.converters[property][self.units[property]][1])
+                (
+                    value + self.converters[property][self.units[property]][0]
+                ) * self.converters[property][self.units[property]][1]
+            )
         else:
             return value * self.converters[property][self.units[property]]
 
     def convert_from_SI(self, value, property):
         """Convert a SI value to value in respecive unit system."""
         if property == 'T':
             return (
-                value / self.converters[property][self.units[property]][1] -
-                self.converters[property][self.units[property]][0])
+                value / self.converters[property][self.units[property]][1]
+                - self.converters[property][self.units[property]][0]
+            )
         else:
             return value / self.converters[property][self.units[property]]
```

### Comparing `fluprodia-2.2/PKG-INFO` & `fluprodia-3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluprodia
-Version: 2.2
+Version: 3.0
 Summary: Create beautiful fluid property diagrams using CoolProp and matplotlib
 Author-email: Francesco Witte <tespy@witte.sh>
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

