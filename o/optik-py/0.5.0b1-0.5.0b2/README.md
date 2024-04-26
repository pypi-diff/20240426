# Comparing `tmp/optik_py-0.5.0b1.tar.gz` & `tmp/optik_py-0.5.0b2.tar.gz`

## Comparing `optik_py-0.5.0b1.tar` & `optik_py-0.5.0b2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0     1001      127      688 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/Cargo.toml
--rw-r--r--   0     1001      127     2047 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/benches/bench.rs
--rw-r--r--   0     1001      127     1507 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/src/config.rs
--rw-r--r--   0     1001      127    10434 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/src/kinematics.rs
--rw-r--r--   0     1001      127    10583 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/src/lib.rs
--rw-r--r--   0     1001      127     6871 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/src/math.rs
--rw-r--r--   0     1001      127     2792 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/src/objective.rs
--rw-r--r--   0     1001      127     6888 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_fk_inputs.json
--rw-r--r--   0     1001      127    11169 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_fk_outputs.json
--rw-r--r--   0     1001      127     2281 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_math_inputs.json
--rw-r--r--   0     1001      127     1162 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_se3_log.json
--rw-r--r--   0     1001      127     5836 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_se3_right_jacobian.json
--rw-r--r--   0     1001      127      808 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_so3_log.json
--rw-r--r--   0     1001      127     1717 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_so3_right_jacobian.json
--rwxr-xr-x   0     1001      127    12531 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/ur3e.urdf
--rw-r--r--   0     1001      127      670 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/test_fk.rs
--rw-r--r--   0     1001      127     1761 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/test_gradient.rs
--rw-r--r--   0     1001      127     4300 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/test_ik.rs
--rw-r--r--   0     1001      127     1897 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/test_math.rs
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 optik_py-0.5.0b1/crates/optik-py/Cargo.toml
--rw-r--r--   0     1001      127       71 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik-py/build.rs
--rw-r--r--   0     1001      127     3408 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik-py/src/lib.rs
--rw-r--r--   0     1001      127    31698 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/Cargo.lock
--rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 optik_py-0.5.0b1/Cargo.toml
--rw-r--r--   0     1001      127      533 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/pyproject.toml
--rw-r--r--   0     1001      127     5866 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/README.md
--rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 optik_py-0.5.0b1/PKG-INFO
+-rw-r--r--   0     1001      127      688 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/Cargo.toml
+-rw-r--r--   0     1001      127     2387 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/benches/bench.rs
+-rw-r--r--   0     1001      127     1531 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/src/config.rs
+-rw-r--r--   0     1001      127    10434 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/src/kinematics.rs
+-rw-r--r--   0     1001      127    10708 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/src/lib.rs
+-rw-r--r--   0     1001      127     6871 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/src/math.rs
+-rw-r--r--   0     1001      127     3616 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/src/objective.rs
+-rw-r--r--   0     1001      127     6888 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_fk_inputs.json
+-rw-r--r--   0     1001      127    11169 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_fk_outputs.json
+-rw-r--r--   0     1001      127     2281 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_math_inputs.json
+-rw-r--r--   0     1001      127     1162 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_se3_log.json
+-rw-r--r--   0     1001      127     5836 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_se3_right_jacobian.json
+-rw-r--r--   0     1001      127      808 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_so3_log.json
+-rw-r--r--   0     1001      127     1717 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_so3_right_jacobian.json
+-rwxr-xr-x   0     1001      127    12531 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/ur3e.urdf
+-rw-r--r--   0     1001      127      670 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/test_fk.rs
+-rw-r--r--   0     1001      127     1829 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/test_gradient.rs
+-rw-r--r--   0     1001      127     4300 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/test_ik.rs
+-rw-r--r--   0     1001      127     1897 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/test_math.rs
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 optik_py-0.5.0b2/crates/optik-py/Cargo.toml
+-rw-r--r--   0     1001      127       71 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik-py/build.rs
+-rw-r--r--   0     1001      127     3458 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik-py/src/lib.rs
+-rw-r--r--   0     1001      127    31698 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/Cargo.lock
+-rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 optik_py-0.5.0b2/Cargo.toml
+-rw-r--r--   0     1001      127      533 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/pyproject.toml
+-rw-r--r--   0     1001      127     5866 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/README.md
+-rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 optik_py-0.5.0b2/PKG-INFO
```

### Comparing `optik_py-0.5.0b1/crates/optik/Cargo.toml` & `optik_py-0.5.0b2/crates/optik/Cargo.toml`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/benches/bench.rs` & `optik_py-0.5.0b2/crates/optik/benches/bench.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use criterion::{black_box, criterion_group, criterion_main, Criterion};
-use nalgebra::Isometry3;
+use nalgebra::{vector, Isometry3};
 
 use optik::*;
 
 const BENCH_MODEL_STR: &str = include_str!("../tests/data/ur3e.urdf");
 
 fn load_benchmark_model() -> Robot {
     Robot::from_urdf_str(BENCH_MODEL_STR, "ur_base_link", "ur_ee_link")
@@ -16,28 +16,45 @@
 
     let q = robot.random_configuration(&mut rand::thread_rng());
     let mut g = vec![0.0; q.len()];
     let tfm_target = Isometry3::identity();
 
     c.bench_function("gradient", |b| {
         let fk = robot.fk(&q);
-        b.iter(|| objective_grad(&robot, &tfm_target, &fk, &mut g, 0.0, 0.0))
+        b.iter(|| {
+            objective_grad(
+                &robot,
+                &tfm_target,
+                &fk,
+                &mut g,
+                vector![1.0, 1.0, 1.0],
+                vector![1.0, 1.0, 1.0],
+            )
+        })
     });
 }
 
 fn bench_objective(c: &mut Criterion) {
     use optik::objective::objective;
 
     let robot = load_benchmark_model();
 
     let q = robot.random_configuration(&mut rand::thread_rng());
     let fk = robot.fk(&q);
     let tfm_target = Isometry3::identity();
     c.bench_function("objective", |b| {
-        b.iter(|| objective(&robot, &tfm_target, &fk, 0.0, 0.0))
+        b.iter(|| {
+            objective(
+                &robot,
+                &tfm_target,
+                &fk,
+                vector![1.0, 1.0, 1.0],
+                vector![1.0, 1.0, 1.0],
+            )
+        })
     });
 }
 
 fn bench_fk(c: &mut Criterion) {
     let robot = load_benchmark_model();
     let x0 = vec![0.1, 0.2, 0.0, 0.3, -0.2, -1.1];
```

