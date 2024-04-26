# Comparing `tmp/nqrduck_pulseprogrammer-0.0.2.tar.gz` & `tmp/nqrduck_pulseprogrammer-0.0.3.tar.gz`

## Comparing `nqrduck_pulseprogrammer-0.0.2.tar` & `nqrduck_pulseprogrammer-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0   102155 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/docs/img/pulseprogrammer_labeled.png
--rw-r--r--   0        0        0   990292 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/docs/img/pulseprogrammer_tx_labeled.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/src/nqrduck_pulseprogrammer/__init__.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/src/nqrduck_pulseprogrammer/controller.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/src/nqrduck_pulseprogrammer/model.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/src/nqrduck_pulseprogrammer/pulseprogrammer.py
--rw-r--r--   0        0        0    35827 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/src/nqrduck_pulseprogrammer/view.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/src/nqrduck_pulseprogrammer/resources/pulseprogrammer.ini
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/LICENSE
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/README.md
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   102155 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/docs/img/pulseprogrammer_labeled.png
+-rw-r--r--   0        0        0   990292 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/docs/img/pulseprogrammer_tx_labeled.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/__init__.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/controller.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/model.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/pulseprogrammer.py
+-rw-r--r--   0        0        0    25627 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/view.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/resources/pulseprogrammer.ini
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/README.md
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 nqrduck_pulseprogrammer-0.0.3/PKG-INFO
```

### Comparing `nqrduck_pulseprogrammer-0.0.2/.github/workflows/python-publish.yml` & `nqrduck_pulseprogrammer-0.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_pulseprogrammer-0.0.2/docs/img/pulseprogrammer_labeled.png` & `nqrduck_pulseprogrammer-0.0.3/docs/img/pulseprogrammer_labeled.png`

 * *Files identical despite different names*

### Comparing `nqrduck_pulseprogrammer-0.0.2/docs/img/pulseprogrammer_tx_labeled.png` & `nqrduck_pulseprogrammer-0.0.3/docs/img/pulseprogrammer_tx_labeled.png`

 * *Files identical despite different names*

### Comparing `nqrduck_pulseprogrammer-0.0.2/src/nqrduck_pulseprogrammer/controller.py` & `nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/controller.py`

 * *Files identical despite different names*

### Comparing `nqrduck_pulseprogrammer-0.0.2/src/nqrduck_pulseprogrammer/model.py` & `nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from decimal import Decimal
 from collections import OrderedDict
 from PyQt6.QtCore import pyqtSignal
 from nqrduck.module.module_model import ModuleModel
 from nqrduck_spectrometer.pulsesequence import PulseSequence
 
 logger = logging.getLogger(__name__)
 
@@ -14,23 +13,23 @@
     pulse_sequence_changed = pyqtSignal()
 
     def __init__(self, module):
         super().__init__(module)
         self.pulse_parameter_options = OrderedDict()
         self.pulse_sequence = PulseSequence("Untitled pulse sequence")
 
-    def add_event(self, event_name: str, duration: Decimal = 20):
+    def add_event(self, event_name: str, duration: float = 20):
         """Add a new event to the current pulse sequence.
 
         Args:
             event_name (str): A human-readable name for the event
-            duration (Decimal): The duration of the event in µs. Defaults to 20.
+            duration (float): The duration of the event in µs. Defaults to 20.
         """
         self.pulse_sequence.events.append(
-            PulseSequence.Event(event_name, "%.16gu" % duration)
+            PulseSequence.Event(event_name, "%.16gu" % float(duration))
         )
         logger.debug(
             "Creating event %s with object id %s",
             event_name,
             id(self.pulse_sequence.events[-1]),
         )
```

### Comparing `nqrduck_pulseprogrammer-0.0.2/src/nqrduck_pulseprogrammer/view.py` & `nqrduck_pulseprogrammer-0.0.3/src/nqrduck_pulseprogrammer/view.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 import logging
 import functools
-from collections import OrderedDict
-from decimal import Decimal
 from PyQt6.QtGui import QValidator
 from PyQt6.QtWidgets import (
-    QMessageBox,
-    QGroupBox,
     QFormLayout,
     QTableWidget,
     QVBoxLayout,
     QPushButton,
     QHBoxLayout,
     QLabel,
     QDialog,
     QLineEdit,
     QDialogButtonBox,
     QWidget,
-    QCheckBox,
     QToolButton,
     QFileDialog,
     QSizePolicy,
 )
 from PyQt6.QtCore import pyqtSlot, pyqtSignal
 from nqrduck.module.module_view import ModuleView
 from nqrduck.assets.icons import Logos
 from nqrduck.helpers.duckwidgets import DuckFloatEdit, DuckEdit
 from nqrduck_spectrometer.pulseparameters import (
     BooleanOption,
     NumericOption,
     FunctionOption,
 )
