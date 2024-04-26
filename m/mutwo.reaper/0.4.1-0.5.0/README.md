# Comparing `tmp/mutwo.reaper-0.4.1.tar.gz` & `tmp/mutwo_reaper-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutwo.reaper-0.4.1.tar", last modified: Mon Nov 13 22:02:59 2023, max compression
+gzip compressed data, was "mutwo_reaper-0.5.0.tar", last modified: Fri Apr 26 15:51:56 2024, max compression
```

## Comparing `mutwo.reaper-0.4.1.tar` & `mutwo_reaper-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-13 22:02:59.037541 mutwo.reaper-0.4.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2023-11-13 22:02:47.000000 mutwo.reaper-0.4.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1305 2023-11-13 22:02:59.037541 mutwo.reaper-0.4.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2023-11-13 22:02:47.000000 mutwo.reaper-0.4.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-13 22:02:59.033541 mutwo.reaper-0.4.1/mutwo/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-13 22:02:59.037541 mutwo.reaper-0.4.1/mutwo/reaper_converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-11-13 22:02:47.000000 mutwo.reaper-0.4.1/mutwo/reaper_converters/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      310 2023-11-13 22:02:47.000000 mutwo.reaper-0.4.1/mutwo/reaper_converters/configurations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5563 2023-11-13 22:02:47.000000 mutwo.reaper-0.4.1/mutwo/reaper_converters/reaper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-13 22:02:59.037541 mutwo.reaper-0.4.1/mutwo/reaper_version/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2023-11-13 22:02:47.000000 mutwo.reaper-0.4.1/mutwo/reaper_version/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-11-13 22:02:59.037541 mutwo.reaper-0.4.1/mutwo.reaper.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1305 2023-11-13 22:02:59.000000 mutwo.reaper-0.4.1/mutwo.reaper.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      365 2023-11-13 22:02:59.000000 mutwo.reaper-0.4.1/mutwo.reaper.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-11-13 22:02:59.000000 mutwo.reaper-0.4.1/mutwo.reaper.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       51 2023-11-13 22:02:59.000000 mutwo.reaper-0.4.1/mutwo.reaper.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-11-13 22:02:59.000000 mutwo.reaper-0.4.1/mutwo.reaper.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2023-11-13 22:02:47.000000 mutwo.reaper-0.4.1/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-11-13 22:02:59.037541 mutwo.reaper-0.4.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-11-13 22:02:47.000000 mutwo.reaper-0.4.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:51:56.837724 mutwo_reaper-0.5.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35149 2024-04-26 15:51:46.000000 mutwo_reaper-0.5.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1304 2024-04-26 15:51:56.837724 mutwo_reaper-0.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2024-04-26 15:51:46.000000 mutwo_reaper-0.5.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:51:56.833724 mutwo_reaper-0.5.0/mutwo/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:51:56.837724 mutwo_reaper-0.5.0/mutwo/reaper_converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2024-04-26 15:51:46.000000 mutwo_reaper-0.5.0/mutwo/reaper_converters/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-04-26 15:51:46.000000 mutwo_reaper-0.5.0/mutwo/reaper_converters/configurations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5377 2024-04-26 15:51:46.000000 mutwo_reaper-0.5.0/mutwo/reaper_converters/reaper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:51:56.837724 mutwo_reaper-0.5.0/mutwo/reaper_version/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      144 2024-04-26 15:51:46.000000 mutwo_reaper-0.5.0/mutwo/reaper_version/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-26 15:51:56.837724 mutwo_reaper-0.5.0/mutwo.reaper.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1304 2024-04-26 15:51:56.000000 mutwo_reaper-0.5.0/mutwo.reaper.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      365 2024-04-26 15:51:56.000000 mutwo_reaper-0.5.0/mutwo.reaper.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-26 15:51:56.000000 mutwo_reaper-0.5.0/mutwo.reaper.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-04-26 15:51:56.000000 mutwo_reaper-0.5.0/mutwo.reaper.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-04-26 15:51:56.000000 mutwo_reaper-0.5.0/mutwo.reaper.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-04-26 15:51:46.000000 mutwo_reaper-0.5.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-26 15:51:56.837724 mutwo_reaper-0.5.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1071 2024-04-26 15:51:46.000000 mutwo_reaper-0.5.0/setup.py
```

### Comparing `mutwo.reaper-0.4.1/LICENSE` & `mutwo_reaper-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mutwo.reaper-0.4.1/PKG-INFO` & `mutwo_reaper-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mutwo.reaper
-Version: 0.4.1
+Version: 0.5.0
 Summary: Reaper extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.reaper
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mutwo.core<2.0.0,>=0.61.4
+Requires-Dist: mutwo.core<3.0.0,>=2.0.0
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.reaper
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.reaper.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.reaper)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

