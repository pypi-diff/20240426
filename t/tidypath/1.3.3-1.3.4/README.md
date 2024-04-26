# Comparing `tmp/tidypath-1.3.3.tar.gz` & `tmp/tidypath-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidypath-1.3.3.tar", last modified: Wed Feb 21 23:01:45 2024, max compression
+gzip compressed data, was "tidypath-1.3.4.tar", last modified: Fri Apr 26 08:30:12 2024, max compression
```

## Comparing `tidypath-1.3.3.tar` & `tidypath-1.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-02-21 23:01:45.761416 tidypath-1.3.3/
--rwxr-xr-x   0 userx     (1000) wheel      (998)    35149 2023-06-08 21:46:44.000000 tidypath-1.3.3/LICENSE.md
--rw-r--r--   0 userx     (1000) wheel      (998)     3682 2024-02-21 23:01:45.761416 tidypath-1.3.3/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)     2804 2023-06-08 21:46:44.000000 tidypath-1.3.3/README.md
--rwxr-xr-x   0 userx     (1000) wheel      (998)      106 2024-02-21 23:01:45.761416 tidypath-1.3.3/setup.cfg
--rwxr-xr-x   0 userx     (1000) wheel      (998)     1161 2024-02-21 23:01:27.000000 tidypath-1.3.3/setup.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-02-21 23:01:45.761416 tidypath-1.3.3/tidypath/
--rwxr-xr-x   0 userx     (1000) wheel      (998)      371 2023-09-01 13:40:54.000000 tidypath-1.3.3/tidypath/__init__.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     1629 2023-06-08 21:46:44.000000 tidypath-1.3.3/tidypath/_helper.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     4998 2024-02-21 23:01:12.000000 tidypath-1.3.3/tidypath/config.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)    13663 2024-02-12 23:35:26.000000 tidypath-1.3.3/tidypath/decorators.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     6165 2023-07-01 08:06:57.000000 tidypath-1.3.3/tidypath/fmt.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     5197 2023-06-08 21:46:44.000000 tidypath-1.3.3/tidypath/inspection.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)    14158 2024-02-14 00:36:13.000000 tidypath-1.3.3/tidypath/paths.py
--rwxr-xr-x   0 userx     (1000) wheel      (998)     9844 2023-06-08 21:46:44.000000 tidypath-1.3.3/tidypath/storage.py
-drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-02-21 23:01:45.761416 tidypath-1.3.3/tidypath.egg-info/
--rwxr-xr-x   0 userx     (1000) wheel      (998)     3682 2024-02-21 23:01:45.000000 tidypath-1.3.3/tidypath.egg-info/PKG-INFO
--rwxr-xr-x   0 userx     (1000) wheel      (998)      358 2024-02-21 23:01:45.000000 tidypath-1.3.3/tidypath.egg-info/SOURCES.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-02-21 23:01:45.000000 tidypath-1.3.3/tidypath.egg-info/dependency_links.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)       63 2024-02-21 23:01:45.000000 tidypath-1.3.3/tidypath.egg-info/requires.txt
--rwxr-xr-x   0 userx     (1000) wheel      (998)        9 2024-02-21 23:01:45.000000 tidypath-1.3.3/tidypath.egg-info/top_level.txt
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-26 08:30:12.323393 tidypath-1.3.4/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    35149 2023-06-08 21:46:44.000000 tidypath-1.3.4/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     3682 2024-04-26 08:30:12.323393 tidypath-1.3.4/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     2804 2023-06-08 21:46:44.000000 tidypath-1.3.4/README.md
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      106 2024-04-26 08:30:12.323393 tidypath-1.3.4/setup.cfg
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     1161 2024-04-26 08:29:52.000000 tidypath-1.3.4/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-26 08:30:12.323393 tidypath-1.3.4/tidypath/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      371 2023-09-01 13:40:54.000000 tidypath-1.3.4/tidypath/__init__.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     1629 2023-06-08 21:46:44.000000 tidypath-1.3.4/tidypath/_helper.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     4998 2024-02-21 23:01:12.000000 tidypath-1.3.4/tidypath/config.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    14366 2024-04-26 08:29:43.000000 tidypath-1.3.4/tidypath/decorators.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     6165 2023-07-01 08:06:57.000000 tidypath-1.3.4/tidypath/fmt.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     5197 2023-06-08 21:46:44.000000 tidypath-1.3.4/tidypath/inspection.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)    14158 2024-02-14 00:36:13.000000 tidypath-1.3.4/tidypath/paths.py
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     9844 2023-06-08 21:46:44.000000 tidypath-1.3.4/tidypath/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-04-26 08:30:12.323393 tidypath-1.3.4/tidypath.egg-info/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     3682 2024-04-26 08:30:12.000000 tidypath-1.3.4/tidypath.egg-info/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      358 2024-04-26 08:30:12.000000 tidypath-1.3.4/tidypath.egg-info/SOURCES.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-04-26 08:30:12.000000 tidypath-1.3.4/tidypath.egg-info/dependency_links.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)       63 2024-04-26 08:30:12.000000 tidypath-1.3.4/tidypath.egg-info/requires.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        9 2024-04-26 08:30:12.000000 tidypath-1.3.4/tidypath.egg-info/top_level.txt
```

### Comparing `tidypath-1.3.3/LICENSE.md` & `tidypath-1.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.3/PKG-INFO` & `tidypath-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.3.3
+Version: 1.3.4
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tidypath-1.3.3/README.md` & `tidypath-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.3/setup.py` & `tidypath-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tidypath',
-    version='1.3.3',
+    version='1.3.4',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=['tidypath'],
     url='https://github.com/medinajorge/tidypath',
     download_url='https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz',
     description="Automatically store/load data in a tidy, efficient way.",
     long_description=open('README.md').read(),
