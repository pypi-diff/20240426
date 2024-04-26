# Comparing `tmp/midi_to_dataframe-0.2.tar.gz` & `tmp/midi_to_dataframe-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midi_to_dataframe-0.2.tar", last modified: Fri Apr 26 16:23:35 2024, max compression
+gzip compressed data, was "midi_to_dataframe-0.3.tar", last modified: Fri Apr 26 16:41:53 2024, max compression
```

## Comparing `midi_to_dataframe-0.2.tar` & `midi_to_dataframe-0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:23:35.389544 midi_to_dataframe-0.2/
--rw-r--r--   0 taylor     (501) staff       (20)     4119 2024-04-26 16:03:04.000000 midi_to_dataframe-0.2/LICENSE
--rw-r--r--   0 taylor     (501) staff       (20)       68 2024-04-26 16:03:54.000000 midi_to_dataframe-0.2/MANIFEST.in
--rw-r--r--   0 taylor     (501) staff       (20)     1327 2024-04-26 16:23:35.388793 midi_to_dataframe-0.2/PKG-INFO
--rw-r--r--   0 taylor     (501) staff       (20)     1038 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/README.md
-drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:23:35.384535 midi_to_dataframe-0.2/midi_to_dataframe/
--rw-r--r--   0 taylor     (501) staff       (20)      108 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/midi_to_dataframe/__init__.py
--rw-r--r--   0 taylor     (501) staff       (20)    16656 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/midi_to_dataframe/midi_reader.py
--rw-r--r--   0 taylor     (501) staff       (20)     8228 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/midi_to_dataframe/midi_writer.py
--rw-r--r--   0 taylor     (501) staff       (20)     5450 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/midi_to_dataframe/note_mapper.py
-drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:23:35.388193 midi_to_dataframe-0.2/midi_to_dataframe.egg-info/
--rw-r--r--   0 taylor     (501) staff       (20)     1327 2024-04-26 16:23:35.000000 midi_to_dataframe-0.2/midi_to_dataframe.egg-info/PKG-INFO
--rw-r--r--   0 taylor     (501) staff       (20)      364 2024-04-26 16:23:35.000000 midi_to_dataframe-0.2/midi_to_dataframe.egg-info/SOURCES.txt
--rw-r--r--   0 taylor     (501) staff       (20)        1 2024-04-26 16:23:35.000000 midi_to_dataframe-0.2/midi_to_dataframe.egg-info/dependency_links.txt
--rw-r--r--   0 taylor     (501) staff       (20)       24 2024-04-26 16:23:35.000000 midi_to_dataframe-0.2/midi_to_dataframe.egg-info/top_level.txt
--rw-r--r--   0 taylor     (501) staff       (20)       38 2024-04-26 16:23:35.389690 midi_to_dataframe-0.2/setup.cfg
--rw-r--r--   0 taylor     (501) staff       (20)      600 2024-04-26 16:23:17.000000 midi_to_dataframe-0.2/setup.py
-drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:23:35.387232 midi_to_dataframe-0.2/tests/
--rw-r--r--   0 taylor     (501) staff       (20)        0 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/tests/__init__.py
--rw-r--r--   0 taylor     (501) staff       (20)      885 2024-04-26 15:58:56.000000 midi_to_dataframe-0.2/tests/tests.py
+drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:41:53.043782 midi_to_dataframe-0.3/
+-rw-r--r--   0 taylor     (501) staff       (20)     4119 2024-04-26 16:03:04.000000 midi_to_dataframe-0.3/LICENSE
+-rw-r--r--   0 taylor     (501) staff       (20)       68 2024-04-26 16:03:54.000000 midi_to_dataframe-0.3/MANIFEST.in
+-rw-r--r--   0 taylor     (501) staff       (20)      970 2024-04-26 16:41:53.043419 midi_to_dataframe-0.3/PKG-INFO
+-rw-r--r--   0 taylor     (501) staff       (20)      681 2024-04-26 16:37:33.000000 midi_to_dataframe-0.3/README.md
+drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:41:53.039385 midi_to_dataframe-0.3/midi_to_dataframe/
+-rw-r--r--   0 taylor     (501) staff       (20)      108 2024-04-26 15:58:56.000000 midi_to_dataframe-0.3/midi_to_dataframe/__init__.py
+-rw-r--r--   0 taylor     (501) staff       (20)    16752 2024-04-26 16:36:47.000000 midi_to_dataframe-0.3/midi_to_dataframe/midi_reader.py
+-rw-r--r--   0 taylor     (501) staff       (20)     8308 2024-04-26 16:36:47.000000 midi_to_dataframe-0.3/midi_to_dataframe/midi_writer.py
+-rw-r--r--   0 taylor     (501) staff       (20)     5450 2024-04-26 15:58:56.000000 midi_to_dataframe-0.3/midi_to_dataframe/note_mapper.py
+drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:41:53.043016 midi_to_dataframe-0.3/midi_to_dataframe.egg-info/
+-rw-r--r--   0 taylor     (501) staff       (20)      970 2024-04-26 16:41:53.000000 midi_to_dataframe-0.3/midi_to_dataframe.egg-info/PKG-INFO
+-rw-r--r--   0 taylor     (501) staff       (20)      364 2024-04-26 16:41:53.000000 midi_to_dataframe-0.3/midi_to_dataframe.egg-info/SOURCES.txt
+-rw-r--r--   0 taylor     (501) staff       (20)        1 2024-04-26 16:41:53.000000 midi_to_dataframe-0.3/midi_to_dataframe.egg-info/dependency_links.txt
+-rw-r--r--   0 taylor     (501) staff       (20)       24 2024-04-26 16:41:53.000000 midi_to_dataframe-0.3/midi_to_dataframe.egg-info/top_level.txt
+-rw-r--r--   0 taylor     (501) staff       (20)       38 2024-04-26 16:41:53.043867 midi_to_dataframe-0.3/setup.cfg
+-rw-r--r--   0 taylor     (501) staff       (20)      600 2024-04-26 16:37:46.000000 midi_to_dataframe-0.3/setup.py
+drwxr-xr-x   0 taylor     (501) staff       (20)        0 2024-04-26 16:41:53.042155 midi_to_dataframe-0.3/tests/
+-rw-r--r--   0 taylor     (501) staff       (20)        0 2024-04-26 15:58:56.000000 midi_to_dataframe-0.3/tests/__init__.py
+-rw-r--r--   0 taylor     (501) staff       (20)      885 2024-04-26 15:58:56.000000 midi_to_dataframe-0.3/tests/tests.py
```

### Comparing `midi_to_dataframe-0.2/LICENSE` & `midi_to_dataframe-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `midi_to_dataframe-0.2/midi_to_dataframe/midi_reader.py` & `midi_to_dataframe-0.3/midi_to_dataframe/midi_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-import midi
+import python3_midi
 import pandas as pd
 from collections import defaultdict
 from collections import OrderedDict
 from enum import Enum
 from collections import namedtuple
 
 # Named time signature tuple, i.e. 4/4, 5/4, etc.
@@ -95,15 +95,15 @@
     def convert_to_dataframe(self, path):
         """
         Loads a MIDI file from disk and creates a Pandas Data Frame representing its MIDI events.
         :param path: the path to the MIDI file to load.
         :return: the Data Frame.
         """
         try:
-            pattern = midi.read_midifile(path)
+            pattern = python3_midi.read_midifile(path)
         except (TypeError, RuntimeWarning):
             self._logger.error("Could not load MIDI file: " + path)
             self._reset_intermediary_variables()
             return pd.DataFrame()
 
         pattern.make_ticks_abs()
 
@@ -261,32 +261,32 @@
         Processes a MIDI event played by a given MIDI program.
         :param event: the MIDI event to process.
         :param program: the current program of the MIDI track the event occurred on.
         :return: the updated program of the MIDI track (since this may have been updated by the MIDI event).
         """
 
         # Set program for drums, since this is set by channel and not explicitly
-        if (type(event) == midi.NoteOnEvent or type(event) == midi.NoteOffEvent) and event.channel == MIDI_DRUM_CHANNEL:
+        if (type(event) == python3_midi.NoteOnEvent or type(event) == python3_midi.NoteOffEvent) and event.channel == MIDI_DRUM_CHANNEL:
             program = DEFAULT_MIDI_PROGRAM_NUM
-        elif (type(event) == midi.NoteOnEvent or type(event) == midi.NoteOffEvent) and program is None:
+        elif (type(event) == python3_midi.NoteOnEvent or type(event) == python3_midi.NoteOffEvent) and program is None:
             # If program was never set, default to 1 (Piano)
             program = 1
 
         # True Note On events have positive velocity
-        if type(event) == midi.NoteOnEvent and event.velocity > 0:
+        if type(event) == python3_midi.NoteOnEvent and event.velocity > 0:
             self._on_notes[event.pitch] = (event.tick, event)
         # Some sequences pass Note Off events encoded as a Note On event with 0 velocity
-        elif type(event) == midi.NoteOffEvent or type(event) == midi.NoteOnEvent and event.velocity == 0:
+        elif type(event) == python3_midi.NoteOffEvent or type(event) == python3_midi.NoteOnEvent and event.velocity == 0:
             self._process_note_off(event.pitch, program, event.tick)
-        elif type(event) == midi.TimeSignatureEvent:
+        elif type(event) == python3_midi.TimeSignatureEvent:
             self._time_signature_by_timestamp[event.tick] = TimeSignature(event.get_numerator(),
                                                                           event.get_denominator())
-        elif type(event) == midi.SetTempoEvent:
+        elif type(event) == python3_midi.SetTempoEvent:
             self._bpm_by_timestamp[event.tick] = event.get_bpm()
-        elif type(event) == midi.ProgramChangeEvent:
+        elif type(event) == python3_midi.ProgramChangeEvent:
             program = event.value
         else:
             # TODO: not currently handled: pitch changes, control changes, ...
             pass
 
         return program
```

