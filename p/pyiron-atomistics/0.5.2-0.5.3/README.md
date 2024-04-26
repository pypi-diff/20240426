# Comparing `tmp/pyiron_atomistics-0.5.2.tar.gz` & `tmp/pyiron_atomistics-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_atomistics-0.5.2.tar", last modified: Wed Apr 17 21:03:05 2024, max compression
+gzip compressed data, was "pyiron_atomistics-0.5.3.tar", last modified: Fri Apr 26 15:54:44 2024, max compression
```

## Comparing `pyiron_atomistics-0.5.2.tar` & `pyiron_atomistics-0.5.3.tar`

### file list

```diff
@@ -1,155 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.435037 pyiron_atomistics-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-04-17 21:03:05.435037 pyiron_atomistics-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.415037 pyiron_atomistics-0.5.2/pyiron_atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-17 21:03:05.435037 pyiron_atomistics-0.5.2/pyiron_atomistics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.415037 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.415037 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/generic/object_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.415037 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42892 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/atomistic.py
--rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/potentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/structurecontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.419036 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23340 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/elasticmatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/murnaghan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    20634 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/quasi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/sqsmaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.419036 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16778 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/analyse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)   121522 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/atoms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.423037 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factories/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factories/atomsk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factories/compound.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factories/materialsproject.py
--rw-r--r--   0 runner    (1001) docker     (127)    20585 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/has_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (127)    17732 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/pyironase.py
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/pyxtal.py
--rw-r--r--   0 runner    (1001) docker     (127)    22356 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/structurestorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.423037 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.423037 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/volumetric/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/volumetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17033 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/volumetric/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.423037 pyiron_atomistics-0.5.2/pyiron_atomistics/calphy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/calphy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35702 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/calphy/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.423037 pyiron_atomistics-0.5.2/pyiron_atomistics/data/
--rw-r--r--   0 runner    (1001) docker     (127)    15648 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/data/periodic_table.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.423037 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/bader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.423037 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18571 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/job/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.423037 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/master/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/master/convergence_encut_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/master/murnaghan_dft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.423037 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/waves/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/waves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/waves/bandstructure.py
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/waves/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30140 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/dft/waves/electronic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.427037 pyiron_atomistics-0.5.2/pyiron_atomistics/gpaw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/gpaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/gpaw/gpaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/gpaw/pyiron_ase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.427037 pyiron_atomistics-0.5.2/pyiron_atomistics/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/interactive/activation_relaxation_technique.py
--rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/interactive/quasi_newton.py
--rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/interactive/scipy_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/interactive/sxextoptint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.427037 pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41067 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    41928 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/control.py
--rw-r--r--   0 runner    (1001) docker     (127)    24686 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/lammps.py
--rw-r--r--   0 runner    (1001) docker     (127)    18735 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)    25569 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    30388 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.431037 pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83187 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/input_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    16340 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.431037 pyiron_atomistics-0.5.2/pyiron_atomistics/table/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/table/datamining.py
--rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/table/funct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.431037 pyiron_atomistics-0.5.2/pyiron_atomistics/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/testing/executable.py
--rw-r--r--   0 runner    (1001) docker     (127)    19297 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/testing/randomatomistic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.431037 pyiron_atomistics-0.5.2/pyiron_atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/thermodynamics/hessian.py
--rw-r--r--   0 runner    (1001) docker     (127)    51126 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/thermodynamics/interfacemethod.py
--rw-r--r--   0 runner    (1001) docker     (127)    18302 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/thermodynamics/sxphonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.435037 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   105588 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/metadyn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.435037 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/parser/oszicar.py
--rw-r--r--   0 runner    (1001) docker     (127)    45802 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/parser/outcar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/parser/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    18752 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/potential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/procar.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    34572 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/vasprun.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/vaspsol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.435037 pyiron_atomistics-0.5.2/pyiron_atomistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9343 2024-04-17 21:03:05.000000 pyiron_atomistics-0.5.2/pyiron_atomistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-17 21:03:05.000000 pyiron_atomistics-0.5.2/pyiron_atomistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 21:03:05.000000 pyiron_atomistics-0.5.2/pyiron_atomistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-17 21:03:05.000000 pyiron_atomistics-0.5.2/pyiron_atomistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 21:03:05.000000 pyiron_atomistics-0.5.2/pyiron_atomistics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-17 21:03:01.000000 pyiron_atomistics-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 21:03:05.435037 pyiron_atomistics-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:03:05.435037 pyiron_atomistics-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-17 21:01:06.000000 pyiron_atomistics-0.5.2/tests/test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.799926 pyiron_atomistics-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-26 15:54:44.799926 pyiron_atomistics-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.775926 pyiron_atomistics-0.5.3/pyiron_atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-26 15:54:44.799926 pyiron_atomistics-0.5.3/pyiron_atomistics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.775926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.775926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/generic/object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.779926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42892 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/atomistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12263 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/structurecontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.779926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/elasticmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17739 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/murnaghan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20634 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/quasi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/sqsmaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7400 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16778 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121522 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/atomsk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/compound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/materialsproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20585 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/has_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17732 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/pyironase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/pyxtal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22356 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/structurestorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/volumetric/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/volumetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17033 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/volumetric/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/calphy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/calphy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35702 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/calphy/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    15648 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/data/periodic_table.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/bader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.783926 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18571 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/job/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.787926 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/convergence_encut_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/murnaghan_dft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.787926 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/bandstructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30140 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/electronic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.787926 pyiron_atomistics-0.5.3/pyiron_atomistics/gpaw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/gpaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/gpaw/gpaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/gpaw/pyiron_ase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.787926 pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/activation_relaxation_technique.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15278 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/quasi_newton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/scipy_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/sxextoptint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.791926 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41067 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41928 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24686 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18735 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25569 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30388 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.791926 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83168 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/input_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15908 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16340 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.791926 pyiron_atomistics-0.5.3/pyiron_atomistics/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/table/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9063 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/table/funct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.791926 pyiron_atomistics-0.5.3/pyiron_atomistics/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/testing/executable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19297 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/testing/randomatomistic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.795926 pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51126 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/interfacemethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18302 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/sxphonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.795926 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106070 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/metadyn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.795926 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/oszicar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45802 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/outcar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18828 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/procar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34572 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/vasprun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/vaspsol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.795926 pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-26 15:54:44.000000 pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-26 15:54:44.000000 pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:54:44.000000 pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-26 15:54:44.000000 pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 15:54:44.000000 pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-26 15:54:39.000000 pyiron_atomistics-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:54:44.799926 pyiron_atomistics-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:54:44.795926 pyiron_atomistics-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-26 15:52:40.000000 pyiron_atomistics-0.5.3/tests/test_toolkit.py
```

### Comparing `pyiron_atomistics-0.5.2/LICENSE` & `pyiron_atomistics-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/PKG-INFO` & `pyiron_atomistics-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_atomistics
-Version: 0.5.2
+Version: 0.5.3
 Summary: An interface to atomistic simulation codes including but not limited to GPAW, LAMMPS, S/Phi/nX and VASP.
 Author-email: "Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department" <pyiron@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -46,26 +46,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: ase==3.22.1