```

### Comparing `tidypath-1.3.3/tidypath/_helper.py` & `tidypath-1.3.4/tidypath/_helper.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.3/tidypath/config.py` & `tidypath-1.3.4/tidypath/config.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.3/tidypath/decorators.py` & `tidypath-1.3.4/tidypath/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                                                  "pos_only"         =>  length of *args
                                                  "args"             =>  attrs != **kwargs, *args.
                                                  "all"              if config.KEYS_ADD_POSONLY_TO_ALL  =>  all attrs
                                                                     else                               =>  all attrs except pos_only: kwargs_full + args
                                                  can combine options using "+" or "-". Example: "args+z", "x+y+kwargs", "all-y".
                                      · iterable: containing a combination of the available string keys (above). ["k1", "k2"] == "k1+k2".
         - skip_computation (bool).     whether to skip computation if the data is not stored.
-        - ext:                     storing extension. Selects 'storage' functions save_ext, load_ext.
+        - ext (str/list/tuple):    storing extension. Selects 'storage' functions save_ext, load_ext.
                                    Supported: 'lzma' (default), 'bz2', 'json', 'csv', 'npz'.
 
 
     Attrs:
         - function:                function to which the decorator is applied
         - include_classes:         include class tree in saving_path.
         - load_opts:               kws for storage.load_ext. default kws are those of 'saving_options', those specified update saving_options dict.
@@ -91,52 +91,59 @@
         load_opts = {**save_opts, **load_opts}
 
     def _savedata(func):
         @wraps(func)
         def wrapper(*args, overwrite=overwrite, keys=keys, save=save, funcname_in_filename=funcname_in_filename, skip_computation=skip_computation, ext=ext, **kwargs):
             key_opts = classify_call_attrs(func, args, kwargs, add_pos_only_to_all=config.KEYS_ADD_POSONLY_TO_ALL)
             save_keys = merge_nested_dict(key_opts, keys, key_default="all")
-            saving_path = datapath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename, iterable_maxsize=iterable_maxsize)
-            filename = os.path.basename(saving_path)
 
