# Comparing `tmp/onekit-1.0.0.tar.gz` & `tmp/onekit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onekit-1.0.0.tar", max compression
+gzip compressed data, was "onekit-1.1.0.tar", max compression
```

## Comparing `onekit-1.0.0.tar` & `onekit-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1514 2024-04-01 17:43:00.839363 onekit-1.0.0/LICENSE
--rw-r--r--   0        0        0     1569 2024-04-01 17:43:00.839363 onekit-1.0.0/README.md
--rw-r--r--   0        0        0     2204 2024-04-01 17:43:55.335367 onekit-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       88 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/__init__.py
--rw-r--r--   0        0        0     3965 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/mathkit.py
--rw-r--r--   0        0        0     1643 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/numpykit.py
--rw-r--r--   0        0        0    14598 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/optfunckit.py
--rw-r--r--   0        0        0     6799 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/pandaskit.py
--rw-r--r--   0        0        0    35788 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/pythonkit.py
--rw-r--r--   0        0        0    37356 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/sparkkit.py
--rw-r--r--   0        0        0    20081 2024-04-01 17:43:00.883363 onekit-1.0.0/src/onekit/vizkit.py
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 onekit-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1514 2024-04-26 19:17:18.569475 onekit-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1569 2024-04-26 19:17:18.569475 onekit-1.1.0/README.md
+-rw-r--r--   0        0        0     2204 2024-04-26 19:18:12.657121 onekit-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-04-26 19:17:18.609475 onekit-1.1.0/src/onekit/__init__.py
+-rw-r--r--   0        0        0     3965 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/mathkit.py
+-rw-r--r--   0        0        0     1643 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/numpykit.py
+-rw-r--r--   0        0        0    14598 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/optfunckit.py
+-rw-r--r--   0        0        0     6799 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/pandaskit.py
+-rw-r--r--   0        0        0    37190 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/pythonkit.py
+-rw-r--r--   0        0        0    37388 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/sparkkit.py
+-rw-r--r--   0        0        0    19542 2024-04-26 19:17:18.613475 onekit-1.1.0/src/onekit/vizkit.py
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 onekit-1.1.0/PKG-INFO
```

### Comparing `onekit-1.0.0/LICENSE` & `onekit-1.1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023 Eugen Stripling
+Copyright (c) 2024 Eugen Stripling
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `onekit-1.0.0/README.md` & `onekit-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `onekit-1.0.0/pyproject.toml` & `onekit-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onekit"
-version = "1.0.0"
+version = "1.1.0"
 description = "All-in-One Python Kit."
 authors = ["Eugen Stripling <estripling042@gmail.com>"]
 license = "BSD 3-Clause"
 readme = "README.md"
 repository = "https://github.com/estripling/onekit"
 documentation = "https://onekit.readthedocs.io/en/stable/"
 keywords = ["onekit"]
```

### Comparing `onekit-1.0.0/src/onekit/mathkit.py` & `onekit-1.1.0/src/onekit/mathkit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.0.0/src/onekit/numpykit.py` & `onekit-1.1.0/src/onekit/numpykit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.0.0/src/onekit/optfunckit.py` & `onekit-1.1.0/src/onekit/optfunckit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.0.0/src/onekit/pandaskit.py` & `onekit-1.1.0/src/onekit/pandaskit.py`

 * *Files identical despite different names*

### Comparing `onekit-1.0.0/src/onekit/pythonkit.py` & `onekit-1.1.0/src/onekit/pythonkit.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     List,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
+import pytz
 import toolz
 from toolz import curried
 
 __all__ = (
     "archive_files",
     "are_predicates_true",
     "check_random_state",
@@ -59,14 +60,15 @@
     "prompt_yes_no",
     "reduce_sets",
     "remove_punctuation",
     "signif",
     "source_code",
     "stopwatch",
     "str_to_date",
+    "timestamp",
     "weekday",
 )
 
 
 Pair = Tuple[float, float]
 Predicate = Callable[[Any], bool]
 Seed = Optional[Union[int, random.Random]]
