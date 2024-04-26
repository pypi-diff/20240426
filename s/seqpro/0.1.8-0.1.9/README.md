# Comparing `tmp/seqpro-0.1.8.tar.gz` & `tmp/seqpro-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqpro-0.1.8.tar", max compression
+gzip compressed data, was "seqpro-0.1.9.tar", max compression
```

## Comparing `seqpro-0.1.8.tar` & `seqpro-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1068 2023-11-20 00:42:49.906283 seqpro-0.1.8/LICENSE
--rw-r--r--   0        0        0      732 2023-11-20 18:28:36.926374 seqpro-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      806 2023-11-20 18:28:36.930374 seqpro-0.1.8/seqpro/__init__.py
--rw-r--r--   0        0        0     5625 2023-11-20 00:40:06.807308 seqpro-0.1.8/seqpro/_analyzers.py
--rw-r--r--   0        0        0     1416 2023-11-06 04:11:08.485873 seqpro-0.1.8/seqpro/_cleaners.py
--rw-r--r--   0        0        0     5651 2023-11-20 00:40:18.743306 seqpro-0.1.8/seqpro/_encoders.py
--rw-r--r--   0        0        0     8229 2023-11-20 00:40:06.855308 seqpro-0.1.8/seqpro/_modifiers.py
--rw-r--r--   0        0        0     3517 2023-11-20 00:40:06.880308 seqpro-0.1.8/seqpro/_numba.py
--rw-r--r--   0        0        0     2661 2023-11-06 05:04:59.160101 seqpro-0.1.8/seqpro/_utils.py
--rw-r--r--   0        0        0     1458 2023-11-06 04:10:57.211876 seqpro-0.1.8/seqpro/alphabets/__init__.py
--rw-r--r--   0        0        0    10344 2023-11-20 00:40:18.747306 seqpro-0.1.8/seqpro/alphabets/_alphabets.py
--rw-r--r--   0        0        0     2504 2023-11-20 00:40:06.943307 seqpro-0.1.8/seqpro/deprecated/_analyzers.py
--rw-r--r--   0        0        0     1358 2023-11-20 00:40:06.945308 seqpro-0.1.8/seqpro/deprecated/_cleaners.py
--rw-r--r--   0        0        0     4364 2023-11-20 00:40:06.962308 seqpro-0.1.8/seqpro/deprecated/_encoders.py
--rw-r--r--   0        0        0     9481 2023-11-20 00:40:06.976307 seqpro-0.1.8/seqpro/deprecated/_helpers.py
--rw-r--r--   0        0        0     6113 2023-11-20 00:40:06.981308 seqpro-0.1.8/seqpro/deprecated/_modifiers.py
--rw-r--r--   0        0        0     1419 2023-11-20 00:40:06.992308 seqpro-0.1.8/seqpro/deprecated/_utils.py
--rw-r--r--   0        0        0     2914 2023-11-20 00:40:06.995308 seqpro-0.1.8/seqpro/experimental/_experimental.py
--rw-r--r--   0        0        0      773 2023-11-20 00:40:06.997308 seqpro-0.1.8/seqpro/experimental/_visualizers.py
--rw-r--r--   0        0        0     6509 2023-11-06 04:11:08.502873 seqpro-0.1.8/seqpro/xr/__init__.py
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 seqpro-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-11-20 00:42:49.906283 seqpro-0.1.9/LICENSE
+-rw-r--r--   0        0        0      732 2023-12-20 19:12:13.410645 seqpro-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      806 2023-12-20 19:12:13.414645 seqpro-0.1.9/seqpro/__init__.py
+-rw-r--r--   0        0        0     5625 2023-11-20 00:40:06.807308 seqpro-0.1.9/seqpro/_analyzers.py
+-rw-r--r--   0        0        0     1416 2023-11-06 04:11:08.485873 seqpro-0.1.9/seqpro/_cleaners.py
+-rw-r--r--   0        0        0     5651 2023-11-20 00:40:18.743306 seqpro-0.1.9/seqpro/_encoders.py
+-rw-r--r--   0        0        0    10214 2023-12-20 19:07:09.513744 seqpro-0.1.9/seqpro/_modifiers.py
+-rw-r--r--   0        0        0     3194 2023-12-20 19:06:17.824756 seqpro-0.1.9/seqpro/_numba.py
+-rw-r--r--   0        0        0     2661 2023-11-06 05:04:59.160101 seqpro-0.1.9/seqpro/_utils.py
+-rw-r--r--   0        0        0     1458 2023-11-06 04:10:57.211876 seqpro-0.1.9/seqpro/alphabets/__init__.py
+-rw-r--r--   0        0        0    10344 2023-11-20 00:40:18.747306 seqpro-0.1.9/seqpro/alphabets/_alphabets.py
+-rw-r--r--   0        0        0     2504 2023-11-20 00:40:06.943307 seqpro-0.1.9/seqpro/deprecated/_analyzers.py
+-rw-r--r--   0        0        0     1358 2023-11-20 00:40:06.945308 seqpro-0.1.9/seqpro/deprecated/_cleaners.py
+-rw-r--r--   0        0        0     4364 2023-11-20 00:40:06.962308 seqpro-0.1.9/seqpro/deprecated/_encoders.py
+-rw-r--r--   0        0        0     9481 2023-11-20 00:40:06.976307 seqpro-0.1.9/seqpro/deprecated/_helpers.py
+-rw-r--r--   0        0        0     6113 2023-11-20 00:40:06.981308 seqpro-0.1.9/seqpro/deprecated/_modifiers.py
+-rw-r--r--   0        0        0     1419 2023-11-20 00:40:06.992308 seqpro-0.1.9/seqpro/deprecated/_utils.py
+-rw-r--r--   0        0        0     2914 2023-11-20 00:40:06.995308 seqpro-0.1.9/seqpro/experimental/_experimental.py
+-rw-r--r--   0        0        0      773 2023-11-20 00:40:06.997308 seqpro-0.1.9/seqpro/experimental/_visualizers.py
+-rw-r--r--   0        0        0     6509 2023-11-06 04:11:08.502873 seqpro-0.1.9/seqpro/xr/__init__.py
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 seqpro-0.1.9/PKG-INFO
```

### Comparing `seqpro-0.1.8/LICENSE` & `seqpro-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/pyproject.toml` & `seqpro-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seqpro"
-version = "0.1.8"
+version = "0.1.9"
 description = "Sequence processing toolkit"
 authors = ["Adam Klie <aklie@ucsd.edu>", "David Laub <dlaub@ucsd.edu>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numba = "^0.57.0"
```

### Comparing `seqpro-0.1.8/seqpro/__init__.py` & `seqpro-0.1.9/seqpro/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ._analyzers import gc_content, length, nucleotide_content
 from ._cleaners import remove_N_seqs, remove_only_N_seqs, sanitize
 from ._encoders import decode_ohe, ohe, pad_seqs
 from ._modifiers import bin_coverage, jitter, k_shuffle, random_seqs, reverse_complement
 from ._utils import cast_seqs
 from .alphabets import AA, DNA, RNA, AminoAlphabet, NucleotideAlphabet
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 __all__ = [
     "cast_seqs",
     "bin_coverage",
     "gc_content",
     "length",
     "nucleotide_content",
```

### Comparing `seqpro-0.1.8/seqpro/_analyzers.py` & `seqpro-0.1.9/seqpro/_analyzers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/_cleaners.py` & `seqpro-0.1.9/seqpro/_cleaners.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/_encoders.py` & `seqpro-0.1.9/seqpro/_encoders.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/_modifiers.py` & `seqpro-0.1.9/seqpro/_modifiers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from enum import Enum
-from typing import Literal, Optional, Tuple, Union, cast
+from typing import List, Literal, Optional, Tuple, Union, cast
 
 import numpy as np
 from numpy.typing import NDArray
 
-from ._numba import gufunc_jitter_helper
 from ._utils import SeqType, _check_axes, cast_seqs
 from .alphabets._alphabets import NucleotideAlphabet
 
 
 def reverse_complement(
     seqs: SeqType,
     alphabet: NucleotideAlphabet,
@@ -95,15 +94,16 @@
             raise ValueError("Need an alphabet to process OHE sequences.")
         seqs = alphabet.decode_ohe(seqs, ohe_axis=ohe_axis)
     else:
         ohe = False
 
     length = seqs.shape[length_axis]
     with np.nditer(
-        seqs.view(f"S{length}").ravel(), op_flags=["readwrite"]  # type: ignore
+        seqs.view(f"S{length}").ravel(),
+        op_flags=["readwrite"],  # type: ignore
     ) as it:
         for seq in it:
             seq[...] = ushuffle.shuffle(seq.tobytes(), k)  # type: ignore
 
     if ohe:
         assert ohe_axis is not None
         assert alphabet is not None
@@ -154,15 +154,15 @@
     seed: Optional[int] = None,
 ):
     """Randomly jitter data from arrays, using the same jitter across arrays.
 
     Parameters
     ----------
     *arrays : NDArray
-        Arrays to be jittered. They must have the same sizez jitter and length
+        Arrays to be jittered. They must have the same sized jitter and length
         axes.
     max_jitter : int
         Maximum jitter amount.
     length_axis : int
     jitter_axes : Tuple[int, ...]
         Each slice along the jitter axes will be randomly jittered *independently*.
         Thus, if jitter_axes = 0, then every slice of data along axis 0 would be
@@ -171,45 +171,119 @@
     seed : Optional[int], optional
         Random seed, by default None
 
     Returns
     -------
     arrays
         Jittered arrays. Each will have a new length equal to length - 2*max_jitter.
+
+    Raises
+    ------
+    ValueError
+        If any arrays have insufficient length to be jittered.
     """
     if isinstance(jitter_axes, int):
         jitter_axes = (jitter_axes,)
 
-    destination_axes = list(range(-len(jitter_axes) - 1, 0))
-    arrays = tuple(
-        np.moveaxis(a, [*jitter_axes, length_axis], destination_axes) for a in arrays
-    )
-
-    jitter_axes_shape = arrays[0].shape[-len(destination_axes) : -1]
-    for arr in arrays:
-        if arr.shape[-len(destination_axes) : -1] != jitter_axes_shape:
-            raise ValueError("Got arrays with different sized jitter axes.")
+    # move jitter axes and length axis to back
+    arrays, destination_axes = _align_axes(*arrays, axes=(*jitter_axes, length_axis))
+    short_arrays = []
+    for i, arr in enumerate(arrays):
         if arr.shape[-1] - 2 * max_jitter <= 0:
-            raise ValueError("Jittered length is <= 0")
+            short_arrays.append(i)
+    if short_arrays:
+        raise ValueError(
+            f"Arrays {short_arrays} have insufficient length to be jittered with max_jitter={max_jitter}."
+        )
 
+    jittered_length = arrays[0].shape[-1] - 2 * max_jitter
+    jitter_axes_shape = arrays[0].shape[-len(jitter_axes) : -1]
     rng = np.random.default_rng(seed)
-    starts = rng.integers(0, max_jitter + 1, jitter_axes_shape)
+    starts = rng.integers(
+        0, arrays[0].shape[-1] - jittered_length + 1, jitter_axes_shape
+    )
 
-    sliced_arrs = []
+    sliced_arrs: List[NDArray] = []
     for arr in arrays:
-        jittered_length = arr.shape[-1] - 2 * max_jitter
-        sliced = np.empty_like(arr)
-        gufunc_jitter_helper(arr, starts, max_jitter, sliced, axis=-1)  # type: ignore
-        sliced = sliced[..., :jittered_length]
+        sliced = _slice_kmers(arr, starts, jittered_length)
         sliced = np.moveaxis(sliced, destination_axes, [*jitter_axes, length_axis])
         sliced_arrs.append(sliced)
 
     return tuple(sliced_arrs)
 
 
+def _align_axes(*arrays: NDArray, axes: Union[int, Tuple[int, ...]]):
+    """Align axes of arrays, moving them to the back while preserving order.
+
+    Parameters
+    ----------
+    *arrays : NDArray
+        Arrays to align axes of.
+    axes : Union[int, Tuple[int, ...]]
+        Axes to align.
+
+    Returns
+    -------
+    Tuple[NDArray]
+        Aligned arrays.
+    Tuple[int]
+        Destination axes.
+
+    Raises
+    ------
+    ValueError
+        If axes cannot be aligned because they have different sizes.
+    """
+    if isinstance(axes, int):
+        source_axes = (axes,)
+    else:
+        source_axes = axes
+
+    destination_axes = tuple(range(-len(source_axes), 0))
+    arrays = tuple(np.moveaxis(a, source_axes, destination_axes) for a in arrays)
+
+    first_axes_shape = arrays[0].shape[-len(destination_axes) : -1]
+    for arr in arrays:
+        if arr.shape[-len(destination_axes) : -1] != first_axes_shape:
+            raise ValueError("Can't align axes with different sizes.")
+
+    return arrays, destination_axes
+
+
+def _slice_kmers(array: NDArray, starts: NDArray, k: int):
+    """Slice an array into k-mers, assuming starts aligns with final axes of array and length is the final axis.
+
+    Parameters
+    ----------
+    array : NDArray
+        Array to slice.
+    starts : NDArray
+        Start indices of k-mers.
+    k : int
+        Size of k-mers.
+
+    Returns
+    -------
+    NDArray
+        Sliced array.
+    """
+    n_axes_sliced = starts.ndim
+    n_axes_not_sliced = array.ndim - n_axes_sliced - 1  # - 1 for length axis
+    idx: List[Union[slice, NDArray]] = [slice(None)] * n_axes_not_sliced
+    for i, size in enumerate(array.shape[-starts.ndim - 1 : -1]):
+        shape = np.ones(starts.ndim, dtype=np.uint32)
+        shape[i] = size
+        idx.append(np.arange(size, dtype=np.intp).reshape(shape))
+    idx.append(starts)
+
+    windows = np.lib.stride_tricks.sliding_window_view(array, k, axis=-1)
+    sliced = windows[tuple(idx)]
+    return sliced
+
+
 def random_seqs(
     shape: Union[int, Tuple[int, ...]],
     alphabet: NucleotideAlphabet,
     seed: Optional[int] = None,
 ):
     """Generate random nucleotide sequences.
```

### Comparing `seqpro-0.1.8/seqpro/_numba.py` & `seqpro-0.1.9/seqpro/_numba.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,18 +95,7 @@
         All amino acids corresponding to each codon, in matching order.
     res : NDArray[np.uint8], optional
         Array to save the result in, by default None
     """
     for i in nb.prange(len(codons)):
         if (seq == codons[i]).all():
             res[0] = aminos_acids[i]  # type: ignore
-
-
-@nb.guvectorize("(n),(),()->(n)", target="parallel", cache=True)
-def gufunc_jitter_helper(
-    arr: NDArray,
-    start: Union[int, NDArray[np.integer]],
-    max_jitter: Union[int, NDArray[np.integer]],
-    res: NDArray,
-):
-    new_length = len(arr) - 2 * max_jitter
-    res[:new_length] = arr[start : start + new_length]
```

### Comparing `seqpro-0.1.8/seqpro/_utils.py` & `seqpro-0.1.9/seqpro/_utils.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/alphabets/__init__.py` & `seqpro-0.1.9/seqpro/alphabets/__init__.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/alphabets/_alphabets.py` & `seqpro-0.1.9/seqpro/alphabets/_alphabets.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/deprecated/_analyzers.py` & `seqpro-0.1.9/seqpro/deprecated/_analyzers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/deprecated/_cleaners.py` & `seqpro-0.1.9/seqpro/deprecated/_cleaners.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/deprecated/_encoders.py` & `seqpro-0.1.9/seqpro/deprecated/_encoders.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/deprecated/_helpers.py` & `seqpro-0.1.9/seqpro/deprecated/_helpers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/deprecated/_modifiers.py` & `seqpro-0.1.9/seqpro/deprecated/_modifiers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/deprecated/_utils.py` & `seqpro-0.1.9/seqpro/deprecated/_utils.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/experimental/_experimental.py` & `seqpro-0.1.9/seqpro/experimental/_experimental.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/experimental/_visualizers.py` & `seqpro-0.1.9/seqpro/experimental/_visualizers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/seqpro/xr/__init__.py` & `seqpro-0.1.9/seqpro/xr/__init__.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.8/PKG-INFO` & `seqpro-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqpro
-Version: 0.1.8
+Version: 0.1.9
 Summary: Sequence processing toolkit
 License: MIT
 Author: Adam Klie
 Author-email: aklie@ucsd.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