-            filename_too_long = len(filename) > max_str_length
-            if filename_too_long:
-                saving_path = hash_path(saving_path)
-
-            if skip_computation and not Path(saving_path).exists():
-                warnings.warn("Skipping computation. Data not stored.", RuntimeWarning)
-                return SavedataSkippedComputation()
-
-            elif Path(saving_path).exists() and not overwrite:
-                try:
-                    result = getattr(storage, f"load_{ext}")(saving_path, **load_opts)
-                except EOFError or LZMAError or _lzma.LZMAError:
-                    if skip_computation:
-                        warnings.warn("Corrupted file. Skipping computation ...", RuntimeWarning)
-                        return SavedataSkippedComputation()
-                    else:
-                        warnings.warn("Corrupted file. Recomputing and storing ...", RuntimeWarning)
-                        result = func(*args, **kwargs)
-                        getattr(storage, f"save_{ext}")(result, saving_path, **save_opts)
-                except KeyboardInterrupt:
-                    raise KeyboardInterrupt
-                except Exception as e:
-                    print(e)
-                    if skip_computation:
-                        warnings.warn("Corrupted file. Skipping computation ...", RuntimeWarning)
-                        return SavedataSkippedComputation()
-                    else:
-                        warnings.warn("Corrupted file. Recomputing and storing ...", RuntimeWarning)
-                        result = func(*args, **kwargs)
-                        getattr(storage, f"save_{ext}")(result, saving_path, **save_opts)
-            else:
-                if filename_too_long:
+            def get_saving_path(ext):
+                saving_path = datapath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename, iterable_maxsize=iterable_maxsize)
+                filename = os.path.basename(saving_path)
+                if len(filename) > max_str_length:
+                    saving_path = hash_path(saving_path)
                     warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
-                result = func(*args, **kwargs)
+                return saving_path
+
+            result = None
+            def compute_and_save(result, ext, saving_path):
+                if result is not None:
+                    result = func(*args, **kwargs)
                 getattr(storage, f"save_{ext}")(result, saving_path, **save_opts)
+                return result
+
+            if isinstance(ext, str):
+                ext = [ext]
+            for ext_i in ext:
+                saving_path = get_saving_path(ext_i)
+                if skip_computation and not Path(saving_path).exists():
+                    warnings.warn("Skipping computation. Data not stored.", RuntimeWarning)
+                    return SavedataSkippedComputation()
+                elif Path(saving_path).exists() and not overwrite:
+                    try:
+                        result = getattr(storage, f"load_{ext}")(saving_path, **load_opts)
+                    except EOFError or LZMAError or _lzma.LZMAError:
+                        if skip_computation:
+                            warnings.warn("Corrupted file. Skipping computation ...", RuntimeWarning)
+                            return SavedataSkippedComputation()
+                        else:
+                            warnings.warn("Corrupted file. Recomputing and storing ...", RuntimeWarning)
+                            result = compute_and_save(result, ext_i, saving_path)
+                    except KeyboardInterrupt:
+                        raise KeyboardInterrupt
+                    except Exception as e:
+                        print(e)
+                        if skip_computation:
+                            warnings.warn("Corrupted file. Skipping computation ...", RuntimeWarning)
+                            return SavedataSkippedComputation()
+                        else:
+                            warnings.warn("Corrupted file. Recomputing and storing ...", RuntimeWarning)
+                            result = compute_and_save(result, ext_i, saving_path)
+                else:
+                    result = compute_and_save(result, ext_i, saving_path)
             return result
 
         wrapper.__signature__ = merge_wrapper_signatures(wrapper, ["overwrite", "keys", "save", "funcname_in_filename", "skip_computation", "ext"])
         wrapper.__out__ = "data"
         return wrapper
 
     if func is None:
@@ -171,15 +178,15 @@
                                                  "kwargs_full"      =>  kws_defaults + kws.
                                                  "pos_only"         =>  length of *args. Also self and cls are counted as pos_only arguments.
                                                  "args"             =>  attrs != **kwargs, *args.
                                                  "all"              if config.KEYS_ADD_POSONLY_TO_ALL  =>  all attrs
                                                                     else                               =>  all attrs except pos_only: kwargs_full + args
                                                  can combine options using "+" or "-". Example: "args+z", "x+y+kwargs", "all-y".
                                      · iterable: containing a combination of the available string keys (above). ["k1", "k2"] == "k1+k2".
-        - ext:                     storing extension. 'eps' recommended for articles.
+        - ext (str/list/tuple):    Storing extension. 'pdf' recommended for articles.
                                    Supported: any extension supported by matplotlib/plotly. Example: 'png', 'eps', 'html' (plotly), etc.
 
 
     Attrs:
         - function:                function to which the decorator is applied
         - include_classes:         include class tree in saving_path.
         - save_opts:               kws for saving function.
