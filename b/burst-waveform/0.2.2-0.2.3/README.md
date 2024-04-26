# Comparing `tmp/burst_waveform-0.2.2.tar.gz` & `tmp/burst_waveform-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burst_waveform-0.2.2.tar", last modified: Wed Apr 24 12:11:06 2024, max compression
+gzip compressed data, was "burst_waveform-0.2.3.tar", last modified: Fri Apr 26 12:40:53 2024, max compression
```

## Comparing `burst_waveform-0.2.2.tar` & `burst_waveform-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:11:06.930463 burst_waveform-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)    35065 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/Makefile
--rw-r--r--   0 root         (0) root         (0)     1589 2024-04-24 12:11:06.929463 burst_waveform-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:11:06.928463 burst_waveform-0.2.2/burst_waveform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/burst_waveform/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-04-24 12:11:06.000000 burst_waveform-0.2.2/burst_waveform/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     3057 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/burst_waveform/generate_waveform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:11:06.928463 burst_waveform-0.2.2/burst_waveform/models/
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/burst_waveform/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/burst_waveform/models/sine_gaussian.py
--rw-rw-rw-   0 root         (0) root         (0)     3698 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/burst_waveform/models/white_noise_burst.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:11:06.929463 burst_waveform-0.2.2/burst_waveform.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1589 2024-04-24 12:11:06.000000 burst_waveform-0.2.2/burst_waveform.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      597 2024-04-24 12:11:06.000000 burst_waveform-0.2.2/burst_waveform.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 12:11:06.000000 burst_waveform-0.2.2/burst_waveform.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-24 12:11:06.000000 burst_waveform-0.2.2/burst_waveform.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-24 12:11:06.000000 burst_waveform-0.2.2/burst_waveform.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:11:06.929463 burst_waveform-0.2.2/notebook/
--rw-rw-rw-   0 root         (0) root         (0)    41872 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/notebook/SGQ_test.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    23999 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/notebook/WNB_test.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1490 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/notebook/cWB_check.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    63532 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/notebook/test.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      542 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 12:11:06.930463 burst_waveform-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1590 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 12:11:06.929463 burst_waveform-0.2.2/test/
--rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-24 12:11:01.000000 burst_waveform-0.2.2/test/test_waveform_generation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:40:53.505057 burst_waveform-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    35065 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/Makefile
+-rw-r--r--   0 root         (0) root         (0)     1589 2024-04-26 12:40:53.504057 burst_waveform-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:40:53.501057 burst_waveform-0.2.3/burst_waveform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/burst_waveform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-04-26 12:40:53.000000 burst_waveform-0.2.3/burst_waveform/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     3057 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/burst_waveform/generate_waveform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:40:53.502057 burst_waveform-0.2.3/burst_waveform/models/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/burst_waveform/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/burst_waveform/models/sine_gaussian.py
+-rw-rw-rw-   0 root         (0) root         (0)     3787 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/burst_waveform/models/white_noise_burst.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:40:53.504057 burst_waveform-0.2.3/burst_waveform.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1589 2024-04-26 12:40:53.000000 burst_waveform-0.2.3/burst_waveform.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-26 12:40:53.000000 burst_waveform-0.2.3/burst_waveform.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 12:40:53.000000 burst_waveform-0.2.3/burst_waveform.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-26 12:40:53.000000 burst_waveform-0.2.3/burst_waveform.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-26 12:40:53.000000 burst_waveform-0.2.3/burst_waveform.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:40:53.503057 burst_waveform-0.2.3/notebook/
+-rw-rw-rw-   0 root         (0) root         (0)    41872 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/notebook/SGQ_test.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    38144 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/notebook/WNB_test.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1490 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/notebook/cWB_check.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    63532 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/notebook/test.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      542 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-26 12:40:53.505057 burst_waveform-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 12:40:53.504057 burst_waveform-0.2.3/test/
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-26 12:40:45.000000 burst_waveform-0.2.3/test/test_waveform_generation.py
```

### Comparing `burst_waveform-0.2.2/.gitlab-ci.yml` & `burst_waveform-0.2.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `burst_waveform-0.2.2/LICENSE` & `burst_waveform-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `burst_waveform-0.2.2/PKG-INFO` & `burst_waveform-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burst-waveform
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for gravitational wave burst waveform
 Home-page: https://git.ligo.org/yumeng.xu/setup.py
 Author: Yumeng Xu
 Author-email: The PycWB team <yumeng.xu@ligo.org>
 Keywords: ligo,sine-gaussian,white noise burst,gravitational waves,burst,waveform model
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `burst_waveform-0.2.2/README.md` & `burst_waveform-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `burst_waveform-0.2.2/burst_waveform/generate_waveform.py` & `burst_waveform-0.2.3/burst_waveform/generate_waveform.py`

 * *Files identical despite different names*

### Comparing `burst_waveform-0.2.2/burst_waveform/models/sine_gaussian.py` & `burst_waveform-0.2.3/burst_waveform/models/sine_gaussian.py`

 * *Files identical despite different names*

### Comparing `burst_waveform-0.2.2/burst_waveform/models/white_noise_burst.py` & `burst_waveform-0.2.3/burst_waveform/models/white_noise_burst.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,17 +17,17 @@
             Name of waveform model
         """
         self.params = self._validate_params(parameters)
 
     @staticmethod
     def _validate_params(parameters):
         default_params = {
-            "frequency": None,
-            "bandwidth": None,
-            "duration": None,
+            "frequency": None,  # start frequency of the white noise burst
+            "bandwidth": None,  # bandwidth of the white noise burst
+            "duration": None,  # duration of the white noise burst
             "sample_rate": 16384.0,
             "inj_length": 1.,
             "seed": 0,
             "mode": 0
         }
 
         waveform_params = parameters.copy()
@@ -72,29 +72,29 @@
         X = fft(x)
         if mode == 1:
             # set zero bins outside the range [0,bandwidth/2]
             # Heterodyne up by frequency+bandwidth/2 (move zero frequency to center of desidered band)
             bFrequency = int(frequency / df)
             bBandwidth = int((bandwidth / 2.) / df)
             y = np.zeros_like(X)
-            bin = 2 * (bFrequency + bBandwidth)
+            bin = (bFrequency + bBandwidth)
             y[bin] = X[0]
-            y[bin + 1] = X[1]
+            # y[bin + 1] = X[1]
             for i in range(1, bBandwidth):
-                y[bin + 2 * i] = X[2 * i]
-                y[bin + 2 * i + 1] = X[2 * i + 1]
-                y[bin - 2 * i] = X[2 * i]
-                y[bin - 2 * i + 1] = -X[2 * i + 1]
+                y[bin + i] = X[i]
+                # y[bin + 2 * i + 1] = X[2 * i + 1]
+                y[bin - i] = X[i]
+                # y[bin - 2 * i + 1] = -X[2 * i + 1]
             X = y
         else:
             # Asymmetric respect to the central frequency
             bLow = int(frequency / df)
             bHigh = int((frequency + bandwidth) / df)
-            X[:2 * bLow] = 0
-            X[2 * bHigh:2 * int(len(X) / 2)] = 0
+            X[:bLow] = 0
+            X[bHigh:int(len(X))] = 0
         x = ifft(X)
 
         # Apply a gaussian shape in time
         function_range = inj_length
         t = np.linspace(0, inj_length, len(x))
         gaussian_envelope = np.exp(-((t - function_range / 2) / duration) **2)
         x *= gaussian_envelope
```

### Comparing `burst_waveform-0.2.2/burst_waveform.egg-info/PKG-INFO` & `burst_waveform-0.2.3/burst_waveform.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burst-waveform
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for gravitational wave burst waveform
 Home-page: https://git.ligo.org/yumeng.xu/setup.py
 Author: Yumeng Xu
 Author-email: The PycWB team <yumeng.xu@ligo.org>
 Keywords: ligo,sine-gaussian,white noise burst,gravitational waves,burst,waveform model
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `burst_waveform-0.2.2/burst_waveform.egg-info/SOURCES.txt` & `burst_waveform-0.2.3/burst_waveform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `burst_waveform-0.2.2/notebook/SGQ_test.ipynb` & `burst_waveform-0.2.3/notebook/SGQ_test.ipynb`

 * *Files identical despite different names*

### Comparing `burst_waveform-0.2.2/notebook/cWB_check.ipynb` & `burst_waveform-0.2.3/notebook/cWB_check.ipynb`

 * *Files identical despite different names*

### Comparing `burst_waveform-0.2.2/notebook/test.ipynb` & `burst_waveform-0.2.3/notebook/test.ipynb`

 * *Files identical despite different names*

### Comparing `burst_waveform-0.2.2/pyproject.toml` & `burst_waveform-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `burst_waveform-0.2.2/setup.py` & `burst_waveform-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `burst_waveform-0.2.2/test/test_waveform_generation.py` & `burst_waveform-0.2.3/test/test_waveform_generation.py`

 * *Files identical despite different names*

