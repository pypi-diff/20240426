# Comparing `tmp/nqrduck_measurement-0.0.2.tar.gz` & `tmp/nqrduck_measurement-0.0.3.tar.gz`

## Comparing `nqrduck_measurement-0.0.2.tar` & `nqrduck_measurement-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0  5520293 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/docs/img/measurement_ui_labeled_v2.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/src/nqrduck_measurement/__init__.py
--rw-r--r--   0        0        0     9748 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/src/nqrduck_measurement/controller.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/src/nqrduck_measurement/measurement.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/src/nqrduck_measurement/model.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/src/nqrduck_measurement/signalprocessing_options.py
--rw-r--r--   0        0        0     9677 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/src/nqrduck_measurement/view.py
--rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/src/nqrduck_measurement/widget.py
--rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/src/nqrduck_measurement/resources/measurement_widget.ui
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/src/nqrduck_measurement/resources/mesurement.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/LICENSE
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/README.md
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0  5520293 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/docs/img/measurement_ui_labeled_v2.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/__init__.py
+-rw-r--r--   0        0        0     8352 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/controller.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/measurement.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/model.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/signalprocessing_options.py
+-rw-r--r--   0        0        0     9677 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/view.py
+-rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/widget.py
+-rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/resources/measurement_widget.ui
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/src/nqrduck_measurement/resources/mesurement.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/README.md
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 nqrduck_measurement-0.0.3/PKG-INFO
```

### Comparing `nqrduck_measurement-0.0.2/.github/workflows/python-publish.yml` & `nqrduck_measurement-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.2/docs/img/measurement_ui_labeled_v2.png` & `nqrduck_measurement-0.0.3/docs/img/measurement_ui_labeled_v2.png`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.2/src/nqrduck_measurement/controller.py` & `nqrduck_measurement-0.0.3/src/nqrduck_measurement/controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import logging
 import json
 import numpy as np
 from decimal import Decimal
 from PyQt6.QtCore import pyqtSlot, pyqtSignal
 from PyQt6.QtWidgets import QApplication
-from nqrduck_pulseprogrammer.view import OptionsDialog
 from nqrduck_spectrometer.pulsesequence import PulseSequence
 from .signalprocessing_options import Apodization
 from nqrduck.module.module_controller import ModuleController
 from nqrduck_spectrometer.measurement import Measurement
 
 logger = logging.getLogger(__name__)
 
@@ -207,52 +206,26 @@
         if not self.module.model.displayed_measurement:
             logger.debug("No measurement to apodize.")
             self.module.nqrduck_signal.emit(
                 "notification", ["Error", "No measurement to apodize."]
             )
             return
 
-        # We need to create a event which corresponds to the measurement.
-        event_duration = self.module.model.displayed_measurement.tdx[-1] * 1e-6
+        measurement = self.module.model.displayed_measurement
 
-        event = PulseSequence.Event(name="Apodization", duration=str(event_duration))
-        parameter = Apodization()
-        parameter.start_x = 0
-        parameter.end_x = event_duration
-        dialog = OptionsDialog(event, parameter, self.module.view)
+        dialog = Apodization(measurement, parent=self.module.view)
         result = dialog.exec()
 
-        if result:
-            for option, function in dialog.return_functions.items():
-                logger.debug(
-                    "Setting option %s of parameter %s in event %s to %s",
-                    option,
-                    parameter,
-                    event,
-                    function(),
-                )
-                option.set_value(function())
+        logger.debug("Dialog result: %s", result)
+        if not result:
+            return
+
+        function = dialog.get_function()
 
-        # Get the function from the Apodization function
-        function = parameter.get_option_by_name(Apodization.APODIZATION_FUNCTIONS).value
         logger.debug("Apodization function: %s", function)
 
-        # Get the y data weights from the function
-        resolution = (
-            self.module.model.displayed_measurement.tdx[1]
-            - self.module.model.displayed_measurement.tdx[0]
-        ) * 1e-6
-        y_weight = function.get_pulse_amplitude(event.duration, Decimal(resolution))
-        # Append the last point to the end of the array
-        y_weight = np.append(y_weight, y_weight[-1])
-
-        tdy_measurement = self.module.model.displayed_measurement.tdy * y_weight
-
-        measurement = Measurement(
-            self.module.model.displayed_measurement.tdx,
-            tdy_measurement,
-            target_frequency=self.module.model.displayed_measurement.target_frequency,
-            IF_frequency=self.module.model.displayed_measurement.IF_frequency,
-        )
+        apodized_measurement = measurement.apodization(function)
+
+        dialog.deleteLater()
 
-        self.module.model.displayed_measurement = measurement
-        self.module.model.add_measurement(measurement)
+        self.module.model.displayed_measurement = apodized_measurement
+        self.module.model.add_measurement(apodized_measurement)
```

