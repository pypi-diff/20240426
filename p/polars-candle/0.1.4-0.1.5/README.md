# Comparing `tmp/polars_candle-0.1.4-cp39-none-win_amd64.whl.zip` & `tmp/polars_candle-0.1.5-cp39-cp39-manylinux_2_34_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 6236867 bytes, number of entries: 6
--rw-r--r--  4.6 unx     4348 b- defN 24-Apr-22 15:14 polars_candle-0.1.4.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Apr-22 15:14 polars_candle-0.1.4.dist-info/WHEEL
--rw-r--r--  4.6 unx     1566 b- defN 24-Apr-22 15:14 polars_candle/candle_ext.py
--rw-r--r--  4.6 unx       49 b- defN 24-Apr-22 15:14 polars_candle/__init__.py
--rwxr-xr-x  4.6 unx 20084736 b- defN 24-Apr-22 15:14 polars_candle/polars_candle.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      495 b- defN 24-Apr-22 15:14 polars_candle-0.1.4.dist-info/RECORD
-6 files, 20091288 bytes uncompressed, 6235975 bytes compressed:  69.0%
+Zip file size: 6934597 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     4054 b- defN 24-Apr-26 09:57 polars_candle-0.1.5.dist-info/METADATA
+-rw-r--r--  4.6 unx      106 b- defN 24-Apr-26 09:57 polars_candle-0.1.5.dist-info/WHEEL
+-rw-r--r--  4.6 unx     2078 b- defN 24-Apr-26 09:57 polars_candle/candle_ext.py
+-rw-r--r--  4.6 unx       48 b- defN 24-Apr-26 09:57 polars_candle/__init__.py
+-rwxr-xr-x  4.6 unx 22005048 b- defN 24-Apr-26 09:57 polars_candle/polars_candle.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      508 b- defN 24-Apr-26 09:57 polars_candle-0.1.5.dist-info/RECORD
+6 files, 22011842 bytes uncompressed, 6933681 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: polars_candle-0.1.4.dist-info/METADATA
+Filename: polars_candle-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: polars_candle-0.1.4.dist-info/WHEEL
+Filename: polars_candle-0.1.5.dist-info/WHEEL
 Comment: 
 
 Filename: polars_candle/candle_ext.py
 Comment: 
 
 Filename: polars_candle/__init__.py
 Comment: 
 
-Filename: polars_candle/polars_candle.cp39-win_amd64.pyd
+Filename: polars_candle/polars_candle.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: polars_candle-0.1.4.dist-info/RECORD
+Filename: polars_candle-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## polars_candle/candle_ext.py

```diff
@@ -1,63 +1,72 @@
-from pathlib import Path
-from typing import Literal
-
-import polars as pl
-from polars.plugins import register_plugin_function
-
-ModelName = Literal["bert-base-uncased", "bert-base-cased"]
-
-
-@pl.api.register_expr_namespace("candle")
-class CandleExt:
-	"""
-	Extension for Polars to use deep learning models using the candle library.
-
-	Polars namespace: candle
-
-	Examples
-	--------
-	>>> df = pl.DataFrame({
-	...     "text": [
-	...         "This is a test.",
-	...         "This is another test.",
-	...     ],
-	... })
-	>>> df.with_columns(
-	...     pl.col("text").candle.embed_text("bert-base-uncased")
-	... )
-	"""
-
-	def __init__(self, expr: pl.Expr) -> None:
-		self._expr = expr
-
-	def embed_text(
-			self,
-			model_repo: str,
-			pooling: Literal["max", "sum", "mean"] = "mean",
-			normalize: bool = False,
-	) -> pl.Expr:
-		"""
-		Embed text using a pre-trained model.
-
-		Parameters
-		----------
-		model_repo
-			The repository name of the text embedding model to use. E.g. "sentence-transformers/all-MiniLM-L6-v2".
-		pooling
-			The pooling strategy to use. One of "max", "sum", or "mean".
-		normalize
-			Whether to normalize (L2) the embeddings - meaning that all embeddings will have a length of 1.
-
-		Returns
-		-------
-		Expr
-			An expression with the embedded text.
-		"""
-
-		return register_plugin_function(
-			plugin_path=Path(__file__).parent,
-			function_name="embed_text",
-			args=[self._expr],
-			kwargs={"model_repo": model_repo, "pooling": pooling, "normalize": normalize},
-			is_elementwise=True,
-		)
+from pathlib import Path
+from typing import Literal
+
+import polars as pl
+from polars.plugins import register_plugin_function
+
+ModelName = Literal["bert-base-uncased", "bert-base-cased"]
+
+
+@pl.api.register_expr_namespace("candle")
+class CandleExt:
+    """
+    Extension for Polars to use deep learning models using the candle library.
+
+    Polars namespace: candle
+
+    Examples
+    --------
+    >>> df = pl.DataFrame({
+    ...     "text": [
+    ...         "This is a test.",
+    ...         "This is another test.",
+    ...     ],
+    ... })
+    >>> df.with_columns(
+    ...     pl.col("text").candle.embed_text("bert-base-uncased")
+    ... )
+    """
+
+    def __init__(self, expr: pl.Expr) -> None:
+        self._expr = expr
+
+    def embed_text(
+        self,
+        model_repo: str,
+        pooling: Literal["max", "sum", "mean"] = "mean",
+        normalize: bool = False,
+        device: Literal["cpu", "gpu"] = "cpu",
+    ) -> pl.Expr:
+        """
+        Embed text using a pre-trained model.
+
+        Parameters
+        ----------
+        model_repo
+                The repository name of the text embedding model to use. E.g. "sentence-transformers/all-MiniLM-L6-v2".
+        pooling
+                The pooling strategy to use. One of "max", "sum", or "mean".
+        normalize
+                Whether to normalize (L2) the embeddings - meaning that all embeddings will have a length of 1.
+        device
+                The device to use for the model. One of "cpu" or "gpu". Will select either a Metal or CUDA device
+                depending on the availability.
+
+        Returns
+        -------
+        Expr
+                An expression with the embedded text.
+        """
+
+        return register_plugin_function(
+            plugin_path=Path(__file__).parent,
+            function_name="embed_text",
+            args=[self._expr],
+            kwargs={
+                "model_repo": model_repo,
+                "pooling": pooling,
+                "normalize": normalize,
+                "device": device,
+            },
+            is_elementwise=True,
+        )
```