+from nqrduck.helpers.formbuilder import (
+    DuckFormBuilder,
+    DuckFormFunctionSelectionField,
+    DuckFormCheckboxField,
+    DuckFormDropdownField,
+    DuckFormFloatField,
+    DuckFormIntField,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class PulseProgrammerView(ModuleView):
 
     def __init__(self, module):
@@ -171,15 +174,15 @@
         event_parameters_label = QLabel("Event lengths:")
         event_layout.addWidget(event_parameters_label)
 
         for event in self.module.model.pulse_sequence.events:
             logger.debug("Adding event to pulseprogrammer view: %s", event.name)
             # Create a label for the event
             event_label = QLabel(
-                "%s : %.16g µs" % (event.name, (event.duration * Decimal(1e6)))
+                "%s : %.16g µs" % (event.name, (event.duration * 1e6))
             )
             event_layout.addWidget(event_label)
 
         # Delete the old widget and create a new one
         self.event_widget.deleteLater()
         self.event_widget = QWidget()
         self.event_widget.setLayout(event_layout)
@@ -256,27 +259,73 @@
                 button.clicked.connect(func)
 
     @pyqtSlot()
     def on_table_button_clicked(self, event, parameter) -> None:
         """This method is called whenever a button in the pulse table is clicked. It opens a dialog to set the options for the parameter."""
         logger.debug("Button for event %s and parameter %s clicked", event, parameter)
         # Create a QDialog to set the options for the parameter.
-        dialog = OptionsDialog(event, parameter, self)
+        description = f"Set options for {parameter}"
+        dialog = DuckFormBuilder(parameter, description=description, parent=self)
+
+        # Adding fields for the options
+        form_options = []
+        for option in event.parameters[parameter].options:
+            if isinstance(option, BooleanOption):
+                boolean_form = DuckFormCheckboxField(
+                    option.name, tooltip=None, default=option.value
+                )
+                dialog.add_field(boolean_form)
+                form_options.append(option)
+            elif isinstance(option, NumericOption):
+                # We only show the slider if both min and max values are set
+                if option.min_value is not None and option.max_value is not None:
+                    slider = True
+                else:
+                    slider = False
+
+                numeric_field = DuckFormFloatField(
+                    option.name,
+                    tooltip=None,
+                    default=option.value,
+                    min_value=option.min_value,
+                    max_value=option.max_value,
+                    slider=slider,
+                )
+
+                dialog.add_field(numeric_field)
+                form_options.append(option)
+            elif isinstance(option, FunctionOption):
+                logger.debug(f"Functions: {option.functions}")
+
+                # When loading a pulse sequence, the instance of the objects will be different
+                # Therefore we need to operate on the classes
+                for function in option.functions:
+                    if function.__class__.__name__ == option.value.__class__.__name__:
+                        default_function = function
+
+                index = option.functions.index(default_function)
+
+                function_field = DuckFormFunctionSelectionField(
+                    option.name,
+                    tooltip=None,
+                    functions=option.functions,
+                    duration=event.duration,
+                    default_function=index,
+                )
+                dialog.add_field(function_field)
+                form_options.append(option)
+
         result = dialog.exec()
 
+        options = event.parameters[parameter].options
+
         if result:
-            for option, function in dialog.return_functions.items():
-                logger.debug(
-                    "Setting option %s of parameter %s in event %s to %s",
-                    option,
-                    parameter,
-                    event,
-                    function(),
-                )
-                option.set_value(function())
+            values = dialog.get_values()
+            for i, value in enumerate(values):
+                options[i].value = value
 
             self.set_parameter_icons()
 
     @pyqtSlot()
     def on_save_button_clicked(self) -> None:
         """This method is called whenever the save button is clicked. It opens a dialog to select a file to save the pulse sequence to."""
         logger.debug("Save button clicked")
@@ -378,15 +427,15 @@
         name_label = QLabel("Name:")
         name_lineedit = QLineEdit(self.event.name)
         event_form_layout.addRow(name_label, name_lineedit)
         duration_layout = QHBoxLayout()
         duration_label = QLabel("Duration:")
         duration_lineedit = QLineEdit()
         unit_label = QLabel("µs")
-        duration_lineedit.setText("%.16g" % (self.event.duration * Decimal(1e6)))
+        duration_lineedit.setText("%.16g" % (self.event.duration * 1e6))
         duration_layout.addWidget(duration_label)
         duration_layout.addWidget(duration_lineedit)
         duration_layout.addWidget(unit_label)
         event_form_layout.addRow(duration_layout)
         layout.addLayout(event_form_layout)
 
         buttons = QDialogButtonBox(
@@ -437,302 +486,14 @@
 
     def move_event_right_button_clicked(self) -> None:
         """This method is called when the move right button is clicked."""
         logger.debug("Move event right: %s", self.event.name)
         self.move_event_right.emit(self.event.name)
 
 
-class OptionsDialog(QDialog):
-    """This dialog is created whenever the edit button for a pulse option is clicked.
-    It allows the user to change the options for the pulse parameter and creates the dialog in accordance to what can be set.
-    """
-
-    def __init__(self, event, parameter, parent=None):
-        super().__init__(parent)
-        self.parent = parent
-
-        self.setWindowTitle("Options")
-
-        self.layout = QVBoxLayout(self)
-
-        numeric_layout = QFormLayout()
-        numeric_layout.setHorizontalSpacing(30)
-
-        self.label = QLabel("Change options for the pulse parameter: %s" % parameter)
-        self.layout.addWidget(self.label)
-
-        self.layout.addLayout(numeric_layout)
-
-        # If the parameter is a string, we first need to get the parameter object from the according event
-        if isinstance(parameter, str):
-            parameter = event.parameters[parameter]
-
-        options = parameter.get_options()
-
-        # Based on these options we will now create our selection widget
-        self.return_functions = OrderedDict()
-
-        # If the options are a list , we will create a QComboBox
-        for option in options:
-            if option == list:
-                pass
-            # If the options are boolean, we will create a QCheckBox
-            elif isinstance(option, BooleanOption):
-                check_box = QCheckBox()
-
-                def checkbox_result():
-                    return check_box.isChecked()
-
-                check_box.setChecked(option.value)
-                self.layout.addWidget(check_box)
-                self.return_functions[option] = checkbox_result
-
-            # If the options are a float/int we will create a QSpinBox
-            elif isinstance(option, NumericOption):
-                numeric_label = QLabel(option.name)
-                numeric_lineedit = QLineEdit(str(option.value))
-                numeric_lineedit.setMaximumWidth(300)
-                numeric_layout.addRow(numeric_label, numeric_lineedit)
-
-                self.return_functions[option] = numeric_lineedit.text
-
-            # If the options are a string we will create a QLineEdit
-            elif option == str:
-                pass
-
-            elif isinstance(option, FunctionOption):
-                function_option = FunctionOptionWidget(option, event, parent)
-                self.layout.addWidget(function_option)
-
-        logger.debug("Return functions are: %s" % self.return_functions.items())
-
-        self.buttons = QDialogButtonBox(
-            QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel,
-            self,
-        )
-        self.buttons.accepted.connect(self.accept)
-        self.buttons.rejected.connect(self.reject)
-
-        self.layout.addWidget(self.buttons)
-
-
-class FunctionOptionWidget(QWidget):
-    """This class is a widget that can be used to set the options for a pulse parameter.
-    It plots the given function in time and frequency domain.
-    One can also select the function from a list of functions represented as buttons.
-    """
-
-    def __init__(self, function_option, event, parent=None):
-        super().__init__(parent)
-        self.parent = parent
-
-        self.function_option = function_option
-        self.event = event
-        layout = QVBoxLayout()
-        inner_layout = QHBoxLayout()
-        for function in function_option.functions:
-            button = QPushButton(function.name)
-            button.clicked.connect(
-                functools.partial(self.on_functionbutton_clicked, function=function)
-            )
-            inner_layout.addWidget(button)
-
-        layout.addLayout(inner_layout)
-        self.setLayout(layout)
-
-        # Add Advanced settings button
-        self.advanced_settings_button = QPushButton("Show Advanced settings")
-        self.advanced_settings_button.clicked.connect(
-            self.on_advanced_settings_button_clicked
-        )
-        layout.addWidget(self.advanced_settings_button)
-
-        # Add advanced settings widget
-        self.advanced_settings = QGroupBox("Advanced Settings")
-        self.advanced_settings.setHidden(True)
-        self.advanced_settings_layout = QFormLayout()
-        self.advanced_settings.setLayout(self.advanced_settings_layout)
-        layout.addWidget(self.advanced_settings)
-
-        # Add the advanced settings
-        # Advanced settings are  resolution, start_x = -1, end_x and the expr of the function_option.value
-        resolution_layout = QHBoxLayout()
-        resolution_label = QLabel("Resolution:")
-        self.resolution_lineedit = QLineEdit(str(function_option.value.resolution))
-        resolution_layout.addWidget(resolution_label)
-        resolution_layout.addWidget(self.resolution_lineedit)
-        resolution_layout.addStretch(1)
-        self.advanced_settings_layout.addRow(resolution_label, resolution_layout)
-
-        start_x_layout = QHBoxLayout()
-        start_x_label = QLabel("Start x:")
-        self.start_x_lineedit = QLineEdit(str(function_option.value.start_x))
-        start_x_layout.addWidget(start_x_label)
-        start_x_layout.addWidget(self.start_x_lineedit)
-        start_x_layout.addStretch(1)
-        self.advanced_settings_layout.addRow(start_x_label, start_x_layout)
-
-        end_x_layout = QHBoxLayout()
-        end_x_label = QLabel("End x:")
-        self.end_x_lineedit = QLineEdit(str(function_option.value.end_x))
-        end_x_layout.addWidget(end_x_label)
-        end_x_layout.addWidget(self.end_x_lineedit)
-        end_x_layout.addStretch(1)
-        self.advanced_settings_layout.addRow(end_x_label, end_x_layout)
-
-        expr_layout = QHBoxLayout()
-        expr_label = QLabel("Expression:")
-        self.expr_lineedit = QLineEdit(str(function_option.value.expr))
-        expr_layout.addWidget(expr_label)
-        expr_layout.addWidget(self.expr_lineedit)
-        expr_layout.addStretch(1)
-        self.advanced_settings_layout.addRow(expr_label, expr_layout)
-
-        # Add buttton for replotting of the active function with the new parameters
-        self.replot_button = QPushButton("Replot")
-        self.replot_button.clicked.connect(self.on_replot_button_clicked)
-        layout.addWidget(self.replot_button)
-
-        # Display the active function
-        self.load_active_function()
-
-    @pyqtSlot()
-    def on_replot_button_clicked(self) -> None:
-        """This function is called when the replot button is clicked.
-        It will update the parameters of the function and replots the function.
-        """
-        logger.debug("Replot button clicked")
-        # Update the resolution, start_x, end_x and expr lineedits
-        self.function_option.value.resolution = self.resolution_lineedit.text()
-        self.function_option.value.start_x = self.start_x_lineedit.text()
-        self.function_option.value.end_x = self.end_x_lineedit.text()
-        try:
-            self.function_option.value.expr = self.expr_lineedit.text()
-        except SyntaxError:
-            logger.debug("Invalid expression: %s", self.expr_lineedit.text())
-            self.expr_lineedit.setText(str(self.function_option.value.expr))
-            # Create message box that tells the user that the expression is invalid
-            self.create_message_box(
-                "Invalid expression",
-                "The expression you entered is invalid. Please enter a valid expression.",
-            )
-
-        self.delete_active_function()
-        self.load_active_function()
-
-    @pyqtSlot()
-    def on_advanced_settings_button_clicked(self) -> None:
-        """This function is called when the advanced settings button is clicked.
-        It will show or hide the advanced settings.
-        """
-        if self.advanced_settings.isHidden():
-            self.advanced_settings.setHidden(False)
-            self.advanced_settings_button.setText("Hide Advanced Settings")
-        else:
-            self.advanced_settings.setHidden(True)
-            self.advanced_settings_button.setText("Show Advanced Settings")
-
-    @pyqtSlot()
-    def on_functionbutton_clicked(self, function) -> None:
-        """This function is called when a function button is clicked.
-        It will update the function_option.value to the function that was clicked.
-        """
-        logger.debug("Button for function %s clicked", function.name)
-        self.function_option.set_value(function)
-        self.delete_active_function()
-        self.load_active_function()
-
-    def delete_active_function(self) -> None:
-        """This function is called when the active function is deleted.
-        It will remove the active function from the layout.
-        """
-        # Remove the plotter with object name "plotter" from the layout
-        for i in reversed(range(self.layout().count())):
-            item = self.layout().itemAt(i)
-            if item.widget() and item.widget().objectName() == "active_function":
-                item.widget().deleteLater()
-                break
-
-    def load_active_function(self) -> None:
-        """This function is called when the active function is loaded.
-        It will add the active function to the layout.
-        """
-        # New QWidget for the active function
-        active_function_Widget = QWidget()
-        active_function_Widget.setObjectName("active_function")
-
-        function_layout = QVBoxLayout()
-
-        plot_layout = QHBoxLayout()
-
-        # Add plot for time domain
-        time_domain_layout = QVBoxLayout()
-        time_domain_label = QLabel("Time domain:")
-        time_domain_layout.addWidget(time_domain_label)
-        plot = self.function_option.value.time_domain_plot(self.event.duration)
-        time_domain_layout.addWidget(plot)
-        plot_layout.addLayout(time_domain_layout)
-
-        # Add plot for frequency domain
-        frequency_domain_layout = QVBoxLayout()
-        frequency_domain_label = QLabel("Frequency domain:")
-        frequency_domain_layout.addWidget(frequency_domain_label)
-        plot = self.function_option.value.frequency_domain_plot(self.event.duration)
-        frequency_domain_layout.addWidget(plot)
-        plot_layout.addLayout(frequency_domain_layout)
-
-        function_layout.addLayout(plot_layout)
-
-        parameter_layout = QFormLayout()
-        parameter_label = QLabel("Parameters:")
-        parameter_layout.addRow(parameter_label)
-        for parameter in self.function_option.value.parameters:
-            parameter_label = QLabel(parameter.name)
-            parameter_lineedit = QLineEdit(str(parameter.value))
-            # Add the parameter_lineedit editingFinished signal to the paramter.set_value slot
-            parameter_lineedit.editingFinished.connect(
-                lambda: parameter.set_value(parameter_lineedit.text())
-            )
-
-            # Create a QHBoxLayout
-            hbox = QHBoxLayout()
-
-            # Add your QLineEdit and a stretch to the QHBoxLayout
-            hbox.addWidget(parameter_lineedit)
-            hbox.addStretch(1)
-
-            # Use addRow() method to add label and the QHBoxLayout next to each other
-            parameter_layout.addRow(parameter_label, hbox)
-
-        function_layout.addLayout(parameter_layout)
-        function_layout.addStretch(1)
-        active_function_Widget.setLayout(function_layout)
-        self.layout().addWidget(active_function_Widget)
-
-        # Update the resolution, start_x, end_x and expr lineedits
-        self.resolution_lineedit.setText(str(self.function_option.value.resolution))
-        self.start_x_lineedit.setText(str(self.function_option.value.start_x))
-        self.end_x_lineedit.setText(str(self.function_option.value.end_x))
-        self.expr_lineedit.setText(str(self.function_option.value.expr))
-
-    def create_message_box(self, message: str, information: str) -> None:
-        """Creates a message box with the given message and information and shows it.
-
-        Args:
-            message (str): The message to be shown in the message box
-        information (str): The information to be shown in the message box
-        """
-        msg = QMessageBox(parent=self.parent)
-        msg.setIcon(QMessageBox.Icon.Warning)
-        msg.setText(message)
-        msg.setInformativeText(information)
-        msg.setWindowTitle("Warning")
-        msg.exec()
-
-
 class AddEventDialog(QDialog):
     """This dialog is created whenever a new event is added to the pulse sequence. It allows the user to enter a name for the event."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         self.setWindowTitle("Add Event")
@@ -778,21 +539,21 @@
         """Returns the name entered by the user.
 
         Returns:
         str: The name entered by the user
         """
         return self.name_input.text()
 
-    def get_duration(self) -> Decimal:
+    def get_duration(self) -> float:
         """Returns the duration entered by the user, or a fallback value."
 
         Returns:
-        Decimal: The duration value provided by the user, or 20
+        float: The duration value provided by the user, or 20
         """
-        return Decimal(self.duration_lineedit.text() or 20)
+        return self.duration_lineedit.text() or 20
 
     def check_input(self) -> None:
         """Checks if the name and duration entered by the user is valid. If it is, the dialog is accepted. If not, the user is informed of the error."""
         if (
             self.duration_lineedit.validator.validate(self.duration_lineedit.text(), 0)[
                 0
             ]
```

### Comparing `nqrduck_pulseprogrammer-0.0.2/LICENSE` & `nqrduck_pulseprogrammer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck_pulseprogrammer-0.0.2/README.md` & `nqrduck_pulseprogrammer-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck_pulseprogrammer-0.0.2/pyproject.toml` & `nqrduck_pulseprogrammer-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nqrduck-pulseprogrammer"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "A module for the NQRduck program (a simple python script™) to do pulse programming."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck_pulseprogrammer-0.0.2/PKG-INFO` & `nqrduck_pulseprogrammer-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck-pulseprogrammer
-Version: 0.0.2
+Version: 0.0.3
 Summary: A module for the NQRduck program (a simple python script™) to do pulse programming.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-pulseprogrammer/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-pulseprogrammer
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
```