-Requires-Dist: atomistics<=0.1.26,>=0.1.12
+Requires-Dist: atomistics==0.1.27
 Requires-Dist: defusedxml<=0.7.1,>=0.7.0
 Requires-Dist: h5py<=3.11.0,>=3.9.0
 Requires-Dist: matplotlib<=3.8.4,>=3.5.3
 Requires-Dist: mendeleev<=0.15.0,>=0.12.0
 Requires-Dist: mp-api<=0.41.2,>=0.37.0
 Requires-Dist: numpy<=1.26.4,>=1.26.0
 Requires-Dist: pandas<=2.2.2,>=2.0.3
 Requires-Dist: phonopy<=2.22.1,>=2.20.0
 Requires-Dist: pint<=0.23,>=0.18
 Requires-Dist: pyiron_base<=0.8.2,>=0.7.7
-Requires-Dist: pylammpsmpi<=0.2.15,>=0.2.7
+Requires-Dist: pylammpsmpi<=0.2.18,>=0.2.7
 Requires-Dist: scipy<=1.13.0,>=1.11.1
 Requires-Dist: scikit-learn<=1.4.2,>=1.2.1
 Requires-Dist: seekpath<=2.1.0,>=1.9.5
 Requires-Dist: spglib<=2.4.0,>=2.0.2
 Requires-Dist: structuretoolkit<=0.0.22,>=0.0.19
 
 pyiron