## polars_candle/__init__.py

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-from .candle_ext import CandleExt  # noqa: F401
+from .candle_ext import CandleExt  # noqa: F401
```

## Comparing `polars_candle-0.1.4.dist-info/METADATA` & `polars_candle-0.1.5.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,104 +1,100 @@
 Metadata-Version: 2.3
-Name: polars_candle
-Version: 0.1.4
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Name: polars-candle
+Version: 0.1.5
 Summary: A text embedding extension for the Polars Dataframe library.
 Keywords: polars,dataframe,embedding,nlp,candle
 Author: Wouter Doppenberg <wouterdoppenberg@gmail.com>
 Author-email: Wouter Doppenberg <wouterdoppenberg@gmail.com>
 License: Apache-2.0
-Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-# `polars-candle`
-
-A [`polars`](https://pola.rs/) extension for running [`candle`](https://github.com/huggingface/candle) ML
-models on `polars` DataFrames. 
-
-# Example
-
-Pull any applicable model from Huggingface, such as the recently released 
-[Snowflake model](https://huggingface.co/Snowflake/snowflake-arctic-embed-xs), and embed text using a simple API.
-
-```python
-import polars as pl
-import polars_candle  # ignore: F401
-
-df = pl.DataFrame({"s": ["This is a sentence", "This is another sentence"]})
-
-embed_kwargs = {
-    "model_repo": "Snowflake/snowflake-arctic-embed-xs",
-    "pooling": "mean", 
-}
-
-df = df.with_columns(
-    pl.col("s").candle.embed_text(**embed_kwargs).alias("s_embedding")
-)
-print(df)
-# ┌──────────────────────────┬───────────────────────────────────┐
-# │ s                        ┆ s_embedding                       │
-# │ ---                      ┆ ---                               │
-# │ str                      ┆ array[f32, 384]                   │
-# ╞══════════════════════════╪═══════════════════════════════════╡
-# │ This is a sentence       ┆ [-0.056457, 0.559411, … -0.20403… │
-# │ This is another sentence ┆ [-0.117206, 0.336827, … 0.174078… │
-# └──────────────────────────┴───────────────────────────────────┘
-```
-
-Currently, Bert, JinaBert, and Distilbert models are supported. More models will be added in the future. Check 
-my other repository [`wdoppenberg/glowrs`](https://github.com/wdoppenberg/glowrs) to learn more about the underlying 
-implementation for sentence embedding.
-
-# Installation
-
-Make sure you have `polars` installed. If not, install it using `pip install polars`. Then, install `polars-candle` using
-
-```bash
-pip install polars-candle
-```
-
-If you want to install the latest version from the repository, you can use:
-
-```bash
-pip install git+https://github.com/wdoppenberg/polars-candle.git
-```
-
-_Note:_ You need to have the Rust toolchain installed on your system to compile the library. See 
-[here](https://www.rust-lang.org/tools/install) for instructions on how to install Rust.
-
-If you're on a Mac with an ARM processor, the library will compile with Metal acceleration by default. 
-Should you want more control over the installation, you can set build features using `maturin`:
-
-```bash
-maturin develop --release -F <feature>
-```
-
-Where `<feature>` can be one of the following:
-* `metal` Install with Metal acceleration.
-* `cuda` Install with CUDA acceleration.
-* `accelerate` Install with the Accelerate framework.
-
-
-# Roadmap
-
-- [x] Embed text using Bert, JinaBert, and Distilbert models.
-- [ ] Add more models.
-- [ ] More configuration options for embedding (e.g. pooling strategy, device selection, etc.).
-- [ ] Support & test streaming workloads.
-
-
-# Credits
-
-- Massive thanks to [`polars`](https://pola.rs/) & their contributors for providing a blazing fast DataFrame library 
-with the ability to extend it with custom functions using [`pyo3-polars`](https://github.com/pola-rs/pyo3-polars).
-- Great work so far by Huggingface on [`candle`](https://github.com/huggingface/candle) for providing a simple
-interface to run ML models.
-
-
-# Note
-
-This is a work in progress and the API might change in the future. Feel free to open an issue if you have any
-suggestions or improvements.
+# `polars-candle`
+
+A [`polars`](https://pola.rs/) extension for running [`candle`](https://github.com/huggingface/candle) ML
+models on `polars` DataFrames. 
+
+# Example
+
+Pull any applicable model from Huggingface, such as the recently released 
+[Snowflake model](https://huggingface.co/Snowflake/snowflake-arctic-embed-xs), and embed text using a simple API.
+
+```python
+import polars as pl
+import polars_candle  # ignore: F401
+
+df = pl.DataFrame({"s": ["This is a sentence", "This is another sentence"]})
+
+embed_kwargs = {
+    "model_repo": "Snowflake/snowflake-arctic-embed-xs",
+    "pooling": "mean", 
+}
+
+df = df.with_columns(
+    pl.col("s").candle.embed_text(**embed_kwargs).alias("s_embedding")
+)
+print(df)
+# ┌──────────────────────────┬───────────────────────────────────┐
+# │ s                        ┆ s_embedding                       │
+# │ ---                      ┆ ---                               │
+# │ str                      ┆ array[f32, 384]                   │
+# ╞══════════════════════════╪═══════════════════════════════════╡
+# │ This is a sentence       ┆ [-0.056457, 0.559411, … -0.20403… │
+# │ This is another sentence ┆ [-0.117206, 0.336827, … 0.174078… │
+# └──────────────────────────┴───────────────────────────────────┘
+```
+
+Currently, Bert, JinaBert, and Distilbert models are supported. More models will be added in the future. Check 
+my other repository [`wdoppenberg/glowrs`](https://github.com/wdoppenberg/glowrs) to learn more about the underlying 
+implementation for sentence embedding.
+
+# Installation
+
+Make sure you have `polars` installed. If not, install it using `pip install polars`. Then, install `polars-candle` using
+
+```bash
+pip install polars-candle
+```
+
+If you want to install the latest version from the repository, you can use:
+
+```bash
+pip install git+https://github.com/wdoppenberg/polars-candle.git
+```
+
+_Note:_ You need to have the Rust toolchain installed on your system to compile the library. See 
+[here](https://www.rust-lang.org/tools/install) for instructions on how to install Rust.
+
+If you're on a Mac with an ARM processor, the library will compile with Metal acceleration by default. 
+Should you want more control over the installation, you can set build features using `maturin`:
+
+```bash
+maturin develop --release -F <feature>
+```
+
+Where `<feature>` can be one of the following:
+* `metal` Install with Metal acceleration.
+* `cuda` Install with CUDA acceleration.
+* `accelerate` Install with the Accelerate framework.
+
+
+# Roadmap
+
+- [x] Embed text using Bert, JinaBert, and Distilbert models.
+- [ ] Add more models.
+- [ ] More configuration options for embedding (e.g. pooling strategy, device selection, etc.).
+- [ ] Support & test streaming workloads.
+
+
+# Credits
+
+- Massive thanks to [`polars`](https://pola.rs/) & their contributors for providing a blazing fast DataFrame library 
+with the ability to extend it with custom functions using [`pyo3-polars`](https://github.com/pola-rs/pyo3-polars).
+- Great work so far by Huggingface on [`candle`](https://github.com/huggingface/candle) for providing a simple
+interface to run ML models.
+
+
+# Note
+
+This is a work in progress and the API might change in the future. Feel free to open an issue if you have any
+suggestions or improvements.
```

