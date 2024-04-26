# Comparing `tmp/jax_tqdm-0.1.2.tar.gz` & `tmp/jax_tqdm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_tqdm-0.1.2.tar", max compression
+gzip compressed data, was "jax_tqdm-0.2.0.tar", max compression
```

## Comparing `jax_tqdm-0.1.2.tar` & `jax_tqdm-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     2817 2023-11-21 19:48:26.044384 jax_tqdm-0.1.2/README.md
--rw-r--r--   0        0        0       47 2023-11-21 19:48:26.044384 jax_tqdm-0.1.2/jax_tqdm/__init__.py
--rw-r--r--   0        0        0     4758 2023-11-21 19:48:26.044384 jax_tqdm-0.1.2/jax_tqdm/pbar.py
--rw-r--r--   0        0        0      843 2023-11-21 19:48:26.044384 jax_tqdm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3576 1970-01-01 00:00:00.000000 jax_tqdm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-25 10:44:36.938920 jax_tqdm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2832 2024-04-26 10:38:40.256768 jax_tqdm-0.2.0/README.md
+-rw-r--r--   0        0        0       47 2023-11-21 19:48:26.044384 jax_tqdm-0.2.0/jax_tqdm/__init__.py
+-rw-r--r--   0        0        0     4657 2024-04-25 10:44:36.938920 jax_tqdm-0.2.0/jax_tqdm/pbar.py
+-rw-r--r--   0        0        0      850 2024-04-26 10:38:40.256768 jax_tqdm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 jax_tqdm-0.2.0/PKG-INFO
```

### Comparing `jax_tqdm-0.1.2/README.md` & `jax_tqdm-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -85,15 +85,16 @@
 last_number, all_numbers = lax.scan(step, 0, jnp.arange(n))
 ```
 
 ## Why JAX-tqdm?
 
 JAX functions are [pure](https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#pure-functions),
 so side effects such as printing progress when running scans and loops are not allowed.
-However, the [host_callback module](https://jax.readthedocs.io/en/latest/jax.experimental.host_callback.html)
+However, the
+[debug module](https://jax.readthedocs.io/en/latest/notebooks/external_callbacks.html#exploring-debug-callback)
 has primitives for calling Python functions on the host from JAX code. This can be used
 to update a Python tqdm progress bar regularly during the computation. JAX-tqdm
 implements this for JAX scans and loops and is used by simply adding a decorator to the
 body of your update function.
 
 Note that as the tqdm progress bar is only updated 20 times during the scan or loop,
 there is no performance penalty.
```

### Comparing `jax_tqdm-0.1.2/jax_tqdm/pbar.py` & `jax_tqdm-0.2.0/jax_tqdm/pbar.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 
 import jax
-from jax.experimental import host_callback
+from jax.debug import callback
 from tqdm.auto import tqdm
 
 
 def scan_tqdm(
     n: int,
     print_rate: typing.Optional[int] = None,
     **kwargs,
@@ -131,42 +131,43 @@
         tqdm_bars[0].set_description(message, refresh=False)
 
     def _update_tqdm(arg, transform):
         tqdm_bars[0].update(arg)
 
     def _update_progress_bar(iter_num):
         "Updates tqdm from a JAX scan or loop"
-        _ = jax.jax.lax.cond(
+        _ = jax.lax.cond(
             iter_num == 0,
-            lambda _: host_callback.id_tap(_define_tqdm, None, result=iter_num),
-            lambda _: iter_num,
+            lambda _: callback(_define_tqdm, None, None),
+            lambda _: None,
             operand=None,
         )
 
         _ = jax.lax.cond(
             # update tqdm every multiple of `print_rate` except at the end
             (iter_num % print_rate == 0) & (iter_num != n - remainder),
-            lambda _: host_callback.id_tap(_update_tqdm, print_rate, result=iter_num),
-            lambda _: iter_num,
+            lambda _: callback(_update_tqdm, print_rate, None),
+            lambda _: None,
             operand=None,
         )
 
         _ = jax.lax.cond(
             # update tqdm by `remainder`
             iter_num == n - remainder,
-            lambda _: host_callback.id_tap(_update_tqdm, remainder, result=iter_num),
-            lambda _: iter_num,
+            lambda _: callback(_update_tqdm, remainder, None),
+            lambda _: None,
             operand=None,
         )
 
     def _close_tqdm(arg, transform):
         tqdm_bars[0].close()
 
     def close_tqdm(result, iter_num):
-        return jax.lax.cond(
+        _ = jax.lax.cond(
             iter_num == n - 1,
-            lambda _: host_callback.id_tap(_close_tqdm, None, result=result),
-            lambda _: result,
+            lambda _: callback(_close_tqdm, None, None),
+            lambda _: None,
             operand=None,
         )
+        return result
 
     return _update_progress_bar, close_tqdm
```

### Comparing `jax_tqdm-0.1.2/pyproject.toml` & `jax_tqdm-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "jax-tqdm"
-version = "0.1.2"
+version = "0.2.0"
 description = "Tqdm progress bar for JAX scans and loops"
 authors = [
     "Jeremie Coullon <jeremie.coullon@gmail.com>",
     "zombie-einstein <zombie-einstein@proton.me>"
 ]
 readme = "README.md"
 packages = [{include = "jax_tqdm"}]
 homepage = "https://github.com/jeremiecoullon/jax-tqdm"
 repository = "https://github.com/jeremiecoullon/jax-tqdm"
 keywords = ["jax", "tqdm"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = ">=3.9,<4.0"
 tqdm = "^4.64.1"
-jax = ">=0.3.5"
+jax = ">=0.4.12"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.21.0"
 taskipy = "^1.10.3"
 pytest = "^7.2.1"
```

### Comparing `jax_tqdm-0.1.2/PKG-INFO` & `jax_tqdm-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: jax-tqdm
-Version: 0.1.2
+Version: 0.2.0
 Summary: Tqdm progress bar for JAX scans and loops
 Home-page: https://github.com/jeremiecoullon/jax-tqdm
 License: MIT
 Keywords: jax,tqdm
 Author: Jeremie Coullon
 Author-email: jeremie.coullon@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: jax (>=0.3.5)
+Requires-Dist: jax (>=0.4.12)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Repository, https://github.com/jeremiecoullon/jax-tqdm
 Description-Content-Type: text/markdown
 
 # JAX-tqdm
 
 Add a [tqdm](https://github.com/tqdm/tqdm) progress bar to your JAX scans and loops.
@@ -106,15 +105,16 @@
 last_number, all_numbers = lax.scan(step, 0, jnp.arange(n))
 ```
 
 ## Why JAX-tqdm?
 
 JAX functions are [pure](https://jax.readthedocs.io/en/latest/notebooks/Common_Gotchas_in_JAX.html#pure-functions),
 so side effects such as printing progress when running scans and loops are not allowed.
-However, the [host_callback module](https://jax.readthedocs.io/en/latest/jax.experimental.host_callback.html)
+However, the
+[debug module](https://jax.readthedocs.io/en/latest/notebooks/external_callbacks.html#exploring-debug-callback)
 has primitives for calling Python functions on the host from JAX code. This can be used
 to update a Python tqdm progress bar regularly during the computation. JAX-tqdm
 implements this for JAX scans and loops and is used by simply adding a decorator to the
 body of your update function.
 
 Note that as the tqdm progress bar is only updated 20 times during the scan or loop,
 there is no performance penalty.
```