```

### Comparing `pyiron_atomistics-0.5.2/README.rst` & `pyiron_atomistics-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/__init__.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 JOB_CLASS_DICT.update(
     {
         "ART": "pyiron_atomistics.interactive.activation_relaxation_technique",
         "AtomisticExampleJob": "pyiron_atomistics.testing.randomatomistic",
         "Calphy": "pyiron_atomistics.calphy.job",
         "ConvEncutParallel": "pyiron_atomistics.dft.master.convergence_encut_parallel",
         "ConvKpointParallel": "pyiron_atomistics.dft.master.convergence_kpoint_parallel",
-        "ElasticTensor": "pyiron_atomistics.atomistics.master.elastic",
         "ElasticMatrixJob": "pyiron_atomistics.atomistics.master.elasticmatrix",
         "ExampleJob": "pyiron_atomistics.testing.randomatomistic",
         "Gpaw": "pyiron_atomistics.gpaw.gpaw",
         "HessianJob": "pyiron_atomistics.thermodynamics.hessian",
         "Lammps": "pyiron_atomistics.lammps.lammps",
         "MapMaster": "pyiron_atomistics.atomistics.master.parallel",
         "Murnaghan": "pyiron_atomistics.atomistics.master.murnaghan",
```

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/_tests.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/_tests.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/generic/object_type.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/generic/object_type.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/atomistic.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/atomistic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/interactive.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/interactivewrapper.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/potentials.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/potentials.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/sqs.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/sqs.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/job/structurecontainer.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/job/structurecontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/elasticmatrix.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/elasticmatrix.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/murnaghan.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/murnaghan.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from atomistics.workflows.evcurve.debye import DebyeModel
 from atomistics.workflows.evcurve.fit import (
     EnergyVolumeFit,
     fitfunction,
     get_error,
     fit_leastsq_eos,
 )
-from atomistics.workflows.evcurve.workflow import _strain_axes
+from atomistics.workflows.evcurve.helper import _strain_axes
 import matplotlib.pyplot as plt
 import numpy as np
 
 from pyiron_atomistics.atomistics.master.parallel import AtomisticParallelMaster
 from pyiron_atomistics.atomistics.structure.atoms import Atoms, ase_to_pyiron
 from pyiron_base import JobGenerator
```

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/parallel.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/phonopy.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/phonopy.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/quasi.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/quasi.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/sqsmaster.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/sqsmaster.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/master/structure.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/master/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/analyse.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/analyse.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/atom.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/atom.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/atoms.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/atoms.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factories/aimsgb.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/aimsgb.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factories/ase.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/ase.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factories/atomsk.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/atomsk.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factories/compound.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/compound.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factories/materialsproject.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factories/materialsproject.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/factory.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/has_structure.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/has_structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/neighbors.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/neighbors.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/periodic_table.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/periodic_table.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/phonopy.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/phonopy.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/pyironase.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/pyironase.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/pyscal.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/pyscal.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/pyxtal.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/pyxtal.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/structure/structurestorage.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/structure/structurestorage.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/atomistics/volumetric/generic.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/atomistics/volumetric/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/calphy/job.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/calphy/job.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/data/periodic_table.csv` & `pyiron_atomistics-0.5.3/pyiron_atomistics/data/periodic_table.csv`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/dft/bader.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/bader.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/dft/job/generic.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/job/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/dft/master/convergence_encut_parallel.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/convergence_encut_parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/dft/master/murnaghan_dft.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/master/murnaghan_dft.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/dft/waves/bandstructure.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/bandstructure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/dft/waves/dos.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/dos.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/dft/waves/electronic.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/dft/waves/electronic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/gpaw/gpaw.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/gpaw/gpaw.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/gpaw/pyiron_ase.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/gpaw/pyiron_ase.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/interactive/activation_relaxation_technique.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/activation_relaxation_technique.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/interactive/quasi_newton.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/quasi_newton.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/interactive/scipy_minimizer.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/scipy_minimizer.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/interactive/sxextoptint.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/interactive/sxextoptint.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/base.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/base.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/control.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/control.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/interactive.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/lammps.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/lammps.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/output.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/output.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/potential.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/structure.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/lammps/units.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/lammps/units.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/project.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/project.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/base.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,29 +167,29 @@
                 element_lst=structure.get_species_symbols().tolist()
             )
 
     @property
     def id_pyi_to_spx(self):
         if self.structure is None:
             raise ValueError("Structure not set")
-        return np.argsort(self.structure.get_chemical_symbols())
-
-    @property
-    def id_spx_to_pyi(self):
-        if self.structure is None:
-            raise ValueError("Structure not set")
         # Translate the chemical symbols into indices
         indices = np.unique(self.structure.get_chemical_symbols(), return_inverse=True)[
             1
         ]
         # Add small ramp to ensure order uniqueness
         indices = indices + np.arange(len(indices)) / len(indices)
         return np.argsort(indices)
 
     @property
+    def id_spx_to_pyi(self):
+        if self.structure is None:
+            raise ValueError("Structure not set")
+        return np.argsort(self.id_pyi_to_spx)
+
+    @property
     def plane_wave_cutoff(self):
         if "eCut" in self.input.sphinx.basis.keys():
             return self.input.sphinx.basis["eCut"] * RYDBERG_TO_EV
         else:
             return self.input["EnCut"]
 
     @property
```

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/input_writer.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/input_writer.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/interactive.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/output_parser.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/output_parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/potential.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/sphinx.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/sphinx.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/structure.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/util.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/sphinx/volumetric_data.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/sphinx/volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/table/datamining.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/table/datamining.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/table/funct.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/table/funct.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/testing/executable.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/testing/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/testing/randomatomistic.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/testing/randomatomistic.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/thermodynamics/hessian.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/hessian.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/thermodynamics/interfacemethod.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/interfacemethod.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/thermodynamics/sxphonons.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/thermodynamics/sxphonons.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/toolkit.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/base.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,18 +130,15 @@
         Args:
             structure:
 
         Returns:
 
         """
         GenericDFTJob.structure.fset(self, structure)
-        if structure is not None:
-            self._potential = VaspPotentialSetter(
-                element_lst=structure.get_species_symbols().tolist()
-            )
+        self._reinit_potential_setter(structure=structure)
 
     @property
     def potential(self):
         return self._potential
 
     @property
     def plane_wave_cutoff(self):
@@ -768,20 +765,25 @@
             else:
                 f.write("LABORT =.TRUE.\n")
 
     def to_dict(self):
         job_dict = super().to_dict()
         job_dict.update({"input/" + k: v for k, v in self._structure_to_dict().items()})
         job_dict.update({"input/" + k: v for k, v in self.input.to_dict().items()})
+        job_dict["input/potential_dict"] = self._potential.to_dict()
         return job_dict
 
     def from_dict(self, job_dict):
         super().from_dict(job_dict=job_dict)
         self._structure_from_dict(job_dict=job_dict)
         self.input.from_dict(input_dict=job_dict["input"])
+        if "potential_dict" in job_dict["input"].keys():
+            self._potential.from_dict(
+                potential_dict=job_dict["input"]["potential_dict"]
+            )
 
     def to_hdf(self, hdf=None, group_name=None):
         """
         Stores the instance attributes into the hdf5 file
 
         Args:
             hdf (pyiron_base.generic.hdfio.ProjectHDFio): The HDF file/path to write the data to
@@ -1157,125 +1159,14 @@
         if retain_charge_density:
             self.write_charge_density = retain_charge_density
         if retain_electrostatic_potential:
             self.write_electrostatic_potential = retain_electrostatic_potential
         for key in kwargs.keys():
             self.logger.warning("Tag {} not relevant for vasp".format(key))
 
-    def _set_kpoints(
-        self,
-        mesh=None,
-        scheme="MP",
-        center_shift=None,
-        symmetry_reduction=True,
-        manual_kpoints=None,
-        weights=None,
-        reciprocal=True,
-        n_path=None,
-        path_name=None,
-    ):
-        """
-        Function to setup the k-points for the VASP job
-
-        Args:
-            mesh (list): Size of the mesh (in the MP scheme)
-            scheme (str): Type of k-point generation scheme (MP/GC(gamma centered)/GP(gamma point)/Manual/Line)
-            center_shift (list): Shifts the center of the mesh from the gamma point by the given vector
-            symmetry_reduction (boolean): Tells if the symmetry reduction is to be applied to the k-points
-            manual_kpoints (list/numpy.ndarray): Manual list of k-points
-            weights(list/numpy.ndarray): Manually supplied weights to each k-point in case of the manual mode
-            reciprocal (bool): Tells if the supplied values are in reciprocal (direct) or cartesian coordinates (in
-            reciprocal space)
-            n_path (int): Number of points per trace part for line mode
-            path_name (str): Name of high symmetry path used for band structure calculations.
-        """
-        if not symmetry_reduction:
-            self.input.incar["ISYM"] = -1
-        scheme_list = ["MP", "GC", "GP", "Line", "Manual"]
-        if not (scheme in scheme_list):
-            raise AssertionError()
-        if scheme == "MP":
-            if mesh is None:
-                mesh = [int(val) for val in self.input.kpoints[3].split()]
-            self.input.kpoints.set_kpoints_file(size_of_mesh=mesh, shift=center_shift)
-        if scheme == "GC":
-            if mesh is None:
-                mesh = [int(val) for val in self.input.kpoints[3].split()]
-            self.input.kpoints.set_kpoints_file(
-                size_of_mesh=mesh, shift=center_shift, method="Gamma centered"
-            )
-        if scheme == "GP":
-            self.input.kpoints.set_kpoints_file(
-                size_of_mesh=[1, 1, 1], method="Gamma Point"
-            )
-        if scheme == "Line":
-            if n_path is None and self.input.kpoints._n_path is None:
-                raise ValueError("n_path has to be defined")
-            high_symmetry_points = self.structure.get_high_symmetry_points()
-            if high_symmetry_points is None:
-                raise ValueError("high_symmetry_points has to be defined")
-
-            if path_name is None and self.input.kpoints._path_name is None:
-                raise ValueError("path_name has to be defined")
-            if path_name not in self.structure.get_high_symmetry_path().keys():
-                raise ValueError("path_name is not a valid key of high_symmetry_path")
-
-            if path_name is not None:
-                self.input.kpoints._path_name = path_name
-            if n_path is not None:
-                self.input.kpoints._n_path = n_path
-
-            self.input.kpoints.set_kpoints_file(
-                method="Line",
-                n_path=self.input.kpoints._n_path,
-                path=self._get_path_for_kpoints(self.input.kpoints._path_name),
-            )
-        if scheme == "Manual":
-            if manual_kpoints is None:
-                raise ValueError(
-                    "For the manual mode, the kpoints list should be specified"
-                )
-            else:
-                if weights is not None:
-                    if not (len(manual_kpoints) == len(weights)):
-                        raise AssertionError()
-                self.input.kpoints.set_value(line=1, val=str(len(manual_kpoints)))
-                if reciprocal:
-                    self.input.kpoints.set_value(line=2, val="Reciprocal")
-                else:
-                    self.input.kpoints.set_value(line=2, val="Cartesian")
-                for i, kpt in enumerate(manual_kpoints):
-                    if weights is not None:
-                        wt = weights[i]
-                    else:
-                        wt = 1.0
-                    self.input.kpoints.set_value(
-                        line=3 + i,
-                        val=" ".join([str(kpt[0]), str(kpt[1]), str(kpt[2]), str(wt)]),
-                    )
-
-    def _get_path_for_kpoints(self, path_name):
-        """
-        gets the trace for k-points line mode in a VASP readable form.
-
-        Args:
-            path_name (str): Name of the path used for band structure calculation from structure instance.
-
-        Returns:
-            list: list of tuples of position and path name
-        """
-        path = self.structure.get_high_symmetry_path()[path_name]
-
-        k_trace = []
-        for t in path:
-            k_trace.append((self.structure.get_high_symmetry_points()[t[0]], t[0]))
-            k_trace.append((self.structure.get_high_symmetry_points()[t[1]], t[1]))
-
-        return k_trace
-
     def set_for_band_structure_calc(
         self, num_points, structure=None, read_charge_density=True
     ):
         """
         Sets up the input for a non self-consistent bandstructure calculation
 
         Args:
@@ -1852,14 +1743,135 @@
         Lists all the possible POTCAR files for the elements in the structure depending on the XC functional
 
         Returns:
            list: a list of available potentials
         """
         return self.potential_list
 
+    def _set_kpoints(
+        self,
+        mesh=None,
+        scheme="MP",
+        center_shift=None,
+        symmetry_reduction=True,
+        manual_kpoints=None,
+        weights=None,
+        reciprocal=True,
+        n_path=None,
+        path_name=None,
+    ):
+        """
+        Function to setup the k-points for the VASP job
+
+        Args:
+            mesh (list): Size of the mesh (in the MP scheme)
+            scheme (str): Type of k-point generation scheme (MP/GC(gamma centered)/GP(gamma point)/Manual/Line)
+            center_shift (list): Shifts the center of the mesh from the gamma point by the given vector
+            symmetry_reduction (boolean): Tells if the symmetry reduction is to be applied to the k-points
+            manual_kpoints (list/numpy.ndarray): Manual list of k-points
+            weights(list/numpy.ndarray): Manually supplied weights to each k-point in case of the manual mode
+            reciprocal (bool): Tells if the supplied values are in reciprocal (direct) or cartesian coordinates (in
+            reciprocal space)
+            n_path (int): Number of points per trace part for line mode
+            path_name (str): Name of high symmetry path used for band structure calculations.
+        """
+        if not symmetry_reduction:
+            self.input.incar["ISYM"] = -1
+        scheme_list = ["MP", "GC", "GP", "Line", "Manual"]
+        if not (scheme in scheme_list):
+            raise AssertionError()
+        if scheme == "MP":
+            if mesh is None:
+                mesh = [int(val) for val in self.input.kpoints[3].split()]
+            self.input.kpoints.set_kpoints_file(size_of_mesh=mesh, shift=center_shift)
+        if scheme == "GC":
+            if mesh is None:
+                mesh = [int(val) for val in self.input.kpoints[3].split()]
+            self.input.kpoints.set_kpoints_file(
+                size_of_mesh=mesh, shift=center_shift, method="Gamma centered"
+            )
+        if scheme == "GP":
+            self.input.kpoints.set_kpoints_file(
+                size_of_mesh=[1, 1, 1], method="Gamma Point"
+            )
+        if scheme == "Line":
+            if n_path is None and self.input.kpoints._n_path is None:
+                raise ValueError("n_path has to be defined")
+            high_symmetry_points = self.structure.get_high_symmetry_points()
+            if high_symmetry_points is None:
+                raise ValueError("high_symmetry_points has to be defined")
+
+            if path_name is None and self.input.kpoints._path_name is None:
+                raise ValueError("path_name has to be defined")
+            if path_name not in self.structure.get_high_symmetry_path().keys():
+                raise ValueError("path_name is not a valid key of high_symmetry_path")
+
+            if path_name is not None:
+                self.input.kpoints._path_name = path_name
+            if n_path is not None:
+                self.input.kpoints._n_path = n_path
+
+            self.input.kpoints.set_kpoints_file(
+                method="Line",
+                n_path=self.input.kpoints._n_path,
+                path=self._get_path_for_kpoints(self.input.kpoints._path_name),
+            )
+        if scheme == "Manual":
+            if manual_kpoints is None:
+                raise ValueError(
+                    "For the manual mode, the kpoints list should be specified"
+                )
+            else:
+                if weights is not None:
+                    if not (len(manual_kpoints) == len(weights)):
+                        raise AssertionError()
+                self.input.kpoints.set_value(line=1, val=str(len(manual_kpoints)))
+                if reciprocal:
+                    self.input.kpoints.set_value(line=2, val="Reciprocal")
+                else:
+                    self.input.kpoints.set_value(line=2, val="Cartesian")
+                for i, kpt in enumerate(manual_kpoints):
+                    if weights is not None:
+                        wt = weights[i]
+                    else:
+                        wt = 1.0
+                    self.input.kpoints.set_value(
+                        line=3 + i,
+                        val=" ".join([str(kpt[0]), str(kpt[1]), str(kpt[2]), str(wt)]),
+                    )
+
+    def _reinit_potential_setter(self, structure):
+        if structure is not None:
+            self._potential.to_dict().update(
+                {
+                    el: None
+                    for el in set(structure.get_chemical_symbols())
+                    if el not in self._potential.to_dict().keys()
+                }
+            )
+
+    def _get_path_for_kpoints(self, path_name):
+        """
+        gets the trace for k-points line mode in a VASP readable form.
+
+        Args:
+            path_name (str): Name of the path used for band structure calculation from structure instance.
+
+        Returns:
+            list: list of tuples of position and path name
+        """
+        path = self.structure.get_high_symmetry_path()[path_name]
+
+        k_trace = []
+        for t in path:
+            k_trace.append((self.structure.get_high_symmetry_points()[t[0]], t[0]))
+            k_trace.append((self.structure.get_high_symmetry_points()[t[1]], t[1]))
+
+        return k_trace
+
     def __del__(self):
         pass
 
 
 class Input:
     """
     Handles setting the input parameters for a VASP job.
```

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/interactive.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,15 @@
     @property
     def structure(self):
         return GenericInteractive.structure.fget(self)
 
     @structure.setter
     def structure(self, structure):
         GenericInteractive.structure.fset(self, structure)
-        if structure is not None:
-            self._potential = VaspPotentialSetter(
-                element_lst=structure.get_species_symbols().tolist()
-            )
+        self._reinit_potential_setter(structure=structure)
 
     @property
     def interactive_enforce_structure_reset(self):
         return self._interactive_enforce_structure_reset
 
     @interactive_enforce_structure_reset.setter
     def interactive_enforce_structure_reset(self, reset):
```

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/metadyn.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/metadyn.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/parser/oszicar.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/oszicar.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/parser/outcar.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/outcar.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/parser/report.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/parser/report.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/potential.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,37 +236,40 @@
     def __init__(self, selected_atoms=None):
         self.pbe = VaspPotentialFile(xc="PBE", selected_atoms=selected_atoms)
         self.lda = VaspPotentialFile(xc="LDA", selected_atoms=selected_atoms)
 
 
 class VaspPotentialSetter(object):
     def __init__(self, element_lst):
-        super(VaspPotentialSetter, self).__setattr__("_element_lst", element_lst)
         super(VaspPotentialSetter, self).__setattr__(
             "_potential_dict", {el: None for el in element_lst}
         )
 
     def __getattr__(self, item):
-        if item in self._element_lst:
+        if item in self._potential_dict.keys():
             return item
         else:
             raise AttributeError
 
     def __setitem__(self, key, value):
         self.__setattr__(key=key, value=value)
 
     def __setattr__(self, key, value):
-        if key in self._element_lst:
+        if key in self._potential_dict.keys():
             self._potential_dict[key] = value
         else:
             raise AttributeError
 
     def to_dict(self):
         return self._potential_dict
 
+    def from_dict(self, potential_dict):
+        for key, value in potential_dict.items():
+            self._potential_dict[key] = value
+
     def __repr__(self):
         return self._potential_dict.__repr__()
 
 
 def find_potential_file(path):
     return find_potential_file_base(
         path=path,
```

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/procar.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/procar.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/structure.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/vasp.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/vasprun.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/vasprun.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/vaspsol.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/vaspsol.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics/vasp/volumetric_data.py` & `pyiron_atomistics-0.5.3/pyiron_atomistics/vasp/volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics.egg-info/PKG-INFO` & `pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_atomistics
-Version: 0.5.2
+Version: 0.5.3
 Summary: An interface to atomistic simulation codes including but not limited to GPAW, LAMMPS, S/Phi/nX and VASP.
 Author-email: "Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department" <pyiron@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -46,26 +46,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: ase==3.22.1
-Requires-Dist: atomistics<=0.1.26,>=0.1.12
+Requires-Dist: atomistics==0.1.27
 Requires-Dist: defusedxml<=0.7.1,>=0.7.0
 Requires-Dist: h5py<=3.11.0,>=3.9.0
 Requires-Dist: matplotlib<=3.8.4,>=3.5.3
 Requires-Dist: mendeleev<=0.15.0,>=0.12.0
 Requires-Dist: mp-api<=0.41.2,>=0.37.0
 Requires-Dist: numpy<=1.26.4,>=1.26.0
 Requires-Dist: pandas<=2.2.2,>=2.0.3
 Requires-Dist: phonopy<=2.22.1,>=2.20.0
 Requires-Dist: pint<=0.23,>=0.18
 Requires-Dist: pyiron_base<=0.8.2,>=0.7.7
-Requires-Dist: pylammpsmpi<=0.2.15,>=0.2.7
+Requires-Dist: pylammpsmpi<=0.2.18,>=0.2.7
 Requires-Dist: scipy<=1.13.0,>=1.11.1
 Requires-Dist: scikit-learn<=1.4.2,>=1.2.1
 Requires-Dist: seekpath<=2.1.0,>=1.9.5
 Requires-Dist: spglib<=2.4.0,>=2.0.2
 Requires-Dist: structuretoolkit<=0.0.22,>=0.0.19
 
 pyiron
```

### Comparing `pyiron_atomistics-0.5.2/pyiron_atomistics.egg-info/SOURCES.txt` & `pyiron_atomistics-0.5.3/pyiron_atomistics.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 pyiron_atomistics/atomistics/job/atomistic.py
 pyiron_atomistics/atomistics/job/interactive.py
 pyiron_atomistics/atomistics/job/interactivewrapper.py
 pyiron_atomistics/atomistics/job/potentials.py
 pyiron_atomistics/atomistics/job/sqs.py
 pyiron_atomistics/atomistics/job/structurecontainer.py
 pyiron_atomistics/atomistics/master/__init__.py
-pyiron_atomistics/atomistics/master/elastic.py
 pyiron_atomistics/atomistics/master/elasticmatrix.py
 pyiron_atomistics/atomistics/master/murnaghan.py
 pyiron_atomistics/atomistics/master/parallel.py
 pyiron_atomistics/atomistics/master/phonopy.py
 pyiron_atomistics/atomistics/master/quasi.py
 pyiron_atomistics/atomistics/master/sqsmaster.py
 pyiron_atomistics/atomistics/master/structure.py
```

### Comparing `pyiron_atomistics-0.5.2/pyproject.toml` & `pyiron_atomistics-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,26 +21,26 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "ase==3.22.1",
-    "atomistics>=0.1.12,<=0.1.26",
+    "atomistics==0.1.27",
     "defusedxml>=0.7.0,<=0.7.1",
     "h5py>=3.9.0,<=3.11.0",
     "matplotlib>=3.5.3,<=3.8.4",
     "mendeleev>=0.12.0,<=0.15.0",
     "mp-api>=0.37.0,<=0.41.2",
     "numpy>=1.26.0,<=1.26.4",
     "pandas>=2.0.3,<=2.2.2",
     "phonopy>=2.20.0,<=2.22.1",
     "pint>=0.18,<=0.23",
     "pyiron_base>=0.7.7,<=0.8.2",
-    "pylammpsmpi>=0.2.7,<=0.2.15",
+    "pylammpsmpi>=0.2.7,<=0.2.18",
     "scipy>=1.11.1,<=1.13.0",
     "scikit-learn>=1.2.1,<=1.4.2",
     "seekpath>=1.9.5,<=2.1.0",
     "spglib>=2.0.2,<=2.4.0",
     "structuretoolkit>=0.0.19,<=0.0.22",
 ]
 dynamic = ["version"]
```

### Comparing `pyiron_atomistics-0.5.2/tests/test_project.py` & `pyiron_atomistics-0.5.3/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pyiron_atomistics-0.5.2/tests/test_toolkit.py` & `pyiron_atomistics-0.5.3/tests/test_toolkit.py`

 * *Files identical despite different names*

