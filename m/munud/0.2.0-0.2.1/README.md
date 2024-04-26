# Comparing `tmp/munud-0.2.0.tar.gz` & `tmp/munud-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "munud-0.2.0.tar", max compression
+gzip compressed data, was "munud-0.2.1.tar", max compression
```

## Comparing `munud-0.2.0.tar` & `munud-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1063 2024-03-27 15:50:13.370314 munud-0.2.0/LICENSE
--rw-r--r--   0        0        0     6364 2024-03-27 15:50:13.370314 munud-0.2.0/README.md
--rw-r--r--   0        0        0     1173 2024-03-27 15:50:13.371314 munud-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       48 2024-03-27 15:50:13.371314 munud-0.2.0/src/munud/__init__.py
--rw-r--r--   0        0        0     6896 2024-03-27 15:50:13.371314 munud-0.2.0/src/munud/cgen.py
--rw-r--r--   0        0        0     4547 2024-03-27 15:50:13.371314 munud-0.2.0/src/munud/cgen_types.py
--rw-r--r--   0        0        0     5279 2024-03-27 15:50:13.371314 munud-0.2.0/src/munud/main.py
--rw-r--r--   0        0        0     5334 2024-03-27 15:50:13.371314 munud-0.2.0/src/munud/munud.py
--rw-r--r--   0        0        0    12280 2024-03-27 15:50:13.372314 munud-0.2.0/src/munud/munud_types.py
--rw-r--r--   0        0        0      711 2024-03-27 15:50:13.372314 munud-0.2.0/src/munud/utils.py
--rw-r--r--   0        0        0     7233 1970-01-01 00:00:00.000000 munud-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-26 13:31:20.432597 munud-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6554 2024-04-26 13:31:20.433597 munud-0.2.1/README.md
+-rw-r--r--   0        0        0     1219 2024-04-26 13:31:20.434597 munud-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-04-26 13:31:20.434597 munud-0.2.1/src/munud/__init__.py
+-rw-r--r--   0        0        0     7483 2024-04-26 13:31:20.434597 munud-0.2.1/src/munud/cgen.py
+-rw-r--r--   0        0        0     4547 2024-04-26 13:31:20.434597 munud-0.2.1/src/munud/cgen_types.py
+-rw-r--r--   0        0        0     5649 2024-04-26 13:31:20.434597 munud-0.2.1/src/munud/main.py
+-rw-r--r--   0        0        0     5334 2024-04-26 13:31:20.434597 munud-0.2.1/src/munud/munud.py
+-rw-r--r--   0        0        0    12280 2024-04-26 13:31:20.434597 munud-0.2.1/src/munud/munud_types.py
+-rw-r--r--   0        0        0      711 2024-04-26 13:31:20.434597 munud-0.2.1/src/munud/utils.py
+-rw-r--r--   0        0        0     7423 1970-01-01 00:00:00.000000 munud-0.2.1/PKG-INFO
```

### Comparing `munud-0.2.0/LICENSE` & `munud-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `munud-0.2.0/README.md` & `munud-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -244,29 +244,32 @@
 
 Many options are available for customisation :
 
 ```bash
 
 $ munud cgen --help
 
-Usage: munud cgen [OPTIONS]
+Usage: munud.cmd cgen [OPTIONS]
 
 Options:
   -f, --fmt TEXT          A file describing the wanted format.
   -o, --output TEXT       The output .h file.
   --crlf                  Use \r\n (crlf) as newline instead of \n (crlf).
   --use-assert            Generate assert check before writing to payload.
   --get-only              Generate only getters.
   --set-only              Generate only setters.
   --without-struct        Do not generate a struct containing the payload.
   --packed-struct         Add the gcc __attribute__((packed)) attribute to the
                           struct.
   -n, --struct-name TEXT  Payload struct name.
   --without-safety-mask   Removes the 0xff mask when writing ints on bytes.
   --payload-type TEXT     The type of the payload, usually uint8_t*.
+  --cpp                   Generate cpp-style namespace.
+  --namespace TEXT        The name of an optional namespace. If cpp is not
+                          enabled, add it as a prefix.
   --help                  Show this message and exit.
 ```
 
 # Development
 
 This library uses poetry as a development tool.
```

