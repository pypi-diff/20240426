# Comparing `tmp/grid_data_models-0.1.2.tar.gz` & `tmp/grid_data_models-0.2.0.tar.gz`

## Comparing `grid_data_models-0.1.2.tar` & `grid_data_models-0.2.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/bus.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/capacitor.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/constants.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/exceptions.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/load.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/quantities.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/transformer.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/dataset/__init__.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/dataset/cost_model.py
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/dataset/dataset_system.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/__init__.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/curve.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/distribution_common.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/distribution_enum.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/distribution_graph.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/distribution_system.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/limitset.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/sequence_pair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/__init__.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_branch.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_bus.py
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_capacitor.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_component.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_feeder.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_fuse.py
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_load.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_recloser.py
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_regulator.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_solar.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_substation.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_switch.py
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_transformer.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/distribution_vsource.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/geometry_branch.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/matrix_impedance_branch.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/matrix_impedance_fuse.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/matrix_impedance_recloser.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/matrix_impedance_switch.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/components/sequence_impedance_branch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/controllers/__init__.py
--rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/controllers/distribution_capacitor_controller.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/controllers/distribution_inverter_controller.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/controllers/distribution_recloser_controller.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/controllers/distribution_regulator_controller.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/controllers/distribution_switch_controller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/__init__.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/bare_conductor_equipment.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/capacitor_equipment.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/concentric_cable_equipment.py
--rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/distribution_transformer_equipment.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/geometry_branch_equipment.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/inverter_equipment.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/load_equipment.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/phase_capacitor_equipment.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/phase_load_equipment.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/recloser_controller_equipment.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/distribution/equipment/solar_equipment.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/transmission/transmission_branch.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/transmission/transmission_bus.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/transmission/transmission_capacitor.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/transmission/transmission_component.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/transmission/transmission_load.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/src/gdm/transmission/transmission_substation.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/.gitignore
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/README.md
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 grid_data_models-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/bus.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/capacitor.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/constants.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/exceptions.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/load.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/quantities.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transformer.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/dataset/__init__.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/dataset/cost_model.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/dataset/dataset_system.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/__init__.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/curve.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/distribution_common.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/distribution_enum.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/distribution_graph.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/distribution_system.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/limitset.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/sequence_pair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/__init__.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_branch.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_bus.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_capacitor.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_component.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_feeder.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_fuse.py
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_load.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_recloser.py
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_regulator.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_solar.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_substation.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_switch.py
+-rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_transformer.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/distribution_vsource.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/geometry_branch.py
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_branch.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_fuse.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_recloser.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_switch.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/components/sequence_impedance_branch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/controllers/__init__.py
+-rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_capacitor_controller.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_inverter_controller.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_recloser_controller.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_regulator_controller.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_switch_controller.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/__init__.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/bare_conductor_equipment.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/capacitor_equipment.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/concentric_cable_equipment.py
+-rw-r--r--   0        0        0     8840 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/distribution_transformer_equipment.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/geometry_branch_equipment.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/inverter_equipment.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/load_equipment.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/phase_capacitor_equipment.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/phase_load_equipment.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/recloser_controller_equipment.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/distribution/equipment/solar_equipment.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transmission/transmission_branch.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transmission/transmission_bus.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transmission/transmission_capacitor.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transmission/transmission_component.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transmission/transmission_load.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/src/gdm/transmission/transmission_substation.py
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/README.md
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 grid_data_models-0.2.0/PKG-INFO
```

### Comparing `grid_data_models-0.1.2/src/gdm/__init__.py` & `grid_data_models-0.2.0/src/gdm/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,122 @@
 """ Managing imports for this package."""
 