@@ -74,29 +76,31 @@
 
 def archive_files(
     target: str,
     /,
     *,
     wildcards: Optional[List[str]] = None,
     name: Optional[str] = None,
+    timezone: Optional[str] = None,
     kind: str = "zip",
 ) -> None:
     """Archive files in target directory.
 
     Parameters
     ----------
     target : str
-        Specify the target directory to archive.
-    wildcards : None, list of str, default=None
-        Specify a wildcard to archive files. If ``wildcards`` is None,
-        all files in target directory are archived.
-    name : None, str, default=None
-        Optionally specify the name of the resulting archive.
-        If ``name`` is None, the name of the resulting archive is the name of the
-        target directory with timestamp.
+        Specify target directory to archive.
+    wildcards : list of str, optional
+        Specify wildcard to archive files.
+        Default: all files in target directory are archived.
+    name : str, optional
+        Specify name of resulting archive.
+        Default: name of target directory with timestamp.
+    timezone : str, optional
+        Specify timezone. Default: local timezone.
     kind : str, default="zip"
         Specify the archive type. Value is passed to the ``format`` argument of
         ``shutil.make_archive``, i.e., possible values are "zip", "tar",
         "gztar", "bztar", "xztar", or any other registered format.
 
     Returns
     -------
@@ -108,16 +112,15 @@
     --------
     >>> # archive all Python files and Notebooks in current working directory
     >>> import onekit.pythonkit as pk
     >>> pk.archive_files("./", wildcards=["*.py", "*.ipynb"])  # doctest: +SKIP
     """
     target = Path(target).resolve()
     wildcards = wildcards or ["**/*"]
-    timestamp = dt.datetime.now().strftime("%Y%m%d%H%M%S")
-    name = name or f"{timestamp}_{target.stem}"
+    name = name or f"{timestamp(zone=timezone, fmt='%Y%m%d%H%M%S')}_{target.stem}"
     makedir = functools.partial(os.makedirs, exist_ok=True)
 
     with TemporaryDirectory() as tmpdir:
         for wildcard in wildcards:
             for src_file in target.rglob(wildcard):
                 if os.path.isdir(src_file):
                     makedir(src_file)
@@ -1036,24 +1039,25 @@
 
 
 class stopwatch(ContextDecorator):
     """Measure elapsed wall-clock time and print it to standard output.
 
     Parameters
     ----------
-    label : None, str, int, default=None
-        Optionally specify label. When used as a decorator and label is not specified,
+    label : str, int, optional
+        Specify label. When used as a decorator and label is not specified,
         label is the name of the function.
     flush : bool, default=True
         Passed to built-in print function:
          - If ``True``, prints start time before stop time.
          - If ``False``, prints start time and stop time all at once.
-    fmt : None, str, default=None
-        Optionally specify a timestamp format to be used in the output message.
-        If ``fmt`` is None, the following format is used: ``%Y-%m-%d %H:%M:%S``.
+    timezone : str, optional
+        Specify timezone. Default: local timezone.
+    fmt : str, optional
+        Specify timestamp format. Default: ``%Y-%m-%d %H:%M:%S``.
 
     Notes
     -----
     - Instantiation and use of an instance's properties is only possible
       when ``stopwatch`` is used as a context manager (see examples).
     - The total elapsed time is computed when multiple ``stopwatch`` instances
       are added (see examples).
@@ -1123,29 +1127,34 @@
 
     def __init__(
         self,
         label: Optional[Union[str, int]] = None,
         /,
         *,
         flush: bool = True,
+        timezone: Optional[str] = None,
         fmt: Optional[str] = None,
     ):
         if isinstance(label, bool) or (
             label is not None and not isinstance(label, (str, int))
         ):
             raise TypeError(f"{label=} - must be str, int, or NoneType")
 
         if not isinstance(flush, bool):
             raise TypeError(f"{flush=} - must be bool")
 
+        if timezone is not None and not isinstance(timezone, str):
+            raise TypeError(f"{timezone=} - must be str or NoneType")
+
         if fmt is not None and not isinstance(fmt, str):
             raise TypeError(f"{fmt=} - must be str or NoneType")
 
         self._label = label
         self._flush = flush
+        self._timezone = timezone
         self._fmt = "%Y-%m-%d %H:%M:%S" if fmt is None else fmt
         self._start_time = None
         self._stop_time = None
         self._elapsed_time = None
         self._is_total = False
 
     def __repr__(self):
@@ -1173,14 +1182,25 @@
         -------
         bool
             Value used in the built-in function when printing to standard output.
         """
         return self._flush
 
     @property
