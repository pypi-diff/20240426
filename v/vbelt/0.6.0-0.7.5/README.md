# Comparing `tmp/vbelt-0.6.0.tar.gz` & `tmp/vbelt-0.7.5.tar.gz`

## Comparing `vbelt-0.6.0.tar` & `vbelt-0.7.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/__init__.py
--rwxr-xr-x   0        0        0     5607 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/charge_utils.py
--rwxr-xr-x   0        0        0    10595 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/coherence.py
--rwxr-xr-x   0        0        0     1386 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/forces.py
--rwxr-xr-x   0        0        0     8560 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/gencalc.py
--rwxr-xr-x   0        0        0     1197 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/incar.py
--rwxr-xr-x   0        0        0     6996 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/jobtool.py
--rwxr-xr-x   0        0        0     2375 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/kpoints.py
--rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/logger.py
--rwxr-xr-x   0        0        0     4656 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/misc.py
--rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/outcar.py
--rwxr-xr-x   0        0        0     3551 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/outcar_utils.py
--rwxr-xr-x   0        0        0    10808 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/poscar.py
--rwxr-xr-x   0        0        0    17257 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/poscartool.py
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/potcar.py
--rwxr-xr-x   0        0        0    13803 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/script_utils.py
--rwxr-xr-x   0        0        0    11831 2020-02-02 00:00:00.000000 vbelt-0.6.0/vbelt/wrapper.py
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 vbelt-0.6.0/.gitignore
--rwxr-xr-x   0        0        0    14663 2020-02-02 00:00:00.000000 vbelt-0.6.0/LICENSE
--rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 vbelt-0.6.0/README.md
--rwxr-xr-x   0        0        0     1200 2020-02-02 00:00:00.000000 vbelt-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 vbelt-0.6.0/PKG-INFO
+-rwxr-xr-x   0        0        0      119 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/__init__.py
+-rwxr-xr-x   0        0        0     5623 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/charge_utils.py
+-rwxr-xr-x   0        0        0    10595 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/coherence.py
+-rwxr-xr-x   0        0        0     1421 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/forces.py
+-rwxr-xr-x   0        0        0     8768 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/gencalc.py
+-rwxr-xr-x   0        0        0     1197 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/incar.py
+-rwxr-xr-x   0        0        0     6996 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/jobtool.py
+-rwxr-xr-x   0        0        0     2416 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/kpoints.py
+-rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/logger.py
+-rwxr-xr-x   0        0        0     4699 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/misc.py
+-rwxr-xr-x   0        0        0     2946 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/outcar.py
+-rwxr-xr-x   0        0        0     3551 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/outcar_utils.py
+-rwxr-xr-x   0        0        0    11129 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/poscar.py
+-rwxr-xr-x   0        0        0    17790 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/poscartool.py
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/potcar.py
+-rwxr-xr-x   0        0        0    14455 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/script_utils.py
+-rwxr-xr-x   0        0        0    13531 2020-02-02 00:00:00.000000 vbelt-0.7.5/vbelt/wrapper.py
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 vbelt-0.7.5/.gitignore
+-rwxr-xr-x   0        0        0    14663 2020-02-02 00:00:00.000000 vbelt-0.7.5/LICENSE
+-rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 vbelt-0.7.5/README.md
+-rwxr-xr-x   0        0        0     1133 2020-02-02 00:00:00.000000 vbelt-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 vbelt-0.7.5/PKG-INFO
```

### Comparing `vbelt-0.6.0/vbelt/charge_utils.py` & `vbelt-0.7.5/vbelt/charge_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # vbelt: The VASP user toolbelt.
 # Copyright (C) 2023  Théo Cavignac
 # Licensed under EUPL
 from math import ceil
 from itertools import islice
 import numpy as np
 
-from .misc import prod
+from .misc import prod, InvalidInput
 
 
 class Charge:
     def __init__(self, poscar, chg, aug):
         self.poscar = poscar
         self.tot_chg = chg
         self.tot_aug = aug
