# Comparing `tmp/py4cli-0.0.3.tar.gz` & `tmp/py4cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\py4cli-0.0.3.tar", last modified: Mon Aug 22 15:49:12 2022, max compression
+gzip compressed data, was "dist\py4cli-0.0.4.tar", last modified: Fri Apr 26 08:24:32 2024, max compression
```

## Comparing `py4cli-0.0.3.tar` & `py4cli-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,81 @@
-drwxrwxrwx   0        0        0        0 2022-08-22 15:49:12.000000 py4cli-0.0.3/
--rw-rw-rw-   0        0        0    35812 2022-06-16 23:39:43.000000 py4cli-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       60 2021-09-19 11:16:31.000000 py4cli-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      673 2022-08-22 15:49:12.000000 py4cli-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       91 2022-06-16 23:38:36.000000 py4cli-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-08-22 15:49:11.000000 py4cli-0.0.3/SRCS/
-drwxrwxrwx   0        0        0        0 2022-08-22 15:49:12.000000 py4cli-0.0.3/SRCS/py4cli/
--rw-rw-rw-   0        0        0     6594 2022-08-22 15:37:05.000000 py4cli-0.0.3/SRCS/py4cli/route_cli.py
-drwxrwxrwx   0        0        0        0 2022-08-22 15:49:12.000000 py4cli-0.0.3/SRCS/py4cli.egg-info/
--rw-rw-rw-   0        0        0      673 2022-08-22 15:49:11.000000 py4cli-0.0.3/SRCS/py4cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2022-08-22 15:49:11.000000 py4cli-0.0.3/SRCS/py4cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-22 15:49:11.000000 py4cli-0.0.3/SRCS/py4cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2022-08-22 15:49:11.000000 py4cli-0.0.3/SRCS/py4cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-08-22 15:49:11.000000 py4cli-0.0.3/SRCS/py4cli.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-22 15:49:12.000000 py4cli-0.0.3/TESTS/
--rw-rw-rw-   0        0        0      910 2022-08-02 02:16:35.000000 py4cli-0.0.3/TESTS/basic.py
--rw-rw-rw-   0        0        0      291 2021-07-21 06:41:20.000000 py4cli-0.0.3/TESTS/conftest.py
--rw-rw-rw-   0        0        0      175 2022-08-21 14:11:02.000000 py4cli-0.0.3/TESTS/test_basic.py
--rw-rw-rw-   0        0        0      144 2022-06-17 00:10:09.000000 py4cli-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-08-22 15:49:12.000000 py4cli-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      931 2022-08-22 15:43:55.000000 py4cli-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/
+-rw-rw-rw-   0        0        0    35812 2024-03-31 05:57:29.000000 py4cli-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      101 2024-04-26 07:58:26.000000 py4cli-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5609 2024-04-26 08:24:32.000000 py4cli-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5074 2024-04-26 08:23:33.000000 py4cli-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/SRCS/
+drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/SRCS/py4cli/
+-rw-rw-rw-   0        0        0     5854 2024-04-26 05:07:42.000000 py4cli-0.0.4/SRCS/py4cli/minimal.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/SRCS/py4cli.egg-info/
+-rw-rw-rw-   0        0        0     5609 2024-04-26 08:24:31.000000 py4cli-0.0.4/SRCS/py4cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1975 2024-04-26 08:24:32.000000 py4cli-0.0.4/SRCS/py4cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 08:24:31.000000 py4cli-0.0.4/SRCS/py4cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-26 08:24:31.000000 py4cli-0.0.4/SRCS/py4cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-26 08:24:31.000000 py4cli-0.0.4/SRCS/py4cli.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/TESTS/
+-rw-rw-rw-   0        0        0      486 2024-04-23 12:35:47.000000 py4cli-0.0.4/TESTS/conftest.py
+drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/TESTS/ref_files/
+-rw-rw-rw-   0        0        0       49 2024-04-26 06:47:42.000000 py4cli-0.0.4/TESTS/ref_files/bool.txt
+-rw-rw-rw-   0        0        0       56 2024-04-26 06:47:42.000000 py4cli-0.0.4/TESTS/ref_files/bool_args.txt
+-rw-rw-rw-   0        0        0      635 2024-04-26 07:42:00.000000 py4cli-0.0.4/TESTS/ref_files/bool_h.txt
+-rw-rw-rw-   0        0        0      639 2024-04-26 07:42:00.000000 py4cli-0.0.4/TESTS/ref_files/bool_help.txt
+-rw-rw-rw-   0        0        0       66 2024-04-26 06:47:42.000000 py4cli-0.0.4/TESTS/ref_files/bool_kwargs.txt
+-rw-rw-rw-   0        0        0       56 2024-04-26 06:47:41.000000 py4cli-0.0.4/TESTS/ref_files/dict.txt
+-rw-rw-rw-   0        0        0       83 2024-04-26 06:47:41.000000 py4cli-0.0.4/TESTS/ref_files/dict_args.txt
+-rw-rw-rw-   0        0        0      675 2024-04-26 07:00:39.000000 py4cli-0.0.4/TESTS/ref_files/dict_h.txt
+-rw-rw-rw-   0        0        0      679 2024-04-26 07:00:39.000000 py4cli-0.0.4/TESTS/ref_files/dict_help.txt
+-rw-rw-rw-   0        0        0       93 2024-04-26 06:47:41.000000 py4cli-0.0.4/TESTS/ref_files/dict_kwargs.txt
+-rw-rw-rw-   0        0        0       49 2024-04-26 06:47:35.000000 py4cli-0.0.4/TESTS/ref_files/float.txt
+-rw-rw-rw-   0        0        0       58 2024-04-26 06:47:35.000000 py4cli-0.0.4/TESTS/ref_files/float_args.txt
+-rw-rw-rw-   0        0        0      652 2024-04-26 06:47:34.000000 py4cli-0.0.4/TESTS/ref_files/float_h.txt
+-rw-rw-rw-   0        0        0      656 2024-04-26 06:47:34.000000 py4cli-0.0.4/TESTS/ref_files/float_help.txt
+-rw-rw-rw-   0        0        0       69 2024-04-26 06:47:35.000000 py4cli-0.0.4/TESTS/ref_files/float_kwargs.txt
+-rw-rw-rw-   0        0        0       43 2024-04-26 06:47:34.000000 py4cli-0.0.4/TESTS/ref_files/int.txt
+-rw-rw-rw-   0        0        0       50 2024-04-26 06:47:34.000000 py4cli-0.0.4/TESTS/ref_files/int_args.txt
+-rw-rw-rw-   0        0        0      615 2024-04-26 06:47:33.000000 py4cli-0.0.4/TESTS/ref_files/int_h.txt
+-rw-rw-rw-   0        0        0      619 2024-04-26 06:47:33.000000 py4cli-0.0.4/TESTS/ref_files/int_help.txt
+-rw-rw-rw-   0        0        0       59 2024-04-26 06:47:34.000000 py4cli-0.0.4/TESTS/ref_files/int_kwargs.txt
+-rw-rw-rw-   0        0        0       50 2024-04-26 06:47:37.000000 py4cli-0.0.4/TESTS/ref_files/list.txt
+-rw-rw-rw-   0        0        0       64 2024-04-26 06:47:37.000000 py4cli-0.0.4/TESTS/ref_files/list_args.txt
+-rw-rw-rw-   0        0        0      647 2024-04-26 06:47:37.000000 py4cli-0.0.4/TESTS/ref_files/list_h.txt
+-rw-rw-rw-   0        0        0      651 2024-04-26 06:47:37.000000 py4cli-0.0.4/TESTS/ref_files/list_help.txt
+-rw-rw-rw-   0        0        0       74 2024-04-26 06:47:37.000000 py4cli-0.0.4/TESTS/ref_files/list_kwargs.txt
+-rw-rw-rw-   0        0        0      321 2024-04-26 06:47:43.000000 py4cli-0.0.4/TESTS/ref_files/multi.txt
+-rw-rw-rw-   0        0        0      469 2024-04-26 06:52:41.000000 py4cli-0.0.4/TESTS/ref_files/multi_args.txt
+-rw-rw-rw-   0        0        0     1254 2024-04-26 06:47:42.000000 py4cli-0.0.4/TESTS/ref_files/multi_h.txt
+-rw-rw-rw-   0        0        0     1258 2024-04-26 06:47:43.000000 py4cli-0.0.4/TESTS/ref_files/multi_help.txt
+-rw-rw-rw-   0        0        0      548 2024-04-26 06:52:41.000000 py4cli-0.0.4/TESTS/ref_files/multi_kwargs.txt
+-rw-rw-rw-   0        0        0      348 2024-04-26 06:47:44.000000 py4cli-0.0.4/TESTS/ref_files/multi_mix1.txt
+-rw-rw-rw-   0        0        0      403 2024-04-26 06:47:44.000000 py4cli-0.0.4/TESTS/ref_files/multi_mix2.txt
+-rw-rw-rw-   0        0        0      404 2024-04-26 06:47:44.000000 py4cli-0.0.4/TESTS/ref_files/multi_mix3.txt
+-rw-rw-rw-   0        0        0       48 2024-04-26 06:47:39.000000 py4cli-0.0.4/TESTS/ref_files/set.txt
+-rw-rw-rw-   0        0        0       68 2024-04-26 06:47:40.000000 py4cli-0.0.4/TESTS/ref_files/set_args.txt
+-rw-rw-rw-   0        0        0      635 2024-04-26 06:47:39.000000 py4cli-0.0.4/TESTS/ref_files/set_h.txt
+-rw-rw-rw-   0        0        0      639 2024-04-26 06:47:39.000000 py4cli-0.0.4/TESTS/ref_files/set_help.txt
+-rw-rw-rw-   0        0        0       77 2024-04-26 06:47:40.000000 py4cli-0.0.4/TESTS/ref_files/set_kwargs.txt
+-rw-rw-rw-   0        0        0       46 2024-04-26 06:47:36.000000 py4cli-0.0.4/TESTS/ref_files/str.txt
+-rw-rw-rw-   0        0        0       56 2024-04-26 06:47:36.000000 py4cli-0.0.4/TESTS/ref_files/str_args.txt
+-rw-rw-rw-   0        0        0      630 2024-04-26 06:47:35.000000 py4cli-0.0.4/TESTS/ref_files/str_h.txt
+-rw-rw-rw-   0        0        0      634 2024-04-26 06:47:36.000000 py4cli-0.0.4/TESTS/ref_files/str_help.txt
+-rw-rw-rw-   0        0        0       65 2024-04-26 06:47:36.000000 py4cli-0.0.4/TESTS/ref_files/str_kwargs.txt
+-rw-rw-rw-   0        0        0       53 2024-04-26 06:47:38.000000 py4cli-0.0.4/TESTS/ref_files/tuple.txt
+-rw-rw-rw-   0        0        0       66 2024-04-26 06:47:38.000000 py4cli-0.0.4/TESTS/ref_files/tuple_args.txt
+-rw-rw-rw-   0        0        0      663 2024-04-26 06:47:38.000000 py4cli-0.0.4/TESTS/ref_files/tuple_h.txt
+-rw-rw-rw-   0        0        0      667 2024-04-26 06:47:38.000000 py4cli-0.0.4/TESTS/ref_files/tuple_help.txt
+-rw-rw-rw-   0        0        0       77 2024-04-26 06:47:39.000000 py4cli-0.0.4/TESTS/ref_files/tuple_kwargs.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 08:24:32.000000 py4cli-0.0.4/TESTS/scripts/
+-rw-rw-rw-   0        0        0     5933 2024-04-26 07:36:42.000000 py4cli-0.0.4/TESTS/scripts/basic_usage.py
+-rw-rw-rw-   0        0        0      372 2024-04-26 06:42:28.000000 py4cli-0.0.4/TESTS/scripts/multi_args.py
+-rw-rw-rw-   0        0        0      139 2024-04-26 06:42:03.000000 py4cli-0.0.4/TESTS/scripts/use_bool.py
+-rw-rw-rw-   0        0        0      141 2024-04-26 06:41:34.000000 py4cli-0.0.4/TESTS/scripts/use_dict.py
+-rw-rw-rw-   0        0        0      143 2024-04-26 06:41:27.000000 py4cli-0.0.4/TESTS/scripts/use_float.py
+-rw-rw-rw-   0        0        0      139 2024-04-26 06:41:16.000000 py4cli-0.0.4/TESTS/scripts/use_int.py
+-rw-rw-rw-   0        0        0      141 2024-04-26 06:41:41.000000 py4cli-0.0.4/TESTS/scripts/use_list.py
+-rw-rw-rw-   0        0        0      139 2024-04-26 06:41:46.000000 py4cli-0.0.4/TESTS/scripts/use_set.py
+-rw-rw-rw-   0        0        0      139 2024-04-26 06:41:50.000000 py4cli-0.0.4/TESTS/scripts/use_str.py
+-rw-rw-rw-   0        0        0      143 2024-04-26 06:41:58.000000 py4cli-0.0.4/TESTS/scripts/use_tuple.py
+-rw-rw-rw-   0        0        0    10198 2024-04-26 06:47:28.000000 py4cli-0.0.4/TESTS/test_basic_call.py
+-rw-rw-rw-   0        0        0     4211 2024-04-26 06:52:22.000000 py4cli-0.0.4/TESTS/test_basic_os.py
+-rw-rw-rw-   0        0        0      144 2024-03-31 05:57:29.000000 py4cli-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 08:24:32.000000 py4cli-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      964 2024-04-26 07:57:37.000000 py4cli-0.0.4/setup.py
```

### Comparing `py4cli-0.0.3/LICENSE.txt` & `py4cli-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py4cli-0.0.3/SRCS/py4cli/route_cli.py` & `py4cli-0.0.4/SRCS/py4cli/minimal.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,115 +1,136 @@
 
 import sys
 import re
 import inspect
 import ast