### Comparing `nqrduck_measurement-0.0.2/src/nqrduck_measurement/model.py` & `nqrduck_measurement-0.0.3/src/nqrduck_measurement/model.py`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.2/src/nqrduck_measurement/signalprocessing_options.py` & `nqrduck_measurement-0.0.3/src/nqrduck_measurement/signalprocessing_options.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """Signal processing options."""
-
+import logging 
+from decimal import Decimal
+import numpy as np
 import sympy
-from nqrduck_spectrometer.base_spectrometer_model import BaseSpectrometerModel
-from nqrduck_spectrometer.pulseparameters import (
-    FunctionOption,
-    GaussianFunction,
-    CustomFunction,
-    Function,
-)
-
-# We implement the signal processing options as PulseParamterOptions because we can then easily use the automatic UI generation
+from nqrduck_spectrometer.measurement import Measurement
+from nqrduck.helpers.functions import Function, GaussianFunction, CustomFunction
+from nqrduck.helpers.formbuilder import DuckFormBuilder, DuckFormFunctionSelectionField
 
+logger = logging.getLogger(__name__)
 
 class FIDFunction(Function):
     """The exponetial FID function."""
 
     name = "FID"
 
     def __init__(self) -> None:
@@ -23,29 +20,41 @@
         super().__init__(expr)
         self.start_x = 0
         self.end_x = 30
 
         self.add_parameter(Function.Parameter("T2star (microseconds)", "T2star", 10))
 
 
-class Apodization(BaseSpectrometerModel.PulseParameter):
+class Apodization(DuckFormBuilder):
     """Apodization parameter.
 
     This parameter is used to apply apodization functions to the signal.
     The apodization functions are used to reduce the noise in the signal.
-
-    Attributes:
-        APODIZATION_FUNCTIONS (str): The name of the apodization functions option.
     """
 
-    APODIZATION_FUNCTIONS = "Apodization functions"
-
-    def __init__(self):
+    def __init__(self, measurement: Measurement, parent=None) -> None:
         """Apodization parameter."""
-        super().__init__("Apodization")
+        super().__init__("Apodization", parent=parent)
+
+        self.measurement = measurement
+        functions = [
+            FIDFunction(),
+            GaussianFunction(),
+            CustomFunction(),
+        ]
 
-        self.add_option(
-            FunctionOption(
-                self.APODIZATION_FUNCTIONS,
-                [FIDFunction(), GaussianFunction(), CustomFunction()],
-            ),
+        self.duration = (self.measurement.tdx[-1] - self.measurement.tdx[0]) * 1e-6
+
+        function_selection_field = DuckFormFunctionSelectionField(
+            text=None, tooltip=None, functions=functions, duration=self.duration, parent=parent, default_function=0
         )
+
+        self.add_field(function_selection_field)
+
+    def get_function(self) -> Function:
+        """Get the selected function.
+
+        Returns:
+            Function: The selected function.
+        """
+        return self.get_values()[0]
+
```

### Comparing `nqrduck_measurement-0.0.2/src/nqrduck_measurement/view.py` & `nqrduck_measurement-0.0.3/src/nqrduck_measurement/view.py`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.2/src/nqrduck_measurement/widget.py` & `nqrduck_measurement-0.0.3/src/nqrduck_measurement/widget.py`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.2/src/nqrduck_measurement/resources/measurement_widget.ui` & `nqrduck_measurement-0.0.3/src/nqrduck_measurement/resources/measurement_widget.ui`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.2/LICENSE` & `nqrduck_measurement-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.2/README.md` & `nqrduck_measurement-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck_measurement-0.0.2/pyproject.toml` & `nqrduck_measurement-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck-measurement"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "A module for the NQRduck program (a simple python script™) to perform single frequency measurements."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck_measurement-0.0.2/PKG-INFO` & `nqrduck_measurement-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck-measurement
-Version: 0.0.2
+Version: 0.0.3
 Summary: A module for the NQRduck program (a simple python script™) to perform single frequency measurements.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-measurement/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-measurement
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
```

