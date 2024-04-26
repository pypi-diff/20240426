# Comparing `tmp/relib-1.0.5-py3-none-any.whl.zip` & `tmp/relib-1.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8646 bytes, number of entries: 10
--rw-r--r--  2.0 unx      456 b- defN 23-Oct-06 12:23 relib/__init__.py
+Zip file size: 8701 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      471 b- defN 24-Apr-26 09:50 relib/__init__.py
 -rw-r--r--  2.0 unx     8943 b- defN 23-Jan-21 17:58 relib/hashing.py
 -rw-r--r--  2.0 unx      555 b- defN 23-Jan-21 18:12 relib/measure_duration.py
 -rw-r--r--  2.0 unx     1905 b- defN 23-Jan-21 17:58 relib/raypipe.py
--rw-r--r--  2.0 unx     5258 b- defN 23-Oct-06 12:23 relib/utils.py
--rw-r--r--  2.0 unx     1054 b- defN 23-Oct-06 12:23 relib-1.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      260 b- defN 23-Oct-06 12:23 relib-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Oct-06 12:23 relib-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Oct-06 12:23 relib-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      749 b- defN 23-Oct-06 12:23 relib-1.0.5.dist-info/RECORD
-10 files, 19278 bytes uncompressed, 7382 bytes compressed:  61.7%
+-rw-r--r--  2.0 unx     5353 b- defN 24-Apr-26 09:50 relib/utils.py
+-rw-r--r--  2.0 unx     1054 b- defN 24-Apr-26 09:52 relib-1.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      260 b- defN 24-Apr-26 09:52 relib-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 09:52 relib-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-26 09:52 relib-1.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      749 b- defN 24-Apr-26 09:52 relib-1.0.6.dist-info/RECORD
+10 files, 19388 bytes uncompressed, 7437 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: relib/raypipe.py
 Comment: 
 
 Filename: relib/utils.py
 Comment: 
 
-Filename: relib-1.0.5.dist-info/LICENSE.txt
+Filename: relib-1.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: relib-1.0.5.dist-info/METADATA
+Filename: relib-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: relib-1.0.5.dist-info/WHEEL
+Filename: relib-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: relib-1.0.5.dist-info/top_level.txt
+Filename: relib-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: relib-1.0.5.dist-info/RECORD
+Filename: relib-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## relib/__init__.py

```diff
@@ -1,12 +1,13 @@
 from .utils import (
   list_split,
   drop_none,
   distinct,
-  find,
+  first,
+  move_value,
   transpose_dict,
   make_combinations_by_dict,
   merge_dicts,
   intersect,
   ensure_tuple,
   key_of,
   omit,
```

## relib/utils.py

```diff
@@ -18,17 +18,22 @@
 
 def drop_none(l: Iterable[Union[T, None]]) -> list[T]:
   return [x for x in l if x is not None]
 
 def distinct(items: Iterable[T]) -> list[T]:
   return list(set(items))
 
-def find(iterable: Iterable[T]) -> Union[T, None]:
+def first(iterable: Iterable[T]) -> Union[T, None]:
   return next(iter(iterable), None)
 
+def move_value(l: Iterable[T], from_i: int, to_i: int) -> list[T]:
+  l = list(l)
+  l.insert(to_i, l.pop(from_i))
+  return l
+
 def transpose_dict(des):
   if isinstance(des, list):
     keys = list(des[0].keys()) if des else []
     length = len(des)
     return {
       key: [des[i][key] for i in range(length)]
       for key in keys
@@ -144,23 +149,22 @@
   dim_labels: list[tuple[str, list[Union[str, int, float]]]],
   indexed=False,
 ):
   import pandas as pd
   dim_names = [name for name, _ in dim_labels]
   dim_sizes = np.array([len(labels) for _, labels in dim_labels])
   assert all(array.shape == tuple(dim_sizes) for array in value_cols.values())
-  repeats_tiles = [
+  array_offsets = [
     (dim_sizes[i + 1:].prod(), dim_sizes[:i].prod())
     for i in range(len(dim_sizes))
   ]
-  label_arrays = [
-    _cat_tile(pd.Categorical(labels).repeat(repeats), tiles)
-    for labels, (repeats, tiles) in zip(dim_labels, repeats_tiles)
-  ]
-  category_cols = dict(zip(dim_names, label_arrays))
+  category_cols = {
+    dim: _cat_tile(pd.Categorical(labels).repeat(repeats), tiles)
+    for dim, labels, (repeats, tiles) in zip(dim_names, dim_labels, array_offsets)
+  }
   value_cols = {name: array.reshape(-1) for name, array in value_cols.items()}
   df = pd.DataFrame({**category_cols, **value_cols}, copy=False)
   if indexed:
     df = df.set_index(dim_names)
   return df
 
 StrFilter = Callable[[str], bool]
```

## Comparing `relib-1.0.5.dist-info/LICENSE.txt` & `relib-1.0.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `relib-1.0.5.dist-info/RECORD` & `relib-1.0.6.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-relib/__init__.py,sha256=Zm6aMrr9A70laX2otqq60JLSO9bLiiwIQQJmk2Qzp_k,456
+relib/__init__.py,sha256=4yr8xPi3VMbiFlApussB4OXU_U6wzhje06qD0Ad3Gq4,471
 relib/hashing.py,sha256=6iAPRiJI_4jaSooZRFJnqK2limXqTmErzcwpd050LAA,8943
 relib/measure_duration.py,sha256=jJa5Kh5FxaBysS__nkwqcnTt8Uc2niLucXfTzFE0j-E,555
 relib/raypipe.py,sha256=ynEoXs1dnD-360_uQC8v89xjiilt3knpocXpFaQ3plA,1905
-relib/utils.py,sha256=Gh_Mb1z8FyzsPAsdCiNLUskztr16ajSrvzQ_lvAn_Tk,5258
-relib-1.0.5.dist-info/LICENSE.txt,sha256=t9LfkVbmcvZjP0x3Sq-jR38UfTNbNtRQvc0Q8HWmLak,1054
-relib-1.0.5.dist-info/METADATA,sha256=a8d2h8VbXerVegSy2fq3gpWhyHubrfs5UVQKz7Ybqls,260
-relib-1.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-relib-1.0.5.dist-info/top_level.txt,sha256=Yc96FwkbRYj4AQVatga8uK4hH9ATKI9XIyEH_1ba6KQ,6
-relib-1.0.5.dist-info/RECORD,,
+relib/utils.py,sha256=JM68czDzWLOa2ADbBEdAb7j4Zv3RFYMws5sy0ghxbW0,5353
+relib-1.0.6.dist-info/LICENSE.txt,sha256=t9LfkVbmcvZjP0x3Sq-jR38UfTNbNtRQvc0Q8HWmLak,1054
+relib-1.0.6.dist-info/METADATA,sha256=NVAMcPbnJrlRd_W8QRuX93F-gHSg47L9dGBf5ap7tnw,260
+relib-1.0.6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+relib-1.0.6.dist-info/top_level.txt,sha256=Yc96FwkbRYj4AQVatga8uK4hH9ATKI9XIyEH_1ba6KQ,6
+relib-1.0.6.dist-info/RECORD,,
```