-import pickle
+import __main__
 
-class cli_router():
+class arg_parser():
 
     def __init__(self, argv=sys.argv):
 
-        derived_class = self.__class__.__name__
-        base_class = cli_router.__name__
-        self.returned = None
-        if derived_class != base_class:
-
-            if len(argv) > 1:
-
-                if argv[1].startswith("~"):
-                    method_name = argv[1][1:]
-                else:
-                    raise SyntaxError(
-                        f"function name should precede positional arguments, eg : ~run")
+        def_func_name = 'parse_args'
+        if len(argv) == 2 and (argv[1] in ['-h', '--help']):
+            self.returned = None
+            self.__doc(def_func_name)
+        else:
+            func_schema = self.__func2schema(def_func_name)
+            args_schema = self.__args2schema(def_func_name, argv[1:])
+            args, kwargs = self.__solve_schema(
+                func_schema[def_func_name], args_schema[def_func_name])
+            if inspect.ismethod(getattr(self, def_func_name)):
+                self.returned = self.__func(def_func_name, args, kwargs)
+                if type(self.returned) != func_schema['ret_type']:
+                    print(
+                        f"WARNING : '{def_func_name}' returns '{type(self.returned).__name__}', but defined to return '{func_schema['ret_type'].__name__}'")
+
+    def __func(self, func, args, kwargs):
+
+        returned = getattr(self, func)(*args, **kwargs)
+        return returned
+
+    def __type(self, dtype, value):
+
+        if dtype == str:
+            return value
+
+        if dtype in [int, float]:
+            type_casted_value = dtype(value)
+        elif dtype in [list, tuple, dict, bool, set]:
+            type_casted_value = ast.literal_eval(value)
+        elif dtype in [inspect._empty]:
+            type_casted_value = value
+        else:
+            raise Exception(
+                f"Unsupported argument data type : {dtype}, try using basic types (int, float, str, list, tuple, set, dict, bool) instead")
 