### Comparing `midi_to_dataframe-0.2/midi_to_dataframe/midi_writer.py` & `midi_to_dataframe-0.3/midi_to_dataframe/midi_writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import midi
+import python3_midi
 
 REST = "rest"
 PERCUSSION = "percussion"
 PERCUSSION_CHANNEL = 9
 DEFAULT_MIDI_RESOLUTION = 120
 DEFAULT_MIDI_BPM = 120
 
@@ -35,15 +35,15 @@
     def convert_to_midi(self, dataframe, save_to_path):
         """
         Converts a (properly-formed) Pandas Data Frame into a MIDI file and writes it to disk.
         :param dataframe: the Pandas Data Frame to convert.
         :param save_to_path: the path to write the MIDI file to.
         :return: None.
         """
-        pattern = midi.Pattern()
+        pattern = python3_midi.Pattern()
         pattern.resolution = self._resolution
 
         # Reset all internal state variables to their defaults
         self._resolution = DEFAULT_MIDI_RESOLUTION
         self._bpm = DEFAULT_MIDI_BPM
         self._midi_tracks_by_track_num = {}
         self._prog_names_by_track_num = {}
@@ -90,24 +90,24 @@
 
                     # Get MIDI track for this program
                     (track_num, midi_track) = self._get_midi_track(program_name)
                     if midi_track is not None:
 
                         # Add NoteOn event to events to be added
                         key = self._note_mapper.get_note_number(note_name)