@@ -127,15 +127,15 @@
 
         if self.dif_part:
             write_channel(file, self.dif_part)
 
     def split(self):
         "Split the Charge object into a spin up and a spin down object."
         if self.dif_part is None:
-            raise ValueError("No spin related data available.")
+            raise InvalidInput("No spin related data available.")
 
         return 0.5 * (self.total_only() + self.dif_part), 0.5 * (
             self.total_only() - self.dif_part
         )
 
 
 def read_channel(file, head=None):
```

### Comparing `vbelt-0.6.0/vbelt/coherence.py` & `vbelt-0.7.5/vbelt/coherence.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.6.0/vbelt/forces.py` & `vbelt-0.7.5/vbelt/forces.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # vbelt: The VASP user toolbelt.
 # Copyright (C) 2023  Théo Cavignac
 # Licensed under EUPL
 from itertools import islice
 import numpy as np
 
+from .misc import InvalidInput
 from .outcar_utils import get_species, get_array, get_float
 
 
 def read_forces(file):
     for line in file:
         if "POTCAR" in line:
             break
     else:
-        raise ValueError("Could not find the list of potential.")
+        raise InvalidInput("Could not find the list of potential.")
 
     first = line
 
     nb_specs = 1
     for line in file:
         if "POTCAR" not in line:
             break  # works in v5
@@ -54,12 +55,12 @@
                 break
         else:
             break  # EOF
 
         raw = list(islice(file, 1, 1 + nb_tot))
 
     if raw is None:
-        raise ValueError("Forces not found.")
+        raise InvalidInput("Forces not found.")
 
     forces = np.array([line.split()[3:] for line in raw], dtype=float)
 
     return list(zip(species, nb_atoms)), forces, tol
```

### Comparing `vbelt-0.6.0/vbelt/gencalc.py` & `vbelt-0.7.5/vbelt/gencalc.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,22 @@
 class Batch:
     def __init__(self):
         self.potcars = ""
         self.batch_preset = "medium2"
         self.ncpu = 1
         self.ncpu_per_node = 1
         self.functional = "GGA"
+        self.tmpl_sp = tmpl_sp
+        self.tmpl_opt = tmpl_opt
+
+    def set_sp_template(self, tmpl):
+        self.tmpl_sp = tmpl
+
+    def set_opt_template(self, tmpl):
+        self.tmpl_opt = tmpl
 
     def gencalcs(self, name, bundle_name, computations, encut, sc, make_faulted_cell):
         sc = sort(sc, tags=[electronegativity[at.symbol] for at in sc])
         faulted = make_faulted_cell(sc)
         self.prepare_bundle(sc, faulted, name, bundle_name, encut, computations)
 
     def prepare_bundle(self, sc, faulted, name, bundle_name, encut, computations):
