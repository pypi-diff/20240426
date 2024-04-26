# Comparing `tmp/sparkautomapper-2.0.6.tar.gz` & `tmp/sparkautomapper-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkautomapper-2.0.6.tar", last modified: Fri Oct  6 20:42:05 2023, max compression
+gzip compressed data, was "sparkautomapper-2.0.7.tar", last modified: Fri Apr 26 10:45:03 2024, max compression
```

## Comparing `sparkautomapper-2.0.6.tar` & `sparkautomapper-2.0.7.tar`

### file list

```diff
@@ -1,346 +1,350 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.224043 sparkautomapper-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9661 2023-10-06 20:42:05.224043 sparkautomapper-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-06 20:42:04.000000 sparkautomapper-2.0.6/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-10-06 20:42:05.224043 sparkautomapper-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.184038 sparkautomapper-2.0.6/spark_auto_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.184038 sparkautomapper-2.0.6/spark_auto_mapper/automappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/automappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31339 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/automappers/automapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/automappers/automapper_analysis_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/automappers/automapper_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/automappers/automapper_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/automappers/check_schema_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/automappers/column_spec_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/automappers/columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/automappers/complex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/automappers/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/automappers/with_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/automappers/with_column_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.192040 sparkautomapper-2.0.6/spark_auto_mapper/data_types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/array_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/array_distinct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/array_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/coalesce.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/column.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/column_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.192040 sparkautomapper-2.0.6/spark_auto_mapper/data_types/complex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/complex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/complex/complex.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/complex/complex_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/complex/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/cross_column_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    41355 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/data_type_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/date_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/exists.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/first.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/first_valid_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/hash_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/if_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/if_column_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/if_not.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/if_not_null.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/if_not_null_or_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/if_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/join_using_delimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/lpad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.192040 sparkautomapper-2.0.6/spark_auto_mapper/data_types/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/nested_array_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/null_if_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/null_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/regex_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/regex_replace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/split_by_delimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/substring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/substring_by_delimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/text_like_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/to_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/trim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/data_types/unix_timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.196040 sparkautomapper-2.0.6/spark_auto_mapper/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30239 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/helpers/automapper_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/helpers/capture_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/helpers/expression_comparer.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/helpers/field_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/helpers/python_keyword_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/helpers/spark_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/helpers/value_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.196040 sparkautomapper-2.0.6/spark_auto_mapper/type_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/type_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/type_definitions/defined_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/type_definitions/native_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/spark_auto_mapper/type_definitions/wrapper_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.196040 sparkautomapper-2.0.6/sparkautomapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9661 2023-10-06 20:42:05.000000 sparkautomapper-2.0.6/sparkautomapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11939 2023-10-06 20:42:05.000000 sparkautomapper-2.0.6/sparkautomapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 20:42:05.000000 sparkautomapper-2.0.6/sparkautomapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 20:42:05.000000 sparkautomapper-2.0.6/sparkautomapper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-10-06 20:42:05.000000 sparkautomapper-2.0.6/sparkautomapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-06 20:42:05.000000 sparkautomapper-2.0.6/sparkautomapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.196040 sparkautomapper-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.200040 sparkautomapper-2.0.6/tests/amount/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/amount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/amount/test_automapper_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/amount/test_automapper_amount_typed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.200040 sparkautomapper-2.0.6/tests/array/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/array/test_automapper_array_typed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.200040 sparkautomapper-2.0.6/tests/array_distinct/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/array_distinct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/array_distinct/test_automapper_array_distinct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.200040 sparkautomapper-2.0.6/tests/array_max/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/array_max/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/array_max/test_automapper_array_max.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.200040 sparkautomapper-2.0.6/tests/base64/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/base64/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/base64/test_automapper_base64.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.200040 sparkautomapper-2.0.6/tests/boolean/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/boolean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/boolean/test_automapper_boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/boolean/test_automapper_boolean_typed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.200040 sparkautomapper-2.0.6/tests/cast/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/cast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/cast/test_cast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.200040 sparkautomapper-2.0.6/tests/cast_to_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/cast_to_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/cast_to_type/test_automapper_cast_to_type_typed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.200040 sparkautomapper-2.0.6/tests/checkpointing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/checkpointing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/checkpointing/test_automapper_full_checkpointing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.200040 sparkautomapper-2.0.6/tests/coalesce/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/coalesce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/coalesce/test_automapper_coalesce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.200040 sparkautomapper-2.0.6/tests/columns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/columns/test_automapper_columns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.200040 sparkautomapper-2.0.6/tests/complex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/complex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/complex/test_automapper_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/complex/test_automapper_complex_with_defined_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/complex/test_automapper_complex_with_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/complex/test_automapper_complex_with_mappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9818 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/complex/test_automapper_complex_with_skip_if_null.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.204041 sparkautomapper-2.0.6/tests/concat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/concat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/concat/test_automapper_add_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/concat/test_automapper_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/concat/test_automapper_concat_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/concat/test_automapper_concat_multiple_items_structs_different_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/concat/test_automapper_concat_multiple_items_structs_different_elements_with_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.204041 sparkautomapper-2.0.6/tests/copy_unmapped_properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/copy_unmapped_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/copy_unmapped_properties/test_automapper_copy_unmapped_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.204041 sparkautomapper-2.0.6/tests/cross_column_filter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/cross_column_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/cross_column_filter/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/cross_column_filter/test_cross_column_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.204041 sparkautomapper-2.0.6/tests/date/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/date/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/date/test_automapper_date_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/date/test_automapper_date_column_typed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/date/test_automapper_date_literal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.204041 sparkautomapper-2.0.6/tests/date_format/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/date_format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/date_format/test_automapper_date_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.204041 sparkautomapper-2.0.6/tests/decimal_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/decimal_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/decimal_type/test_automapper_decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/decimal_type/test_automapper_decimal_typed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.204041 sparkautomapper-2.0.6/tests/duplicates_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/duplicates_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/duplicates_test/test_automapper_duplicates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.204041 sparkautomapper-2.0.6/tests/exists/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/exists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/exists/test_automapper_exists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.204041 sparkautomapper-2.0.6/tests/field/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/field/test_automapper_field.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.208041 sparkautomapper-2.0.6/tests/filter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/filter/test_automapper_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.208041 sparkautomapper-2.0.6/tests/first/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/first/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/first/test_automapper_first.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.208041 sparkautomapper-2.0.6/tests/first_valid_column/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/first_valid_column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/first_valid_column/test_automapper_first_valid_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/first_valid_column/test_automapper_first_valid_column_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.208041 sparkautomapper-2.0.6/tests/flatten/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/flatten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/flatten/test_automapper_flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/flatten/test_automapper_flatten_with_null.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.208041 sparkautomapper-2.0.6/tests/hash/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/hash/test_automapper_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.208041 sparkautomapper-2.0.6/tests/hash_abs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/hash_abs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/hash_abs/test_automapper_hash_abs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.208041 sparkautomapper-2.0.6/tests/if_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_/test_automapper_if_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_/test_automapper_if_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.208041 sparkautomapper-2.0.6/tests/if_column_exists/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_column_exists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_column_exists/test_automapper_if_column_exists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.208041 sparkautomapper-2.0.6/tests/if_not/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_not/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_not/test_automapper_if_not.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_not/test_automapper_if_not_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.208041 sparkautomapper-2.0.6/tests/if_not_null/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_not_null/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6085 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_not_null/test_automapper_if_not_null.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.208041 sparkautomapper-2.0.6/tests/if_not_null_or_empty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_not_null_or_empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_not_null_or_empty/test_automapper_if_not_null_or_empty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.208041 sparkautomapper-2.0.6/tests/if_regex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_regex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/if_regex/test_automapper_if_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.212042 sparkautomapper-2.0.6/tests/join_using_delimiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/join_using_delimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/join_using_delimiter/test_automapper_join_using_delimiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.212042 sparkautomapper-2.0.6/tests/left/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/left/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/left/test_automapper_left.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.212042 sparkautomapper-2.0.6/tests/list/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/list/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.212042 sparkautomapper-2.0.6/tests/list/addition/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/list/addition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements_with_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/list/test_automapper_list_multiple_items.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/list/test_automapper_list_multiple_items_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/list/test_automapper_list_multiple_items_structs_different_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/list/test_automapper_list_multiple_items_structs_different_elements_with_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/list/test_automapper_list_multiple_items_with_null.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/list/test_automapper_list_single_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/list/test_automapper_list_single_item_with_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.212042 sparkautomapper-2.0.6/tests/lpad/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/lpad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/lpad/test_auto_mapper_lpad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.212042 sparkautomapper-2.0.6/tests/map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/map/test_automapper_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/map/test_automapper_map_col_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/map/test_automapper_map_no_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/map/test_automapper_map_null.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.212042 sparkautomapper-2.0.6/tests/multiple_columns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/multiple_columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/multiple_columns/test_automapper_multiple_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/multiple_columns/test_automapper_multiple_columns_simpler_syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.216042 sparkautomapper-2.0.6/tests/nested_array_filter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/nested_array_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/nested_array_filter/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/nested_array_filter/schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.216042 sparkautomapper-2.0.6/tests/nested_array_filter/simple/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/nested_array_filter/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/nested_array_filter/simple/test_automapper_nested_array_filter_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.216042 sparkautomapper-2.0.6/tests/nested_array_filter/simple_with_array/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/nested_array_filter/simple_with_array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/nested_array_filter/simple_with_array/test_automapper_nested_array_filter_simple_with_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/nested_array_filter/test_automapper_nested_array_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/nested_array_filter/test_automapper_nested_array_filter_expression_only.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.216042 sparkautomapper-2.0.6/tests/null_if_empty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/null_if_empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/null_if_empty/test_automapper_null_if_empty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.216042 sparkautomapper-2.0.6/tests/null_remover/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/null_remover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/null_remover/test_automapper_null_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.216042 sparkautomapper-2.0.6/tests/number/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/number/test_automapper_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/number/test_automapper_number_typed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.216042 sparkautomapper-2.0.6/tests/regex_extract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/regex_extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/regex_extract/test_auto_mapper_regex_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.216042 sparkautomapper-2.0.6/tests/regex_replace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/regex_replace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/regex_replace/test_auto_mapper_regex_replace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/regex_replace/test_auto_mapper_regex_replace_unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.216042 sparkautomapper-2.0.6/tests/right/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/right/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/right/test_automapper_right.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.216042 sparkautomapper-2.0.6/tests/sanitize/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/sanitize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/sanitize/test_auto_mapper_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.216042 sparkautomapper-2.0.6/tests/schema_pruning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/schema_pruning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/schema_pruning/test_automapper_schema_pruning_with_defined_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/schema_pruning/test_automapper_schema_pruning_with_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/schema_pruning/test_automapper_schema_pruning_with_extension_different_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.220043 sparkautomapper-2.0.6/tests/select_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/select_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/select_one/test_automapper_select_one.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.220043 sparkautomapper-2.0.6/tests/split_by_delimiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/split_by_delimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/split_by_delimiter/test_automapper_split_by_delimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform_fluent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.220043 sparkautomapper-2.0.6/tests/string_after_delimiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/string_after_delimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/string_after_delimiter/test_automapper_string_after_delimiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.220043 sparkautomapper-2.0.6/tests/string_before_delimiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/string_before_delimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/string_before_delimiter/test_automapper_string_before_delimiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.220043 sparkautomapper-2.0.6/tests/struct_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/struct_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/struct_type/test_automapper_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/struct_type/test_automapper_struct_with_mappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.220043 sparkautomapper-2.0.6/tests/substring_by_delimiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/substring_by_delimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/substring_by_delimiter/test_automapper_substring_by_delimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/test_automapper_full.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/test_automapper_full_no_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/test_automapper_full_no_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/test_automapper_full_view_exists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.220043 sparkautomapper-2.0.6/tests/to_json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/to_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/to_json/test_automapper_to_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.220043 sparkautomapper-2.0.6/tests/transform/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/transform/test_automapper_filter_and_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/transform/test_automapper_filter_and_transform_fluent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/transform/test_automapper_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.220043 sparkautomapper-2.0.6/tests/trim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/trim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/trim/test_auto_mapper_trim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.220043 sparkautomapper-2.0.6/tests/unix_timestamp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/unix_timestamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/unix_timestamp/test_automapper_unix_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/unix_timestamp/test_automapper_unix_timestamp_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/unix_timestamp/test_automapper_unix_timestamp_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 20:42:05.224043 sparkautomapper-2.0.6/tests/withColumn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/withColumn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/withColumn/test_automapper_with_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/withColumn/test_automapper_with_column_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/withColumn/test_automapper_with_column_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2023-10-06 20:40:48.000000 sparkautomapper-2.0.6/tests/withColumn/test_automapper_with_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.467862 sparkautomapper-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-04-26 10:45:03.467862 sparkautomapper-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 10:45:03.000000 sparkautomapper-2.0.7/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-26 10:45:03.471861 sparkautomapper-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.423862 sparkautomapper-2.0.7/spark_auto_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.423862 sparkautomapper-2.0.7/spark_auto_mapper/automappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/automappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31339 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/automappers/automapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/automappers/automapper_analysis_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/automappers/automapper_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/automappers/automapper_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/automappers/check_schema_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/automappers/column_spec_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/automappers/columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/automappers/complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/automappers/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/automappers/with_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/automappers/with_column_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.435862 sparkautomapper-2.0.7/spark_auto_mapper/data_types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/array_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/array_distinct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/array_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/coalesce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/column_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.435862 sparkautomapper-2.0.7/spark_auto_mapper/data_types/complex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/complex/complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/complex/complex_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/complex/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/cross_column_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41355 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/data_type_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/date_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/first_valid_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/hash_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/if_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/if_column_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/if_not.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/if_not_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/if_not_null_or_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/if_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/join_using_delimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/lower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/lpad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.435862 sparkautomapper-2.0.7/spark_auto_mapper/data_types/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/nested_array_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/null_if_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/null_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/regex_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/regex_replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/split_by_delimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/substring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/substring_by_delimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/text_like_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/to_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/trim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/data_types/unix_timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.435862 sparkautomapper-2.0.7/spark_auto_mapper/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30633 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/helpers/automapper_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/helpers/capture_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/helpers/expression_comparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/helpers/field_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/helpers/python_keyword_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/helpers/spark_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/helpers/value_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.439862 sparkautomapper-2.0.7/spark_auto_mapper/type_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/type_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/type_definitions/defined_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/type_definitions/native_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/spark_auto_mapper/type_definitions/wrapper_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.439862 sparkautomapper-2.0.7/sparkautomapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-04-26 10:45:03.000000 sparkautomapper-2.0.7/sparkautomapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-04-26 10:45:03.000000 sparkautomapper-2.0.7/sparkautomapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:45:03.000000 sparkautomapper-2.0.7/sparkautomapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:45:03.000000 sparkautomapper-2.0.7/sparkautomapper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-26 10:45:03.000000 sparkautomapper-2.0.7/sparkautomapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 10:45:03.000000 sparkautomapper-2.0.7/sparkautomapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.439862 sparkautomapper-2.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.439862 sparkautomapper-2.0.7/tests/amount/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/amount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/amount/test_automapper_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/amount/test_automapper_amount_typed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.439862 sparkautomapper-2.0.7/tests/array/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/array/test_automapper_array_typed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.439862 sparkautomapper-2.0.7/tests/array_distinct/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/array_distinct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/array_distinct/test_automapper_array_distinct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.439862 sparkautomapper-2.0.7/tests/array_max/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/array_max/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/array_max/test_automapper_array_max.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.439862 sparkautomapper-2.0.7/tests/base64/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/base64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/base64/test_automapper_base64.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.443862 sparkautomapper-2.0.7/tests/boolean/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/boolean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/boolean/test_automapper_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/boolean/test_automapper_boolean_typed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.443862 sparkautomapper-2.0.7/tests/cast/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/cast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/cast/test_cast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.443862 sparkautomapper-2.0.7/tests/cast_to_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/cast_to_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/cast_to_type/test_automapper_cast_to_type_typed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.443862 sparkautomapper-2.0.7/tests/checkpointing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/checkpointing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/checkpointing/test_automapper_full_checkpointing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.443862 sparkautomapper-2.0.7/tests/coalesce/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/coalesce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/coalesce/test_automapper_coalesce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.443862 sparkautomapper-2.0.7/tests/columns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/columns/test_automapper_columns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.443862 sparkautomapper-2.0.7/tests/complex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/complex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/complex/test_automapper_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/complex/test_automapper_complex_with_defined_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/complex/test_automapper_complex_with_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/complex/test_automapper_complex_with_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9818 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/complex/test_automapper_complex_with_skip_if_null.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.447862 sparkautomapper-2.0.7/tests/concat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/concat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/concat/test_automapper_add_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/concat/test_automapper_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/concat/test_automapper_concat_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/concat/test_automapper_concat_multiple_items_structs_different_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/concat/test_automapper_concat_multiple_items_structs_different_elements_with_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.447862 sparkautomapper-2.0.7/tests/copy_unmapped_properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/copy_unmapped_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/copy_unmapped_properties/test_automapper_copy_unmapped_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.447862 sparkautomapper-2.0.7/tests/cross_column_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/cross_column_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/cross_column_filter/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/cross_column_filter/test_cross_column_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.447862 sparkautomapper-2.0.7/tests/date/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/date/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/date/test_automapper_date_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/date/test_automapper_date_column_typed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/date/test_automapper_date_literal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.447862 sparkautomapper-2.0.7/tests/date_format/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/date_format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/date_format/test_automapper_date_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.447862 sparkautomapper-2.0.7/tests/decimal_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/decimal_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/decimal_type/test_automapper_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/decimal_type/test_automapper_decimal_typed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.447862 sparkautomapper-2.0.7/tests/duplicates_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/duplicates_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/duplicates_test/test_automapper_duplicates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.447862 sparkautomapper-2.0.7/tests/exists/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/exists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/exists/test_automapper_exists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.447862 sparkautomapper-2.0.7/tests/field/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/field/test_automapper_field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.451862 sparkautomapper-2.0.7/tests/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/filter/test_automapper_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.451862 sparkautomapper-2.0.7/tests/first/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/first/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/first/test_automapper_first.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.451862 sparkautomapper-2.0.7/tests/first_valid_column/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/first_valid_column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/first_valid_column/test_automapper_first_valid_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/first_valid_column/test_automapper_first_valid_column_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.451862 sparkautomapper-2.0.7/tests/flatten/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/flatten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/flatten/test_automapper_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/flatten/test_automapper_flatten_with_null.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.451862 sparkautomapper-2.0.7/tests/hash/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/hash/test_automapper_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.451862 sparkautomapper-2.0.7/tests/hash_abs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/hash_abs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/hash_abs/test_automapper_hash_abs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.451862 sparkautomapper-2.0.7/tests/if_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_/test_automapper_if_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_/test_automapper_if_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.451862 sparkautomapper-2.0.7/tests/if_column_exists/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_column_exists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_column_exists/test_automapper_if_column_exists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.451862 sparkautomapper-2.0.7/tests/if_not/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_not/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_not/test_automapper_if_not.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_not/test_automapper_if_not_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.451862 sparkautomapper-2.0.7/tests/if_not_null/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_not_null/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_not_null/test_automapper_if_not_null.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.455862 sparkautomapper-2.0.7/tests/if_not_null_or_empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_not_null_or_empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_not_null_or_empty/test_automapper_if_not_null_or_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.455862 sparkautomapper-2.0.7/tests/if_regex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_regex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/if_regex/test_automapper_if_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.455862 sparkautomapper-2.0.7/tests/join_using_delimiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/join_using_delimiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/join_using_delimiter/test_automapper_join_using_delimiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.455862 sparkautomapper-2.0.7/tests/left/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/left/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/left/test_automapper_left.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.455862 sparkautomapper-2.0.7/tests/list/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/list/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.455862 sparkautomapper-2.0.7/tests/list/addition/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/list/addition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements_with_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/list/test_automapper_list_multiple_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/list/test_automapper_list_multiple_items_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/list/test_automapper_list_multiple_items_structs_different_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/list/test_automapper_list_multiple_items_structs_different_elements_with_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/list/test_automapper_list_multiple_items_with_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/list/test_automapper_list_single_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/list/test_automapper_list_single_item_with_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.455862 sparkautomapper-2.0.7/tests/lower/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/lower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/lower/test_automapper_lower.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.455862 sparkautomapper-2.0.7/tests/lpad/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/lpad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/lpad/test_auto_mapper_lpad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.459862 sparkautomapper-2.0.7/tests/map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/map/test_automapper_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/map/test_automapper_map_col_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/map/test_automapper_map_no_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/map/test_automapper_map_null.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.459862 sparkautomapper-2.0.7/tests/multiple_columns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/multiple_columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/multiple_columns/test_automapper_multiple_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/multiple_columns/test_automapper_multiple_columns_simpler_syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.459862 sparkautomapper-2.0.7/tests/nested_array_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/nested_array_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/nested_array_filter/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/nested_array_filter/schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.459862 sparkautomapper-2.0.7/tests/nested_array_filter/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/nested_array_filter/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/nested_array_filter/simple/test_automapper_nested_array_filter_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.459862 sparkautomapper-2.0.7/tests/nested_array_filter/simple_with_array/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/nested_array_filter/simple_with_array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/nested_array_filter/simple_with_array/test_automapper_nested_array_filter_simple_with_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/nested_array_filter/test_automapper_nested_array_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/nested_array_filter/test_automapper_nested_array_filter_expression_only.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.459862 sparkautomapper-2.0.7/tests/null_if_empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/null_if_empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/null_if_empty/test_automapper_null_if_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.459862 sparkautomapper-2.0.7/tests/null_remover/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/null_remover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/null_remover/test_automapper_null_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.459862 sparkautomapper-2.0.7/tests/number/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/number/test_automapper_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/number/test_automapper_number_typed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.463862 sparkautomapper-2.0.7/tests/regex_extract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/regex_extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/regex_extract/test_auto_mapper_regex_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.463862 sparkautomapper-2.0.7/tests/regex_replace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/regex_replace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/regex_replace/test_auto_mapper_regex_replace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/regex_replace/test_auto_mapper_regex_replace_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.463862 sparkautomapper-2.0.7/tests/right/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/right/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/right/test_automapper_right.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.463862 sparkautomapper-2.0.7/tests/sanitize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/sanitize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/sanitize/test_auto_mapper_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.463862 sparkautomapper-2.0.7/tests/schema_pruning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/schema_pruning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/schema_pruning/test_automapper_schema_pruning_with_defined_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/schema_pruning/test_automapper_schema_pruning_with_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/schema_pruning/test_automapper_schema_pruning_with_extension_different_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.463862 sparkautomapper-2.0.7/tests/select_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/select_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/select_one/test_automapper_select_one.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.463862 sparkautomapper-2.0.7/tests/split_by_delimiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/split_by_delimiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/split_by_delimiter/test_automapper_split_by_delimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform_fluent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.463862 sparkautomapper-2.0.7/tests/string_after_delimiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/string_after_delimiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/string_after_delimiter/test_automapper_string_after_delimiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.463862 sparkautomapper-2.0.7/tests/string_before_delimiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/string_before_delimiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/string_before_delimiter/test_automapper_string_before_delimiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.467862 sparkautomapper-2.0.7/tests/struct_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/struct_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/struct_type/test_automapper_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/struct_type/test_automapper_struct_with_mappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.467862 sparkautomapper-2.0.7/tests/substring_by_delimiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/substring_by_delimiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/substring_by_delimiter/test_automapper_substring_by_delimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/test_automapper_full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/test_automapper_full_no_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/test_automapper_full_no_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/test_automapper_full_view_exists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.467862 sparkautomapper-2.0.7/tests/to_json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/to_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/to_json/test_automapper_to_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.467862 sparkautomapper-2.0.7/tests/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/transform/test_automapper_filter_and_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/transform/test_automapper_filter_and_transform_fluent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/transform/test_automapper_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.467862 sparkautomapper-2.0.7/tests/trim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/trim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/trim/test_auto_mapper_trim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.467862 sparkautomapper-2.0.7/tests/unix_timestamp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/unix_timestamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/unix_timestamp/test_automapper_unix_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/unix_timestamp/test_automapper_unix_timestamp_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/unix_timestamp/test_automapper_unix_timestamp_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:45:03.467862 sparkautomapper-2.0.7/tests/withColumn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/withColumn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/withColumn/test_automapper_with_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/withColumn/test_automapper_with_column_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/withColumn/test_automapper_with_column_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-26 10:44:06.000000 sparkautomapper-2.0.7/tests/withColumn/test_automapper_with_filter.py
```

### Comparing `sparkautomapper-2.0.6/LICENSE` & `sparkautomapper-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/PKG-INFO` & `sparkautomapper-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkautomapper
-Version: 2.0.6
+Version: 2.0.7
 Summary: AutoMapper for Spark
 Home-page: https://github.com/imranq2/SparkAutoMapper
 Author: Imran Qureshi
 Author-email: imranq2@hotmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sparkautomapper-2.0.6/README.md` & `sparkautomapper-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/setup.py` & `sparkautomapper-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/automappers/automapper.py` & `sparkautomapper-2.0.7/spark_auto_mapper/automappers/automapper.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/automappers/automapper_analysis_exception.py` & `sparkautomapper-2.0.7/spark_auto_mapper/automappers/automapper_analysis_exception.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/automappers/automapper_base.py` & `sparkautomapper-2.0.7/spark_auto_mapper/automappers/automapper_base.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/automappers/check_schema_result.py` & `sparkautomapper-2.0.7/spark_auto_mapper/automappers/check_schema_result.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/automappers/column_spec_wrapper.py` & `sparkautomapper-2.0.7/spark_auto_mapper/automappers/column_spec_wrapper.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/automappers/columns.py` & `sparkautomapper-2.0.7/spark_auto_mapper/automappers/columns.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/automappers/complex.py` & `sparkautomapper-2.0.7/spark_auto_mapper/automappers/complex.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/automappers/container.py` & `sparkautomapper-2.0.7/spark_auto_mapper/automappers/container.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/automappers/with_column.py` & `sparkautomapper-2.0.7/spark_auto_mapper/automappers/with_column.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/automappers/with_column_base.py` & `sparkautomapper-2.0.7/spark_auto_mapper/automappers/with_column_base.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/amount.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/amount.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/array.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/array.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/array_base.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/array_base.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/array_distinct.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/array_distinct.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/array_max.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/array_max.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/base64.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/base64.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/boolean.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/boolean.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/cast_to_type.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/cast_to_type.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/coalesce.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/coalesce.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/column.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/column.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/column_wrapper.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/column_wrapper.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/complex/complex.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/complex/complex.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/complex/complex_base.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/complex/complex_base.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/complex/struct_type.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/complex/struct_type.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/concat.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/concat.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/cross_column_filter.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/cross_column_filter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/data_type_base.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/data_type_base.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/date.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/date.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/date_format.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/date_format.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/datetime.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/datetime.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/decimal.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/decimal.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/exists.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/exists.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/expression.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/expression.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/field.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/field.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/filter.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/filter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/first.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/first.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/first_valid_column.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/first_valid_column.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/flatten.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/flatten.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/float.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/float.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/hash.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/hash.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/hash_abs.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/hash_abs.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/if_.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/if_.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/if_column_exists.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/if_column_exists.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/if_not.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/if_not.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/if_not_null.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/if_not_null.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/if_not_null_or_empty.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/if_not_null_or_empty.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/if_regex.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/if_regex.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/join_using_delimiter.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/join_using_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/list.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/list.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/literal.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/literal.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/lpad.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/lpad.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/map.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/map.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/nested_array_filter.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/nested_array_filter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/null_if_empty.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/null_if_empty.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/null_remover.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/null_remover.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/number.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/number.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/regex_extract.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/regex_extract.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/regex_replace.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/regex_replace.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/split_by_delimiter.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/split_by_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/substring.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/substring.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/substring_by_delimiter.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/substring_by_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/text_like_base.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/text_like_base.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/to_json.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/to_json.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/transform.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/transform.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/trim.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/trim.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/data_types/unix_timestamp.py` & `sparkautomapper-2.0.7/spark_auto_mapper/data_types/unix_timestamp.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/helpers/automapper_helpers.py` & `sparkautomapper-2.0.7/spark_auto_mapper/helpers/automapper_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # noinspection PyPackageRequirements
 from pyspark.sql import Column
 
 from spark_auto_mapper.data_types.array_distinct import AutoMapperArrayDistinctDataType
 from spark_auto_mapper.data_types.base64 import AutoMapperBase64DataType
 from spark_auto_mapper.data_types.exists import AutoMapperExistsDataType
 from spark_auto_mapper.data_types.hash_abs import AutoMapperHashAbsDataType