### Comparing `optik_py-0.5.0b1/crates/optik/src/kinematics.rs` & `optik_py-0.5.0b2/crates/optik/src/kinematics.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/src/lib.rs` & `optik_py-0.5.0b2/crates/optik/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     sync::{
         atomic::{AtomicBool, Ordering},
         Arc,
     },
     time::Instant,
 };
 
-use nalgebra::{DVectorView, Isometry3, Matrix6xX};
+use nalgebra::{DVectorView, Isometry3, Matrix6xX, Vector3};
 use nlopt::{Algorithm, Nlopt, SuccessState, Target};
 use ordered_float::OrderedFloat;
 use rand::SeedableRng;
 use rand_chacha::ChaCha8Rng;
 use rayon::{
     prelude::{IntoParallelIterator, ParallelIterator},
     ThreadPool, ThreadPoolBuilder,
@@ -169,26 +169,26 @@
                             // the optimizer.
                             if let Some(g) = grad {
                                 objective_grad(
                                     self,
                                     tfm_target,
                                     fk,
                                     g,
-                                    config.tol_linear,
-                                    config.tol_angular,
+                                    Vector3::from_row_slice(&config.linear_weight),
+                                    Vector3::from_row_slice(&config.angular_weight),
                                 );
                             }
 
                             // Always compute the objective value.
                             Some(objective(
                                 self,
                                 tfm_target,
                                 fk,
-                                config.tol_linear,
-                                config.tol_angular,
+                                Vector3::from_row_slice(&config.linear_weight),
+                                Vector3::from_row_slice(&config.angular_weight),
                             ))
                         },
                         Target::Minimize,
                         // Cache the forward kinematic container within each
                         // thread to avoid re-allocating memory each objective
                         // iteration.
                         ForwardKinematics::default(),
```

### Comparing `optik_py-0.5.0b1/crates/optik/src/math.rs` & `optik_py-0.5.0b2/crates/optik/src/math.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/tests/data/test_fk_inputs.json` & `optik_py-0.5.0b2/crates/optik/tests/data/test_fk_inputs.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/tests/data/test_fk_outputs.json` & `optik_py-0.5.0b2/crates/optik/tests/data/test_fk_outputs.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/tests/data/test_math_inputs.json` & `optik_py-0.5.0b2/crates/optik/tests/data/test_math_inputs.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_se3_log.json` & `optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_se3_log.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_se3_right_jacobian.json` & `optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_se3_right_jacobian.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_so3_log.json` & `optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_so3_log.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_so3_right_jacobian.json` & `optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_so3_right_jacobian.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/tests/data/ur3e.urdf` & `optik_py-0.5.0b2/crates/optik/tests/data/ur3e.urdf`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/tests/test_fk.rs` & `optik_py-0.5.0b2/crates/optik/tests/test_fk.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/tests/test_gradient.rs` & `optik_py-0.5.0b2/crates/optik/tests/test_gradient.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use approx::assert_abs_diff_eq;
-use nalgebra::{DVector, Vector6};
+use nalgebra::{vector, DVector, Vector6};
 use optik::{
     objective::{objective, objective_grad},
     Robot,
 };
 use rand::{rngs::StdRng, Rng, SeedableRng};
 
 const TEST_MODEL_STR: &str = include_str!("data/ur3e.urdf");
@@ -30,39 +30,39 @@
 
     DVector::from_row_slice(&g)
 }
 
 #[test]
 fn test_gradient_analytical_vs_numerical() {
     let robot = Robot::from_urdf_str(TEST_MODEL_STR, "ur_base_link", "ur_ee_link");
-    let tol_linear = 0.0;
-    let tol_angular = 0.0;
+    let linear_weight = vector![0.0, 5.0, 0.25];
+    let angular_weight = vector![0.005, 1.0, 0.99];
 
     let mut rng = StdRng::seed_from_u64(42);
-    for _ in 0..100 {
+    for i in 0..100 {
         let x0: Vector6<f64> = rng.gen();
         let tfm_target = rng.gen();
         let fk = robot.fk(x0.as_slice());
 
         // Analytical gradient
         let mut g_a = Vector6::zeros();
         objective_grad(
             &robot,
             &tfm_target,
             &fk,
             g_a.as_mut_slice(),
-            tol_linear,
-            tol_angular,
+            linear_weight,
+            angular_weight,
         );
 
         // Numerical gradient
         let g_n = finite_difference(
             |x| {
                 let fk = robot.fk(x);
-                objective(&robot, &tfm_target, &fk, tol_linear, tol_angular)
+                objective(&robot, &tfm_target, &fk, linear_weight, angular_weight)
             },
             x0.as_slice(),
         );
 
         assert_abs_diff_eq!(g_a.as_slice(), g_n.as_slice(), epsilon = 1e-6);
     }
 }
```