-                if not method_name.startswith("_"):
+        return type_casted_value
 
-                    method_obj = getattr(self, method_name)
+    def __solve_schema(self, func, inps):
 
-                    if inspect.ismethod(method_obj):
+        mod_args = []
+        for i in range(len(inps['args'])):
+            type = func['kwargs'][func['args'][i]]['type']
+            val = inps['args'][i]
+            mod_args.append(self.__type(type, val))
 
-                        sign = inspect.signature(method_obj)
-                        args, kwargs = self.__get_args(argv[2:], sign)
-                        self.returned = method_obj(*args, **kwargs)
-                        if sign.return_annotation == pickle:
-                            print(f"writing pickle file as '{method_name}.pkl'")
-                            with open(f'{method_name}.pkl', 'wb') as handle:
-                                pickle.dump(self.returned, handle, protocol=pickle.HIGHEST_PROTOCOL)
+        mod_kwargs = {}
+        for key, val in inps['kwargs'].items():
+            type = func['kwargs'][key]['type']
+            val = val['value']
+            mod_kwargs[key] = self.__type(type, val)
 
-                    else:
-                        raise SyntaxError(
-                            f"class {derived_class} derived from {base_class} should have method '{method_name}' defined")
+        return mod_args, mod_kwargs
 
-                else:
-                    raise SyntaxError(
-                        f"~{method_name} : not supported, method name should not start with underscore, i.e _ ")
+    def __func2schema(self, func_name):
 