+from spark_auto_mapper.data_types.lower import AutoMapperLowerDataType
 from spark_auto_mapper.data_types.nested_array_filter import (
     AutoMapperNestedArrayFilterDataType,
 )
 from spark_auto_mapper.data_types.cross_column_filter import (
     AutoMapperCrossColumnFilterDataType,
 )
 from spark_auto_mapper.data_types.array_max import AutoMapperArrayMaxDataType
@@ -356,14 +357,24 @@
         :param column: column whose contents to use
         :param length: number of characters to take from left
         :return: a concat automapper type
         """
         return AutoMapperSubstringDataType(column=column, start=0, length=length)
 
     @staticmethod
+    def lower(column: AutoMapperColumnOrColumnLikeType) -> AutoMapperLowerDataType:
+        """
+        Converts a string column to lower case.
+
+        :param column: column whose contents to use
+        :return: a lower automapper type
+        """
+        return AutoMapperLowerDataType(column=column)
+
+    @staticmethod
     def right(
         column: AutoMapperColumnOrColumnLikeType, length: int
     ) -> AutoMapperSubstringDataType:
         """
         Take the specified number of last characters in a string
 
         :param column: column whose contents to use
```

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/helpers/capture_arguments.py` & `sparkautomapper-2.0.7/spark_auto_mapper/helpers/capture_arguments.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/helpers/expression_comparer.py` & `sparkautomapper-2.0.7/spark_auto_mapper/helpers/expression_comparer.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/helpers/python_keyword_cleaner.py` & `sparkautomapper-2.0.7/spark_auto_mapper/helpers/python_keyword_cleaner.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/helpers/value_parser.py` & `sparkautomapper-2.0.7/spark_auto_mapper/helpers/value_parser.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/type_definitions/defined_types.py` & `sparkautomapper-2.0.7/spark_auto_mapper/type_definitions/defined_types.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/type_definitions/native_types.py` & `sparkautomapper-2.0.7/spark_auto_mapper/type_definitions/native_types.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/spark_auto_mapper/type_definitions/wrapper_types.py` & `sparkautomapper-2.0.7/spark_auto_mapper/type_definitions/wrapper_types.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/sparkautomapper.egg-info/PKG-INFO` & `sparkautomapper-2.0.7/sparkautomapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkautomapper
-Version: 2.0.6
+Version: 2.0.7
 Summary: AutoMapper for Spark
 Home-page: https://github.com/imranq2/SparkAutoMapper
 Author: Imran Qureshi
 Author-email: imranq2@hotmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sparkautomapper-2.0.6/sparkautomapper.egg-info/SOURCES.txt` & `sparkautomapper-2.0.7/sparkautomapper.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 spark_auto_mapper/data_types/if_not.py
 spark_auto_mapper/data_types/if_not_null.py
 spark_auto_mapper/data_types/if_not_null_or_empty.py
 spark_auto_mapper/data_types/if_regex.py
 spark_auto_mapper/data_types/join_using_delimiter.py
 spark_auto_mapper/data_types/list.py
 spark_auto_mapper/data_types/literal.py
+spark_auto_mapper/data_types/lower.py
 spark_auto_mapper/data_types/lpad.py
 spark_auto_mapper/data_types/map.py
 spark_auto_mapper/data_types/nested_array_filter.py
 spark_auto_mapper/data_types/null_if_empty.py
 spark_auto_mapper/data_types/null_remover.py
 spark_auto_mapper/data_types/number.py
 spark_auto_mapper/data_types/regex_extract.py
@@ -196,14 +197,16 @@
 tests/list/test_automapper_list_multiple_items_structs_different_elements_with_schema.py
 tests/list/test_automapper_list_multiple_items_with_null.py
 tests/list/test_automapper_list_single_item.py
 tests/list/test_automapper_list_single_item_with_mapper.py
 tests/list/addition/__init__.py
 tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements.py
 tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements_with_schema.py
+tests/lower/__init__.py
+tests/lower/test_automapper_lower.py
 tests/lpad/__init__.py
 tests/lpad/test_auto_mapper_lpad.py
 tests/map/__init__.py
 tests/map/test_automapper_map.py
 tests/map/test_automapper_map_col_default.py
 tests/map/test_automapper_map_no_default.py
 tests/map/test_automapper_map_null.py
```