-                        on_event = midi.NoteOnEvent(velocity=127, pitch=key, channel=track_num)
+                        on_event = python3_midi.NoteOnEvent(velocity=127, pitch=key, channel=track_num)
                         if current_timestamp in midi_events_by_timestamp:
                             events = midi_events_by_timestamp[current_timestamp]
                             events.append(on_event)
                         else:
                             events = [on_event]
                         midi_events_by_timestamp[current_timestamp] = events
 
                         # Add NoteOff event to events to be added
-                        off_event = midi.NoteOffEvent(pitch=key, channel=track_num)
+                        off_event = python3_midi.NoteOffEvent(pitch=key, channel=track_num)
                         off_timestamp = current_timestamp + int((float(note_duration) * self._resolution))
                         if off_timestamp in midi_events_by_timestamp:
                             events = midi_events_by_timestamp[off_timestamp]
                             events.append(off_event)
                         else:
                             events = [off_event]
                         midi_events_by_timestamp[off_timestamp] = events
@@ -122,18 +122,18 @@
                 event.tick = delta
                 midi_track = self._midi_tracks_by_track_num[event.channel]
                 midi_track.append(event)
                 self._prev_timestamps_by_track_num[track_num] = timestamp
 
         # Add End-of-track event to every MIDI track
         for track_num, midi_track in self._midi_tracks_by_track_num.items():
