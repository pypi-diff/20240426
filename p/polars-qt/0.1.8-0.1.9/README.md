# Comparing `tmp/polars_qt-0.1.8.tar.gz` & `tmp/polars_qt-0.1.9.tar.gz`

## Comparing `polars_qt-0.1.8.tar` & `polars_qt-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 polars_qt-0.1.8/Cargo.toml
--rw-r--r--   0     1001      127     3716 2024-04-23 07:29:12.000000 polars_qt-0.1.8/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0     1001      127      111 2024-04-23 07:29:12.000000 polars_qt-0.1.8/.gitignore
--rw-r--r--   0     1001      127        8 2024-04-23 07:29:12.000000 polars_qt-0.1.8/.python-version
--rw-r--r--   0     1001      127      665 2024-04-23 07:29:12.000000 polars_qt-0.1.8/Makefile
--rw-r--r--   0     1001      127     1786 2024-04-23 07:29:12.000000 polars_qt-0.1.8/README.md
--rw-r--r--   0     1001      127       62 2024-04-23 07:29:12.000000 polars_qt-0.1.8/polars_qt/__init__.py
--rw-r--r--   0     1001      127     3143 2024-04-23 07:29:12.000000 polars_qt-0.1.8/polars_qt/funcs.py
--rw-r--r--   0     1001      127     3429 2024-04-23 07:29:12.000000 polars_qt-0.1.8/polars_qt/qt.py
--rw-r--r--   0     1001      127     6413 2024-04-23 07:29:12.000000 polars_qt-0.1.8/polars_qt/strategy.py
--rw-r--r--   0     1001      127     2567 2024-04-23 07:29:12.000000 polars_qt-0.1.8/polars_qt/utils.py
--rw-r--r--   0     1001      127       34 2024-04-23 07:29:12.000000 polars_qt-0.1.8/requirements.txt
--rw-r--r--   0     1001      127       42 2024-04-23 07:29:12.000000 polars_qt-0.1.8/rust-toolchain.toml
--rw-r--r--   0     1001      127     1993 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/compose.rs
--rw-r--r--   0     1001      127     1598 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/equity.rs
--rw-r--r--   0     1001      127      649 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/if_then.rs
--rw-r--r--   0     1001      127      332 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/lib.rs
--rw-r--r--   0     1001      127     3250 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/rolling_rank.rs
--rw-r--r--   0     1001      127     1151 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/strategy/boll.rs
--rw-r--r--   0     1001      127      580 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/strategy/from_input.rs
--rw-r--r--   0     1001      127      672 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/strategy/martingale.rs
--rw-r--r--   0     1001      127       42 2024-04-23 07:29:12.000000 polars_qt-0.1.8/src/strategy/mod.rs
--rw-r--r--   0     1001      127      521 2024-04-23 07:29:12.000000 polars_qt-0.1.8/tests/test_compose_by.py
--rw-r--r--   0     1001      127     1375 2024-04-23 07:29:12.000000 polars_qt-0.1.8/tests/test_equity.py
--rw-r--r--   0     1001      127      867 2024-04-23 07:29:12.000000 polars_qt-0.1.8/tests/test_if_then.py
--rw-r--r--   0     1001      127      662 2024-04-23 07:29:12.000000 polars_qt-0.1.8/tests/test_rolling_rank.py
--rw-r--r--   0     1001      127     1919 2024-04-23 07:29:12.000000 polars_qt-0.1.8/tests/test_strategy.py
--rw-r--r--   0     1001      127    43442 2024-04-23 07:29:28.000000 polars_qt-0.1.8/Cargo.lock
--rw-r--r--   0     1001      127     1773 2024-04-23 07:29:12.000000 polars_qt-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 polars_qt-0.1.9/Cargo.toml
+-rw-r--r--   0     1001      127     3716 2024-04-26 06:02:01.000000 polars_qt-0.1.9/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0     1001      127      111 2024-04-26 06:02:01.000000 polars_qt-0.1.9/.gitignore
+-rw-r--r--   0     1001      127        8 2024-04-26 06:02:01.000000 polars_qt-0.1.9/.python-version
+-rw-r--r--   0     1001      127      665 2024-04-26 06:02:01.000000 polars_qt-0.1.9/Makefile
+-rw-r--r--   0     1001      127     1786 2024-04-26 06:02:01.000000 polars_qt-0.1.9/README.md
+-rw-r--r--   0     1001      127       62 2024-04-26 06:02:01.000000 polars_qt-0.1.9/polars_qt/__init__.py
+-rw-r--r--   0     1001      127     3382 2024-04-26 06:02:01.000000 polars_qt-0.1.9/polars_qt/funcs.py
+-rw-r--r--   0     1001      127     3460 2024-04-26 06:02:01.000000 polars_qt-0.1.9/polars_qt/qt.py
+-rw-r--r--   0     1001      127     6413 2024-04-26 06:02:01.000000 polars_qt-0.1.9/polars_qt/strategy.py
+-rw-r--r--   0     1001      127     2567 2024-04-26 06:02:01.000000 polars_qt-0.1.9/polars_qt/utils.py
+-rw-r--r--   0     1001      127       34 2024-04-26 06:02:01.000000 polars_qt-0.1.9/requirements.txt
+-rw-r--r--   0     1001      127       42 2024-04-26 06:02:01.000000 polars_qt-0.1.9/rust-toolchain.toml
+-rw-r--r--   0     1001      127     1993 2024-04-26 06:02:01.000000 polars_qt-0.1.9/src/compose.rs
+-rw-r--r--   0     1001      127     1598 2024-04-26 06:02:01.000000 polars_qt-0.1.9/src/equity.rs
+-rw-r--r--   0     1001      127      649 2024-04-26 06:02:01.000000 polars_qt-0.1.9/src/if_then.rs
+-rw-r--r--   0     1001      127      350 2024-04-26 06:02:01.000000 polars_qt-0.1.9/src/lib.rs
+-rw-r--r--   0     1001      127     1419 2024-04-26 06:02:01.000000 polars_qt-0.1.9/src/rolling_rank.rs
+-rw-r--r--   0     1001      127     1151 2024-04-26 06:02:01.000000 polars_qt-0.1.9/src/strategy/boll.rs
+-rw-r--r--   0     1001      127      580 2024-04-26 06:02:01.000000 polars_qt-0.1.9/src/strategy/from_input.rs
+-rw-r--r--   0     1001      127      672 2024-04-26 06:02:01.000000 polars_qt-0.1.9/src/strategy/martingale.rs
+-rw-r--r--   0     1001      127       42 2024-04-26 06:02:01.000000 polars_qt-0.1.9/src/strategy/mod.rs
+-rw-r--r--   0     1001      127      521 2024-04-26 06:02:01.000000 polars_qt-0.1.9/tests/test_compose_by.py
+-rw-r--r--   0     1001      127     1375 2024-04-26 06:02:01.000000 polars_qt-0.1.9/tests/test_equity.py
+-rw-r--r--   0     1001      127      867 2024-04-26 06:02:01.000000 polars_qt-0.1.9/tests/test_if_then.py
+-rw-r--r--   0     1001      127      662 2024-04-26 06:02:01.000000 polars_qt-0.1.9/tests/test_rolling_rank.py
+-rw-r--r--   0     1001      127     1919 2024-04-26 06:02:01.000000 polars_qt-0.1.9/tests/test_strategy.py
+-rw-r--r--   0     1001      127    42295 2024-04-26 06:02:16.000000 polars_qt-0.1.9/Cargo.lock
+-rw-r--r--   0     1001      127     1773 2024-04-26 06:02:01.000000 polars_qt-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 polars_qt-0.1.9/PKG-INFO
```

### Comparing `polars_qt-0.1.8/.github/workflows/publish_to_pypi.yml` & `polars_qt-0.1.9/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/Makefile` & `polars_qt-0.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/README.md` & `polars_qt-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/polars_qt/funcs.py` & `polars_qt-0.1.9/polars_qt/funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,16 +39,24 @@
     expr2 = parse_into_expr(expr2)
     return register_plugin(
         args=[flag_expr, expr1, expr2],
         symbol="if_then",
         is_elementwise=False,
     )
 
