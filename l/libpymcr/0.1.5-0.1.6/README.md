# Comparing `tmp/libpymcr-0.1.5-cp39-cp39-win_amd64.whl.zip` & `tmp/libpymcr-0.1.6-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 200476 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat    11938 b- defN 23-Oct-02 12:58 libpymcr/IPythonMagics.py
--rw-rw-rw-  2.0 fat     7040 b- defN 23-Oct-02 12:58 libpymcr/Matlab.py
--rw-rw-rw-  2.0 fat     9787 b- defN 23-Oct-02 12:58 libpymcr/MatlabProxyObject.py
--rw-rw-rw-  2.0 fat      203 b- defN 23-Oct-02 12:58 libpymcr/__init__.py
--rw-rw-rw-  2.0 fat   451072 b- defN 23-Oct-02 13:05 libpymcr/_libpymcr.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      518 b- defN 23-Oct-02 13:05 libpymcr/_version.py
--rw-rw-rw-  2.0 fat    12472 b- defN 23-Oct-02 12:58 libpymcr/utils.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Oct-02 13:06 libpymcr-0.1.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2586 b- defN 23-Oct-02 13:06 libpymcr-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Oct-02 13:06 libpymcr-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Oct-02 13:06 libpymcr-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      959 b- defN 23-Oct-02 13:06 libpymcr-0.1.5.dist-info/RECORD
-12 files, 532507 bytes uncompressed, 198882 bytes compressed:  62.7%
+Zip file size: 203799 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat    11938 b- defN 24-Apr-26 00:18 libpymcr/IPythonMagics.py
+-rw-rw-rw-  2.0 fat     7227 b- defN 24-Apr-26 00:18 libpymcr/Matlab.py
+-rw-rw-rw-  2.0 fat    10743 b- defN 24-Apr-26 00:18 libpymcr/MatlabProxyObject.py
+-rw-rw-rw-  2.0 fat      203 b- defN 24-Apr-26 00:18 libpymcr/__init__.py
+-rw-rw-rw-  2.0 fat   458240 b- defN 24-Apr-26 00:23 libpymcr/_libpymcr.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      518 b- defN 24-Apr-26 00:22 libpymcr/_version.py
+-rw-rw-rw-  2.0 fat    13420 b- defN 24-Apr-26 00:18 libpymcr/utils.py
+-rw-rw-rw-  2.0 fat    35823 b- defN 24-Apr-26 00:23 libpymcr-0.1.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2586 b- defN 24-Apr-26 00:23 libpymcr-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-26 00:23 libpymcr-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-26 00:23 libpymcr-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      960 b- defN 24-Apr-26 00:23 libpymcr-0.1.6.dist-info/RECORD
+12 files, 541767 bytes uncompressed, 202205 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: libpymcr/_version.py
 Comment: 
 
 Filename: libpymcr/utils.py
 Comment: 
 
-Filename: libpymcr-0.1.5.dist-info/LICENSE
+Filename: libpymcr-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: libpymcr-0.1.5.dist-info/METADATA
+Filename: libpymcr-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: libpymcr-0.1.5.dist-info/WHEEL
+Filename: libpymcr-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: libpymcr-0.1.5.dist-info/top_level.txt
+Filename: libpymcr-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: libpymcr-0.1.5.dist-info/RECORD
+Filename: libpymcr-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libpymcr/Matlab.py

```diff
@@ -99,14 +99,20 @@
         return a MatlabProxyObject
 
         :param name: The function/class to be called.
         :return: MatlabProxyObject of class/function given by name
         """
         return NamespaceWrapper(self._interface, name)
 
+    def type(self, obj):
+        if hasattr(obj, 'handle'):
+            return self._interface.call('class', obj.handle, nargout=1)
+        else:
+            return str(type(obj))
+
     def get_matlab_functions(self):
         """
         Returns a list of public functions in this CTF archive
         """
         def _get_xml_val(in_str):
             return in_str.split('=')[1].replace('"', '').replace('/', '')
         def _get_xml_tag(lis, tag_start, tag_end):
```

## libpymcr/MatlabProxyObject.py

