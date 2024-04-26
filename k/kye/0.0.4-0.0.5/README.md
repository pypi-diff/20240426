# Comparing `tmp/kye-0.0.4.tar.gz` & `tmp/kye-0.0.5.tar.gz`

## Comparing `kye-0.0.4.tar` & `kye-0.0.5.tar`

### file list

```diff
@@ -1,88 +1,45 @@
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 kye-0.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kye-0.0.4/publish.sh
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 kye-0.0.4/requirements.txt
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 kye-0.0.4/setup.cfg
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 kye-0.0.4/.github/workflows/python-app.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/.gitignore
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/api.py
--rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/compile.old.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/compiled.py
--rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/environment.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/evaluate.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/expressions.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/flatten_ast.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/parser.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/py_evaluate.py
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/selection.py
--rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/types.1.py
--rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/types.py
--rw-r--r--   0        0        0    13581 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/validate.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/loader/json_lines.py
--rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/loader/loader.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 kye-0.0.4/.trash/translate/to_json_schema.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 kye-0.0.4/data/.gitignore
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 kye-0.0.4/data/User.jsonl
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 kye-0.0.4/data/Yellow.jsonl
--rw-r--r--   0        0        0  1060864 2020-02-02 00:00:00.000000 kye-0.0.4/data/data.db
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/coverage_html.js
--rw-r--r--   0        0        0    28299 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_1664f9f2c88134c6_json_lines_py.html
--rw-r--r--   0        0        0    49872 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_1664f9f2c88134c6_loader_py.html
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_56f4dd0dacba1e5e___about___py.html
--rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_56f4dd0dacba1e5e___init___py.html
--rw-r--r--   0        0        0    18752 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_56f4dd0dacba1e5e_api_py.html
--rw-r--r--   0        0        0    71929 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_56f4dd0dacba1e5e_compile_py.html
--rw-r--r--   0        0        0    23928 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_56f4dd0dacba1e5e_compiled_py.html
--rw-r--r--   0        0        0   109729 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_56f4dd0dacba1e5e_compiler_py.html
--rw-r--r--   0        0        0    46685 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_56f4dd0dacba1e5e_dataset_py.html
--rw-r--r--   0        0        0    25131 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_56f4dd0dacba1e5e_errors_py.html
--rw-r--r--   0        0        0     6674 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_56f4dd0dacba1e5e_evaluate_py.html
--rw-r--r--   0        0        0    66210 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_56f4dd0dacba1e5e_types_py.html
--rw-r--r--   0        0        0   117838 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_56f4dd0dacba1e5e_validate_py.html
--rw-r--r--   0        0        0    39177 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_9ccc2a893861ae93_engine_py.html
--rw-r--r--   0        0        0    15959 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_9ccc2a893861ae93_load_json_py.html
--rw-r--r--   0        0        0    40370 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_9ccc2a893861ae93_validate_py.html
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b___init___py.html
--rw-r--r--   0        0        0    19538 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_assign_scopes_py.html
--rw-r--r--   0        0        0    11694 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_assign_type_refs_py.html
--rw-r--r--   0        0        0    32969 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_compile_py.html
--rw-r--r--   0        0        0    29985 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_edges_py.html
--rw-r--r--   0        0        0    45631 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_environment_py.html
--rw-r--r--   0        0        0    26711 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_evaluate_py.html
--rw-r--r--   0        0        0    82633 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_expressions_py.html
--rw-r--r--   0        0        0    32129 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_flatten_ast_py.html
--rw-r--r--   0        0        0    54933 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_kye_ast_py.html
--rw-r--r--   0        0        0    22015 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_kye_evaluate_py.html
--rw-r--r--   0        0        0    52041 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_kye_transformer_py.html
--rw-r--r--   0        0        0    12081 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_parser_py.html
--rw-r--r--   0        0        0    38758 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_type_evaluation_py.html
--rw-r--r--   0        0        0    91531 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/d_aaef51656e53cb8b_types_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     6666 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 kye-0.0.4/htmlcov/style.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 kye-0.0.4/kye/__about__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 kye-0.0.4/kye/__init__.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 kye-0.0.4/kye/api.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 kye-0.0.4/kye/errors.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 kye-0.0.4/kye/compiler/assertion.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 kye-0.0.4/kye/compiler/compiled.py
--rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 kye-0.0.4/kye/compiler/from_ast.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 kye-0.0.4/kye/compiler/from_compiled.py
--rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 kye-0.0.4/kye/compiler/models.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 kye-0.0.4/kye/engine/engine.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 kye-0.0.4/kye/engine/load_json.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 kye-0.0.4/kye/engine/validate.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 kye-0.0.4/kye/parser/kye_ast.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 kye-0.0.4/kye/parser/kye_transformer.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 kye-0.0.4/kye/parser/parser.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 kye-0.0.4/kye/parser/grammars/definitions.lark
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 kye-0.0.4/kye/parser/grammars/expressions.lark
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kye-0.0.4/kye/parser/grammars/tokens.lark
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 kye-0.0.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 kye-0.0.4/LICENSE
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 kye-0.0.4/README.md
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 kye-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 kye-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 kye-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kye-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 kye-0.0.5/setup.cfg
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 kye-0.0.5/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/.gitignore
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/api.py
+-rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/compile.old.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/compiled.py
+-rw-r--r--   0        0        0     4147 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/environment.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/evaluate.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/expressions.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/flatten_ast.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/parser.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/py_evaluate.py
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/selection.py
+-rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/types.1.py
+-rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/types.py
+-rw-r--r--   0        0        0    13561 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/validate.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/engine/engine.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/engine/load_json.py
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/engine/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/inspired_by_sqlglot/__init__.py
+-rw-r--r--   0        0        0    34718 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/inspired_by_sqlglot/expressions.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/inspired_by_sqlglot/iter_utils.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/inspired_by_sqlglot/types.2.py
+-rw-r--r--   0        0        0     9243 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/inspired_by_sqlglot/types.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/loader/json_lines.py
+-rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/loader/loader.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 kye-0.0.5/.trash/translate/to_json_schema.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 kye-0.0.5/kye/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kye-0.0.5/kye/__init__.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 kye-0.0.5/kye/cli.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 kye-0.0.5/kye/errors.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 kye-0.0.5/kye/expressions.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 kye-0.0.5/kye/grammar.lark
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 kye-0.0.5/kye/interpreter.py
+-rw-r--r--   0        0        0    25136 2020-02-02 00:00:00.000000 kye-0.0.5/kye/kye_parser.py
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 kye-0.0.5/kye/parser.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 kye-0.0.5/kye/tests.md
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 kye-0.0.5/kye/types.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 kye-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 kye-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 kye-0.0.5/README.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 kye-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 kye-0.0.5/PKG-INFO
```