@@ -84,15 +92,15 @@
                 with in_dir(d):
                     if exc:
                         ferwe, ferdo = make_fer(nelect, nband, nkpt, exc)
 
                     with open("INCAR", "w") as f:
                         f.write(
                             chevron.render(
-                                tmpl_sp if sp else tmpl_opt,
+                                self.tmpl_sp if sp else self.tmpl_opt,
                                 {
                                     "encut": encut,
                                     "name": name,
                                     "ncore": ncore,
                                     "kpar": kpar,
                                     "base": not exc,
                                     "excited": (
```

### Comparing `vbelt-0.6.0/vbelt/incar.py` & `vbelt-0.7.5/vbelt/incar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.6.0/vbelt/jobtool.py` & `vbelt-0.7.5/vbelt/jobtool.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.6.0/vbelt/kpoints.py` & `vbelt-0.7.5/vbelt/kpoints.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # vbelt: The VASP user toolbelt.
 # Copyright (C) 2023  Théo Cavignac
 # Licensed under EUPL
+from .misc import InvalidInput
+
+
 class Kpoints:
     def __init__(self, kind, data):
         self.kind = kind
         self.data = data
 
     @classmethod
     def from_file(cls, path):
@@ -13,30 +16,30 @@
             next(f)  # first line is ignored
 
             n = int(next(f).strip())
             mode = next(f).strip()[0].lower()
 
             if n == 0:
                 if mode not in {"m", "g"}:
-                    raise ValueError(
+                    raise InvalidInput(
                         f"Unknown k-point generation automatic mode {mode}"
                     )
 
                 n1, n2, n3 = map(int, next(f).strip().split()[:3])
 
                 return cls(mode, (n1, n2, n3))
 
             else:
                 if mode not in {"c", "k", "r", "l"}:
-                    raise ValueError("Unknown k-point explicit mode")
+                    raise InvalidInput("Unknown k-point explicit mode")
 
                 if mode == "l":
                     line_coord = next(f).strip()[0].lower()
                     if line_coord != "f" and line_coord != "r":
-                        raise ValueError(
+                        raise InvalidInput(
                             "I don't want to deal with anything but fractional k points."
                         )
 
                     segments = []
                     first = None
                     for line in f:
                         if l := line.strip():
@@ -51,16 +54,16 @@
 
                 elif mode == "r":
                     points = []
 
                     for line in f:
                         if l := line.strip():
                             # FIXME does VASP actually takes empty lines here?
-                            points.append(tuple(map(float(l.split()[:3]))))
+                            points.append(tuple(map(float, l.split()[:3])))
 
                     return cls("list", points)
 
                 elif mode == "c":
                     # If you like cartesian mode feel free to implement the logic missing here
-                    raise ValueError(
+                    raise InvalidInput(
                         "Please don't use cartesian mode, it's a dumb mode I don't like it."
                     )
```

### Comparing `vbelt-0.6.0/vbelt/misc.py` & `vbelt-0.7.5/vbelt/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,18 @@
         return f"{int(floor(n))} {name}"
     elif left == 1:
         return f"{int(floor(n))} and a half {name}"
     else:
         return f"{int(round(n))} {name}"
 
 
+class InvalidInput(ValueError):
+    pass
+
+
 try:
     from math import prod
 except ImportError:
 
     def prod(numbers):
         t = 1
         for n in numbers:
```

### Comparing `vbelt-0.6.0/vbelt/outcar_utils.py` & `vbelt-0.7.5/vbelt/outcar_utils.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.6.0/vbelt/poscar.py` & `vbelt-0.7.5/vbelt/poscar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # vbelt: The VASP user toolbelt.
 # Copyright (C) 2023  Théo Cavignac
 # Licensed under EUPL
 import numpy as np
-from .misc import electronegativity
+from .misc import electronegativity, InvalidInput
 
 
 def nudge(poscar_src, poscar_dest, forces, A=0.01, rattle=0.0, cartesian=True):
     src = Poscar.from_file(poscar_src)
 
     if forces is not None and src.raw.shape != forces.shape:
         raise ValueError("Incompatible shapes of forces and positions.")
@@ -34,49 +34,62 @@
 
         nudged += rattle * rd
 
     src.raw = nudged
     src.to_file(poscar_dest, cartesian=cartesian)
 
 
-def change_bond_length(poscar_src, poscar_dest, fixed_species, moved_species, amplitude=0, relative_amplitude=0, cartesian=True):
-    """Change the length of bonds from the source and write it to the dest.
+def change_bond_length(
+    poscar_src,
+    poscar_dest,
+    fixed_points,
+    moved_species,
+    amplitude=0,
+    relative_amplitude=0,
+    cartesian=True,
+):
+    """Change the length of bonds between `moved_species` and the closest of fixed_points.
 
     Exactly one of `amplitude` and `relative_amplitude` must be non-zero.
     Positive amplitudes lengthen the bonds, negative shorten them.
 
-    :param poscar_src: the source POSCAR path
-    :param poscar_dest: the destination POSCAR path
-    :param fixed_species: the name of the species to keep fixed
+    :param poscar_src: source :class:`Poscar` instance
+    :param fixed_points: array of coordinates of the fixed centers
     :param moved_species: the name of the species to move
     :param amplitude: (optional) the absolute amplitude of the move in A
     :param relative_amplitude: (optional) the relative amplitude of the move in fraction
     :param cartesian: if True, write the file in cartesian representation,
+    :return: a new :class:`Poscar` instance with modified bonds.
     """
     if amplitude == 0 and relative_amplitude == 0:
         raise ValueError("One of amplitude or relative_amplitude must be non-zero.")
 
     if amplitude != 0 and relative_amplitude != 0:
         raise ValueError("Only one of amplitude or relative_amplitude can be non-zero.")
 
     relative = amplitude == 0
-    src = Poscar.from_file(poscar_src)
 
-    for k, p1 in enumerate(src.species[moved_species]):
-        d = periodic_dist(src.cell_parameters, np.array([p1]), src.species[fixed_species])
+    dest = poscar_src.copy()
+
+    for k, p1 in enumerate(dest.species[moved_species]):
+        d = periodic_dist(dest.cell_parameters, np.array([p1]), fixed_points)
         i = np.argmin(d)
-        v = periodic_diff(src.cell_parameters, np.array([p1]), np.array([src.species[fixed_species][i]]))[0]
+        v = periodic_diff(
+            dest.cell_parameters,
+            np.array([p1]),
+            np.array([fixed_points[i]]),
+        )[0]
 
         if relative:
-            src.species[moved_species][k] += relative_amplitude * v
+            dest.species[moved_species][k] += relative_amplitude * v
         else:
             v /= np.linalg.norm(v)
-            src.species[moved_species][k] += amplitude * v
+            dest.species[moved_species][k] += amplitude * v
 
-    src.to_file(poscar_dest, cartesian=cartesian)
+    return dest
 
 
 def distance(poscar, i, j):
     sp, si = i
     pi = poscar.species[sp][si, :]
 
     sp, sj = j
@@ -208,14 +221,22 @@
             species.sort(key=lambda p: electronegativity[p[0]])
             return " ".join(f"{label}{len(pos)}" for label, pos in species)
 
     @system_name.setter
     def system_name(self, val):
         self._system_name = val if val is None else str(val)
 
+    def copy(self):
+        "Fresh copy of the object."
+        return self.__class__(
+            self.cell_parameters.copy(),
+            {sp: pos.copy() for sp, pos in self.species.items()},
+            species_names=self._species_names,
+        )
+
     @classmethod
     def from_cell(cls, cell):
         species = {}
         positions = cell.positions
         accum = 0
         for name, number in zip(cell.atoms_types, cell.nb_atoms):
             species[name] = positions[accum : accum + number]
@@ -242,15 +263,15 @@
                     for _, l in zip(range(3), f)
                 ]
             )
 
             labels = next(f).strip().split()
             atoms_pop = list(map(int, next(f).strip().split()))
             if len(labels) != len(atoms_pop):
-                raise ValueError(f"{filename} is not a coherent POSCAR file.")
+                raise InvalidInput(f"{filename} is not a coherent POSCAR file.")
 
             mode = next(f).strip()[0].lower()
 
             if mode == "s":
                 # selective dynamics, skip line
                 mode = next(f).strip()[0].lower()
 
@@ -260,15 +281,15 @@
                     raise NotImplementedError(
                         "Repeated non contiguous species block is not supported."
                     )
                 pos = []
                 for _, line in zip(range(n), f):
                     ls = line.strip()
                     if not ls:
-                        raise ValueError(f"{filename} is not a coherent POSCAR file.")
+                        raise InvalidInput(f"{filename} is not a coherent POSCAR file.")
                     x, y, z, *_ = ls.split()
                     if mode == "d":
                         # Fractional coordinates
                         pos.append(np.array([x, y, z], dtype="float").dot(params))
                     else:
                         # Cartesian coordinates
                         pos.append(np.array([x, y, z], dtype="float"))
```

### Comparing `vbelt-0.6.0/vbelt/poscartool.py` & `vbelt-0.7.5/vbelt/poscartool.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,41 +71,66 @@
             A=opts.amplitude,
             rattle=opts.rattle,
             cartesian=opts.cartesian,
         )
 
     return 0
 
+
 @poscartool.subcmd(
     positional("POSCAR", help="Source file."),
-    positional("FIXED", type=str, help="Atoms to keep fixed."),
+    positional("FIXED", type=str, help="Atom(s) to keep fixed."),
     positional("MOVED", type=str, help="Atoms to move."),
     positional("AMPLITUDE", help="Amplitude of the move in A or in %."),
     optional("--dest", "-o", type=str, default=None, help="Destionation file."),
     flag("--cartesian", "-C", help="Write POSCAR in cartesian coordinates."),
 )
 def nudge_bonds(opts):
     """Change the length of the bonds.
 
+    Fixed atom can be either a species ("V": all vanadium atoms are concerned) or an atom specification
+    ("V3", only the third vanadium atom is concerned).
+
     Negative amplitudes shorten the bonds, positive amplitudes lengthen them.
     Write 0.15 to mean "lengthen the bond by 0.15 A" and -1% to mean "shorten
     the bond by 1%"
     """
-    from .poscar import change_bond_length
+    from .poscar import change_bond_length, Poscar
+    import numpy as np
 
     src = opts.poscar
     dest = opts.poscar + ".nudged" if opts.dest is None else opts.dest
 
+    src = Poscar.from_file(src)
+
+    sp_name, sp_id = parse_spec(src, opts.fixed)
+
+    if sp_id is None:
+        fixed = src.species[sp_name]
+    else:
+        fixed = np.array([src.species[sp_name][sp_id]])
+
     if opts.amplitude.endswith("%"):
         amplitude = float(opts.amplitude[:-1]) / 100
         print(amplitude)
-        change_bond_length(src, dest, opts.fixed, opts.moved, relative_amplitude=amplitude, cartesian=opts.cartesian)
+        res = change_bond_length(
+            src,
+            dest,
+            fixed,
+            opts.moved,
+            relative_amplitude=amplitude,
+            cartesian=opts.cartesian,
+        )
     else:
         amplitude = float(opts.amplitude)
-        change_bond_length(src, dest, opts.fixed, opts.moved, amplitude=amplitude, cartesian=opts.cartesian)
+        res = change_bond_length(
+            src, dest, fixed, opts.moved, amplitude=amplitude, cartesian=opts.cartesian
+        )
+
+    res.to_file(dest)
 
 
 @poscartool.subcmd(
     positional("POSCAR", help="Source file."),
     positional("DEST", default=None, help="Destionation file."),
 )
 def xyz(opts):
```

### Comparing `vbelt-0.6.0/vbelt/potcar.py` & `vbelt-0.7.5/vbelt/potcar.py`

 * *Files identical despite different names*

### Comparing `vbelt-0.6.0/vbelt/script_utils.py` & `vbelt-0.7.5/vbelt/script_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,24 +99,28 @@
     CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
     SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
     INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
     CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
     ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
     POSSIBILITY OF SUCH DAMAGE.
 """
+
 import sys
 import os
 from argparse import ArgumentParser, Namespace
 from contextlib import contextmanager
 from functools import wraps
 from statistics import mean, stdev, variance
 from time import perf_counter
 
 from typing import Callable, List, TypeVar, Optional, Generic
 
+from . import __name__ as pkg_name
+from . import __version__ as pkg_version
+
 _debug = os.environ.get("DEBUG", False) in {"1", "yes", "true"}
 
 
 T = TypeVar("T")
 ArgSpec = Callable[[ArgumentParser], None]
 
 ScriptWrapper = Callable[[Callable[[Namespace], T]], Callable[[List[str]], T]]
@@ -134,21 +138,25 @@
     """A CLI with several subcommands.
 
     Build an entrypoint with several subcommands.
     Register subcommands with MultiCmd.subcmd.
     Call the instance (or its run method) to run the script.
     """
 
-    def __init__(self, **kwargs) -> None:
+    def __init__(self, *, version=None, **kwargs) -> None:
         self.main_parser = ArgumentParser(**kwargs)
         self.sub_parsers = self.main_parser.add_subparsers()
 
         self._pre: Optional[Callable[[Namespace], None]] = None
         self._post: PostFn[T] = _default_post
 
+        self.version = version or f"{pkg_name} {pkg_version}"
+
+        self.add(flag("--version", "-V", help="show program's version number and exit"))
+
     def add(self, option: ArgSpec):
         "Add a global parameter, common to all subcommands."
         option(self.main_parser)
 
     def pre(self, f: Callable[[Namespace], None]):
         "Register a function to be called on the namespace before the command."
         assert callable(f), "pre applies to functions"
@@ -201,53 +209,68 @@
         """
 
         if argv is None:
             opts = self.main_parser.parse_args()
         else:
             opts = self.main_parser.parse_args(argv)
 
+        if opts.version:
+            print(self.version_msg)
+            return 0
+
         if self._pre:
             self._pre(opts)
 
         if not hasattr(opts, "handler"):
             self.main_parser.print_help()
-            exit(1)
+            return 1
 
         return self._post(opts.handler(opts))
 
 
 def script(
-    *args: ArgSpec, name: Optional[str] = None, doc: Optional[str] = None
+    *args: ArgSpec,
+    version: Optional[str] = None,
+    name: Optional[str] = None,
+    doc: Optional[str] = None,
 ) -> ScriptWrapper:
     """Wrap a function for a script.
 
     Each argument of specify an element of the CLI wrapping the function (see
     positional, optional, flag, rest). The function will be called with a
     argparse.Namespace instance containing the parser parameters.
     """
+    version_ = version or f"{pkg_name} {pkg_version}"
 
     def decorator(f):
         if doc is None:
             doc_ = f.__doc__ and f.__doc__.replace("%", "%%")
         else:  # doc == "" is valid and cause the description to be empty
             doc_ = doc.replace("%", "%%")
         parser = ArgumentParser(prog=name or f.__name__, description=doc_)
+        flag("--version", "-V", help="show program's version number and exit")(parser)
 
         for param in args:
             param(parser)
 
         @wraps(f)
         def wrapper(argv=None):
             if argv is None:
                 opts = parser.parse_args()
             else:
                 opts = parser.parse_args(argv)
 
+            if opts.version:
+                print(version_)
+                return 0
+
             return f(opts)
 
+        wrapper.__doc__ = parser.format_help()
+
         return wrapper
 
     return decorator
 
 
 def error(msg: str):
     "Write msg to stderr and exit with -1 return code."
```

### Comparing `vbelt-0.6.0/vbelt/wrapper.py` & `vbelt-0.7.5/vbelt/wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -106,36 +106,43 @@
     optional(
         "--tol",
         type=float,
         default=None,
         help="Maximum converged force ampliture (A/eV)",
     ),
     flag("--silent", "-q", help="quite mode, just use the return code"),
+    flag("--short", "-S", help="short summary"),
 )
 def check_forces(opts):
     import numpy as np
     from .forces import read_forces
 
-    with error_catch(), open(opts.outcar) as f:
-        species, forces, tol = read_forces(f)
+    with error_catch():
+        try:
+            with open(opts.outcar) as f:
+                species, forces, tol = read_forces(f)
+        except OSError:
+            if not opts.silent:
+                print("OUTCAR does not exist.")
+            return 1
 
     if opts.tol is not None:
         tol = opts.tol
 
     of = 0
 
     norms = np.linalg.norm(forces, axis=-1)
     (non_conv_where,) = np.where(norms > tol)
     non_conv_where = set(non_conv_where)
 
-    if not opts.silent:
+    if not (opts.silent or opts.short):
         for sp, n in species:
             print(f"{sp:2} {n:3}")
 
-    if not opts.silent:
+    if not (opts.silent or opts.short):
         print("       ---        X          Y          Z")
         print("===========================================")
         for sp, n in species:
             for j, (x, y, z) in enumerate(forces[of : of + n], start=of):
                 if j in non_conv_where:
                     m = [" ", " ", " "]
                     m[np.argmax(np.abs([x, y, z]))] = "<"
@@ -143,34 +150,52 @@
                         f"{sp:2} {j+1:3} >>> {x: .05f} {m[0]} {y: .05f} {m[1]} {z: .05f} {m[2]}"
                     )
                 else:
                     print(f"{sp:2} {j+1:3}     {x: .05f}   {y: .05f}   {z: .05f}  ")
             of += n
 
     if non_conv_where:
-        if not opts.silent:
+        if opts.short:
+            i = np.argmax(norms)
+            left = i
+            for sp, n in species:
+                if left < n:
+                    spec = f"{sp}{left+1}"
+                    break
+                else:
+                    left -= n
+            print(f"atom {i}/{spec} : max force (eV/A) = {np.max(norms):.05}")
+        elif not opts.silent:
             print(
                 f"Convergence not reached: max force {np.max(norms):.05} eV/A > {tol:.02}."
             )
         return 1
     else:
-        if not opts.silent:
+        if opts.short:
+            print("Converged.")
+        elif not opts.silent:
             print("Convergence reached.")
         return 0
 
 
 @script(
     positional("OUTCAR", default="OUTCAR", type=str, help="VASP output file"),
     flag("--silent", "-q", help="quite mode, just use the return code"),
 )
 def check_end(opts):
     from .outcar import normal_end
 
-    with error_catch(), open(opts.outcar) as f:
-        res = normal_end(f)
+    with error_catch():
+        try:
+            with open(opts.outcar) as f:
+                res = normal_end(f)
+        except OSError:
+            if not opts.silent:
+                print("OUTCAR does not exist.")
+            return 1
 
     if not opts.silent:
         if res:
             print("Computation ended normally.")
         else:
             print("Computation ended early.")
 
@@ -196,15 +221,20 @@
 
     if opts.out is None:
         out = os.path.join(opts.dir, "OUTCAR")
     else:
         out = opts.out
 
     with error_catch():
-        res, tol, residue = converged(osz, out, tol=opts.tol)
+        try:
+            res, tol, residue = converged(osz, out, tol=opts.tol)
+        except OSError:
+            if not opts.silent:
+                print("OUTCAR or OSZICAR does not exist.")
+            return 1
 
     if not opts.silent:
         if res:
             print(f"Computation converged with tolerance {tol}.")
         elif residue is None:
             print("Abnormal ending of the computation.")
         else:
@@ -354,59 +384,83 @@
 
 def quantize(ny, val, max):
     return int(ny * val / max)
 
 
 @script(
     positional("PATH", default=".", help="Computation directory"),
+    flag("--timing", help="show the timing informations"),
 )
 def report(opts):
-    import numpy as np
-    from datetime import datetime, timedelta
-    from .outcar_utils import get_val, get_int, get_float
-    from .outcar import converged
-    from .forces import read_forces
+    pc = PerfCounterCollec()
+
+    with pc.imports:
+        # numpy may be a significant time consumer
+        import numpy as np
+        from datetime import datetime, timedelta
+        from .outcar_utils import get_val, get_int, get_float
+        from .outcar import converged
+        from .forces import read_forces
 
     outcar = os.path.join(opts.path, "OUTCAR")
     oszicar = os.path.join(opts.path, "OSZICAR")
 
-    last_tot = "0.0"
+    last_tot = None
 
-    with open(outcar) as f:
-        date, time = get_val(f, "date").split()
-        ncore = get_int(f, "running on", after="total cores")
-
-        for line in f:
-            if line.startswith("--------------------------------------- Iteration"):
-                break
-
-        for line in f:
-            if "free  energy" in line:  # line.startswith("  free  energy"):
-                last_tot = line
-            elif line.startswith(" total amount of memory"):
-                break
+    with pc.first_pass:
+        with open(outcar) as f:
+            date, time = get_val(f, "date").split()
+            line = next(f)
+
+            if line.startswith(" running on"):
+                # vasp 5
+                ncore = get_int([line], "running on", after="total cores")
+            else:
+                # vasp 6
+                nmpi = get_int([line], "running", after="mpi-ranks")
+                nthreads = get_int([line], "with", after="threads/rank")
+                ncore = nmpi * nthreads
+
+            for line in f:
+                if line.startswith("  free  energy"):
+                    last_tot = line
+                    break
+
+            for line in f:
+                if line.startswith("  free  energy"):
+                    last_tot = line
+                elif line.startswith(" total amount of memory"):
+                    break
 
-        try:
-            elapsed = timedelta(seconds=get_float(f, "Elapsed time (sec):"))
-        except Exception:
-            pass
+            if last_tot is not None:
+                elapsed = timedelta(seconds=get_float(f, "Elapsed time (sec):"))
 
     dt = datetime.fromisoformat(date.replace(".", "-") + " " + time)
     ago = datetime.now() - dt
-    total_energy = float(last_tot.split("=")[1].split()[0].strip())
 
     print("At", time, "on", date, f"({naturaldelta(ago)} ago)")
     print("Running on", ncore, "cores")
 
-    conv, _, _ = converged(oszicar, outcar)
+    if last_tot is None:
+        print("Calculation stopped abnormally.")
+        return
+
+    total_energy = float(last_tot.split("=")[1].split()[0].strip())
+
+    with pc.convergence_check:
+        conv, _, _ = converged(oszicar, outcar)
+
     if conv:
         print(f"Computation converged within {naturaldelta(elapsed)}.")
     else:
         print("Computation did not converge.")
 
-    with error_catch(), open(outcar) as f:
+    with pc.get_forces, error_catch(), open(outcar) as f:
         species, forces, tol = read_forces(f)
 
-    max_f = np.max(np.linalg.norm(forces))
+    max_f = np.max(np.linalg.norm(forces, axis=-1))
 
     print(f"Total energy: {total_energy:0.05f} eV")
     print(f"Maximum residual force: {max_f:0.02e}")
+
+    if opts.timing:
+        print(pc.summary())
```

### Comparing `vbelt-0.6.0/LICENSE` & `vbelt-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vbelt-0.6.0/README.md` & `vbelt-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `vbelt-0.6.0/pyproject.toml` & `vbelt-0.7.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 readme = "README.md"
 license = "EUPL-1.2"
 authors = [
     { name = "Théo Cavignac", email = "theo.cavignac@gmail.com" },
 ]
 classifiers = [
     "Environment :: Console",
-    "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python :: 3.7",
 ]
 dependencies = [
     "numpy >=1.16",
 ]
 
 [project.optional-dependencies]
```

### Comparing `vbelt-0.6.0/PKG-INFO` & `vbelt-0.7.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: vbelt
-Version: 0.6.0
+Version: 0.7.5
 Summary: The VASP user's tool belt.
 Project-URL: Homepage, https://git.sr.ht/~lattay/vbelt
 Author-email: Théo Cavignac <theo.cavignac@gmail.com>
 License-Expression: EUPL-1.2
 License-File: LICENSE
 Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: numpy>=1.16
 Provides-Extra: gencalc
 Requires-Dist: ase>=3.22; extra == 'gencalc'
 Requires-Dist: chevron>=0.14.0; extra == 'gencalc'
 Requires-Dist: tc-pysh>=0.2.0; extra == 'gencalc'
 Provides-Extra: symmetry
```

