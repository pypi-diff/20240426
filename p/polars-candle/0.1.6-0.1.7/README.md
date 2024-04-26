# Comparing `tmp/polars_candle-0.1.6.tar.gz` & `tmp/polars_candle-0.1.7.tar.gz`

## Comparing `polars_candle-0.1.6.tar` & `polars_candle-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 polars_candle-0.1.6/Cargo.toml
--rw-r--r--   0     1001      127     5753 2024-04-26 14:43:18.000000 polars_candle-0.1.6/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      876 2024-04-26 14:43:18.000000 polars_candle-0.1.6/.gitignore
--rw-r--r--   0     1001      127      490 2024-04-26 14:43:18.000000 polars_candle-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      552 2024-04-26 14:43:18.000000 polars_candle-0.1.6/Makefile
--rw-r--r--   0     1001      127     3517 2024-04-26 14:43:18.000000 polars_candle-0.1.6/README.md
--rw-r--r--   0     1001      127    23652 2024-04-26 14:43:18.000000 polars_candle-0.1.6/poetry.lock
--rw-r--r--   0     1001      127       48 2024-04-26 14:43:18.000000 polars_candle-0.1.6/polars_candle/__init__.py
--rw-r--r--   0     1001      127     2078 2024-04-26 14:43:18.000000 polars_candle-0.1.6/polars_candle/candle_ext.py
--rw-r--r--   0     1001      127     3319 2024-04-26 14:43:18.000000 polars_candle-0.1.6/src/candle_ext/embed.rs
--rw-r--r--   0     1001      127       22 2024-04-26 14:43:18.000000 polars_candle-0.1.6/src/candle_ext/mod.rs
--rw-r--r--   0     1001      127     1548 2024-04-26 14:43:18.000000 polars_candle-0.1.6/src/candle_ext/utils.rs
--rw-r--r--   0     1001      127      206 2024-04-26 14:43:18.000000 polars_candle-0.1.6/src/lib.rs
--rw-r--r--   0     1001      127     3456 2024-04-26 14:43:18.000000 polars_candle-0.1.6/tests/test_candle.py
--rw-r--r--   0     1001      127    98069 2024-04-26 14:43:18.000000 polars_candle-0.1.6/Cargo.lock
--rw-r--r--   0     1001      127      870 2024-04-26 14:43:18.000000 polars_candle-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4173 1970-01-01 00:00:00.000000 polars_candle-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      986 1970-01-01 00:00:00.000000 polars_candle-0.1.7/Cargo.toml
+-rw-r--r--   0     1001      127     5775 2024-04-26 15:33:39.000000 polars_candle-0.1.7/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      876 2024-04-26 15:33:39.000000 polars_candle-0.1.7/.gitignore
+-rw-r--r--   0     1001      127      490 2024-04-26 15:33:39.000000 polars_candle-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      552 2024-04-26 15:33:39.000000 polars_candle-0.1.7/Makefile
+-rw-r--r--   0     1001      127     3740 2024-04-26 15:33:39.000000 polars_candle-0.1.7/README.md
+-rw-r--r--   0     1001      127    23652 2024-04-26 15:33:39.000000 polars_candle-0.1.7/poetry.lock
+-rw-r--r--   0     1001      127       48 2024-04-26 15:33:39.000000 polars_candle-0.1.7/polars_candle/__init__.py
+-rw-r--r--   0     1001      127     2078 2024-04-26 15:33:39.000000 polars_candle-0.1.7/polars_candle/candle_ext.py
+-rw-r--r--   0     1001      127     3319 2024-04-26 15:33:39.000000 polars_candle-0.1.7/src/candle_ext/embed.rs
+-rw-r--r--   0     1001      127       22 2024-04-26 15:33:39.000000 polars_candle-0.1.7/src/candle_ext/mod.rs
+-rw-r--r--   0     1001      127     1548 2024-04-26 15:33:39.000000 polars_candle-0.1.7/src/candle_ext/utils.rs
+-rw-r--r--   0     1001      127      206 2024-04-26 15:33:39.000000 polars_candle-0.1.7/src/lib.rs
+-rw-r--r--   0     1001      127     3456 2024-04-26 15:33:39.000000 polars_candle-0.1.7/tests/test_candle.py
+-rw-r--r--   0     1001      127    98069 2024-04-26 15:33:39.000000 polars_candle-0.1.7/Cargo.lock
+-rw-r--r--   0     1001      127      870 2024-04-26 15:33:39.000000 polars_candle-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4396 1970-01-01 00:00:00.000000 polars_candle-0.1.7/PKG-INFO
```

### Comparing `polars_candle-0.1.6/Cargo.toml` & `polars_candle-0.1.7/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 name = "polars-candle"
-version = "0.1.6"
+version = "0.1.7"
 edition = "2021"
 authors = ["Wouter Doppenberg <wouterdoppenberg@gmail.com>"]
 description = "A text embedding extension for the Polars Dataframe library."
 keywords = ["polars", "dataframe", "embedding", "nlp", "candle"]
 license = "Apache-2.0"
 
 [lib]
 name = "polars_candle"
 crate-type = ["cdylib"]
 
 
 [dependencies]
 anyhow = "1.0.79"
