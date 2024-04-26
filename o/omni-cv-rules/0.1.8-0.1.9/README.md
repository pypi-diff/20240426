# Comparing `tmp/omni-cv-rules-0.1.8.tar.gz` & `tmp/omni-cv-rules-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omni-cv-rules-0.1.8.tar", max compression
+gzip compressed data, was "omni-cv-rules-0.1.9.tar", max compression
```

## Comparing `omni-cv-rules-0.1.8.tar` & `omni-cv-rules-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        0 2022-01-27 06:37:55.360724 omni-cv-rules-0.1.8/omni_cv_rules/__init__.py
--rw-r--r--   0        0        0    46245 2022-03-03 14:39:41.016373 omni-cv-rules-0.1.8/omni_cv_rules/coconut/__coconut__.py
--rw-r--r--   0        0        0     2638 2022-01-27 07:27:01.109116 omni-cv-rules-0.1.8/omni_cv_rules/coconut/__init__.py
--rw-r--r--   0        0        0    52610 2022-03-03 15:19:50.509177 omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/__coconut__.cpython-39.pyc
--rw-r--r--   0        0        0     2265 2022-01-27 18:37:13.408714 omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    51445 2022-03-03 15:19:50.519779 omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/convert.cpython-39.pyc
--rw-r--r--   0        0        0    42515 2022-03-03 15:19:50.576569 omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/omni_converter.cpython-39.pyc
--rw-r--r--   0        0        0     3594 2022-01-28 06:59:38.849345 omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/recursive.cpython-39.pyc
--rw-r--r--   0        0        0     3504 2022-01-27 18:37:35.972077 omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/to_bytes.cpython-39.pyc
--rw-r--r--   0        0        0     8294 2022-01-27 18:37:35.899795 omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/visualization.cpython-39.pyc
--rw-r--r--   0        0        0     3376 2022-01-27 18:37:35.973025 omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/widgets.cpython-39.pyc
--rw-r--r--   0        0        0   189401 2022-03-03 14:39:41.013316 omni-cv-rules-0.1.8/omni_cv_rules/coconut/convert.py
--rw-r--r--   0        0        0   146030 2022-03-03 13:08:33.253396 omni-cv-rules-0.1.8/omni_cv_rules/coconut/omni_converter.py
--rw-r--r--   0        0        0     4576 2022-01-28 06:43:58.194510 omni-cv-rules-0.1.8/omni_cv_rules/coconut/recursive.py
--rw-r--r--   0        0        0     4935 2022-01-27 07:27:01.098044 omni-cv-rules-0.1.8/omni_cv_rules/coconut/to_bytes.py
--rw-r--r--   0        0        0     3180 2022-01-28 15:00:43.221077 omni-cv-rules-0.1.8/omni_cv_rules/coconut/torch_rules.py
--rw-r--r--   0        0        0    21561 2022-01-27 14:24:24.368759 omni-cv-rules-0.1.8/omni_cv_rules/coconut/visualization.py
--rw-r--r--   0        0        0     4139 2022-01-27 16:59:29.980600 omni-cv-rules-0.1.8/omni_cv_rules/coconut/widgets.py
--rw-r--r--   0        0        0     1206 2022-01-28 13:56:49.893570 omni-cv-rules-0.1.8/omni_cv_rules/custom_rules.py
--rw-r--r--   0        0        0        0 2022-02-02 17:10:38.198461 omni-cv-rules-0.1.8/omni_cv_rules/image_ops.py
--rw-r--r--   0        0        0     2950 2022-03-02 17:47:11.514558 omni-cv-rules-0.1.8/omni_cv_rules/nrm_quiver.py
--rw-r--r--   0        0        0        0 2022-01-28 14:43:42.590842 omni-cv-rules-0.1.8/omni_cv_rules/place_holder/__init__.py
--rw-r--r--   0        0        0      331 2022-01-28 15:07:30.640035 omni-cv-rules-0.1.8/omni_cv_rules/place_holder/torch_proxy.py
--rw-r--r--   0        0        0        0 2022-01-28 14:03:11.735617 omni-cv-rules-0.1.8/omni_cv_rules/py_310/__init__.py
--rw-r--r--   0        0        0        0 2022-01-28 14:06:48.525680 omni-cv-rules-0.1.8/omni_cv_rules/py_38/__init__.py
--rw-r--r--   0        0        0     2364 2022-01-28 14:31:19.334394 omni-cv-rules-0.1.8/omni_cv_rules/py_38/torch_rules.py
--rw-r--r--   0        0        0     3776 2022-03-03 13:25:39.023693 omni-cv-rules-0.1.8/omni_cv_rules/rulebook.py
--rw-r--r--   0        0        0      461 2022-03-04 17:17:33.015618 omni-cv-rules-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      794 2022-03-04 17:17:35.235932 omni-cv-rules-0.1.8/setup.py
--rw-r--r--   0        0        0      616 2022-03-04 17:17:35.236105 omni-cv-rules-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-01-27 06:37:55.360724 omni-cv-rules-0.1.9/omni_cv_rules/__init__.py
+-rw-r--r--   0        0        0    46245 2022-03-03 14:39:41.016373 omni-cv-rules-0.1.9/omni_cv_rules/coconut/__coconut__.py
+-rw-r--r--   0        0        0     2638 2022-01-27 07:27:01.109116 omni-cv-rules-0.1.9/omni_cv_rules/coconut/__init__.py
+-rw-r--r--   0        0        0    52610 2022-03-03 15:19:50.509177 omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/__coconut__.cpython-39.pyc
+-rw-r--r--   0        0        0     2265 2022-01-27 18:37:13.408714 omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    51445 2022-03-03 15:19:50.519779 omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/convert.cpython-39.pyc
+-rw-r--r--   0        0        0    42515 2022-03-03 15:19:50.576569 omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/omni_converter.cpython-39.pyc
+-rw-r--r--   0        0        0     3594 2022-01-28 06:59:38.849345 omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/recursive.cpython-39.pyc
+-rw-r--r--   0        0        0     3504 2022-01-27 18:37:35.972077 omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/to_bytes.cpython-39.pyc
+-rw-r--r--   0        0        0     8294 2022-01-27 18:37:35.899795 omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/visualization.cpython-39.pyc
+-rw-r--r--   0        0        0     3376 2022-01-27 18:37:35.973025 omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/widgets.cpython-39.pyc
+-rw-r--r--   0        0        0   189401 2022-03-03 14:39:41.013316 omni-cv-rules-0.1.9/omni_cv_rules/coconut/convert.py
+-rw-r--r--   0        0        0   146030 2022-03-03 13:08:33.253396 omni-cv-rules-0.1.9/omni_cv_rules/coconut/omni_converter.py
+-rw-r--r--   0        0        0     4576 2022-01-28 06:43:58.194510 omni-cv-rules-0.1.9/omni_cv_rules/coconut/recursive.py
+-rw-r--r--   0        0        0     4935 2022-01-27 07:27:01.098044 omni-cv-rules-0.1.9/omni_cv_rules/coconut/to_bytes.py
+-rw-r--r--   0        0        0     3180 2022-01-28 15:00:43.221077 omni-cv-rules-0.1.9/omni_cv_rules/coconut/torch_rules.py
+-rw-r--r--   0        0        0    21561 2022-01-27 14:24:24.368759 omni-cv-rules-0.1.9/omni_cv_rules/coconut/visualization.py
+-rw-r--r--   0        0        0     4139 2022-01-27 16:59:29.980600 omni-cv-rules-0.1.9/omni_cv_rules/coconut/widgets.py
+-rw-r--r--   0        0        0     1254 2022-03-08 11:17:53.057278 omni-cv-rules-0.1.9/omni_cv_rules/custom_rules.py
+-rw-r--r--   0        0        0        0 2022-02-02 17:10:38.198461 omni-cv-rules-0.1.9/omni_cv_rules/image_ops.py
+-rw-r--r--   0        0        0     2950 2022-03-02 17:47:11.514558 omni-cv-rules-0.1.9/omni_cv_rules/nrm_quiver.py
+-rw-r--r--   0        0        0        0 2022-01-28 14:43:42.590842 omni-cv-rules-0.1.9/omni_cv_rules/place_holder/__init__.py
+-rw-r--r--   0        0        0      331 2022-01-28 15:07:30.640035 omni-cv-rules-0.1.9/omni_cv_rules/place_holder/torch_proxy.py
+-rw-r--r--   0        0        0        0 2022-01-28 14:03:11.735617 omni-cv-rules-0.1.9/omni_cv_rules/py_310/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-28 14:06:48.525680 omni-cv-rules-0.1.9/omni_cv_rules/py_38/__init__.py
+-rw-r--r--   0        0        0     2364 2022-01-28 14:31:19.334394 omni-cv-rules-0.1.9/omni_cv_rules/py_38/torch_rules.py
+-rw-r--r--   0        0        0     3814 2022-03-08 11:18:43.423248 omni-cv-rules-0.1.9/omni_cv_rules/rulebook.py
+-rw-r--r--   0        0        0      461 2022-03-08 11:20:08.214956 omni-cv-rules-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      794 2022-03-08 11:20:19.086902 omni-cv-rules-0.1.9/setup.py
+-rw-r--r--   0        0        0      616 2022-03-08 11:20:19.087050 omni-cv-rules-0.1.9/PKG-INFO
```

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/__coconut__.py` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/__init__.py` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/__coconut__.cpython-39.pyc` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/__coconut__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/__init__.cpython-39.pyc` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/convert.cpython-39.pyc` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/convert.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/omni_converter.cpython-39.pyc` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/omni_converter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/recursive.cpython-39.pyc` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/recursive.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/to_bytes.cpython-39.pyc` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/to_bytes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/visualization.cpython-39.pyc` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/visualization.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/__pycache__/widgets.cpython-39.pyc` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/__pycache__/widgets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/convert.py` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/convert.py`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/omni_converter.py` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/omni_converter.py`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/recursive.py` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/recursive.py`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/to_bytes.py` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/to_bytes.py`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/torch_rules.py` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/torch_rules.py`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/visualization.py` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/visualization.py`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/coconut/widgets.py` & `omni-cv-rules-0.1.9/omni_cv_rules/coconut/widgets.py`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/custom_rules.py` & `omni-cv-rules-0.1.9/omni_cv_rules/custom_rules.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,12 +41,12 @@
         else:
             return repr(item)
 
     formatters = {k: _formatter for k in df.columns}
     return df.to_html(escape=False, formatters=formatters)
 
 