-            midi_track.append(midi.EndOfTrackEvent(tick=1))
+            midi_track.append(python3_midi.EndOfTrackEvent(tick=1))
 
         # Write MIDI file to disk
-        midi.write_midifile(save_to_path, pattern)
+        python3_midi.write_midifile(save_to_path, pattern)
 
     def _get_midi_track(self, program_name):
         """
         Returns the index and MIDI track for a given MIDI program name.
         :param program_name: the program name to look up.
         :return: a tuple: (track number, MIDI track) for the program name, or None if none was found.
         """
@@ -147,35 +147,35 @@
         """
         Creates a new track in the designated MIDI pattern at the given track index and program name.
         :param track_index: the track number to use.
         :param program_name: the program name to use.
         :param pattern: the MIDI pattern to append the track to.
         :return: None.
         """
-        track = midi.Track()
+        track = python3_midi.Track()
         if program_name == PERCUSSION:
             # Set general track information on percussion channel
 
             # TODO: Set time signature information:
             # time_signature_event = midi.TimeSignatureEvent(tick=0)
             # time_signature_event.set_numerator(4)
             # time_signature_event.set_denominator(4)
             # time_signature_event.set_metronome(24)
             # time_signature_event.set_thirtyseconds(8)
             # track.append(time_signature_event)
 
             # Set tempo (BPM)
-            tempo_event = midi.SetTempoEvent(tick=0, bpm=int(self._bpm))
+            tempo_event = python3_midi.SetTempoEvent(tick=0, bpm=int(self._bpm))
             track.append(tempo_event)
 
             # Set drum channel
-            track.append(midi.ProgramChangeEvent(tick=0, channel=PERCUSSION_CHANNEL))
+            track.append(python3_midi.ProgramChangeEvent(tick=0, channel=PERCUSSION_CHANNEL))
         else:
             program_num = self._note_mapper.get_program_number(program_name)
-            program_change_event = midi.ProgramChangeEvent(tick=0, data=[program_num])
+            program_change_event = python3_midi.ProgramChangeEvent(tick=0, data=[program_num])
             track.append(program_change_event)
 
         pattern.append(track)
         self._midi_tracks_by_track_num[track_index] = track
         self._prev_timestamps_by_track_num[track_index] = 0
 
     @staticmethod
```

### Comparing `midi_to_dataframe-0.2/midi_to_dataframe/note_mapper.py` & `midi_to_dataframe-0.3/midi_to_dataframe/note_mapper.py`

 * *Files identical despite different names*

### Comparing `midi_to_dataframe-0.2/setup.py` & `midi_to_dataframe-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 # Define version information
-VERSION = '0.2'
+VERSION = '0.3'
 FULLVERSION = VERSION
 
 requirements = [
 ]
 
 setup(name='midi_to_dataframe',
       version=VERSION,
```

### Comparing `midi_to_dataframe-0.2/tests/tests.py` & `midi_to_dataframe-0.3/tests/tests.py`

 * *Files identical despite different names*