```diff
@@ -28,14 +28,40 @@
     elif isinstance(inputs, list):
         return [unwrap(v, interface) for v in inputs]
     elif isinstance(inputs, dict):
         return {k:unwrap(v, interface) for k, v in inputs.items()}
     else:
         return inputs
 
+
+class DictPropertyWrapper:
+    # A proxy for dictionary properties of classes to allow Matlab .dot syntax
+    def __init__(self, val, name, parent):
+        assert isinstance(val, dict), "DictPropertyWrapper can only wrap dict objects"
+        self.__dict__['val'] = val
+        self.__dict__['name'] = name
+        self.__dict__['parent'] = parent
+
+    def __getattr__(self, name):
+        rv = self.val[name]
+        if isinstance(rv, dict):
+            rv = DictPropertyWrapper(rv, name, self)
+        return rv
+
+    def __setattr__(self, name, value):
+        self.val[name] = value
+        setattr(self.parent, self.name, self.val)
+
+    def __repr__(self):
+        rv = "Matlab struct with fields:\n"
+        for k, v in self.val.items():
+            rv += f"    {k}: {v}\n"
+        return rv
+
+
 class matlab_method:
     def __init__(self, proxy, method):
         self.proxy = proxy
         self.method = method
 
     def __call__(self, *args, **kwargs):
         nreturn = get_nlhs(self.method)
@@ -110,15 +136,18 @@
         Functions are returned as :class:`MatlabFunction` objects.
 
         """
         m = self.interface
         # if it's a property, just retrieve it
         if name in self._getAttributeNames():
             try:
-                return wrap(self.interface.call('subsref', self.handle, {'type':'.', 'subs':name}), self.interface)
+                rv = wrap(self.interface.call('subsref', self.handle, {'type':'.', 'subs':name}), self.interface)
+                if isinstance(rv, dict):
+                    rv = DictPropertyWrapper(rv, name, self)
+                return rv
             except TypeError:
                 return None
         # if it's a method, wrap it in a functor
         elif name in self._methods:
             return matlab_method(self, name)
 
     def __setattr__(self, name, value):
```

## libpymcr/_version.py

```diff
@@ -4,18 +4,18 @@
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
 {
- "date": "2023-10-02T13:44:28+0100",
+ "date": "2024-04-26T01:02:27+0100",
  "dirty": false,
  "error": null,
- "full-revisionid": "f34229fd6010de0cc3ad0998c32f88ffe9e51331",
- "version": "0.1.5"
+ "full-revisionid": "3db55072cc2bbac9b2848bb3951752a67b24a534",
+ "version": "0.1.6"
 }
 '''  # END VERSION_JSON
 
 
 def get_versions():
     return json.loads(version_json)
```

## libpymcr/utils.py