### Comparing `munud-0.2.0/pyproject.toml` & `munud-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "munud"
-version = "0.2.0"
+version = "0.2.1"
 description = "Building sub-byte payloads, and generating according C code"
 authors = ["Ulysse Moreau <u.moreau@hexa-h.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Topic :: Software Development :: Embedded Systems",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pyyaml = "^6.0.1"
 click = "^8.1.7"
```

### Comparing `munud-0.2.0/src/munud/cgen.py` & `munud-0.2.1/src/munud/cgen.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 def build_getter(
     var_name,
     var_type,
     bit_size,
     offset,
     newline="\n",
     payload_type="uint8_t",
+    func_prefix="",
 ) -> str:
 
     get_function_args = [
         CFuncArg("payload", payload_type),
     ]
 
     ub = UnalignedBytes(
         offset,
         bit_size,
     )
 
     get_function = CFunc(
         var_type,
-        f"get_{var_name}",
+        f"{func_prefix}get_{var_name}",
         get_function_args,
         CCodeBlock(
             [
                 CCodeStatement(
                     ub.op_read().to_c_expr(),
                 ),
             ],
@@ -53,14 +54,15 @@
     var_type,
     bit_size,
     offset,
     newline="\n",
     safety_mask=True,
     payload_type="uint8_t",
     use_assert=False,
+    func_prefix="",
 ) -> str:
 
     set_function_args = [
         CFuncArg("payload", payload_type),
         CFuncArg("value", var_type),
     ]
 
@@ -82,15 +84,15 @@
             CCodeStatement(
                 statement.to_c_expr(),
             ),
         )
 
     get_function = CFunc(
         "void",
-        f"set_{var_name}",
+        f"{func_prefix}set_{var_name}",
         set_function_args,
         CCodeBlock(
             cstatements,
             newline,
         ),
         ub.setter_c_docstring(var_name, newline),
         newline,
@@ -133,14 +135,16 @@
     newline="\n",
     use_assert=False,
     generate_getters=True,
     generate_setters=True,
     generate_struct=True,
     packed_struct=False,
     safety_mask=True,
+    cpp=False,
+    namespace=None,
     payload_type="uint8_t*",
     struct_name="Payload",
 ) -> str:
     """Generates C code from a payload representation.
 
     Args:
         format_list (list[dict]): The format of the payload.
@@ -156,14 +160,25 @@
     Returns:
         str: The according c code.
     """
     generated_c_code = ""
     generated_c_code += get_header_with_date()
     generated_c_code += get_includes(no_assert=use_assert)
 
+    funcs_prefix = ""
+
+    if namespace:
+        if cpp:
+            generated_c_code += f"\nnamespace {namespace} {{"
+        else:
+            funcs_prefix = namespace
+
+    if funcs_prefix:
+        funcs_prefix += "_"
+
     struct_components: list[CStructArg] = []
 
     for var_name, offset, var_size, var_type in payload_generator(format_list):
 
         if var_type not in ALLOWED_VAR_TYPES:
             raise ValueError(
                 f"{var_type} : unknown variable type (should be one of uint8_t, uint16_t, uint32_t, uint64_t)"
@@ -178,14 +193,15 @@
             generated_c_code += build_getter(
                 var_name,
                 var_type,
                 var_size,
                 offset,
                 newline=newline,
                 payload_type=payload_type,
+                func_prefix=funcs_prefix,
             )
 
         if generate_setters:
 
             generated_c_code += newline * 2
 
             generated_c_code += build_setter(
@@ -193,14 +209,15 @@
                 var_type,
                 var_size,
                 offset,
                 newline=newline,
                 safety_mask=safety_mask,
                 payload_type=payload_type,
                 use_assert=use_assert,
+                func_prefix=funcs_prefix,
             )
 
         generated_c_code += "\n"
 
     if generate_struct:
 
         generated_c_code += newline * 2
@@ -209,15 +226,15 @@
         )
         generated_c_code += newline * 2
 
     if generate_getters and generate_struct:
 
         decode_all = CFunc(
             "void",
-            "decode",
+            f"{funcs_prefix}decode",
             [
                 CFuncArg("payload", f"struct {struct_name}*"),
                 CFuncArg("packed", "uint8_t*"),
             ],
             CCodeBlock(
                 [
                     *[
@@ -234,15 +251,15 @@
         generated_c_code += newline * 2
         generated_c_code += str(decode_all)
 
     if generate_setters and generate_struct:
 
         encode_all = CFunc(
             "void",
-            "encode",
+            f"{funcs_prefix}encode",
             [
                 CFuncArg("payload", f"struct {struct_name}*"),
                 CFuncArg("packed", "uint8_t*"),
             ],
             CCodeBlock(
                 [
                     *[
@@ -255,8 +272,14 @@
             ),
             "",
         )
 
         generated_c_code += newline * 2
         generated_c_code += str(encode_all)
 
+    if namespace and cpp:
+        generated_c_code += "\n"
+        generated_c_code += f"\n}} // namespace {namespace}"
+
+    generated_c_code += "\n"
+
     return generated_c_code
```

### Comparing `munud-0.2.0/src/munud/cgen_types.py` & `munud-0.2.1/src/munud/cgen_types.py`

 * *Files identical despite different names*

### Comparing `munud-0.2.0/src/munud/main.py` & `munud-0.2.1/src/munud/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,28 +77,42 @@
     help="Removes the 0xff mask when writing ints on bytes.",
 )
 @click.option(
     "--payload-type",
     default="uint8_t*",
     help="The type of the payload, usually uint8_t*.",
 )
+@click.option(
+    "--cpp",
+    is_flag=True,
+    show_default=True,
+    default=False,
+    help="Generate cpp-style namespace.",
+)
+@click.option(
+    "--namespace",
+    default="",
+    help="The name of an optional namespace. If cpp is not enabled, add it as a prefix.",
+)
 @click.pass_context
 def cgen(
     ctx,
     fmt,
     output,
     crlf,
     use_assert,
     get_only,
     set_only,
     without_struct,
     packed_struct,
     struct_name,
     without_safety_mask,
     payload_type,
+    cpp,
+    namespace,
 ):
 
     if not fmt:
         if not hasattr(ctx, "obj"):
             print("Please specify a format (--fmt).")
             return
 
@@ -119,22 +133,24 @@
             generate_getters=not set_only,
             generate_setters=not get_only,
             generate_struct=not without_struct,
             packed_struct=packed_struct,
             safety_mask=not without_safety_mask,
             payload_type=payload_type,
             struct_name=struct_name,
+            cpp=cpp,
+            namespace=namespace,
         )
 
     if output:
         with open(output, "w") as outfile:
             outfile.write(c_file_result)
     else:
         console = Console()
-        syntax = Syntax(c_file_result, "c")
+        syntax = Syntax(c_file_result, "cpp" if cpp else "c")
         console.print(syntax)
 
 
 @main.command()
 @click.option("-f", "--fmt", help="A file describing the wanted format.")
 @click.pass_context
 def show(ctx, fmt):
```

### Comparing `munud-0.2.0/src/munud/munud.py` & `munud-0.2.1/src/munud/munud.py`

 * *Files identical despite different names*

### Comparing `munud-0.2.0/src/munud/munud_types.py` & `munud-0.2.1/src/munud/munud_types.py`

 * *Files identical despite different names*

### Comparing `munud-0.2.0/src/munud/utils.py` & `munud-0.2.1/src/munud/utils.py`

 * *Files identical despite different names*

### Comparing `munud-0.2.0/PKG-INFO` & `munud-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: munud
-Version: 0.2.0
+Version: 0.2.1
 Summary: Building sub-byte payloads, and generating according C code
 License: MIT
 Author: Ulysse Moreau
 Author-email: u.moreau@hexa-h.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -267,29 +267,32 @@
 
 Many options are available for customisation :
 
 ```bash
 
 $ munud cgen --help
 
-Usage: munud cgen [OPTIONS]
+Usage: munud.cmd cgen [OPTIONS]
 
 Options:
   -f, --fmt TEXT          A file describing the wanted format.
   -o, --output TEXT       The output .h file.
   --crlf                  Use \r\n (crlf) as newline instead of \n (crlf).
   --use-assert            Generate assert check before writing to payload.
   --get-only              Generate only getters.
   --set-only              Generate only setters.
   --without-struct        Do not generate a struct containing the payload.
   --packed-struct         Add the gcc __attribute__((packed)) attribute to the
                           struct.
   -n, --struct-name TEXT  Payload struct name.
   --without-safety-mask   Removes the 0xff mask when writing ints on bytes.
   --payload-type TEXT     The type of the payload, usually uint8_t*.
+  --cpp                   Generate cpp-style namespace.
+  --namespace TEXT        The name of an optional namespace. If cpp is not
+                          enabled, add it as a prefix.
   --help                  Show this message and exit.
 ```
 
 # Development
 
 This library uses poetry as a development tool.
```