### Comparing `kye-0.0.4/CODE_OF_CONDUCT.md` & `kye-0.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.github/workflows/python-app.yml` & `kye-0.0.5/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/api.py` & `kye-0.0.5/.trash/api.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/compile.old.py` & `kye-0.0.5/.trash/compile.old.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/compiled.py` & `kye-0.0.5/.trash/compiled.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/environment.py` & `kye-0.0.5/.trash/environment.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/evaluate.py` & `kye-0.0.5/.trash/evaluate.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/expressions.py` & `kye-0.0.5/.trash/expressions.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/flatten_ast.py` & `kye-0.0.5/.trash/flatten_ast.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/parser.py` & `kye-0.0.5/.trash/parser.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/py_evaluate.py` & `kye-0.0.5/.trash/py_evaluate.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/selection.py` & `kye-0.0.5/.trash/selection.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/types.1.py` & `kye-0.0.5/.trash/types.1.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/types.py` & `kye-0.0.5/.trash/types.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/validate.py` & `kye-0.0.5/.trash/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,14 @@
             if partial_index is None:
                 partial_index = r
             else:
                 partial_index = partial_index.union(r)
         r = partial_index.join(global_index, 'row', how='left')
         partial_map = r.aggregate('partial, unnest(list_distinct(list(idx))) as idx').set_alias('partial_map')
         r = r.select('row, partial').join(partial_map, 'partial').aggregate('row, list(distinct idx) as idx')
-        print('hi')
         # r = self.collect('row',{
         #     'idx': self.row_index(self.typ.index),
         #     **({
         #         f'idx_{i}': self.row_index(idx)
         #         for i,idx in enumerate(self.typ.indexes)
         #     }),
         # })