```diff
@@ -3,14 +3,15 @@
 import glob
 import platform
 import zipfile
 import ast
 import inspect
 import dis
 import linecache
+import shutil
 from pathlib import Path
 
 
 OPERATOR_NAMES = {
     "CALL_FUNCTION", "CALL_FUNCTION_VAR", "CALL_FUNCTION_KW", "CALL_FUNCTION_VAR_KW", "CALL",
     "UNARY_POSITIVE", "UNARY_NEGATIVE", "UNARY_NOT", "UNARY_CONVERT", "UNARY_INVERT", "GET_ITER",
     "BINARY_POWER", "BINARY_MULTIPLY", "BINARY_DIVIDE", "BINARY_FLOOR_DIVIDE", "BINARY_TRUE_DIVIDE",
@@ -18,14 +19,16 @@
     "BINARY_RSHIFT", "BINARY_AND", "BINARY_XOR", "BINARY_OR",
     "INPLACE_POWER", "INPLACE_MULTIPLY", "INPLACE_DIVIDE", "INPLACE_TRUE_DIVIDE", "INPLACE_FLOOR_DIVIDE",
     "INPLACE_MODULO", "INPLACE_ADD", "INPLACE_SUBTRACT", "INPLACE_LSHIFT", "INPLACE_RSHIFT",
     "INPLACE_AND", "INPLACE_XOR", "INPLACE_OR", "COMPARE_OP", "SET_UPDATE", "BUILD_CONST_KEY_MAP",
     "CALL_FUNCTION_EX", "LOAD_METHOD", "CALL_METHOD", "DICT_MERGE", "DICT_UPDATE", "LIST_EXTEND",
 }
 
+MLVERDIC = {f'R{rv[0]}{rv[1]}':f'9.{vr}' for rv, vr in zip([[yr, ab] for yr in range(2017,2023) for ab in ['a', 'b']], range(2, 14))}
+MLVERDIC.update({'R2023a':'9.14', 'R2023b':'23.2'})
 
 def get_nret_from_dis(frame):
     # Tries to get the number of return values for a function
     # Code adapted from Mantid/Framework/PythonInterface/mantid/kernel/funcinspect.py
     ins_stack = []
     call_fun_locs = {}
     start_i = 0
@@ -160,16 +163,26 @@
             self.sep = ':'
         elif self.system == 'Darwin':
             self.file_to_find = ''.join((self.lib_prefix, 'mclmcrrt', '.', self.ver, '.', self.ext))
             self.sep = ':'
         else:
             raise RuntimeError(f'Operating system {self.system} is not supported.')
 
+    @property
+    def ver(self):
+        return self._ver
+
+    @ver.setter
+    def ver(self, val):
+        self._ver = str(val)
+        if self._ver.startswith('R') and self._ver in MLVERDIC.keys():
+            self._ver = MLVERDIC[self._ver]
+
     def find_version(self, root_dir):
-        print(f'Searching for Matlab in {root_dir}')
+        print(f'Searching for Matlab {self.ver} in {root_dir}')
         def find_file(path, filename, max_depth=3):
             """ Finds a file, will return first match"""
             for depth in range(max_depth + 1):
                 dirglobs = f'*{os.sep}'*depth
                 files = glob.glob(f'{path}{os.sep}{dirglobs}{filename}')
                 files = list(filter(os.path.isfile, files))
                 if len(files) > 0:
@@ -198,30 +211,37 @@
             mlPath += get_matlab_from_registry(self.ver) + GUESSES['Windows']
         if 'MATLABEXECUTABLE' in os.environ: # Running in CI
             ml_env = os.environ['MATLABEXECUTABLE']
             if self.system == 'Windows' and ':' not in ml_env:
                 pp = ml_env.split('/')[1:]
                 ml_env = pp[0] + ':\\' + '\\'.join(pp[1:])
             mlPath += [os.path.abspath(os.path.join(ml_env, '..', '..'))]
-            print(f'mlPath={mlPath}')
         for possible_dir in mlPath + GUESSES[self.system]:
             if os.path.isdir(possible_dir):
                 rv = self.find_version(possible_dir)
                 if rv is not None:
                    return rv
         return None
 
-    def guess_from_env(self):
-        ld_path = os.getenv(self.path_var)
+    def guess_from_env(self, ld_path=None):
+        if ld_path is None:
+            ld_path = os.getenv(self.path_var)
         if ld_path is None: return None
         for possible_dir in ld_path.split(self.sep):
             if os.path.exists(os.path.join(possible_dir, self.file_to_find)):
                 return os.path.abspath(os.path.join(possible_dir, '..', '..'))
         return None
 
+    def guess_from_syspath(self):
+        matlab_exe = shutil.which('matlab')
+        if matlab_exe is None:
+            return None if self.system == 'Windows' else self.guess_from_env('PATH')
+        mlbinpath = os.path.dirname(os.path.realpath(matlab_exe))
+        return self.find_version(os.path.abspath(os.path.join(mlbinpath, '..')))
+
     def env_not_set(self):
         # Determines if the environment variables required by the MCR are set
         if self.path_var not in os.environ:
             return True
         rt = os.path.join('runtime', self.arch)
         pv = os.getenv(self.path_var).split(self.sep)
         for path in [dd for dd in pv if rt in dd]:
@@ -238,15 +258,15 @@
         if self.path_var not in os.environ:
             os.environ[self.path_var] = req_matlab_dirs
         else:
             os.environ[self.path_var] += self.sep + req_matlab_dirs
         return None
 
 
-def checkPath(runtime_version, mlPath=None):
+def checkPath(runtime_version, mlPath=None, error_if_not_found=True):
     """
     Sets the environmental variables for Win, Mac, Linux
 
     :param mlPath: Path to the SDK i.e. '/MATLAB/MATLAB_Runtime/v96' or to the location where matlab is installed
     (MATLAB root directory)
     :return: None
     """
@@ -257,18 +277,20 @@
     if mlPath:
         if not os.path.exists(os.path.join(mlPath)):
             if not os.path.exists(mlPath):
                 raise FileNotFoundError(f'Input Matlab folder {mlPath} not found')
     else:
         mlPath = obj.guess_from_env()
         if mlPath is None:
+            mlPath = obj.guess_from_syspath()
+        if mlPath is None:
             mlPath = obj.guess_path()
-            if mlPath is None:
-                raise RuntimeError('Cannot find Matlab')
-            else:
+            if mlPath is not None:
                 ld_path = obj.sep.join([os.path.join(mlPath, sub, obj.arch) for sub in obj.required_dirs])
                 os.environ[obj.path_var] = ld_path
                 #print('Set ' + os.environ.get(obj.path_var))
+            elif error_if_not_found:
+                raise RuntimeError('Cannot find Matlab')
         #else:
         #    print('Found: ' + os.environ.get(obj.path_var))
 
     return mlPath
```

