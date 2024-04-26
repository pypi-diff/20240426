# Comparing `tmp/nqrduck_spectrometer_limenqr-0.0.4.tar.gz` & `tmp/nqrduck_spectrometer_limenqr-0.0.5.tar.gz`

## Comparing `nqrduck_spectrometer_limenqr-0.0.4.tar` & `nqrduck_spectrometer_limenqr-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/src/nqrduck_spectrometer_limenqr/__init__.py
--rw-r--r--   0        0        0    27869 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/src/nqrduck_spectrometer_limenqr/controller.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/src/nqrduck_spectrometer_limenqr/limenqr.py
--rw-r--r--   0        0        0     9697 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/src/nqrduck_spectrometer_limenqr/model.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/src/nqrduck_spectrometer_limenqr/view.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/src/nqrduck_spectrometer_limenqr/resources/limenqr.ini
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/src/nqrduck_spectrometer_limenqr/resources/limenqr_widget.ui
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/LICENSE
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/README.md
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/__init__.py
+-rw-r--r--   0        0        0    27840 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/controller.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/limenqr.py
+-rw-r--r--   0        0        0     9697 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/model.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/view.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/resources/limenqr.ini
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/resources/limenqr_widget.ui
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/README.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.5/PKG-INFO
```

### Comparing `nqrduck_spectrometer_limenqr-0.0.4/.github/workflows/python-publish.yml` & `nqrduck_spectrometer_limenqr-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.4/src/nqrduck_spectrometer_limenqr/controller.py` & `nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import tempfile
 from pathlib import Path
 import numpy as np
-from decimal import Decimal
 
 from limedriver.binding import PyLimeConfig
 from limedriver.hdf_reader import HDF
 
 from nqrduck_spectrometer.base_spectrometer_controller import BaseSpectrometerController
 from nqrduck_spectrometer.measurement import Measurement
 from nqrduck_spectrometer.pulseparameters import TXPulse, RXReadout
@@ -403,15 +402,15 @@
             parameter (Parameter): The parameter that contains the pulse shape and amplitude
         
         Returns:
         tuple: A tuple containing the pulse shape and the pulse amplitude
         """
         pulse_shape = parameter.get_option_by_name(TXPulse.TX_PULSE_SHAPE).value
         pulse_amplitude = abs(pulse_shape.get_pulse_amplitude(event.duration)) * \
-                          parameter.get_option_by_name(TXPulse.RELATIVE_AMPLITUDE).value
+                          (parameter.get_option_by_name(TXPulse.RELATIVE_AMPLITUDE).value / 100)
         pulse_amplitude = np.clip(pulse_amplitude, -0.99, 0.99)
         return pulse_shape, pulse_amplitude
 
     def modulate_pulse_amplitude(self, pulse_amplitude, event, lime):
         """This method modulates the pulse amplitude for the limr object. We need to do this to have the pulse at IF frequency instead  of LO frequency.
         
         Args:
@@ -449,15 +448,15 @@
             modulated_phase (float): The modulated phase
         """
         pfr = [float(self.module.model.if_frequency)] * len(pulse_amplitude)
         # We set the first  len(pulse_amplitude) of the p_dur 
         pdr = [float(pulse_shape.resolution)] * len(pulse_amplitude)
         pam = list(pulse_amplitude)
         pof = ([self.module.model.OFFSET_FIRST_PULSE] +
-                    [int(pulse_shape.resolution * Decimal(lime.srate))] * (len(pulse_amplitude) - 1))
+                    [int(pulse_shape.resolution * lime.srate)] * (len(pulse_amplitude) - 1))
         pph = list(modulated_phase)
 
         return  pfr, pdr, pam, pof, pph
 
     def extend_pulse_lists(self, lime, pulse_amplitude, pulse_shape, modulated_phase):
         """This method extends the pulse lists of the limr object.
```

### Comparing `nqrduck_spectrometer_limenqr-0.0.4/src/nqrduck_spectrometer_limenqr/model.py` & `nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/model.py`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.4/src/nqrduck_spectrometer_limenqr/resources/limenqr_widget.ui` & `nqrduck_spectrometer_limenqr-0.0.5/src/nqrduck_spectrometer_limenqr/resources/limenqr_widget.ui`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.4/LICENSE` & `nqrduck_spectrometer_limenqr-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.4/README.md` & `nqrduck_spectrometer_limenqr-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.4/pyproject.toml` & `nqrduck_spectrometer_limenqr-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck-spectrometer-limenqr"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "A submodule for the nqrduck-spectrometer module which implements the functionality for the LimeNQR spectrometer."
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
 ]
```

### Comparing `nqrduck_spectrometer_limenqr-0.0.4/PKG-INFO` & `nqrduck_spectrometer_limenqr-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck-spectrometer-limenqr
-Version: 0.0.4
+Version: 0.0.5
 Summary: A submodule for the nqrduck-spectrometer module which implements the functionality for the LimeNQR spectrometer.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-spectrometer-limenqr/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-spectrometer-limenqr
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
         
@@ -27,15 +27,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Requires-Dist: h5py
 Requires-Dist: limedriver
 Requires-Dist: nqrduck-spectrometer
 Requires-Dist: pyqt6
 Requires-Dist: pyserial
 Description-Content-Type: text/markdown
```

