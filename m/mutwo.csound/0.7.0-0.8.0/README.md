# Comparing `tmp/mutwo.csound-0.7.0.tar.gz` & `tmp/mutwo_csound-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.csound-0.7.0.tar", last modified: Thu Apr 27 07:14:47 2023, max compression
+gzip compressed data, was "mutwo_csound-0.8.0.tar", last modified: Fri Apr 26 15:47:04 2024, max compression
```

## Comparing `mutwo.csound-0.7.0.tar` & `mutwo_csound-0.8.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 07:14:47.719942 mutwo.csound-0.7.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1239 2023-04-27 07:14:47.719942 mutwo.csound-0.7.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      783 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 07:14:47.715942 mutwo.csound-0.7.0/mutwo/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 07:14:47.719942 mutwo.csound-0.7.0/mutwo/csound_converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      159 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/mutwo/csound_converters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      496 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/mutwo/csound_converters/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      871 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/mutwo/csound_converters/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12721 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/mutwo/csound_converters/csound.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 07:14:47.719942 mutwo.csound-0.7.0/mutwo/csound_version/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/mutwo/csound_version/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-27 07:14:47.719942 mutwo.csound-0.7.0/mutwo.csound.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1239 2023-04-27 07:14:47.000000 mutwo.csound-0.7.0/mutwo.csound.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-04-27 07:14:47.000000 mutwo.csound-0.7.0/mutwo.csound.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-27 07:14:47.000000 mutwo.csound-0.7.0/mutwo.csound.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2023-04-27 07:14:47.000000 mutwo.csound-0.7.0/mutwo.csound.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-04-27 07:14:47.000000 mutwo.csound-0.7.0/mutwo.csound.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-27 07:14:47.719942 mutwo.csound-0.7.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1120 2023-04-27 07:14:37.000000 mutwo.csound-0.7.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:47:04.342945 mutwo_csound-0.8.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2024-04-26 15:46:52.000000 mutwo_csound-0.8.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1353 2024-04-26 15:47:04.342945 mutwo_csound-0.8.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      783 2024-04-26 15:46:52.000000 mutwo_csound-0.8.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:47:04.342945 mutwo_csound-0.8.0/mutwo/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:47:04.342945 mutwo_csound-0.8.0/mutwo/csound_converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      159 2024-04-26 15:46:52.000000 mutwo_csound-0.8.0/mutwo/csound_converters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      508 2024-04-26 15:46:52.000000 mutwo_csound-0.8.0/mutwo/csound_converters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      871 2024-04-26 15:46:52.000000 mutwo_csound-0.8.0/mutwo/csound_converters/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12645 2024-04-26 15:46:52.000000 mutwo_csound-0.8.0/mutwo/csound_converters/csound.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:47:04.342945 mutwo_csound-0.8.0/mutwo/csound_version/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2024-04-26 15:46:52.000000 mutwo_csound-0.8.0/mutwo/csound_version/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:47:04.342945 mutwo_csound-0.8.0/mutwo.csound.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1353 2024-04-26 15:47:04.000000 mutwo_csound-0.8.0/mutwo.csound.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2024-04-26 15:47:04.000000 mutwo_csound-0.8.0/mutwo.csound.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-26 15:47:04.000000 mutwo_csound-0.8.0/mutwo.csound.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2024-04-26 15:47:04.000000 mutwo_csound-0.8.0/mutwo.csound.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-04-26 15:47:04.000000 mutwo_csound-0.8.0/mutwo.csound.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-04-26 15:46:52.000000 mutwo_csound-0.8.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-26 15:47:04.342945 mutwo_csound-0.8.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2024-04-26 15:46:52.000000 mutwo_csound-0.8.0/setup.py
```

### Comparing `mutwo.csound-0.7.0/LICENSE` & `mutwo_csound-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.csound-0.7.0/PKG-INFO` & `mutwo_csound-0.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: mutwo.csound
-Version: 0.7.0
+Version: 0.8.0
 Summary: csound extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.ext-csound
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
-Project-URL: Documentation, https://mutwo.readthedocs.io/en/latest/
+Project-URL: Documentation, https://mutwo-org.github.io
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: mutwo.core<3.0.0,>=2.0.0
+Requires-Dist: natsort<9.0.0,>=8.0.0
+Provides-Extra: testing
+Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.csound
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.csound.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.csound)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version](https://badge.fury.io/py/mutwo.csound.svg)](https://badge.fury.io/py/mutwo.csound)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `mutwo.csound-0.7.0/README.md` & `mutwo_csound-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mutwo.csound-0.7.0/mutwo/csound_converters/constants.py` & `mutwo_csound-0.8.0/mutwo/csound_converters/constants.py`

 * *Files identical despite different names*

### Comparing `mutwo.csound-0.7.0/mutwo/csound_converters/csound.py` & `mutwo_csound-0.8.0/mutwo/csound_converters/csound.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from mutwo import core_parameters
 from mutwo import csound_converters
 
 __all__ = ("EventToCsoundScore", "EventToSoundFile")
 
 SupportedPFieldTypes = typing.Union[core_constants.Real, str]
 SupportedPFieldTypesForTypeChecker = typing.Union[numbers.Real, str]
-PFieldFunction = typing.Callable[[core_events.SimpleEvent], SupportedPFieldTypes]
+PFieldFunction = typing.Callable[[core_events.Chronon], SupportedPFieldTypes]
 PFieldDict = dict[str, typing.Optional[PFieldFunction]]
 
 
 class MissingPFieldWarning(Warning):
     pass
 
 
@@ -60,27 +60,27 @@
     automatically adds quotations marks around the string in the score file.
 
     All p-fields can be overwritten in the following manner:
 
     >>> from mutwo import csound_converters
     >>> my_converter = csound_converters.EventToCsoundScore(
     ...     p1=lambda event: 2,
-    ...     p4=lambda event: event.pitch.frequency,
+    ...     p4=lambda event: event.pitch.hertz,
     ...     p5=lambda event: event.volume
     ... )
 
     For easier debugging of faulty score files, :mod:`mutwo` adds annotations
-    when a new :class:`SequentialEvent` or a new :class:`SimultaneousEvent`
+    when a new :class:`~mutwo.core_events.Consecution` or a new :class:`~mutwo.core_events.Concurrence`
     starts.
     """
 
     _default_p_field_dict: PFieldDict = {
         "p1": lambda event: 1,  # default instrument name "1"
         "p2": None,  # default to absolute start time
-        "p3": lambda event: event.duration.duration_in_floats  # type: ignore
+        "p3": lambda event: event.duration.beat_count # type: ignore
         if event.duration > 0
         else None,  # default key for duration
     }
 
     def __init__(self, **pfield: PFieldFunction):
         concatenated_p_field_dict: PFieldDict = dict([])
         for (
@@ -161,77 +161,79 @@
             )
             return None
 
     # ###################################################################### #
     #           private methods (conversion of different event types)        #
     # ###################################################################### #
 
-    def _convert_simple_event(
+    def _convert_chronon(
         self,
-        simple_event: core_events.SimpleEvent,
+        chronon: core_events.Chronon,
         absolute_entry_delay: core_parameters.abc.Duration,
     ) -> tuple[str, ...]:
-        """Extract p-field data from simple event and write one Csound-Score line."""
+        """Extract p-field data from chronon and write one Csound-Score line."""
 
         csound_score_line = "i"
         for nth_p_field, p_field_function in enumerate(self.pfield_tuple):
             # special case of absolute start time initialization
             if nth_p_field == 1 and p_field_function is None:
-                csound_score_line += " {}".format(absolute_entry_delay.duration_in_floats)
+                csound_score_line += " {}".format(
+                    absolute_entry_delay.beat_count
+                )
 
             else:
                 try:
-                    p_field_value = p_field_function(simple_event)  # type: ignore
+                    p_field_value = p_field_function(chronon)  # type: ignore
 
                 except AttributeError:
                     # if attribute couldn't be found, just make a rest
                     return tuple([])
 
                 p_field_value = EventToCsoundScore._process_p_field_value(
                     nth_p_field, p_field_value
                 )
                 if p_field_value is not None:
                     csound_score_line += " {}".format(p_field_value)
 
         return (csound_score_line,)
 
-    def _convert_sequential_event(
+    def _convert_consecution(
         self,
-        sequential_event: core_events.SequentialEvent,
+        consecution: core_events.Consecution,
         absolute_entry_delay: core_parameters.abc.Duration,
     ) -> tuple[str, ...]:
         csound_score_line_list = [
-            csound_converters.configurations.SEQUENTIAL_EVENT_ANNOTATION
+            csound_converters.configurations.CONSECUTION_ANNOTATION
         ]
         csound_score_line_list.extend(
-            super()._convert_sequential_event(sequential_event, absolute_entry_delay)
+            super()._convert_consecution(consecution, absolute_entry_delay)
         )
 
         for _ in range(
-            csound_converters.configurations.N_EMPTY_LINES_AFTER_COMPLEX_EVENT
+            csound_converters.configurations.N_EMPTY_LINES_AFTER_COMPOUND
         ):
             csound_score_line_list.append("")
 
         return tuple(csound_score_line_list)
 
-    def _convert_simultaneous_event(
+    def _convert_concurrence(
         self,
-        simultaneous_event: core_events.SimultaneousEvent,
+        concurrence: core_events.Concurrence,
         absolute_entry_delay: core_parameters.abc.Duration,
     ) -> tuple[str, ...]:
         csound_score_line_list = [
-            csound_converters.configurations.SIMULTANEOUS_EVENT_ANNOTATION
+            csound_converters.configurations.CONCURRENCE_ANNOTATION
         ]
         csound_score_line_list.extend(
-            super()._convert_simultaneous_event(
-                simultaneous_event, absolute_entry_delay
+            super()._convert_concurrence(
+                concurrence, absolute_entry_delay
             )
         )
         for _ in range(
-            csound_converters.configurations.N_EMPTY_LINES_AFTER_COMPLEX_EVENT
+            csound_converters.configurations.N_EMPTY_LINES_AFTER_COMPOUND
         ):
             csound_score_line_list.append("")
         return tuple(csound_score_line_list)
 
     # ###################################################################### #
     #                             public api                                 #
     # ###################################################################### #
@@ -247,23 +249,23 @@
 
         >>> import random
         >>> from mutwo import core_events
         >>> from mutwo import csound_converters
         >>> converter = csound_converters.EventToCsoundScore(
         ...    p4=lambda event: event.tempo_envelope.duration
         ... )
-        >>> event = core_events.SequentialEvent(
+        >>> event = core_events.Consecution(
         ...    [
-        ...        core_events.SimpleEvent(
+        ...        core_events.Chronon(
         ...             random.uniform(0.3, 1.2)
         ...        ) for _ in range(15)
         ...    ]
         ... )
         >>> for e in event:
-        ...     e.tempo_envelope = core_events.TempoEnvelope(
+        ...     e.tempo = core_parameters.FlexTempo(
         ...         [[0, 1], [random.uniform(10, 20), 0]]
         ...     )
         >>> converter.convert(event, 'score.sco')
         """
 
         csound_score_line_tuple = self._convert_event(
             event_to_convert, core_parameters.DirectDuration(0)
@@ -318,16 +320,15 @@
         :type score_path: typing.Optional[str]
         """
 
         if not score_path:
             score_path = path + ".sco"
 
         self.event_to_csound_score.convert(event_to_convert, score_path)
-        command = "csound -o {}".format(path)
-        for flag in self.flags:
-            command += " {} ".format(flag)
+        flags = " ".join(self.flags)
+        command = f"{csound_converters.configurations.CSOUND_BINARY} -o {path} {flags}"
         command += " {} {}".format(self.csound_orchestra_path, score_path)
 
         os.system(command)
 
         if self.remove_score_file:
             os.remove(score_path)
```

### Comparing `mutwo.csound-0.7.0/mutwo.csound.egg-info/PKG-INFO` & `mutwo_csound-0.8.0/mutwo.csound.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: mutwo.csound
-Version: 0.7.0
+Version: 0.8.0
 Summary: csound extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.ext-csound
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
-Project-URL: Documentation, https://mutwo.readthedocs.io/en/latest/
+Project-URL: Documentation, https://mutwo-org.github.io
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: mutwo.core<3.0.0,>=2.0.0
+Requires-Dist: natsort<9.0.0,>=8.0.0
+Provides-Extra: testing
+Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.csound
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.csound.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.csound)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![PyPI version](https://badge.fury.io/py/mutwo.csound.svg)](https://badge.fury.io/py/mutwo.csound)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `mutwo.csound-0.7.0/setup.py` & `mutwo_csound-0.8.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     license="GPL",
     description="csound extension for event based framework for generative art",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Levin Eric Zimmermann",
     author_email="levin.eric.zimmermann@posteo.eu",
     url="https://github.com/mutwo-org/mutwo.ext-csound",
-    project_urls={"Documentation": "https://mutwo.readthedocs.io/en/latest/"},
+    project_urls={"Documentation": "https://mutwo-org.github.io"},
     packages=[
         package
         for package in setuptools.find_namespace_packages(include=["mutwo.*"])
         if package[:5] != "tests"
     ],
     setup_requires=[],
     install_requires=[
-        "mutwo.core>=1.0.0, <2.0.0",
+        "mutwo.core>=2.0.0, <3.0.0",
         "natsort>=8.0.0, <9.0.0",
     ],
     extras_require=extras_require,
     python_requires=">=3.10, <4",
 )
```