### Comparing `mutwo.reaper-0.4.1/README.md` & `mutwo_reaper-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mutwo.reaper-0.4.1/mutwo/reaper_converters/reaper.py` & `mutwo_reaper-0.5.0/mutwo/reaper_converters/reaper.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from mutwo import core_converters
 from mutwo import core_events
 from mutwo import core_parameters
 from mutwo import reaper_converters
 
 __all__ = (
     "EventToReaperMarkerString",
-    "SimpleEventToMarkerName",
-    "SimpleEventToMarkerColor",
+    "ChrononToMarkerName",
+    "ChrononToMarkerColor",
 )
 
 
-class SimpleEventToMarkerName(core_converters.SimpleEventToAttribute):
-    """Convert :class:`~mutwo.core_events.SimpleEvent` to a name of a marker.
+class ChrononToMarkerName(core_converters.ChrononToAttribute):
+    """Convert :class:`~mutwo.core_events.Chronon` to a name of a marker.
 
     By default `mutwo` will fetch from an event the
     :const:`~mutwo.reaper_converters.configurations.DEFAULT_MARKER_NAME_ATTRIBUTE_NAME`.
     If no attribute with `attribute_name` can be found the converter will simply return
     ``None``.
     """
 
@@ -30,16 +30,16 @@
         if attribute_name is None:
             attribute_name = (
                 reaper_converters.configurations.DEFAULT_MARKER_NAME_ATTRIBUTE_NAME
             )
         super().__init__(attribute_name, exception_value)
 
 
-class SimpleEventToMarkerColor(core_converters.SimpleEventToAttribute):
-    """Convert :class:`~mutwo.core_events.SimpleEvent` to the color of a marker.
+class ChrononToMarkerColor(core_converters.ChrononToAttribute):
+    """Convert :class:`~mutwo.core_events.Chronon` to the color of a marker.
 
     By default `mutwo` will fetch from an event the
     :const:`~mutwo.reaper_converters.configurations.DEFAULT_MARKER_COLOR_ATTRIBUTE_NAME`.
     If no attribute with `attribute_name` can be found the converter will simply return
     ``None``.
     """
 
@@ -54,73 +54,73 @@
             )
         super().__init__(attribute_name, exception_value)
 
 
 class EventToReaperMarkerString(core_converters.abc.EventConverter):
     """Make Reaper Marker entries.
 
-    :param simple_event_to_marker_name: A function which converts a
-        :class:`~mutwo.core_events.SimpleEvent` to the marker
+    :param chronon_to_marker_name: A function which converts a
+        :class:`~mutwo.core_events.Chronon` to the marker
         name. If the function returns ``None`` `mutwo` will ignore`
-        the current event. By default `simple_event_to_marker_name` is set
-        to :class:`SimpleEventToMarkerName`.
-    :type simple_event_to_marker_name: typing.Callable[[core_events.SimpleEvent], str]
-    :param simple_event_to_marker_color: A function which converts a
-        :class:`~mutwo.core_events.SimpleEvent` to the marker
+        the current event. By default `chronon_to_marker_name` is set
+        to :class:`ChrononToMarkerName`.
+    :type chronon_to_marker_name: typing.Callable[[core_events.Chronon], str]
+    :param chronon_to_marker_color: A function which converts a
+        :class:`~mutwo.core_events.Chronon` to the marker
         color. If the function returns ``None`` `mutwo` will ignore`
-        the current event. By default `simple_event_to_marker_name` is set
-        to :class:`SimpleEventToMarkerColor`.
-    :type simple_event_to_marker_color: typing.Callable[[core_events.SimpleEvent], str]
+        the current event. By default `chronon_to_marker_name` is set
+        to :class:`ChrononToMarkerColor`.
+    :type chronon_to_marker_color: typing.Callable[[core_events.Chronon], str]
 
     The resulting string can be copied into the respective reaper
     project file one line before the '<PROJBAY' tag.
 
     **Example:**
 
     >>> from mutwo import reaper_converters
     >>> from mutwo import core_events
     >>> marker_converter = reaper_converters.EventToReaperMarkerString()
-    >>> events = core_events.SequentialEvent([core_events.SimpleEvent(2), core_events.SimpleEvent(3)])
+    >>> events = core_events.Consecution([core_events.Chronon(2), core_events.Chronon(3)])
     >>> events[0].name = 'beginning'
     >>> events[0].color = r'0 16797088 1 B {A4376701-5AA5-246B-900B-28ABC969123A}'
     >>> events[1].name = 'center'
     >>> events[1].color = r'0 18849803 1 B {E4DD7D23-98F4-CA97-8587-F4259A9498F7}'
     >>> print(marker_converter.convert(events))
     MARKER 0 0.0 beginning 0 16797088 1 B {A4376701-5AA5-246B-900B-28ABC969123A}
     MARKER 1 2.0 center 0 18849803 1 B {E4DD7D23-98F4-CA97-8587-F4259A9498F7}
     """
 
     def __init__(
         self,
-        simple_event_to_marker_name: typing.Callable[
-            [core_events.SimpleEvent], str
-        ] = SimpleEventToMarkerName(),  # type: ignore
-        simple_event_to_marker_color: typing.Callable[
-            [core_events.SimpleEvent], str
-        ] = SimpleEventToMarkerColor(),  # type: ignore
+        chronon_to_marker_name: typing.Callable[
+            [core_events.Chronon], str
+        ] = ChrononToMarkerName(),  # type: ignore
+        chronon_to_marker_color: typing.Callable[
+            [core_events.Chronon], str
+        ] = ChrononToMarkerColor(),  # type: ignore
     ):