```

### Comparing `kye-0.0.4/.trash/loader/json_lines.py` & `kye-0.0.5/.trash/loader/json_lines.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/loader/loader.py` & `kye-0.0.5/.trash/loader/loader.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/.trash/translate/to_json_schema.py` & `kye-0.0.5/.trash/translate/to_json_schema.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/kye/engine/engine.py` & `kye-0.0.5/.trash/engine/engine.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/kye/engine/load_json.py` & `kye-0.0.5/.trash/engine/load_json.py`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/kye/engine/validate.py` & `kye-0.0.5/.trash/engine/validate.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,17 +4,28 @@
 def struct_pack(edges: list[str], r: DuckDBPyRelation):
     return 'struct_pack(' + ','.join(
         f'''"{edge_name}":="{edge_name}"'''
         for edge_name in edges
             if edge_name in r.columns
     ) + ')'
 
-def string_list(strings: list[str]):
-    # TODO: Escape strings
-    return "'" + "','".join(strings) + "'"
+def format_value(val):
+    if isinstance(val, float):
+        val = str(val)
+        return val[:-2] if val.endswith('.0') else val
+    if isinstance(val, int):
+        return str(val)
+    if isinstance(val, bool):
+        return 'true' if val else 'false'
+    if isinstance(val, str):
+        return "'" + val.replace('\\', '\\\\').replace("'","\\'") + "'"
+    raise ValueError('Unknown value type')
+
+def value_list(strings: list[str]):
+    return ','.join(format_value(string) for string in strings)
 
 def flag(err_msg: str, condition: str, r: DuckDBPyRelation, **kwargs):
     fields = ["'" + err_msg + "'"]
     for field in ['tbl','idx','row','col','val']:
         if field in kwargs:
             if kwargs[field] is None:
                 fields.append('NULL')
@@ -53,15 +64,15 @@
     # Create a map of partial ids to full ids
     partial_map = r.aggregate('partial, unnest(list_distinct(list(idx))) as idx').set_alias('partial_map')
     # Redefine index using the partial_map
     r = r.select('row, partial').join(partial_map, 'partial', how='left')
     return r
 
 def compute_index(typ: Type, table: DuckDBPyRelation):
-    edges = table.filter(f'''col in ({string_list(typ.index)})''')
+    edges = table.filter(f'''col in ({value_list(typ.index)})''')
     edges = flag('CONFLICTING_INDEX', 'cnt > 1',
         edges.aggregate('''row, col, first(val) as val, count(distinct(val)) as cnt'''), tbl=typ.ref, val=None)
     edges = collect('row', {
         col: edges.filter(f"col = '{col}'").select('row, val')
         for col in typ.index
     })
     indexes = row_indexes(edges, typ)
@@ -84,17 +95,29 @@
              table.aggregate('tbl,idx').join(column.select('tbl,idx').set_alias('col'), 'tbl,idx', how='anti'))
     check_value(typ.get_edge(edge), column)
 
 def check_value(typ: Type, col: DuckDBPyRelation):
     for assertion in typ.assertions:
         if assertion.op == 'type':
             if assertion.arg == 'number':
-                flag('INVALID_VALUE_TYPE', 'TRY_CAST(val as DOUBLE) IS NULL', col)
-            if assertion.arg == 'boolean':
-                flag('INVALID_VALUE_TYPE', 'TRY_CAST(val as BOOLEAN) IS NULL', col)
+                col = flag('INVALID_VALUE', 'TRY_CAST(val as DOUBLE) IS NULL', col)
+            elif assertion.arg == 'boolean':
+                col = flag('INVALID_VALUE', 'TRY_CAST(val as BOOLEAN) IS NULL', col)
+        elif assertion.op == 'eq':
+            col = flag('INVALID_VALUE', f'val NOT IN ({value_list(assertion.arg)})', col)
+        elif assertion.op == 'ne':
+            col = flag('INVALID_VALUE', f'val IN ({value_list(assertion.arg)})', col)
+        elif assertion.op == 'gt':
+            col = flag('INVALID_VALUE', f'val <= {format_value(assertion.arg)}', col)
+        elif assertion.op == 'gte':
+            col = flag('INVALID_VALUE', f'val < {format_value(assertion.arg)}', col)
+        elif assertion.op == 'lt':
+            col = flag('INVALID_VALUE', f'val >= {format_value(assertion.arg)}', col)
+        elif assertion.op == 'lte':
+            col = flag('INVALID_VALUE', f'val > {format_value(assertion.arg)}', col)
 
 def check_table(typ: Type, db: DuckDBPyConnection):
     table = db.table('edges').filter(f'''tbl = '{typ.ref}' ''')
     index = compute_index(typ, table)
     db.sql(f'''
     UPDATE edges
         SET idx=index.idx
```

### Comparing `kye-0.0.4/LICENSE` & `kye-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/README.md` & `kye-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `kye-0.0.4/pyproject.toml` & `kye-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,20 +14,21 @@
   { name = "Benjamin Earl", email = "14208829+benjameep@users.noreply.github.com" },
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
-  "pydantic",
-  "duckdb",
   "lark",
   "lark[interegular]",
 ]
 
 [project.urls]
 Documentation = "https://github.com/kyelabs/kyepy#readme"
 Issues = "https://github.com/kyelabs/kyepy/issues"
 Source = "https://github.com/kyelabs/kyepy"
 
+[project.scripts]
+kye = "kye.cli:main"
+
 [tool.hatch.version]
 path = "kye/__about__.py"
```

### Comparing `kye-0.0.4/PKG-INFO` & `kye-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: kye
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Data Validation Framework
 Project-URL: Documentation, https://github.com/kyelabs/kyepy#readme
 Project-URL: Issues, https://github.com/kyelabs/kyepy/issues
 Project-URL: Source, https://github.com/kyelabs/kyepy
 Author-email: Benjamin Earl <14208829+benjameep@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: duckdb
 Requires-Dist: lark
 Requires-Dist: lark[interegular]
-Requires-Dist: pydantic
 Description-Content-Type: text/markdown
 
 # Kye Validation Tool
 Kye is a validation tool in progress that allows you to define and validate
 models for your data.
 
 # Getting Started
```