### Comparing `sparkautomapper-2.0.6/tests/amount/test_automapper_amount.py` & `sparkautomapper-2.0.7/tests/amount/test_automapper_amount.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/amount/test_automapper_amount_typed.py` & `sparkautomapper-2.0.7/tests/amount/test_automapper_amount_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/array/test_automapper_array_typed.py` & `sparkautomapper-2.0.7/tests/array/test_automapper_array_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/array_distinct/test_automapper_array_distinct.py` & `sparkautomapper-2.0.7/tests/array_distinct/test_automapper_array_distinct.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/array_max/test_automapper_array_max.py` & `sparkautomapper-2.0.7/tests/array_max/test_automapper_array_max.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/base64/test_automapper_base64.py` & `sparkautomapper-2.0.7/tests/base64/test_automapper_base64.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/boolean/test_automapper_boolean.py` & `sparkautomapper-2.0.7/tests/boolean/test_automapper_boolean.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/boolean/test_automapper_boolean_typed.py` & `sparkautomapper-2.0.7/tests/boolean/test_automapper_boolean_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/cast/test_cast.py` & `sparkautomapper-2.0.7/tests/cast/test_cast.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/cast_to_type/test_automapper_cast_to_type_typed.py` & `sparkautomapper-2.0.7/tests/cast_to_type/test_automapper_cast_to_type_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/checkpointing/test_automapper_full_checkpointing.py` & `sparkautomapper-2.0.7/tests/checkpointing/test_automapper_full_checkpointing.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/coalesce/test_automapper_coalesce.py` & `sparkautomapper-2.0.7/tests/coalesce/test_automapper_coalesce.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/columns/test_automapper_columns.py` & `sparkautomapper-2.0.7/tests/columns/test_automapper_columns.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/complex/test_automapper_complex.py` & `sparkautomapper-2.0.7/tests/complex/test_automapper_complex.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/complex/test_automapper_complex_with_defined_class.py` & `sparkautomapper-2.0.7/tests/complex/test_automapper_complex_with_defined_class.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/complex/test_automapper_complex_with_extension.py` & `sparkautomapper-2.0.7/tests/complex/test_automapper_complex_with_extension.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/complex/test_automapper_complex_with_mappers.py` & `sparkautomapper-2.0.7/tests/complex/test_automapper_complex_with_mappers.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/complex/test_automapper_complex_with_skip_if_null.py` & `sparkautomapper-2.0.7/tests/complex/test_automapper_complex_with_skip_if_null.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/concat/test_automapper_add_array.py` & `sparkautomapper-2.0.7/tests/concat/test_automapper_add_array.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/concat/test_automapper_concat.py` & `sparkautomapper-2.0.7/tests/concat/test_automapper_concat.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/concat/test_automapper_concat_array.py` & `sparkautomapper-2.0.7/tests/concat/test_automapper_concat_array.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/concat/test_automapper_concat_multiple_items_structs_different_elements.py` & `sparkautomapper-2.0.7/tests/concat/test_automapper_concat_multiple_items_structs_different_elements.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/concat/test_automapper_concat_multiple_items_structs_different_elements_with_schema.py` & `sparkautomapper-2.0.7/tests/concat/test_automapper_concat_multiple_items_structs_different_elements_with_schema.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/conftest.py` & `sparkautomapper-2.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/copy_unmapped_properties/test_automapper_copy_unmapped_properties.py` & `sparkautomapper-2.0.7/tests/copy_unmapped_properties/test_automapper_copy_unmapped_properties.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/cross_column_filter/location.py` & `sparkautomapper-2.0.7/tests/cross_column_filter/location.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/cross_column_filter/test_cross_column_filter.py` & `sparkautomapper-2.0.7/tests/cross_column_filter/test_cross_column_filter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/date/test_automapper_date_column.py` & `sparkautomapper-2.0.7/tests/date/test_automapper_date_column.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/date/test_automapper_date_column_typed.py` & `sparkautomapper-2.0.7/tests/date/test_automapper_date_column_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/date/test_automapper_date_literal.py` & `sparkautomapper-2.0.7/tests/date/test_automapper_date_literal.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/date_format/test_automapper_date_format.py` & `sparkautomapper-2.0.7/tests/date_format/test_automapper_date_format.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/decimal_type/test_automapper_decimal.py` & `sparkautomapper-2.0.7/tests/decimal_type/test_automapper_decimal.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/decimal_type/test_automapper_decimal_typed.py` & `sparkautomapper-2.0.7/tests/decimal_type/test_automapper_decimal_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/duplicates_test/test_automapper_duplicates.py` & `sparkautomapper-2.0.7/tests/duplicates_test/test_automapper_duplicates.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/exists/test_automapper_exists.py` & `sparkautomapper-2.0.7/tests/exists/test_automapper_exists.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/field/test_automapper_field.py` & `sparkautomapper-2.0.7/tests/field/test_automapper_field.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/filter/test_automapper_filter.py` & `sparkautomapper-2.0.7/tests/filter/test_automapper_filter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/first/test_automapper_first.py` & `sparkautomapper-2.0.7/tests/first/test_automapper_first.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/first_valid_column/test_automapper_first_valid_column.py` & `sparkautomapper-2.0.7/tests/first_valid_column/test_automapper_first_valid_column.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/first_valid_column/test_automapper_first_valid_column_expressions.py` & `sparkautomapper-2.0.7/tests/first_valid_column/test_automapper_first_valid_column_expressions.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/flatten/test_automapper_flatten.py` & `sparkautomapper-2.0.7/tests/flatten/test_automapper_flatten.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/flatten/test_automapper_flatten_with_null.py` & `sparkautomapper-2.0.7/tests/flatten/test_automapper_flatten_with_null.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/hash/test_automapper_hash.py` & `sparkautomapper-2.0.7/tests/hash/test_automapper_hash.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/hash_abs/test_automapper_hash_abs.py` & `sparkautomapper-2.0.7/tests/hash_abs/test_automapper_hash_abs.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/if_/test_automapper_if_.py` & `sparkautomapper-2.0.7/tests/if_/test_automapper_if_.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/if_/test_automapper_if_list.py` & `sparkautomapper-2.0.7/tests/if_/test_automapper_if_list.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/if_column_exists/test_automapper_if_column_exists.py` & `sparkautomapper-2.0.7/tests/if_column_exists/test_automapper_if_column_exists.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/if_not/test_automapper_if_not.py` & `sparkautomapper-2.0.7/tests/if_not/test_automapper_if_not.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/if_not/test_automapper_if_not_list.py` & `sparkautomapper-2.0.7/tests/if_not/test_automapper_if_not_list.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/if_not_null/test_automapper_if_not_null.py` & `sparkautomapper-2.0.7/tests/if_not_null/test_automapper_if_not_null.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/if_not_null_or_empty/test_automapper_if_not_null_or_empty.py` & `sparkautomapper-2.0.7/tests/if_not_null_or_empty/test_automapper_if_not_null_or_empty.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/if_regex/test_automapper_if_regex.py` & `sparkautomapper-2.0.7/tests/if_regex/test_automapper_if_regex.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/join_using_delimiter/test_automapper_join_using_delimiter.py` & `sparkautomapper-2.0.7/tests/join_using_delimiter/test_automapper_join_using_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/left/test_automapper_left.py` & `sparkautomapper-2.0.7/tests/left/test_automapper_left.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements.py` & `sparkautomapper-2.0.7/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements_with_schema.py` & `sparkautomapper-2.0.7/tests/list/addition/test_automapper_list_addition_multiple_items_structs_different_elements_with_schema.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/list/test_automapper_list_multiple_items.py` & `sparkautomapper-2.0.7/tests/list/test_automapper_list_multiple_items.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/list/test_automapper_list_multiple_items_structs.py` & `sparkautomapper-2.0.7/tests/list/test_automapper_list_multiple_items_structs.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/list/test_automapper_list_multiple_items_structs_different_elements.py` & `sparkautomapper-2.0.7/tests/list/test_automapper_list_multiple_items_structs_different_elements.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/list/test_automapper_list_multiple_items_structs_different_elements_with_schema.py` & `sparkautomapper-2.0.7/tests/list/test_automapper_list_multiple_items_structs_different_elements_with_schema.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/list/test_automapper_list_multiple_items_with_null.py` & `sparkautomapper-2.0.7/tests/list/test_automapper_list_multiple_items_with_null.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/list/test_automapper_list_single_item.py` & `sparkautomapper-2.0.7/tests/list/test_automapper_list_single_item.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/list/test_automapper_list_single_item_with_mapper.py` & `sparkautomapper-2.0.7/tests/list/test_automapper_list_single_item_with_mapper.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/lpad/test_auto_mapper_lpad.py` & `sparkautomapper-2.0.7/tests/lpad/test_auto_mapper_lpad.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/map/test_automapper_map.py` & `sparkautomapper-2.0.7/tests/map/test_automapper_map.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/map/test_automapper_map_col_default.py` & `sparkautomapper-2.0.7/tests/map/test_automapper_map_col_default.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/map/test_automapper_map_no_default.py` & `sparkautomapper-2.0.7/tests/map/test_automapper_map_no_default.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/map/test_automapper_map_null.py` & `sparkautomapper-2.0.7/tests/map/test_automapper_map_null.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/multiple_columns/test_automapper_multiple_columns.py` & `sparkautomapper-2.0.7/tests/multiple_columns/test_automapper_multiple_columns.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/multiple_columns/test_automapper_multiple_columns_simpler_syntax.py` & `sparkautomapper-2.0.7/tests/multiple_columns/test_automapper_multiple_columns_simpler_syntax.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/nested_array_filter/location.py` & `sparkautomapper-2.0.7/tests/nested_array_filter/location.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/nested_array_filter/schedule.py` & `sparkautomapper-2.0.7/tests/nested_array_filter/schedule.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/nested_array_filter/simple/test_automapper_nested_array_filter_simple.py` & `sparkautomapper-2.0.7/tests/nested_array_filter/simple/test_automapper_nested_array_filter_simple.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/nested_array_filter/simple_with_array/test_automapper_nested_array_filter_simple_with_array.py` & `sparkautomapper-2.0.7/tests/nested_array_filter/simple_with_array/test_automapper_nested_array_filter_simple_with_array.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/nested_array_filter/test_automapper_nested_array_filter.py` & `sparkautomapper-2.0.7/tests/nested_array_filter/test_automapper_nested_array_filter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/nested_array_filter/test_automapper_nested_array_filter_expression_only.py` & `sparkautomapper-2.0.7/tests/nested_array_filter/test_automapper_nested_array_filter_expression_only.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/null_if_empty/test_automapper_null_if_empty.py` & `sparkautomapper-2.0.7/tests/null_if_empty/test_automapper_null_if_empty.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/null_remover/test_automapper_null_remover.py` & `sparkautomapper-2.0.7/tests/null_remover/test_automapper_null_remover.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/number/test_automapper_number.py` & `sparkautomapper-2.0.7/tests/number/test_automapper_number.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/number/test_automapper_number_typed.py` & `sparkautomapper-2.0.7/tests/number/test_automapper_number_typed.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/regex_extract/test_auto_mapper_regex_extract.py` & `sparkautomapper-2.0.7/tests/regex_extract/test_auto_mapper_regex_extract.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/regex_replace/test_auto_mapper_regex_replace.py` & `sparkautomapper-2.0.7/tests/regex_replace/test_auto_mapper_regex_replace.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/regex_replace/test_auto_mapper_regex_replace_unicode.py` & `sparkautomapper-2.0.7/tests/regex_replace/test_auto_mapper_regex_replace_unicode.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/right/test_automapper_right.py` & `sparkautomapper-2.0.7/tests/right/test_automapper_right.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/sanitize/test_auto_mapper_sanitize.py` & `sparkautomapper-2.0.7/tests/sanitize/test_auto_mapper_sanitize.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/schema_pruning/test_automapper_schema_pruning_with_defined_class.py` & `sparkautomapper-2.0.7/tests/schema_pruning/test_automapper_schema_pruning_with_defined_class.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/schema_pruning/test_automapper_schema_pruning_with_extension.py` & `sparkautomapper-2.0.7/tests/schema_pruning/test_automapper_schema_pruning_with_extension.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/schema_pruning/test_automapper_schema_pruning_with_extension_different_properties.py` & `sparkautomapper-2.0.7/tests/schema_pruning/test_automapper_schema_pruning_with_extension_different_properties.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/select_one/test_automapper_select_one.py` & `sparkautomapper-2.0.7/tests/select_one/test_automapper_select_one.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/split_by_delimiter/test_automapper_split_by_delimiter.py` & `sparkautomapper-2.0.7/tests/split_by_delimiter/test_automapper_split_by_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform.py` & `sparkautomapper-2.0.7/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform_fluent.py` & `sparkautomapper-2.0.7/tests/split_by_delimiter/test_automapper_split_by_delimiter_and_transform_fluent.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/string_after_delimiter/test_automapper_string_after_delimiter.py` & `sparkautomapper-2.0.7/tests/string_after_delimiter/test_automapper_string_after_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/string_before_delimiter/test_automapper_string_before_delimiter.py` & `sparkautomapper-2.0.7/tests/string_before_delimiter/test_automapper_string_before_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/struct_type/test_automapper_struct.py` & `sparkautomapper-2.0.7/tests/struct_type/test_automapper_struct.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/struct_type/test_automapper_struct_with_mappers.py` & `sparkautomapper-2.0.7/tests/struct_type/test_automapper_struct_with_mappers.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/substring_by_delimiter/test_automapper_substring_by_delimiter.py` & `sparkautomapper-2.0.7/tests/substring_by_delimiter/test_automapper_substring_by_delimiter.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/test_automapper_full.py` & `sparkautomapper-2.0.7/tests/test_automapper_full.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/test_automapper_full_no_keys.py` & `sparkautomapper-2.0.7/tests/test_automapper_full_no_keys.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/test_automapper_full_no_views.py` & `sparkautomapper-2.0.7/tests/test_automapper_full_no_views.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/test_automapper_full_view_exists.py` & `sparkautomapper-2.0.7/tests/test_automapper_full_view_exists.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/to_json/test_automapper_to_json.py` & `sparkautomapper-2.0.7/tests/to_json/test_automapper_to_json.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/transform/test_automapper_filter_and_transform.py` & `sparkautomapper-2.0.7/tests/transform/test_automapper_filter_and_transform.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/transform/test_automapper_filter_and_transform_fluent.py` & `sparkautomapper-2.0.7/tests/transform/test_automapper_filter_and_transform_fluent.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/transform/test_automapper_transform.py` & `sparkautomapper-2.0.7/tests/transform/test_automapper_transform.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/trim/test_auto_mapper_trim.py` & `sparkautomapper-2.0.7/tests/trim/test_auto_mapper_trim.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/unix_timestamp/test_automapper_unix_timestamp.py` & `sparkautomapper-2.0.7/tests/unix_timestamp/test_automapper_unix_timestamp.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/unix_timestamp/test_automapper_unix_timestamp_literal.py` & `sparkautomapper-2.0.7/tests/unix_timestamp/test_automapper_unix_timestamp_literal.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/unix_timestamp/test_automapper_unix_timestamp_string.py` & `sparkautomapper-2.0.7/tests/unix_timestamp/test_automapper_unix_timestamp_string.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/withColumn/test_automapper_with_column.py` & `sparkautomapper-2.0.7/tests/withColumn/test_automapper_with_column.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/withColumn/test_automapper_with_column_expression.py` & `sparkautomapper-2.0.7/tests/withColumn/test_automapper_with_column_expression.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/withColumn/test_automapper_with_column_literal.py` & `sparkautomapper-2.0.7/tests/withColumn/test_automapper_with_column_literal.py`

 * *Files identical despite different names*

### Comparing `sparkautomapper-2.0.6/tests/withColumn/test_automapper_with_filter.py` & `sparkautomapper-2.0.7/tests/withColumn/test_automapper_with_filter.py`

 * *Files identical despite different names*