## Comparing `libpymcr-0.1.5.dist-info/LICENSE` & `libpymcr-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `libpymcr-0.1.5.dist-info/METADATA` & `libpymcr-0.1.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libpymcr
-Version: 0.1.5
+Version: 0.1.6
 Summary: A module to allow Python to call functions from a compiled Matlab archive
 Home-page: https://github.com/pace-neutrons/libpymcr
 Author: Duc Le
 Author-email: duc.le@stfc.ac.uk
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

## Comparing `libpymcr-0.1.5.dist-info/RECORD` & `libpymcr-0.1.6.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 libpymcr/IPythonMagics.py,sha256=pXQHHYagcEXw7iZGF3VMJUmyvWmQMxL-sldW-RN2SKI,11938
-libpymcr/Matlab.py,sha256=w6v2XsjpmL1Lvp7QNVfnykVE95CNwH03uiKmy4aq1LY,7040
-libpymcr/MatlabProxyObject.py,sha256=w6fX-jh2WML8Dv497VNYEtzeYUKVZ3GerNL4zezdwFs,9787
+libpymcr/Matlab.py,sha256=gZJ_UOMF3S4VMBCzBl5HO7kkjHlnYop0YynIaFVv9qE,7227
+libpymcr/MatlabProxyObject.py,sha256=D5dJ1rDfj03rN-rotjGLnijp8jiwUDLoDWXr2zEmO9Q,10743
 libpymcr/__init__.py,sha256=8JZK4bh6W7u1D08OTswo67YzlP5JxLmmHTx-9MPazqU,203
-libpymcr/_libpymcr.cp39-win_amd64.pyd,sha256=oew8eIioPA_ErxnQHxVqf-ZA07DrG5FOnXGfoec4K3c,451072
-libpymcr/_version.py,sha256=-jrnx_0sYgG1MF7lTGN4SKJ4HKaINVX7LOgmLuVpB44,518
-libpymcr/utils.py,sha256=cjaeyGwn9346iyZ2ZkkmABTij_2rx3zA4uvDbL9aDH8,12472
-libpymcr-0.1.5.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-libpymcr-0.1.5.dist-info/METADATA,sha256=h1hcrbuqqxImVMdrnD_rMGrAW0TlTe3JfOzHQ65Vwxk,2586
-libpymcr-0.1.5.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
-libpymcr-0.1.5.dist-info/top_level.txt,sha256=7E4jMHPIgnPj46vaLZmiMiSc-OFs_0oKOg4MSISOxDU,9
-libpymcr-0.1.5.dist-info/RECORD,,
+libpymcr/_libpymcr.cp39-win_amd64.pyd,sha256=n4k2m77sI3gzEULxfMLZ7WTHeunHBk7ExRlqiPDDLdk,458240
+libpymcr/_version.py,sha256=xIQBOoQxoIhgIErrBDa-aTtbSWREZdHc3qvqr3RK_nk,518
+libpymcr/utils.py,sha256=cu80K_8s82IBWdTd4DZCNyqzJe5N1Jl1eu5pdaU_8Kw,13420
+libpymcr-0.1.6.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+libpymcr-0.1.6.dist-info/METADATA,sha256=-omDSLe_FLyCQWuBwVPgjXS59pmGm8o4UVCM7ppWOko,2586
+libpymcr-0.1.6.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+libpymcr-0.1.6.dist-info/top_level.txt,sha256=7E4jMHPIgnPj46vaLZmiMiSc-OFs_0oKOg4MSISOxDU,9
+libpymcr-0.1.6.dist-info/RECORD,,
```