### Comparing `optik_py-0.5.0b1/crates/optik/tests/test_ik.rs` & `optik_py-0.5.0b2/crates/optik/tests/test_ik.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik/tests/test_math.rs` & `optik_py-0.5.0b2/crates/optik/tests/test_math.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/crates/optik-py/src/lib.rs` & `optik_py-0.5.0b2/crates/optik-py/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -14,42 +14,42 @@
     #[new]
     #[pyo3(signature=(solution_mode="speed",
                       max_time=0.1,
                       max_restarts=u64::MAX,
                       tol_f=1e-6,
                       tol_df=-1.0,
                       tol_dx=-1.0,
-                      tol_linear=-1.0,
-                      tol_angular=-1.0))]
+                      linear_weight=[1.0, 1.0, 1.0],
+                      angular_weight=[1.0, 1.0, 1.0]))]
     #[allow(clippy::too_many_arguments)]
     fn py_new(
         solution_mode: &str,
         max_time: f64,
         max_restarts: u64,
         tol_f: f64,
         tol_df: f64,
         tol_dx: f64,
-        tol_linear: f64,
-        tol_angular: f64,
+        linear_weight: [f64; 3],
+        angular_weight: [f64; 3],
     ) -> Self {
         let solution_mode = solution_mode.parse().expect("invalid solution mode");
 
         if max_time == 0.0 && max_restarts == 0 {
             panic!("no time or restart limit applied -- solver would run forever")
         }
 
         PySolverConfig(SolverConfig {
             solution_mode,
             max_time,
             max_restarts,
             tol_f,
             tol_df,
             tol_dx,
-            tol_linear,
-            tol_angular,
+            linear_weight,
+            angular_weight,
         })
     }
 }
 
 #[pyclass]
 #[pyo3(name = "Robot")]
 pub struct PyRobot(Robot);
```

### Comparing `optik_py-0.5.0b1/Cargo.lock` & `optik_py-0.5.0b2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -451,15 +451,15 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "optik"
-version = "0.5.0-beta.1"
+version = "0.5.0-beta.2"
 dependencies = [
  "approx",
  "criterion",
  "nalgebra",
  "nlopt",
  "ordered-float",
  "petgraph",
@@ -469,24 +469,24 @@
  "serde",
  "serde_json",
  "urdf-rs",
 ]
 
 [[package]]
 name = "optik-cpp"
-version = "0.5.0-beta.1"
+version = "0.5.0-beta.2"
 dependencies = [
  "nalgebra",
  "optik",
  "rand",
 ]
 
 [[package]]
 name = "optik-py"
-version = "0.5.0-beta.1"
+version = "0.5.0-beta.2"
 dependencies = [
  "nalgebra",
  "optik",
  "pyo3",
  "pyo3-build-config",
 ]
```

### Comparing `optik_py-0.5.0b1/pyproject.toml` & `optik_py-0.5.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/README.md` & `optik_py-0.5.0b2/README.md`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b1/PKG-INFO` & `optik_py-0.5.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: optik-py
-Version: 0.5.0b1
+Version: 0.5.0b2
 Classifier: Topic :: Scientific/Engineering
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 Summary: An optimizing IK solver based on the Lie group of rigid transforms SE(3)
 Author: Kyle Cesare
 Author-email: kcesare@gmail.com
 License: MIT OR Apache-2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: optik-py Version: 0.5.0b1 Classifier: Topic ::
+Metadata-Version: 2.3 Name: optik-py Version: 0.5.0b2 Classifier: Topic ::
 Scientific/Engineering License-File: LICENSE-APACHE License-File: LICENSE-MIT
 Summary: An optimizing IK solver based on the Lie group of rigid transforms SE
 (3) Author: Kyle Cesare Author-email: kcesare@gmail.com License: MIT OR Apache-
 2.0 Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Project-URL: homepage, https://github.com/kylc/optik
 # OptIK
 _[_M_I_T_]_[_A_p_a_c_h_e_]_[_c_i_]_[_P_y_P_I_]_[_D_O_I_]
```