+    def timezone(self):
+        """Retrieve timezone value.
+
+        Returns
+        -------
+        str
+            Value used for timezone.
+        """
+        return self._timezone
+
+    @property
     def fmt(self):
         """Retrieve timestamp format.
 
         The timestamp format can be changed by passing a new value that is accepted
         by ``strftime``. Note that the underlying data remain unchanged.
 
         Returns
@@ -1231,21 +1251,25 @@
 
     def __call__(self, func):
         if self.label is None:
             self._label = func.__name__
         return super().__call__(func)
 
     def __enter__(self):
-        self._start_time = dt.datetime.now()
+        self._start_time = dt.datetime.now(
+            tz=None if self.timezone is None else pytz.timezone(self.timezone)
+        )
         if self.flush:
             print(self._message_part_1(), end="", flush=True)
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
-        self._stop_time = dt.datetime.now()
+        self._stop_time = dt.datetime.now(
+            tz=None if self.timezone is None else pytz.timezone(self.timezone)
+        )
         self._elapsed_time = self.stop_time - self.start_time
         print(self._message_part_2() if self.flush else self._output_message())
         return False
 
     def _output_message(self):
         return (
             f"{self._human_readable_elapsed_time()} - {self.label}"
@@ -1301,14 +1325,43 @@
     >>> import onekit.pythonkit as pk
     >>> pk.str_to_date("2022-01-01")
     datetime.date(2022, 1, 1)
     """
     return dt.datetime.strptime(string, "%Y-%m-%d").date()
 
 
+def timestamp(zone: Optional[str] = None, fmt: Optional[str] = None) -> str:
+    """Get timezone-dependent timestamp.
+
+    Parameters
+    ----------
+    zone : str, optional
+        Specify timezone. Default: local timezone.
+    fmt : str, optional
+        Specify timestamp format. Default: ``%Y-%m-%d %H:%M:%S``.
+
+    Notes
+    -----
+    - Look up available timezones: ``pytz.all_timezones`` ``pytz.common_timezones``
+    - Look up timezones per country:  ``pytz.country_names`` ``pytz.country_timezones``
+
+    Examples
+    --------
+    >>> import onekit.pythonkit as pk
+    >>> pk.timestamp()  # doctest: +SKIP
+    '2024-01-01 00:00:00'
+
+    >>> pk.timestamp("CET")  # doctest: +SKIP
+    '2024-01-01 01:00:00'
+    """
+    zone = None if zone is None else pytz.timezone(zone)
+    fmt = fmt or "%Y-%m-%d %H:%M:%S"
+    return dt.datetime.now(tz=zone).strftime(fmt)
+
+
 def weekday(d: dt.date, /) -> str:
     """Get name of the weekday.
 
     Examples
     --------
     >>> import datetime as dt
     >>> import onekit.pythonkit as pk
```

### Comparing `onekit-1.0.0/src/onekit/sparkkit.py` & `onekit-1.1.0/src/onekit/sparkkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,19 +703,19 @@
     +----------+
     <BLANKLINE>
     """
     if not isinstance(n, int) or n < 1:
         raise ValueError(f"{n=} - must be a positive integer")
 
     def inner(df: SparkDF, /) -> SparkDF:
-        date_diff = "_date_diff_"
+        date_diff_ago = "_date_diff_ago_"
         return (
-            df.withColumn(date_diff, F.datediff(F.lit(d0), date_col))
-            .where((F.col(date_diff) >= 0) & (F.col(date_diff) < n))
-            .drop(date_diff)
+            df.transform(with_date_diff_ago(date_col, d0, new_col=date_diff_ago))
+            .where((F.col(date_diff_ago) >= 0) & (F.col(date_diff_ago) < n))
+            .drop(date_diff_ago)
         )
 
     return inner
 
 
 @toolz.curry
 def has_column(df: SparkDF, /, *, cols: Sequence[str]) -> bool:
```

### Comparing `onekit-1.0.0/src/onekit/vizkit.py` & `onekit-1.1.0/src/onekit/vizkit.py`

 * *Files 5% similar despite different names*

```diff
@@ -441,25 +441,24 @@
 ) -> Axes:
     """Plot :math:`z` versus :math:`(x, y)` as contour.
 
     Parameters
     ----------
     xyz_pts : XyzPoints
         :math:`(x, y, z)` coordinate points to plot.
-    kws_contour : dict of keyword arguments, default=None
-        Specify keyword arguments to pass to ``matplotlib.axes.Axes.contour``.
-        By default, using configuration: ``VizConfig.get_kws_contour__base()``.
-        Optionally specify a dict of keyword arguments to update configurations.
-    kws_contourf : dict of keyword arguments, default=None
-        Specify keyword arguments to pass to ``matplotlib.axes.Axes.contourf``.
-        By default, using configuration: ``VizConfig.get_kws_contourf__YlOrBr_r()``.
-        Optionally specify a dict of keyword arguments to update configurations.
-    ax : matplotlib.axes.Axes, default=None
-        Optionally specify an ``Axes`` object.
-        If None, current ``Axes`` object is retrieved.
+    kws_contour : dict of keyword arguments, optional
+        Keyword arguments to pass to ``matplotlib.axes.Axes.contour``.
+        Default: ``VizConfig.get_kws_contour__base()``.
+        Specify dict of keyword arguments to update configurations.
+    kws_contourf : dict of keyword arguments, optional
+        Keyword arguments to pass to ``matplotlib.axes.Axes.contourf``.
+        Default: `VizConfig.get_kws_contourf__YlOrBr_r()``.
+        Specify dict of keyword arguments to update configurations.
+    ax : matplotlib.axes.Axes, optional
+        Specify ``Axes`` object. Default: current ``Axes`` object.
 
     Examples
     --------
     >>> import toolz
     >>> import onekit.optfunckit as ofk
     >>> import onekit.vizkit as vk
     >>> ax = toolz.pipe(  # doctest: +SKIP
@@ -488,21 +487,20 @@
 def plot_line(xy_pts: XyPoints, /, *, kws_plot=None, ax=None) -> Axes:
     """Plot :math:`y` versus :math:`x` as line.
 
     Parameters
     ----------
     xy_pts : XyPoints
         :math:`(x, y)` coordinate points to plot.
-    kws_plot : dict of keyword arguments, default=None
-        Specify keyword arguments to pass to ``matplotlib.axes.Axes.plot``.
-        By default, using configuration: ``VizConfig.get_kws_plot__base()``.
-        Optionally specify a dict of keyword arguments to update configurations.
-    ax : matplotlib.axes.Axes, default=None
-        Optionally specify an ``Axes`` object.
-        If None, current ``Axes`` object is retrieved.
+    kws_plot : dict of keyword arguments, optional
+        Keyword arguments to pass to ``matplotlib.axes.Axes.plot``.
+        Default: ``VizConfig.get_kws_plot__base()``.
+        Specify dict of keyword arguments to update configurations.
+    ax : matplotlib.axes.Axes, optional
+        Specify ``Axes`` object. Default: current ``Axes`` object.
 
     Examples
     --------
     >>> import toolz
     >>> import onekit.optfunckit as ofk
     >>> import onekit.vizkit as vk
     >>> ax = toolz.pipe(  # doctest: +SKIP
@@ -529,26 +527,25 @@
 ) -> Axes3D:
     """Plot :math:`z` versus :math:`(x, y)` as surface.
 
     Parameters
     ----------
     xyz_pts : XyzPoints
         :math:`(x, y, z)` coordinate points to plot.
-    kws_surface : dict of keyword arguments, default=None
-        Specify keyword arguments to pass to
+    kws_surface : dict of keyword arguments, optional
+        Keyword arguments to pass to
         ``mpl_toolkits.mplot3d.axes3d.Axes3D.plot_surface``.
-        By default, using configuration: ``VizConfig.get_kws_surface__YlOrBr_r()``.
-        Optionally specify a dict of keyword arguments to update configurations.
-    kws_contourf : dict of keyword arguments, default=None
-        Specify keyword arguments to pass to ``matplotlib.axes.Axes.contourf``.
-        By default, using configuration: ``VizConfig.get_kws_contourf__YlOrBr_r()``.
-        Optionally specify a dict of keyword arguments to update configurations.
-    ax : mpl_toolkits.mplot3d.axes3d.Axes3D, default=None
-        Optionally specify an ``Axes3D`` object.
-        If None, current ``Axes3D`` object is retrieved.
+        Default: ``VizConfig.get_kws_surface__YlOrBr_r()``.
+        Specify dict of keyword arguments to update configurations.
+    kws_contourf : dict of keyword arguments, optional
+        Keyword arguments to pass to ``matplotlib.axes.Axes.contourf``.
+        Default: ``VizConfig.get_kws_contourf__YlOrBr_r()``.
+        Specify dict of keyword arguments to update configurations.
+    ax : mpl_toolkits.mplot3d.axes3d.Axes3D, optional
+        Specify ``Axes3D`` object. Default: current ``Axes3D`` object.
 
     Examples
     --------
     >>> import toolz
     >>> import onekit.optfunckit as ofk
     >>> import onekit.vizkit as vk
     >>> ax = toolz.pipe(  # doctest: +SKIP
@@ -586,21 +583,20 @@
 def plot_xy_points(xy_pts: XyPoints, /, *, kws_scatter=None, ax=None) -> Axes:
     """Plot :math:`y` versus :math:`x` as scatter points.
 
     Parameters
     ----------
     xy_pts : XyPoints
         :math:`(x, y)` coordinate points to plot.