-from gdm.distribution.components.distribution_substation import DistributionSubstation
-from gdm.distribution.components.distribution_component import DistributionComponent
+from infrasys.quantities import (
+    Current,
+    Distance,
+    Angle,
+    ActivePower,
+    Energy,
+    Time,
+    Resistance,
+)
+from gdm.quantities import (
+    PositiveResistance,
+    ResistancePULength,
+    PositiveResistancePULength,
+    Reactance,
+    ReactancePULength,
+    PositiveReactancePULength,
+    PositiveReactance,
+    Capacitance,
+    CapacitancePULength,
+    PositiveCapacitancePULength,
+    PositiveCapacitance,
+    ReactivePower,
+    PositiveReactivePower,
+    ApparentPower,
+    PositiveApparentPower,
+    PositiveActivePower,
+    PositiveCurrent,
+    PositiveVoltage,
+    PositiveDistance,
+    ActivePowerPUTime,
+    Irradiance,
+)
+
+from gdm.distribution.components.distribution_substation import (
+    DistributionSubstation,
+)
+from gdm.distribution.components.distribution_component import (
+    DistributionComponent,
+)
 from gdm.distribution.components.distribution_feeder import DistributionFeeder
 from gdm.distribution.components.distribution_bus import DistributionBus
 from gdm.distribution.components.distribution_vsource import (
     PhaseVoltageSourceEquipment,
     VoltageSourceEquipment,
     DistributionVoltageSource,
 )
 from gdm.distribution.components.distribution_branch import (
     DistributionBranch,
     SwitchedDistributionBranch,
 )
-from gdm.distribution.components.sequence_impedance_branch import SequenceImpedanceBranch
-from gdm.distribution.components.matrix_impedance_branch import MatrixImpedanceBranch
+from gdm.distribution.components.sequence_impedance_branch import (
+    SequenceImpedanceBranch,
+)
+from gdm.distribution.components.matrix_impedance_branch import (
+    MatrixImpedanceBranch,
+)
 from gdm.distribution.components.geometry_branch import GeometryBranch
 from gdm.distribution.components.distribution_switch import DistributionSwitch
-from gdm.distribution.components.matrix_impedance_switch import MatrixImpedanceSwitch
+from gdm.distribution.components.matrix_impedance_switch import (
+    MatrixImpedanceSwitch,
+)
 from gdm.distribution.components.distribution_fuse import DistributionFuse
-from gdm.distribution.components.matrix_impedance_fuse import MatrixImpedanceFuse
-from gdm.distribution.components.distribution_recloser import DistributionRecloser
-from gdm.distribution.components.matrix_impedance_recloser import MatrixImpedanceRecloser
+from gdm.distribution.components.matrix_impedance_fuse import (
+    MatrixImpedanceFuse,
+)
+from gdm.distribution.components.distribution_recloser import (
+    DistributionRecloser,
+)
+from gdm.distribution.components.matrix_impedance_recloser import (
+    MatrixImpedanceRecloser,
+)
 from gdm.distribution.components.distribution_load import DistributionLoad
 from gdm.distribution.components.distribution_transformer import (
     DistributionTransformer,
 )
-from gdm.distribution.components.distribution_regulator import DistributionRegulator
+from gdm.distribution.components.distribution_regulator import (
+    DistributionRegulator,
+)
 from gdm.distribution.components.distribution_solar import (
     DistributionSolar,
 )
-from gdm.distribution.components.distribution_capacitor import DistributionCapacitor
+from gdm.distribution.components.distribution_capacitor import (
+    DistributionCapacitor,
+)
 
 from gdm.distribution.equipment.matrix_impedance_branch_equipment import (
     MatrixImpedanceBranchEquipment,
 )
-from gdm.distribution.equipment.bare_conductor_equipment import BareConductorEquipment
-from gdm.distribution.equipment.concentric_cable_equipment import ConcentricCableEquipment
-from gdm.distribution.equipment.matrix_impedance_fuse_equipment import MatrixImpedanceFuseEquipment
+from gdm.distribution.equipment.bare_conductor_equipment import (
+    BareConductorEquipment,
+)
+from gdm.distribution.equipment.concentric_cable_equipment import (
+    ConcentricCableEquipment,
+)
+from gdm.distribution.equipment.matrix_impedance_fuse_equipment import (
+    MatrixImpedanceFuseEquipment,
+)
 from gdm.distribution.equipment.matrix_impedance_recloser_equipment import (
     MatrixImpedanceRecloserEquipment,
 )
 from gdm.distribution.equipment.matrix_impedance_switch_equipment import (
     MatrixImpedanceSwitchEquipment,
 )