-        self._simple_event_to_marker_name = simple_event_to_marker_name
-        self._simple_event_to_marker_color = simple_event_to_marker_color
+        self._chronon_to_marker_name = chronon_to_marker_name
+        self._chronon_to_marker_color = chronon_to_marker_color
 
-    def _convert_simple_event(
+    def _convert_chronon(
         self,
-        simple_event: core_events.SimpleEvent,
+        chronon: core_events.Chronon,
         absolute_entry_delay: core_parameters.abc.Duration,
     ) -> tuple[str, ...]:
-        marker_name = self._simple_event_to_marker_name(simple_event)
-        marker_color = self._simple_event_to_marker_color(simple_event)
+        marker_name = self._chronon_to_marker_name(chronon)
+        marker_color = self._chronon_to_marker_color(chronon)
 
         # If any of the functions return ``None`` `mutwo` will ignore`
         # the current event.
         if marker_name is None or marker_color is None:
             return tuple([])
 
         return (
             "{} {} {}".format(
-                absolute_entry_delay.duration_in_floats, marker_name, marker_color
+                absolute_entry_delay.beat_count, marker_name, marker_color
             ),
         )
 
     def convert(self, event_to_convert: core_events.abc.Event) -> str:
         """Convert event to reaper markers (as plain string).
 
         :param event_to_convert: The event which shall be
```

### Comparing `mutwo.reaper-0.4.1/mutwo.reaper.egg-info/PKG-INFO` & `mutwo_reaper-0.5.0/mutwo.reaper.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: mutwo.reaper
-Version: 0.4.1
+Version: 0.5.0
 Summary: Reaper extension for event based framework for generative art
 Home-page: https://github.com/mutwo-org/mutwo.reaper
 Author: Levin Eric Zimmermann
 Author-email: levin.eric.zimmermann@posteo.eu
 License: GPL
 Project-URL: Documentation, https://mutwo-org.github.io
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mutwo.core<2.0.0,>=0.61.4
+Requires-Dist: mutwo.core<3.0.0,>=2.0.0
 Provides-Extra: testing
 Requires-Dist: pytest>=7.1.1; extra == "testing"
 
 # mutwo.reaper
 
 [![Build Status](https://circleci.com/gh/mutwo-org/mutwo.reaper.svg?style=shield)](https://circleci.com/gh/mutwo-org/mutwo.reaper)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
```

### Comparing `mutwo.reaper-0.4.1/setup.py` & `mutwo_reaper-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,12 +26,12 @@
     packages=[
         package
         for package in setuptools.find_namespace_packages(include=["mutwo.*"])
         if package[:5] != "tests"
     ],
     setup_requires=[],
     install_requires=[
-        "mutwo.core>=0.61.4, <2.0.0",
+        "mutwo.core>=2.0.0, <3.0.0",
     ],
     extras_require=extras_require,
     python_requires=">=3.9, <4",
 )
```