-def compose_by(expr: IntoExpr, by: IntoExpr) -> pl.Expr:
-    expr = parse_into_expr(expr).diff()
+def compose_by(expr: IntoExpr, by: IntoExpr, method='diff') -> pl.Expr:
+    expr = parse_into_expr(expr)
+    if method == 'diff':
+        expr = expr.diff()
+    elif method is None:
+        pass
+    elif method == 'pct_change':
+        expr = expr.pct_change()
+    else:
+        raise ValueError("method '{}' is not supported", method)
     by = parse_into_expr(by)
     return register_plugin(
         args=[expr, by],
         symbol="compose_by",
         is_elementwise=False,
     )
```

### Comparing `polars_qt-0.1.8/polars_qt/qt.py` & `polars_qt-0.1.9/polars_qt/qt.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         return rolling_rank(
             self.expr, window=window, min_periods=min_periods, pct=pct, rev=rev
         )
 
     def if_then(self, flag, then):
         return if_then(flag, then, self.expr)
 
-    def compose_by(self, by):
-        return compose_by(self.expr, by)
+    def compose_by(self, by, method='diff'):
+        return compose_by(self.expr, by, method==method)
 
     def calc_future_ret(
         self,
         open: IntoExpr,
         close: IntoExpr,
         *,
         is_signal: bool = True,
```

### Comparing `polars_qt-0.1.8/polars_qt/strategy.py` & `polars_qt-0.1.9/polars_qt/strategy.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/polars_qt/utils.py` & `polars_qt-0.1.9/polars_qt/utils.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/src/compose.rs` & `polars_qt-0.1.9/src/compose.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/src/equity.rs` & `polars_qt-0.1.9/src/equity.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/src/if_then.rs` & `polars_qt-0.1.9/src/if_then.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/src/strategy/boll.rs` & `polars_qt-0.1.9/src/strategy/boll.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/src/strategy/from_input.rs` & `polars_qt-0.1.9/src/strategy/from_input.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/src/strategy/martingale.rs` & `polars_qt-0.1.9/src/strategy/martingale.rs`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/tests/test_compose_by.py` & `polars_qt-0.1.9/tests/test_compose_by.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/tests/test_equity.py` & `polars_qt-0.1.9/tests/test_equity.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/tests/test_if_then.py` & `polars_qt-0.1.9/tests/test_if_then.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/tests/test_rolling_rank.py` & `polars_qt-0.1.9/tests/test_rolling_rank.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/tests/test_strategy.py` & `polars_qt-0.1.9/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/Cargo.lock` & `polars_qt-0.1.9/Cargo.lock`

 * *Files 5% similar despite different names*

```diff
@@ -85,20 +85,14 @@
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
-
-[[package]]
-name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
 version = "3.16.0"
@@ -159,15 +153,15 @@
 version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
- "windows-targets 0.52.5",
+ "windows-targets",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
@@ -402,17 +396,17 @@
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -538,33 +532,33 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets",
 ]
 
 [[package]]
 name = "parquet-format-safe"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1131c54b167dd4e4799ce762e1ab01549ebb94d5bdd13e6ec1b467491c378e1f"
@@ -588,17 +582,17 @@
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
  "array-init-cursor",
 ]
 
 [[package]]
 name = "polars"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f01006048a264047d6cba081fed8e11adbd69c15956f9e53185a9ac4a541853c"
+checksum = "0ea21b858b16b9c0e17a12db2800d11aa5b4bd182be6b3022eb537bbfc1f2db5"
 dependencies = [
  "getrandom",
  "polars-arrow",
  "polars-core",
  "polars-error",
  "polars-io",
  "polars-lazy",
@@ -606,17 +600,17 @@
  "polars-time",
  "polars-utils",
  "version_check",
 ]
 
 [[package]]
 name = "polars-arrow"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25197f40d71f82b2f79bb394f03e555d3cc1ce4db1dd052c28318721c71e96ad"
+checksum = "725b09f2b5ef31279b66e27bbab63c58d49d8f6696b66b1f46c7eaab95e80f75"
 dependencies = [
  "ahash",
  "atoi_simd",
  "bytemuck",
  "chrono",
  "dyn-clone",
  "either",
@@ -648,36 +642,36 @@
 dependencies = [
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "polars-compute"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c354515f73cdbbad03c2bf723fcd68e6825943b3ec503055abc8a8cb08ce46bb"
+checksum = "a796945b14b14fbb79b91ef0406e6fddca2be636e889f81ea5d6ee7d36efb4fe"
 dependencies = [
  "bytemuck",
  "either",
  "num-traits",
  "polars-arrow",
  "polars-error",
  "polars-utils",
  "strength_reduce",
  "version_check",
 ]
 
 [[package]]
 name = "polars-core"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f20d3c227186f74aa3c228c64ef72f5a15617322fed30b4323eaf53b25f8e7b"
+checksum = "465f70d3e96b6d0b1a43c358ba451286b8c8bd56696feff020d65702aa33e35c"
 dependencies = [
  "ahash",
- "bitflags 2.5.0",
+ "bitflags",
  "bytemuck",
  "chrono",
  "either",
  "hashbrown",
  "indexmap",
  "num-traits",
  "once_cell",
@@ -694,39 +688,39 @@
  "thiserror",
  "version_check",
  "xxhash-rust",
 ]
 
 [[package]]
 name = "polars-error"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d66dd0ce51f8bd620eb8bd376502fe68a2b1a446d5433ecd2e75270b0755ce76"
+checksum = "5224d5d05e6b8a6f78b75951ae1b5f82c8ab1979e11ffaf5fd41941e3d5b0757"
 dependencies = [
  "polars-arrow-format",
  "regex",
  "simdutf8",
  "thiserror",
 ]
 
 [[package]]
 name = "polars-ffi"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6c93ea335ccca3dc7fd8ca4a8d129178afc9634c8caf2237500a3390e4aa60b"
+checksum = "dcdd5a0b45dea8df72db9dfca694a1acc753bd868f3a751903b83cacdb896d2b"
 dependencies = [
  "polars-arrow",
  "polars-core",
 ]
 
 [[package]]
 name = "polars-io"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b40bef2edcdc58394792c4d779465144283a09ff1836324e7b72df7978a6e992"
+checksum = "b2c8589e418cbe4a48228d64b2a8a40284a82ec3c98817c0c2bcc0267701338b"
 dependencies = [
  "ahash",
  "bytes",
  "chrono",
  "home",
  "memchr",
  "memmap2",
@@ -741,20 +735,20 @@
  "rayon",
  "regex",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-lazy"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c27df26a19d3092298d31d47614ad84dc330c106e38aa8cd53727cd91c07cf56"
+checksum = "89b2632b1af668e2058d5f8f916d8fbde3cac63d03ae29a705f598e41dcfeb7f"
 dependencies = [
  "ahash",
- "bitflags 2.5.0",
+ "bitflags",
  "glob",
  "once_cell",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-pipe",
@@ -764,17 +758,17 @@
  "rayon",
  "smartstring",
  "version_check",
 ]
 
 [[package]]
 name = "polars-ops"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f8a51c3bdc9e7c34196ff6f5c3cb17da134e5aafb1756aaf24b76c7118e63dc"
+checksum = "efdbdb4d9a92109bc2e0ce8e17af5ae8ab643bb5b7ee9d1d74f0aeffd1fbc95f"
 dependencies = [
  "ahash",
  "argminmax",
  "bytemuck",
  "either",
  "hashbrown",
  "indexmap",
@@ -789,17 +783,17 @@
  "regex",
  "smartstring",
  "version_check",
 ]
 
 [[package]]
 name = "polars-parquet"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b8824ee00fbbe83d69553f2711014c50361238d210ed81a7a297695b7db97d42"
+checksum = "b421d2196f786fdfe162db614c8485f8308fe41575d4de634a39bbe460d1eb6a"
 dependencies = [
  "ahash",
  "base64",
  "ethnum",
  "num-traits",
  "parquet-format-safe",
  "polars-arrow",
@@ -808,17 +802,17 @@
  "seq-macro",
  "simdutf8",
  "streaming-decompression",
 ]
 
 [[package]]
 name = "polars-pipe"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c5e2c1f14e81d60cfa9afe4e611a9bad9631a2cb7cd19b7c0094d0dc32f0231"
+checksum = "48700f1d5bd56a15451e581f465c09541492750360f18637b196f995470a015c"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-queue",
  "enum_dispatch",
  "hashbrown",
  "num-traits",
  "polars-arrow",
@@ -833,63 +827,65 @@
  "smartstring",
  "uuid",
  "version_check",
 ]
 
 [[package]]
 name = "polars-plan"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff48362bd1b078bbbec7e7ba9ec01fea58fee2887db22a8e3deaf78f322fa3c4"
+checksum = "2fb8e2302e20c44defd5be8cad9c96e75face63c3a5f609aced8c4ec3b3ac97d"
 dependencies = [
  "ahash",
  "bytemuck",
+ "hashbrown",
  "once_cell",
  "percent-encoding",
  "polars-arrow",
  "polars-core",
  "polars-io",
  "polars-ops",
  "polars-time",
  "polars-utils",
  "rayon",
+ "recursive",
  "smartstring",
  "strum_macros",
  "version_check",
 ]
 
 [[package]]
 name = "polars-qt"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "itertools",
  "polars",
  "pyo3",
  "pyo3-polars",
  "serde",
  "tea_strategy",
 ]
 
 [[package]]
 name = "polars-row"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63029da56ff6a720b190490bbc7b6263f9b72d1134311b1f381fc8d306d37770"
+checksum = "a515bdc68c2ae3702e3de70d89601f3b71ca8137e282a226dddb53ee4bacfa2e"
 dependencies = [
  "bytemuck",
  "polars-arrow",
  "polars-error",
  "polars-utils",
 ]
 
 [[package]]
 name = "polars-time"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86eb74ea6ddfe675aa5c3f33c00dadbe2b85f0e8e3887b85db1fd5a3397267fd"
+checksum = "efc18e3ad92eec55db89d88f16c22d436559ba7030cf76f86f6ed7a754b673f1"
 dependencies = [
  "atoi",
  "chrono",
  "now",
  "once_cell",
  "polars-arrow",
  "polars-core",
@@ -898,28 +894,29 @@
  "polars-utils",
  "regex",
  "smartstring",
 ]
 
 [[package]]
 name = "polars-utils"
-version = "0.38.3"
+version = "0.39.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "694656a7d2b0cd8f07660dbc8d0fb7a81066ff57a452264907531d805c1e58c4"
+checksum = "c760b6c698cfe2fbbbd93d6cfb408db14ececfe1d92445dae2229ce1b5b21ae8"
 dependencies = [
  "ahash",
  "bytemuck",
  "hashbrown",
  "indexmap",
  "num-traits",
  "once_cell",
  "polars-error",
  "raw-cpuid",
  "rayon",
  "smartstring",
+ "stacker",
  "sysinfo",
  "version_check",
 ]
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
@@ -938,18 +935,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "psm"
+version = "0.1.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -957,79 +963,79 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-polars"
-version = "0.12.0"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6ab8ad08494161085fb0d2d9de82c7fde7398da1778ee7e7a5a596ff4201f5b"
+checksum = "469bd1d378fb3a34c1b182383e84741d9e7c5451a5d29a3f9c557aac161876cd"
 dependencies = [
  "polars",
  "polars-core",
  "polars-ffi",
  "polars-plan",
  "pyo3",
  "pyo3-polars-derive",
  "serde",
  "serde-pickle",
  "thiserror",
 ]
 
 [[package]]
 name = "pyo3-polars-derive"
-version = "0.6.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56c67d6b47b05d3827ef8e5f4449ae1a1861f5d7086ee18c5429e347b0d03c19"
+checksum = "3ba3d428667917efd2c233534db5779f55b398e123aea75243da8491856e1131"
 dependencies = [
  "polars-core",
  "polars-ffi",
  "polars-plan",
  "proc-macro2",
  "quote",
  "syn 2.0.60",
@@ -1086,15 +1092,15 @@
 
 [[package]]
 name = "raw-cpuid"
 version = "11.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d86a7c4638d42c44551f4791a20e687dbb4c3de1f33c43dd71e355cd429def1"
 dependencies = [
- "bitflags 2.5.0",
+ "bitflags",
 ]
 
 [[package]]
 name = "rayon"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
@@ -1110,20 +1116,40 @@
 checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "recursive"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0786a43debb760f491b1bc0269fe5e84155353c67482b9e60d0cfb596054b43e"
+dependencies = [
+ "recursive-proc-macro-impl",
+ "stacker",
+]
+
+[[package]]
+name = "recursive-proc-macro-impl"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "76009fbe0614077fc1a2ce255e3a1881a2e3a3527097d5dc6d8212c585e7e38b"
+dependencies = [
+ "quote",
+ "syn 2.0.60",
+]
+
+[[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
@@ -1228,14 +1254,27 @@
 dependencies = [
  "autocfg",
  "static_assertions",
  "version_check",
 ]
 
 [[package]]
+name = "stacker"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c886bd4480155fd3ef527d45e9ac8dd7118a898a46530b7b94c3e21866259fce"
+dependencies = [
+ "cc",
+ "cfg-if",
+ "libc",
+ "psm",
+ "winapi",
+]
+
+[[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "streaming-decompression"
@@ -1318,63 +1357,63 @@
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tea-core"
 version = "0.1.2"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#2fe153b8e1c3de7188f15881532e868435da6ca1"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#ba0b510fe602c9a22a1776bc744b014f53759e57"
 dependencies = [
  "num-traits",
  "polars",
  "polars-arrow",
  "serde",
  "tea-dtype",
 ]
 
 [[package]]
 name = "tea-dtype"
 version = "0.1.2"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#2fe153b8e1c3de7188f15881532e868435da6ca1"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#ba0b510fe602c9a22a1776bc744b014f53759e57"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "tea-map"
 version = "0.1.2"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#2fe153b8e1c3de7188f15881532e868435da6ca1"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#ba0b510fe602c9a22a1776bc744b014f53759e57"
 dependencies = [
  "num-traits",
  "tea-core",
 ]
 
 [[package]]
 name = "tea-rolling"
 version = "0.1.2"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#2fe153b8e1c3de7188f15881532e868435da6ca1"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#ba0b510fe602c9a22a1776bc744b014f53759e57"
 dependencies = [
  "num-traits",
  "tea-core",
 ]
 
 [[package]]
 name = "tea_strategy"
 version = "0.1.0"
-source = "git+https://github.com/Teamon9161/tea_strategy.git?rev=577932f#577932f9989c4df65a815a5b514cb7a036ccaa4c"
+source = "git+https://github.com/Teamon9161/tea_strategy.git?branch=master#614c5ece6bdc4b3fd70d1633f547339752cfe149"
 dependencies = [
  "itertools",
  "serde",
  "tevec",
 ]
 
 [[package]]
 name = "tevec"
 version = "0.1.2"
-source = "git+https://github.com/Teamon9161/tevec.git?branch=master#2fe153b8e1c3de7188f15881532e868435da6ca1"
+source = "git+https://github.com/Teamon9161/tevec.git?branch=master#ba0b510fe602c9a22a1776bc744b014f53759e57"
 dependencies = [
  "tea-core",
  "tea-dtype",
  "tea-map",
  "tea-rolling",
 ]
 
@@ -1510,152 +1549,95 @@
 [[package]]
 name = "windows"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e48a53791691ab099e5e2ad123536d0fff50652600abaf43bbf952894110d0be"
 dependencies = [
  "windows-core",
- "windows-targets 0.52.5",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.5",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.5",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
-dependencies = [
- "windows_aarch64_gnullvm 0.48.5",
- "windows_aarch64_msvc 0.48.5",
- "windows_i686_gnu 0.48.5",
- "windows_i686_msvc 0.48.5",
- "windows_x86_64_gnu 0.48.5",
- "windows_x86_64_gnullvm 0.48.5",
- "windows_x86_64_msvc 0.48.5",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.5",
- "windows_aarch64_msvc 0.52.5",
- "windows_i686_gnu 0.52.5",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
  "windows_i686_gnullvm",
- "windows_i686_msvc 0.52.5",
- "windows_x86_64_gnu 0.52.5",
- "windows_x86_64_gnullvm 0.52.5",
- "windows_x86_64_msvc 0.52.5",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
 
 [[package]]
 name = "windows_i686_gnullvm"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "xxhash-rust"
 version = "0.8.10"
```

### Comparing `polars_qt-0.1.8/pyproject.toml` & `polars_qt-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_qt-0.1.8/PKG-INFO` & `polars_qt-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars-qt
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars >=0.20.16
 Author-email: Teamon9161 <teamon9161@163.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