@@ -203,34 +210,43 @@
         @wraps(func)
         def wrapper(*args, overwrite=overwrite, keys=keys, save=save, return_fig=return_fig, funcname_in_filename=funcname_in_filename, ext=ext, **kwargs):
             fig = func(*args, **kwargs)
             is_mpl_axes = type(fig).__name__ == 'AxesSubplot'
             if isinstance(fig, (mpl_figure, plotly_figure)) or is_mpl_axes:
                 key_opts = classify_call_attrs(func, args, kwargs, add_pos_only_to_all=config.KEYS_ADD_POSONLY_TO_ALL)
                 save_keys = merge_nested_dict(key_opts, keys, key_default="all")
-                saving_path = figpath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename, iterable_maxsize=iterable_maxsize)
-                filename = os.path.basename(saving_path)
-
-                if len(filename) > max_str_length:
-                    saving_path = hash_path(saving_path)
-                    warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
-
-                if not Path(saving_path).exists() or overwrite:
-                    if is_mpl_axes:
-                        fig = fig.get_figure()
-                    if isinstance(fig, mpl_figure):
-                        fig.savefig(saving_path, format=ext, **{**mpl_save_defaults, **save_opts})
-                        plt.close(fig)
-                    elif isinstance(fig, plotly_figure):
-                        if ext == "html":
-                            fig.write_html(saving_path, **save_opts)
+                def get_saving_path(ext):
+                    saving_path = figpath(keys=save_keys, func=func, ext=ext, include_classes=include_classes, funcname_in_filename=funcname_in_filename, iterable_maxsize=iterable_maxsize)
+                    filename = os.path.basename(saving_path)
+                    if len(filename) > max_str_length:
+                        saving_path = hash_path(saving_path)
+                        warnings.warn("Filename too long. Hashing it ...", RuntimeWarning)
+                    return saving_path
+
+                if is_mpl_axes:
+                    fig = fig.get_figure()
+                is_mpl = isinstance(fig, mpl_figure)
+
+                if isinstance(ext, str):
+                    ext = [ext]
+                for ext_i in ext:
+                    saving_path = get_saving_path(ext_i)
+                    if not Path(saving_path).exists() or overwrite:
+                        if is_mpl:
+                            fig.savefig(saving_path, format=ext_i, **{**mpl_save_defaults, **save_opts})
+                        elif isinstance(fig, plotly_figure):
+                            if ext_i == "html":
+                                fig.write_html(saving_path, **save_opts)
+                            else:
+                                fig.write_image(saving_path, format=ext_i, **save_opts)
                         else:
-                            fig.write_image(saving_path, format=ext, **save_opts)
-                    else:
-                        raise TypeError(f"fig type '{type(fig)}' not valid. Available: 'matplotlib.figure.Figure', 'matplotlib.axes._subplots.AxesSubplot', 'plotly.grap_objs._figure.Figure'.")
+                            raise TypeError(f"fig type '{type(fig)}' not valid. Available: 'matplotlib.figure.Figure', 'matplotlib.axes._subplots.AxesSubplot', 'plotly.grap_objs._figure.Figure'.")
+
+                if is_mpl:
+                    plt.close(fig)
 
                 if return_fig:
                     return fig
                 else:
                     return
             elif fig is None or math.isnan(fig):
                 warnings.warn("Expected output figure (plotly or matplotlib) and received None or NaN.", RuntimeWarning)
```

### Comparing `tidypath-1.3.3/tidypath/fmt.py` & `tidypath-1.3.4/tidypath/fmt.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.3/tidypath/inspection.py` & `tidypath-1.3.4/tidypath/inspection.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.3/tidypath/paths.py` & `tidypath-1.3.4/tidypath/paths.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.3/tidypath/storage.py` & `tidypath-1.3.4/tidypath/storage.py`

 * *Files identical despite different names*

### Comparing `tidypath-1.3.3/tidypath.egg-info/PKG-INFO` & `tidypath-1.3.4/tidypath.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidypath
-Version: 1.3.3
+Version: 1.3.4
 Summary: Automatically store/load data in a tidy, efficient way.
 Home-page: https://github.com/medinajorge/tidypath
 Download-URL: https://github.com/medinajorge/tidypath/archive/refs/tags/v1.0.5.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