+        sign = inspect.signature(getattr(self, func_name))
+        args = []
+        kwargs = {}
+        for key, val in sign.parameters.items():
+            if val.default == inspect._empty:
+                kwargs[key] = {'value': '_empty',
+                               'type': val.annotation}
             else:
-                self._help()
+                kwargs[key] = {'value': val.default,
+                               'type': val.annotation}
+            args.append(key)
+
+        if sign.return_annotation == inspect._empty:
+            ret_anno = '_empty'
         else:
-            raise SyntaxError(
-                f"{base_class} should be used as parent class only")
+            ret_anno = sign.return_annotation
+
+        func_dict = {
+            func_name: {
+                'args': args,
+                'kwargs': kwargs
+            },
+            'ret_type': ret_anno
+        }
+        return func_dict
 
-    def __get_args(self, inp_args, sign):
+    def __args2schema(self, func_name, inp_args):
 
         args = []
         kwargs = {}
         kwargs_started = False
-        ordered_type_list = list(sign.parameters.items())
-        ordered_type_dict = dict(sign.parameters.items())
         for i in range(len(inp_args)):
             kwargs_found = re.match("^-(\\S+)=(\\S+)$", inp_args[i])
             if kwargs_found:
                 key, value = kwargs_found.groups()
-                kwarg_type = ordered_type_dict[key].annotation if key in ordered_type_dict.keys(
-                ) else None
-                if kwarg_type and kwarg_type != str:
-                    kwarg_val = ast.literal_eval(value)
-                    if(type(kwarg_val) != kwarg_type):
-                        raise SyntaxError(
-                            f"Input for {key} should be of type {kwarg_type.__name__}")
-                else:
-                    kwarg_val = value
-                kwargs[key] = kwarg_val
+                kwargs[key] = {'value': value}
                 kwargs_started = True
             else:
                 if kwargs_started:
                     raise SyntaxError(
                         f"positional argument follows keyword argument {key}")
                 else:
-                    arg_type = ordered_type_list[i][1].annotation if i < len(
-                        ordered_type_list) else None
-                    if arg_type and arg_type != str:
-                        arg_key = ordered_type_list[i][0]
-                        arg_val = ast.literal_eval(inp_args[i])
-                        if(type(arg_val) != arg_type):
-                            raise SyntaxError(
-                                f"Input for {arg_key} should be of type {arg_type.__name__}")
-                    else:
-                        arg_val = inp_args[i]
-                    args.append(arg_val)
+                    args.append(inp_args[i])
 
-        return args, kwargs
+        func_dict = {func_name: {'args': args, 'kwargs': kwargs}}
+        return func_dict
 
-    def __func(self, name, obj):
+    def __doc(self, name):
 
-        print(f" > ~{name} ")
+        print()
+        print(f" | > def {name} ")
         print(f" |    ")
-
+        obj = getattr(self, name)
         func_comments = inspect.getcomments(obj)
         if func_comments:
             print(" |  Description :")
             print(f" |    ")
             comments = func_comments.splitlines()
             if len(comments) == 1:
                 print(f" |    { comments[0].replace('#', '').strip() }  ")
             else:
                 print(f" |    { comments[0].replace('#', '').strip() }  ")
-                for i in range(1,len(comments)-1):
+                for i in range(1, len(comments)-1):
                     print(f" |    { comments[i].replace('#', '').strip() } ")
                 print(f" |    { comments[-1].replace('#', '').strip() }  ")
             print(f" |    ")
 
         sign = inspect.signature(obj)
         args = [str(val) for var, val in sign.parameters.items()]
         if args:
@@ -121,54 +142,21 @@
 
         func_docs = inspect.getdoc(obj)
         if func_docs:
             print(" |  Usage :")
             print(f" |    ")
             docs = func_docs.splitlines()
             if len(docs) == 1:
-                print(f" |    { docs[0].strip() }  ")
+                print(f" |    { docs[0].strip().replace('<__file__>', __main__.__file__) }  ")
             else:
-                print(f" |    { docs[0].strip() }  ")
-                for i in range(1,len(docs)-1):
-                    print(f" |    { docs[i].strip() } ")
-                print(f" |    { docs[-1].strip() }  ")
+                print(f" |    { docs[0].strip().replace('<__file__>', __main__.__file__) }  ")
+                for i in range(1, len(docs)-1):
+                    print(f" |    { docs[i].strip().replace('<__file__>', __main__.__file__) } ")
+                print(f" |    { docs[-1].strip().replace('<__file__>', __main__.__file__) }  ")
             print(f" |    ")
 
         if sign.return_annotation != sign.empty:
-            if sign.return_annotation == pickle:
-                print(f" | -> {sign.return_annotation.__name__} (Writable as '{name}.pkl')")
-            elif sign.return_annotation == None:
+            if sign.return_annotation == None:
                 print(f" | -> {None} (Returnable)")
             else:
-                print(f" | -> {sign.return_annotation.__name__} (Returnable)")
-
-        # print(inspect.getdoc(obj))
-        # return {
-        #     "comment": comment.rstrip('\n') if comment else None,
-        #     "docs": inspect.getdoc(obj),
-        #     "args": [str(val) for var, val in sign.parameters.items()],
-        #     "ret": sign.return_annotation.__name__ if sign.return_annotation else None
-        # }
-
-    def _help(self, func: str = None):
-
-        if func:
-            
-            func_obj = getattr(self, func)
-            if inspect.ismethod(func_obj):
-                print()
-                self.__func(func, func_obj)
-        else:
-            method_list = filter(
-                lambda tup: not tup[0].startswith("_"),
-                inspect.getmembers(self, predicate=inspect.ismethod)
-            )
-            print()
-            for name, obj in method_list:
-                self.__func(name, obj)
-                print()
-
-
-
-if __name__ == "__main__":
-
-    cli_router()
+                print(
+                    f" | -> {sign.return_annotation.__name__} (Returnable)")
```