-    kws_scatter : dict of keyword arguments, default=None
-        Specify keyword arguments to pass to ``matplotlib.axes.Axes.scatter``.
-        By default, using configuration: ``VizConfig.get_kws_scatter__base()``.
-        Optionally specify a dict of keyword arguments to update configurations.
-    ax : matplotlib.axes.Axes, default=None
-        Optionally specify an ``Axes`` object.
-        If None, current ``Axes`` object is retrieved.
+    kws_scatter : dict of keyword arguments, optional
+        Keyword arguments to pass to ``matplotlib.axes.Axes.scatter``.
+        Default: ``VizConfig.get_kws_scatter__base()``.
+        Specify dict of keyword arguments to update configurations.
+    ax : matplotlib.axes.Axes, optional
+        Specify ``Axes`` object. Default: current ``Axes`` object.
 
     Examples
     --------
     >>> import toolz
     >>> import onekit.optfunckit as ofk
     >>> import onekit.vizkit as vk
     >>> ax = toolz.pipe(  # doctest: +SKIP
@@ -620,22 +616,21 @@
 def plot_xyz_points(xyz_pts: XyzPoints, /, *, kws_scatter=None, ax=None) -> Axes3D:
     """Plot :math:`z` versus :math:`(x, y)` as scatter points.
 
     Parameters
     ----------
     xyz_pts : XyzPoints
         :math:`(x, y, z)` coordinate points to plot.
-    kws_scatter : dict of keyword arguments, default=None
-        Specify keyword arguments to pass to
+    kws_scatter : dict of keyword arguments, optional
+        Keyword arguments to pass to
         ``mpl_toolkits.mplot3d.axes3d.Axes3D.scatter``.
-        By default, using configuration: ``VizConfig.get_kws_scatter__base()``.
-        Optionally specify a dict of keyword arguments to update configurations.
-    ax : mpl_toolkits.mplot3d.axes3d.Axes3D, default=None
-        Optionally specify an ``Axes3D`` object.
-        If None, current ``Axes3D`` object is retrieved.
+        Default: ``VizConfig.get_kws_scatter__base()``.
+        Specify dict of keyword arguments to update configurations.
+    ax : mpl_toolkits.mplot3d.axes3d.Axes3D, optional
+        Specify ``Axes3D`` object. Default: current ``Axes3D`` object.
 
     Examples
     --------
     >>> import toolz
     >>> import onekit.optfunckit as ofk
     >>> import onekit.vizkit as vk
     >>> ax = toolz.pipe(  # doctest: +SKIP
```

### Comparing `onekit-1.0.0/PKG-INFO` & `onekit-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onekit
-Version: 1.0.0
+Version: 1.1.0
 Summary: All-in-One Python Kit.
 Home-page: https://github.com/estripling/onekit
 License: BSD 3-Clause
 Keywords: onekit
 Author: Eugen Stripling
 Author-email: estripling042@gmail.com
 Requires-Python: >=3.8.1,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onekit Version: 1.0.0 Summary: All-in-One Python
+Metadata-Version: 2.1 Name: onekit Version: 1.1.0 Summary: All-in-One Python
 Kit. Home-page: https://github.com/estripling/onekit License: BSD 3-Clause
 Keywords: onekit Author: Eugen Stripling Author-email: estripling042@gmail.com
 Requires-Python: >=3.8.1,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
```

