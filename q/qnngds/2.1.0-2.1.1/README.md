# Comparing `tmp/qnngds-2.1.0.tar.gz` & `tmp/qnngds-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnngds-2.1.0.tar", last modified: Wed Apr 24 12:31:43 2024, max compression
+gzip compressed data, was "qnngds-2.1.1.tar", last modified: Thu Apr 25 22:45:05 2024, max compression
```

## Comparing `qnngds-2.1.0.tar` & `qnngds-2.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1081 2024-04-24 12:31:36.945616 qnngds-2.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1129 2024-04-24 12:31:36.945616 qnngds-2.1.0/README.md
--rw-r--r--   0        0        0     1161 2024-04-24 12:31:43.621630 qnngds-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      508 2024-04-24 12:31:36.957616 qnngds-2.1.0/src/qnngds/__init__.py
--rw-r--r--   0        0        0      291 2024-04-24 12:31:36.957616 qnngds-2.1.0/src/qnngds/_default_param.py
--rw-r--r--   0        0        0    23310 2024-04-24 12:31:36.957616 qnngds-2.1.0/src/qnngds/cells.py
--rw-r--r--   0        0        0    10495 2024-04-24 12:31:36.957616 qnngds-2.1.0/src/qnngds/circuits.py
--rw-r--r--   0        0        0    28386 2024-04-24 12:31:36.961616 qnngds-2.1.0/src/qnngds/design.py
--rw-r--r--   0        0        0      160 2024-04-24 12:31:36.961616 qnngds-2.1.0/src/qnngds/devices/__init__.py
--rw-r--r--   0        0        0       90 2024-04-24 12:31:36.961616 qnngds-2.1.0/src/qnngds/devices/htron.py
--rw-r--r--   0        0        0     1177 2024-04-24 12:31:36.961616 qnngds-2.1.0/src/qnngds/devices/nanowire.py
--rw-r--r--   0        0        0     4453 2024-04-24 12:31:36.961616 qnngds-2.1.0/src/qnngds/devices/ntron.py
--rw-r--r--   0        0        0     5860 2024-04-24 12:31:36.961616 qnngds-2.1.0/src/qnngds/devices/resistor.py
--rw-r--r--   0        0        0     2376 2024-04-24 12:31:36.961616 qnngds-2.1.0/src/qnngds/devices/snspd.py
--rw-r--r--   0        0        0     1237 2024-04-24 12:31:36.961616 qnngds-2.1.0/src/qnngds/geometries.py
--rw-r--r--   0        0        0     7907 2024-04-24 12:31:36.961616 qnngds-2.1.0/src/qnngds/tests.py
--rw-r--r--   0        0        0    21104 2024-04-24 12:31:36.961616 qnngds-2.1.0/src/qnngds/utilities.py
--rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-25 22:45:02.792756 qnngds-2.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2024-04-25 22:45:02.792756 qnngds-2.1.1/README.md
+-rw-r--r--   0        0        0     1161 2024-04-25 22:45:05.580779 qnngds-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      508 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/_default_param.py
+-rw-r--r--   0        0        0    23463 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/cells.py
+-rw-r--r--   0        0        0    10495 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/circuits.py
+-rw-r--r--   0        0        0    28386 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/design.py
+-rw-r--r--   0        0        0      160 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/devices/__init__.py
+-rw-r--r--   0        0        0      231 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/devices/htron.py
+-rw-r--r--   0        0        0     1214 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/devices/nanowire.py
+-rw-r--r--   0        0        0     4526 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/devices/ntron.py
+-rw-r--r--   0        0        0     5935 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/devices/resistor.py
+-rw-r--r--   0        0        0     2443 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/devices/snspd.py
+-rw-r--r--   0        0        0     1237 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/geometries.py
+-rw-r--r--   0        0        0     7907 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/tests.py
+-rw-r--r--   0        0        0    21104 2024-04-25 22:45:02.804756 qnngds-2.1.1/src/qnngds/utilities.py
+-rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-2.1.1/PKG-INFO
```

### Comparing `qnngds-2.1.0/LICENSE.txt` & `qnngds-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.0/README.md` & `qnngds-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.0/pyproject.toml` & `qnngds-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "qnngds"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
     { name = "A. Jacquillat", email = "audrey.jacquillat@gmail.com" },
     { name = "R. Foster", email = "reedf@mit.edu" },
 ]
 maintainers = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
```

### Comparing `qnngds-2.1.0/src/qnngds/cells.py` & `qnngds-2.1.1/src/qnngds/cells.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+"""Library of pre-built cells containing text, border marks, and an experiment,
+connected to pads for wirebonding."""
+
 from phidl import Device
 import phidl.geometry as pg
 import phidl.routing as pr
 from typing import Tuple, List, Union
 import math
 
 import qnngds.tests as test
 import qnngds.devices as device
 import qnngds.circuits as circuit
 import qnngds.utilities as utility
 import qnngds._default_param as dflt
 
 # basics
 
+
 def alignment(
     die_w: Union[int, float] = dflt.die_w,
     layers_to_align: List[int] = [dflt.layers["die"], dflt.layers["pad"]],
     outline_die: Union[int, float] = dflt.die_outline,
     die_layer: int = dflt.layers["die"],
     text: Union[None, str] = dflt.text,
 ) -> Device:
@@ -85,21 +89,25 @@
         DIE_VANDP (Device): The created device.
     """
     # Initialize parameters left to default (=None)
 
     if text is None:
         text = str(layers_to_probe)
     if layers_to_outline is None:
-        layers_to_outline = [die_layer] # default layer to outline if None is given
-    
+        layers_to_outline = [die_layer]  # default layer to outline if None is given
+
     DIE_VANDP = Device(f"DIE VAN DER PAUW {text} ")
 
-    device_max_w = die_w - 2 * (pad_size[1] + 2 * outline)  # width of max device size for this cell
-    contact_w = device_max_w/10            # choosing a contact width 10 times smaller
-    device_w = device_max_w - 2*contact_w  # choosing a smaller device to have space for routing from pad to contact
+    device_max_w = die_w - 2 * (
+        pad_size[1] + 2 * outline
+    )  # width of max device size for this cell
+    contact_w = device_max_w / 10  # choosing a contact width 10 times smaller
+    device_w = (
+        device_max_w - 2 * contact_w
+    )  # choosing a smaller device to have space for routing from pad to contact
 
     # Creates the DIE, it contains only the cell text and bordure
 
     DIE = utility.die_cell(
         die_size=(die_w, die_w),
         device_max_size=(device_max_w, device_max_w),
         ports={},
@@ -134,15 +142,15 @@
         layer=0,
         pad_layer=pad_layer,
         invert=False,
     )
     PADS.remove_layers([pad_layer], invert_selection=True)
     VDP << PADS
 
-    ## routes from pads to probing area 
+    ## routes from pads to probing area
     ROUTES = utility.route_to_dev(PADS.get_ports(), AREA.ports)
     VDP << ROUTES
 
     VDP.flatten(0)
 
     # Outline the vdp structure for layers that need to be outlined
 
@@ -385,15 +393,17 @@
         nanowire_ref.movex(BORDER.ports[f"N{i+1}"].x)
         NANOWIRES.add_port(port=nanowire_ref.ports[1], name=f"N{i+1}")
         NANOWIRES.add_port(port=nanowire_ref.ports[2], name=f"S{i+1}")
 
     ## Route the nanowires and the die
 
     # hyper tapers
-    HT, dev_ports = utility.add_hyptap_to_cell(BORDER.get_ports(), overlap_w, dev_contact_w)
+    HT, dev_ports = utility.add_hyptap_to_cell(
+        BORDER.get_ports(), overlap_w, dev_contact_w
+    )
     DEVICE.ports = dev_ports.ports
     DEVICE << HT
 
     # routes from nanowires to hyper tapers
     ROUTES = utility.route_to_dev(HT.get_ports(), NANOWIRES.ports)
     DEVICE << ROUTES
 
@@ -655,8 +665,7 @@
     DIE_SNSPD_NTRON << DEVICE
     DIE_SNSPD_NTRON << BORDER
 
     DIE_SNSPD_NTRON = pg.union(DIE_SNSPD_NTRON, by_layer=True)
     DIE_SNSPD_NTRON.name = f"SNSPD \n{w_snspd} {w_choke} "
 
     return DIE_SNSPD_NTRON
-
```

### Comparing `qnngds-2.1.0/src/qnngds/circuits.py` & `qnngds-2.1.1/src/qnngds/circuits.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.0/src/qnngds/design.py` & `qnngds-2.1.1/src/qnngds/design.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.0/src/qnngds/devices/nanowire.py` & `qnngds-2.1.1/src/qnngds/devices/nanowire.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Single nanowire constriction."""
+
 from phidl import Device
 
 import phidl.geometry as pg
 from typing import Tuple, Optional
 
 
 def spot(
```

### Comparing `qnngds-2.1.0/src/qnngds/devices/ntron.py` & `qnngds-2.1.1/src/qnngds/devices/ntron.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Nanocryotron `[1] <https://doi.org/10.1021/nl502629x>`_ variants."""
+
 from phidl import Device
 
 import phidl.geometry as pg
 from typing import Tuple, Optional
 
 
 def smooth(
```

### Comparing `qnngds-2.1.0/src/qnngds/devices/resistor.py` & `qnngds-2.1.1/src/qnngds/devices/resistor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Layouts for resistors and resistors with superconducting contacts."""
+
 from phidl import Device
 
 import phidl.geometry as pg
 from typing import Tuple, Optional
 
 
 def meander(
@@ -101,14 +103,15 @@
     stub_bot.connect(stub_bot.ports[1], hp_prev.ports[2 - (n_turn % 2)])
     D = pg.union(D, by_layer=True, precision=0.01)
     D.add_port(name=1, port=stub_top.ports[2])
     D.add_port(name=2, port=stub_bot.ports[2])
     D.info = locals()
     return D
 
+
 def sc_contacts(
     width: float = 1,
     squares: float = 60,
     max_length: float = 10,
     meander_pitch: float = 2,
     contact_width: float = 8,
     contact_height: float = 2,
```

### Comparing `qnngds-2.1.0/src/qnngds/devices/snspd.py` & `qnngds-2.1.1/src/qnngds/devices/snspd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Superconducting nanowire single photon detector geometries."""
+
 from phidl import Device
 
 import phidl.geometry as pg
 from typing import Tuple, Optional
 
 
 def vertical(
```

### Comparing `qnngds-2.1.0/src/qnngds/geometries.py` & `qnngds-2.1.1/src/qnngds/geometries.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.0/src/qnngds/tests.py` & `qnngds-2.1.1/src/qnngds/tests.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.0/src/qnngds/utilities.py` & `qnngds-2.1.1/src/qnngds/utilities.py`

 * *Files identical despite different names*

### Comparing `qnngds-2.1.0/PKG-INFO` & `qnngds-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qnngds
-Version: 2.1.0
+Version: 2.1.1
 Summary: The QNN library for creating gds files
 Keywords: phidl,nanowire_electronics,nanofabrication,gds
 Author-Email: "A. Jacquillat" <audrey01@mit.edu>, "A. Jacquillat" <audrey.jacquillat@gmail.com>, "R. Foster" <reedf@mit.edu>
 Maintainer-Email: "A. Jacquillat" <audrey01@mit.edu>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