-custom_rule_book = AutoRuleBook().add_rules(
+custom_rule_book = AutoRuleBook(id="custom_rule_book").add_rules(
     pil_img_to_base64,
     base64_png_to_html,
     custom_dataframe_viz
-).add_alias("html", "_repr_html_").add_alias("base64","base64_png")
+).add_alias("html", "_repr_html_").add_alias("base64","base64_png").set_id("custom_rule_book")
```

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/nrm_quiver.py` & `omni-cv-rules-0.1.9/omni_cv_rules/nrm_quiver.py`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/py_38/torch_rules.py` & `omni-cv-rules-0.1.9/omni_cv_rules/py_38/torch_rules.py`

 * *Files identical despite different names*

### Comparing `omni-cv-rules-0.1.8/omni_cv_rules/rulebook.py` & `omni-cv-rules-0.1.9/omni_cv_rules/rulebook.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         return [RuleEdge(
             converter = lambda img:img.convert("HSV"),
             new_format="image,HSV,HSV",
             cost=1,
             name=f"PIL RGB to PIL HSV"
         )]
 
-CV_RULEBOOK = AutoRuleBook().add_rules(
+CV_RULEBOOK = AutoRuleBook(id="CV_RULEBOOK").add_rules(
     imdef_neighbors,
     rule_xyz_to_rgb,
     rule_batch_xyz_to_rgb,
     rule_VR_None_to_normalized,
     rule_add_channel,
     rule_swap_RGB_BGR,
     create_cast_rule(cast_imdef_to_dict, "cast_imdef_to_dict"),
@@ -79,8 +79,8 @@
     # AutoSolver.create_conversion_rule(intra_tuple_conversions),
     create_conversion_rule(rule_to_spectrum),
     create_conversion_rule(auto_tuple2widget),
     create_alias_rule("numpy_rgb", "numpy,uint8,HWC,RGB,0_255"),
     create_alias_rule("numpy_rgba", "numpy,uint8,HWC,RGBA,0_255"),
 ) + custom_rule_book.add_recursive_rule(
     intra_list_conversions
-)
+).set_id("CV_RULEBOOK")
```

### Comparing `omni-cv-rules-0.1.8/setup.py` & `omni-cv-rules-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'numpy',
  'pandas',
  'pprintpp',
  'py-omni-converter']
 
 setup_kwargs = {
     'name': 'omni-cv-rules',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': None,
     'author': 'Kento Masui',
     'author_email': 'nameissoap@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `omni-cv-rules-0.1.8/PKG-INFO` & `omni-cv-rules-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-cv-rules
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Kento Masui
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