-from gdm.distribution.equipment.recloser_controller_equipment import RecloserControllerEquipment
-from gdm.distribution.equipment.phase_capacitor_equipment import PhaseCapacitorEquipment
+from gdm.distribution.equipment.recloser_controller_equipment import (
+    RecloserControllerEquipment,
+)
+from gdm.distribution.equipment.phase_capacitor_equipment import (
+    PhaseCapacitorEquipment,
+)
 from gdm.distribution.equipment.capacitor_equipment import CapacitorEquipment
-from gdm.distribution.equipment.geometry_branch_equipment import GeometryBranchEquipment
+from gdm.distribution.equipment.geometry_branch_equipment import (
+    GeometryBranchEquipment,
+)
 from gdm.distribution.equipment.sequence_impedance_branch_equipment import (
     SequenceImpedanceBranchEquipment,
 )
 from gdm.distribution.equipment.phase_load_equipment import PhaseLoadEquipment
 from gdm.distribution.equipment.load_equipment import LoadEquipment
 
 from gdm.distribution.equipment.distribution_transformer_equipment import (
```

### Comparing `grid_data_models-0.1.2/src/gdm/bus.py` & `grid_data_models-0.2.0/src/gdm/bus.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/capacitor.py` & `grid_data_models-0.2.0/src/gdm/capacitor.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/load.py` & `grid_data_models-0.2.0/src/gdm/load.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/quantities.py` & `grid_data_models-0.2.0/src/gdm/quantities.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/version.py` & `grid_data_models-0.2.0/src/gdm/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 import subprocess
 import platform
 import sys
 
-VERSION = "0.1.2"
+VERSION = "0.2.0"
 
 
 def is_git_repo(dir: Path) -> bool:
     """Returns true if it is a git repo."""
     git_path = dir / ".git"
     return git_path.exists()
```

### Comparing `grid_data_models-0.1.2/src/gdm/dataset/cost_model.py` & `grid_data_models-0.2.0/src/gdm/dataset/cost_model.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/dataset/dataset_system.py` & `grid_data_models-0.2.0/src/gdm/dataset/dataset_system.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/curve.py` & `grid_data_models-0.2.0/src/gdm/distribution/curve.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/distribution_enum.py` & `grid_data_models-0.2.0/src/gdm/distribution/distribution_enum.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/distribution_graph.py` & `grid_data_models-0.2.0/src/gdm/distribution/distribution_graph.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/distribution_system.py` & `grid_data_models-0.2.0/src/gdm/distribution/distribution_system.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/limitset.py` & `grid_data_models-0.2.0/src/gdm/distribution/limitset.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/distribution_branch.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_branch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/distribution_bus.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_bus.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/distribution_capacitor.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_capacitor.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/distribution_component.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_component.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/distribution_load.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_load.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/distribution_regulator.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_regulator.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/distribution_solar.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_solar.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/distribution_substation.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_substation.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/distribution_transformer.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_transformer.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/distribution_vsource.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/distribution_vsource.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/geometry_branch.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/geometry_branch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/matrix_impedance_branch.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_branch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/matrix_impedance_fuse.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_fuse.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/matrix_impedance_recloser.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_recloser.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/matrix_impedance_switch.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/matrix_impedance_switch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/components/sequence_impedance_branch.py` & `grid_data_models-0.2.0/src/gdm/distribution/components/sequence_impedance_branch.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/controllers/distribution_capacitor_controller.py` & `grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_capacitor_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/controllers/distribution_inverter_controller.py` & `grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_inverter_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/controllers/distribution_recloser_controller.py` & `grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_recloser_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/controllers/distribution_regulator_controller.py` & `grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_regulator_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/controllers/distribution_switch_controller.py` & `grid_data_models-0.2.0/src/gdm/distribution/controllers/distribution_switch_controller.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/bare_conductor_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/bare_conductor_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/capacitor_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/capacitor_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/concentric_cable_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/concentric_cable_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/distribution_transformer_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/distribution_transformer_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/geometry_branch_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/geometry_branch_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/inverter_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/inverter_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/load_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/load_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_branch_equipment.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 from typing import Annotated, Optional
 
 from infrasys import Component
 from pydantic import Field, model_validator
 
 from gdm.quantities import (
-    PositiveResistancePULength,
+    ResistancePULength,
     ReactancePULength,
     CapacitancePULength,
     PositiveCurrent,
 )
 from gdm.distribution.limitset import ThermalLimitSet
 from gdm.constants import PINT_SCHEMA
 
 
 class MatrixImpedanceBranchEquipment(Component):
     """Interface for impedance based branch."""
 
     r_matrix: Annotated[
-        PositiveResistancePULength,
+        ResistancePULength,
         PINT_SCHEMA,
         Field(..., description="Per unit length resistance matrix."),
     ]
     x_matrix: Annotated[
         ReactancePULength,
         PINT_SCHEMA,
         Field(..., description="Per unit length reactance matrix."),
@@ -51,12 +51,12 @@
         raise ValueError(msg)
 
     @classmethod
     def example(cls) -> "MatrixImpedanceBranchEquipment":
         """Example for matrix impedance model."""
         return MatrixImpedanceBranchEquipment(
             name="matrix-impedance-branch-1",
-            r_matrix=PositiveResistancePULength([[1, 2, 3] for _ in range(3)], "ohm/mi"),
+            r_matrix=ResistancePULength([[1, 2, 3] for _ in range(3)], "ohm/mi"),
             x_matrix=ReactancePULength([[1, 2, 3] for _ in range(3)], "ohm/mi"),
             c_matrix=CapacitancePULength([[1, 2, 3] for _ in range(3)], "farad/mi"),
             ampacity=PositiveCurrent(90, "ampere"),
         )
```

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_fuse_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_recloser_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/matrix_impedance_switch_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/phase_capacitor_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/phase_capacitor_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/phase_load_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/phase_load_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/sequence_impedance_branch_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/src/gdm/distribution/equipment/solar_equipment.py` & `grid_data_models-0.2.0/src/gdm/distribution/equipment/solar_equipment.py`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/.gitignore` & `grid_data_models-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/LICENSE.txt` & `grid_data_models-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/README.md` & `grid_data_models-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `grid_data_models-0.1.2/pyproject.toml` & `grid_data_models-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   { name = "Tarek Elgindy", email = "tarek.elgindy@nrel.gov" },
 ]
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
 ]
-dependencies = ["networkx", "infrasys"]
+dependencies = ["networkx", "infrasys", "importlib_metadata"]
 
 [project.optional-dependencies]
 dev = ["pre-commit", "pytest", "pytest-cov", "ruff"]
 doc = [
   "sphinx",
   "pydata-sphinx-theme",
   "myst-parser",
```

### Comparing `grid_data_models-0.1.2/PKG-INFO` & `grid_data_models-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.3
 Name: grid-data-models
-Version: 0.1.2
+Version: 0.2.0
 Project-URL: Documentation, https://github.com/NREL-Distribution-Suites/grid-data-models#readme
 Project-URL: Issues, https://github.com/NREL-Distribution-Suites/grid-data-models/issues
 Project-URL: Source, https://github.com/NREL-Distribution-Suites/grid-data-models
 Author-email: Kapil Duwadi <Kapil.Duwadi@nrel.gov>, Aadil Latif <Aadil.Latif@nrel.gov>, Tarek Elgindy <tarek.elgindy@nrel.gov>
 License-Expression: BSD-3-Clause
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
+Requires-Dist: importlib-metadata
 Requires-Dist: infrasys
 Requires-Dist: networkx
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
```