-glowrs = "0.4.0"
+glowrs = "0.4.1"
 chrono = "0.4.35"
 ndarray = "0.15.6"
 polars = { version = "0.39.2", features = ["lazy", "dtype-array", "dtype-categorical", "ndarray", "log"] }
 pyo3 = { version = "0.21.2", features = ["extension-module"] }
 pyo3-polars = { version = "0.13.0", features = ["derive"] }
 serde = { version = "1.0.197", features = ["derive"] }
 serde_json = "1.0.115"
```

### Comparing `polars_candle-0.1.6/.github/workflows/ci.yml` & `polars_candle-0.1.7/.github/workflows/ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     - name: Build wheels
       if: matrix.runner == 'macos-14'
       uses: PyO3/maturin-action@v1
       with:
         command: develop
         target: aarch64-apple-darwin
-        args: --release -F metal
+        args: --release -F metal,accelerate
         sccache: true
       env:
         VIRUTAL_ENV: ${{ github.workspace }}/.venv
     
     - name: poetry pytest
       run: poetry run pytest tests -s
       working-directory: ${{ github.workspace }}
@@ -90,15 +90,15 @@
       - name: Rustup install aarch64 target
         run: rustup target add aarch64-apple-darwin
 
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: aarch64-apple-darwin
-          args: --release -F metal --out dist -i ${{ matrix.py-version }}
+          args: --release -F metal,accelerate --out dist -i ${{ matrix.py-version }}
 
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheel-darwin-${{ matrix.py-version }}
           path: ${{ github.workspace }}/dist/*
```

### Comparing `polars_candle-0.1.6/.gitignore` & `polars_candle-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `polars_candle-0.1.6/Makefile` & `polars_candle-0.1.7/Makefile`

 * *Files identical despite different names*

### Comparing `polars_candle-0.1.6/README.md` & `polars_candle-0.1.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 
 Make sure you have `polars` installed. If not, install it using `pip install polars`. Then, install `polars-candle` using
 
 ```bash
 pip install polars-candle
 ```
 
+_Note:_ The macOS ARM wheels of this library come with Metal support out of the box. For CUDA, check the below 
+instructions on how to build from source. 
+
 If you want to install the latest version from the repository, you can use:
 
 ```bash
 pip install git+https://github.com/wdoppenberg/polars-candle.git
 ```
 
 _Note:_ You need to have the Rust toolchain installed on your system to compile the library. See 
@@ -57,16 +60,16 @@
 You can set build features using `maturin`:
 
 ```bash
 maturin develop --release -F <feature>
 ```
 
 Where `<feature>` can be one of the following:
-* `metal` Install with Metal acceleration.
-* `cuda` Install with CUDA acceleration.
+* `metal` Install with Metal acceleration. 
+* `cuda` Install with CUDA acceleration. Might require additional setup such as installing CUDA libraries.
 * `accelerate` Install with the Accelerate framework.
 
 
 # Roadmap
 
 - [x] Embed text using Bert, JinaBert, and Distilbert models.
 - [ ] Add more models.
```

### Comparing `polars_candle-0.1.6/poetry.lock` & `polars_candle-0.1.7/poetry.lock`

 * *Files identical despite different names*

### Comparing `polars_candle-0.1.6/polars_candle/candle_ext.py` & `polars_candle-0.1.7/polars_candle/candle_ext.py`

 * *Files identical despite different names*

### Comparing `polars_candle-0.1.6/src/candle_ext/embed.rs` & `polars_candle-0.1.7/src/candle_ext/embed.rs`

 * *Files identical despite different names*

### Comparing `polars_candle-0.1.6/src/candle_ext/utils.rs` & `polars_candle-0.1.7/src/candle_ext/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_candle-0.1.6/tests/test_candle.py` & `polars_candle-0.1.7/tests/test_candle.py`

 * *Files identical despite different names*

### Comparing `polars_candle-0.1.6/Cargo.lock` & `polars_candle-0.1.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1082,17 +1082,17 @@
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "glowrs"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c6f343362dee2a660f62c931db49cd6e9cfde0c29619dc867bd0a6eab66a164"
+checksum = "df9a37b31b449d324bfc99f3847946bc8ab6ac5d555ab414458415c900859a9f"
 dependencies = [
  "candle-core",
  "candle-nn",
  "candle-transformers",
  "clap",
  "hf-hub",
  "once_cell",
@@ -2040,15 +2040,15 @@
 dependencies = [
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "polars-candle"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
  "anyhow",
  "candle-core",
  "chrono",
  "glowrs",
  "ndarray",
  "polars",
```

### Comparing `polars_candle-0.1.6/pyproject.toml` & `polars_candle-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "polars_candle"
-version = "0.1.6"
+version = "0.1.7"
 requires-python = ">=3.9"
 license = "Apache-2.0"
 classifiers = [
   "Programming Language :: Rust",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 urls = { repository = "https://github.com/wdoppenberg/polars-candle" }
 keywords = ["polars", "dataframe", "embedding", "nlp", "candle"]
 
 
 [tool.poetry]
 name = "polars_candle"
-version = "0.1.6"
+version = "0.1.7"
 description = "A text embedding extension for the Polars Dataframe library."
 authors = ["Wouter Doppenberg <wouterdoppenberg@gmail.com>"]
 
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `polars_candle-0.1.6/PKG-INFO` & `polars_candle-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: polars_candle
-Version: 0.1.6
+Version: 0.1.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: A text embedding extension for the Polars Dataframe library.
 Keywords: polars,dataframe,embedding,nlp,candle
 Author: Wouter Doppenberg <wouterdoppenberg@gmail.com>
 Author-email: Wouter Doppenberg <wouterdoppenberg@gmail.com>
@@ -56,14 +56,17 @@
 
 Make sure you have `polars` installed. If not, install it using `pip install polars`. Then, install `polars-candle` using
 
 ```bash
 pip install polars-candle
 ```
 
+_Note:_ The macOS ARM wheels of this library come with Metal support out of the box. For CUDA, check the below 
+instructions on how to build from source. 
+
 If you want to install the latest version from the repository, you can use:
 
 ```bash
 pip install git+https://github.com/wdoppenberg/polars-candle.git
 ```
 
 _Note:_ You need to have the Rust toolchain installed on your system to compile the library. See 
@@ -72,16 +75,16 @@
 You can set build features using `maturin`:
 
 ```bash
 maturin develop --release -F <feature>
 ```
 
 Where `<feature>` can be one of the following:
-* `metal` Install with Metal acceleration.
-* `cuda` Install with CUDA acceleration.
+* `metal` Install with Metal acceleration. 
+* `cuda` Install with CUDA acceleration. Might require additional setup such as installing CUDA libraries.
 * `accelerate` Install with the Accelerate framework.
 
 
 # Roadmap
 
 - [x] Embed text using Bert, JinaBert, and Distilbert models.
 - [ ] Add more models.
```

