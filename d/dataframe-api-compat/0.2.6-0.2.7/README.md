# Comparing `tmp/dataframe_api_compat-0.2.6.tar.gz` & `tmp/dataframe_api_compat-0.2.7.tar.gz`

## Comparing `dataframe_api_compat-0.2.6.tar` & `dataframe_api_compat-0.2.7.tar`

### file list

```diff
@@ -1,155 +1,165 @@
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/contributing.md
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/mkdocs.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/mypy.ini
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/requirements-dev.txt
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/.github/workflows/earliest_versions.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/.github/workflows/pre-commit.yml
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/.github/workflows/random_version.yml
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/.github/workflows/tox.yml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/py.typed
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/utils.py
--rw-r--r--   0        0        0    15203 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/pandas_standard/__init__.py
--rw-r--r--   0        0        0    17583 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/pandas_standard/column_object.py
--rw-r--r--   0        0        0    18045 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/pandas_standard/dataframe_object.py
--rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/pandas_standard/group_by_object.py
--rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/pandas_standard/scalar_object.py
--rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/polars_standard/__init__.py
--rw-r--r--   0        0        0    16052 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/polars_standard/column_object.py
--rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/polars_standard/dataframe_object.py
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/polars_standard/group_by_object.py
--rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/dataframe_api_compat/polars_standard/scalar_object.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/generate_members.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/index.md
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/installation.md
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/pandas-column.md
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/pandas-dataframe.md
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/pandas-namespace.md
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/pandas-scalar.md
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/polars-column.md
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/polars-dataframe.md
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/polars-namespace.md
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/polars-scalar.md
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/quick_start.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/reference.md
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/requirements-docs.txt
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/basics/column.md
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/basics/complete_example.md
--rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/basics/dataframe.md
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/basics/persist.md
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/docs/basics/scalar.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/__init__.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/conftest.py
--rw-r--r--   0        0        0    22088 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/__init__.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/and_or_test.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/any_all_test.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/cast_test.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/col_sorted_indices_test.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/col_to_array_object_test.py
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/comparisons_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/conftest.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/cross_df_comparisons_test.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/cumulative_test.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/divmod_test.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/fill_nan_test.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/fill_null_test.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/get_rows_by_mask_test.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/get_rows_test.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/get_value_test.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/invalid_pandas_test.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/invert_test.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/is_in_test.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/is_nan_test.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/is_null_test.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/len_test.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/n_unique_test.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/name_test.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/parent_dataframe_test.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/pow_test.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/reductions_test.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/rename_test.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/schema_test.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/shift_test.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/slice_rows_test.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/sort_test.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/statistics_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/temporal/__init__.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/temporal/components_test.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/temporal/filter_test.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/column/temporal/floor_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/all_rowwise_test.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/and_test.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/any_all_test.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/any_rowwise_test.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/assign_test.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/cast_test.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/columns_iter_test.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/comparisons_test.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/cross_df_comparison_test.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/divmod_test.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/drop_column_test.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/drop_nulls_test.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/fill_nan_test.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/fill_null_test.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/get_column_by_name_test.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/get_column_names_test.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/get_rows_by_mask_test.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/get_rows_test.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/invert_test.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/is_nan_test.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/is_null_test.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/join_test.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/or_test.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/pow_test.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/reductions_test.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/rename_columns_test.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/schema_test.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/select_test.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/shape_test.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/slice_rows_test.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/sort_test.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/to_array_object_test.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/update_columns_test.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/dataframe/update_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/groupby/__init__.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/groupby/aggregate_test.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/groupby/groupby_any_all_test.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/groupby/invalid_test.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/groupby/numeric_test.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/groupby/size_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/integration/__init__.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/integration/free_vs_w_parent_test.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/integration/persistedness_test.py
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/integration/scale_column_test.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/integration/upstream_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/namespace/__init__.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/namespace/column_from_1d_array_test.py
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/namespace/column_from_sequence_test.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/namespace/concat_test.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/namespace/convert_to_standard_column_test.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/namespace/dataframe_from_2d_array_test.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/namespace/is_dtype_test.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/namespace/namespace_is_null_test.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/namespace/sorted_indices_test.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/namespace/to_array_object_test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/scalars/__init__.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/tests/scalars/float_test.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/typings/pandas/__init__.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/utils/__init__.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/utils/bump_version.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/utils/generate_random_versions.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/utils/make.sh
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/utils/pandas_versions.txt
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/utils/polars_versions.txt
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/utils/update-pandas.sh
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/utils/upgrade-dataframe-api.sh
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/LICENSE
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/README.md
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/contributing.md
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/mkdocs.yml
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/mypy.ini
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/requirements-dev-modin.txt
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/requirements-dev.txt
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/.github/workflows/earliest_versions.yml
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/.github/workflows/pre-commit.yml
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/.github/workflows/random_version.yml
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/.github/workflows/tox.yml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/py.typed
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/utils.py
+-rw-r--r--   0        0        0    15706 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/modin_standard/__init__.py
+-rw-r--r--   0        0        0    18267 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/modin_standard/column_object.py
+-rw-r--r--   0        0        0    18241 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/modin_standard/dataframe_object.py
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/modin_standard/group_by_object.py
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/modin_standard/scalar_object.py
+-rw-r--r--   0        0        0    15391 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/pandas_standard/__init__.py
+-rw-r--r--   0        0        0    17635 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/pandas_standard/column_object.py
+-rw-r--r--   0        0        0    18045 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/pandas_standard/dataframe_object.py
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/pandas_standard/group_by_object.py
+-rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/pandas_standard/scalar_object.py
+-rw-r--r--   0        0        0    13331 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/polars_standard/__init__.py
+-rw-r--r--   0        0        0    16052 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/polars_standard/column_object.py
+-rw-r--r--   0        0        0    19131 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/polars_standard/dataframe_object.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/polars_standard/group_by_object.py
+-rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/dataframe_api_compat/polars_standard/scalar_object.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/generate_members.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/index.md
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/installation.md
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/modin-column.md
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/modin-dataframe.md
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/modin-namespace.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/modin-scalar.md
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/pandas-column.md
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/pandas-dataframe.md
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/pandas-namespace.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/pandas-scalar.md
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/polars-column.md
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/polars-dataframe.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/polars-namespace.md
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/polars-scalar.md
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/quick_start.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/reference.md
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/requirements-docs.txt
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/basics/column.md
+-rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/basics/complete_example.md
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/basics/dataframe.md
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/basics/persist.md
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/docs/basics/scalar.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/__init__.py
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/conftest.py
+-rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/__init__.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/and_or_test.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/any_all_test.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/cast_test.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/col_sorted_indices_test.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/col_to_array_object_test.py
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/comparisons_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/conftest.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/cross_df_comparisons_test.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/cumulative_test.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/divmod_test.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/fill_nan_test.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/fill_null_test.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/get_rows_by_mask_test.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/get_rows_test.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/get_value_test.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/invert_test.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/is_in_test.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/is_nan_test.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/is_null_test.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/len_test.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/n_unique_test.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/name_test.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/non_unique_column_names_test.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/parent_dataframe_test.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/pow_test.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/reductions_test.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/rename_test.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/schema_test.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/shift_test.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/slice_rows_test.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/sort_test.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/statistics_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/temporal/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/temporal/components_test.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/temporal/filter_test.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/column/temporal/floor_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/__init__.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/all_rowwise_test.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/and_test.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/any_all_test.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/any_rowwise_test.py
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/assign_test.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/cast_test.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/columns_iter_test.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/comparisons_test.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/cross_df_comparison_test.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/divmod_test.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/drop_column_test.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/drop_nulls_test.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/fill_nan_test.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/fill_null_test.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/get_column_by_name_test.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/get_column_names_test.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/get_rows_by_mask_test.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/get_rows_test.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/invert_test.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/is_nan_test.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/is_null_test.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/join_test.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/or_test.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/pow_test.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/reductions_test.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/rename_columns_test.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/schema_test.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/select_test.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/shape_test.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/slice_rows_test.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/sort_test.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/to_array_object_test.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/update_columns_test.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/dataframe/update_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/groupby/__init__.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/groupby/aggregate_test.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/groupby/groupby_any_all_test.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/groupby/invalid_test.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/groupby/numeric_test.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/groupby/size_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/integration/__init__.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/integration/free_vs_w_parent_test.py
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/integration/persistedness_test.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/integration/scale_column_test.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/integration/upstream_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/namespace/__init__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/namespace/column_from_1d_array_test.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/namespace/column_from_sequence_test.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/namespace/concat_test.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/namespace/convert_to_standard_column_test.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/namespace/dataframe_from_2d_array_test.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/namespace/is_dtype_test.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/namespace/namespace_is_null_test.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/namespace/sorted_indices_test.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/namespace/to_array_object_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/scalars/__init__.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/tests/scalars/float_test.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/typings/pandas/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/utils/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/utils/bump_version.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/utils/generate_random_versions.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/utils/make.sh
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/utils/pandas_versions.txt
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/utils/polars_versions.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/utils/update-pandas.sh
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/utils/upgrade-dataframe-api.sh
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/LICENSE
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/README.md
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 dataframe_api_compat-0.2.7/PKG-INFO
```

### Comparing `dataframe_api_compat-0.2.6/.pre-commit-config.yaml` & `dataframe_api_compat-0.2.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/mkdocs.yml` & `dataframe_api_compat-0.2.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/.github/workflows/earliest_versions.yml` & `dataframe_api_compat-0.2.7/.github/workflows/earliest_versions.yml`

 * *Files 9% similar despite different names*

```diff
@@ -27,8 +27,8 @@
             ~\AppData\Local\pip\Cache
           key: ${{ runner.os }}-build-${{ matrix.python-version }}
       - name: install-earliest-versions
         run: python -m pip install pandas==1.2.0 polars==0.17.0
       - name: install-reqs
         run: python -m pip install --upgrade tox virtualenv setuptools pip && python -m pip install -r requirements-dev.txt
       - name: Run pytest
-        run: pytest tests --cov=dataframe_api_compat --cov=tests --cov-fail-under=80
+        run: pytest tests --cov=dataframe_api_compat/pandas_standard --cov=dataframe_api_compat/polars_standard --cov=tests --cov-fail-under=80
```

### Comparing `dataframe_api_compat-0.2.6/.github/workflows/mkdocs.yml` & `dataframe_api_compat-0.2.7/.github/workflows/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,15 @@
         run: |
           git config user.name github-actions[bot]
           git config user.email 41898282+github-actions[bot]@users.noreply.github.com
       - uses: actions/setup-python@v4
         with:
           python-version: 3.x
       - run: echo "cache_id=$(date --utc '+%V')" >> $GITHUB_ENV
-
-
       - uses: actions/cache@v3
         with:
           key: mkdocs-material-${{ env.cache_id }}
           path: .cache
           restore-keys: |
             mkdocs-material-
-      - run: pip install -r docs/requirements-docs.txt -e . pandas polars
-
+      - run: pip install -r docs/requirements-docs.txt -e . pandas "polars<0.20.8"
       - run: mkdocs gh-deploy --force
```

### Comparing `dataframe_api_compat-0.2.6/.github/workflows/publish-to-pypi.yml` & `dataframe_api_compat-0.2.7/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/.github/workflows/random_version.yml` & `dataframe_api_compat-0.2.7/.github/workflows/random_version.yml`

 * *Files 22% similar despite different names*

```diff
@@ -31,8 +31,8 @@
       - name: generate-random-versions
         run: python utils/generate_random_versions.py
       - name: install-random-verions
         run: python -m pip install -r random-requirements.txt
       - name: install-reqs
         run: python -m pip install --upgrade tox virtualenv setuptools pip && python -m pip install -r requirements-dev.txt
       - name: Run pytest
-        run: pytest tests --cov=dataframe_api_compat --cov=tests --cov-fail-under=80
+        run: pytest tests --cov=dataframe_api_compat/pandas_standard --cov=dataframe_api_compat/polars_standard --cov=tests --cov-fail-under=80
```

### Comparing `dataframe_api_compat-0.2.6/dataframe_api_compat/utils.py` & `dataframe_api_compat-0.2.7/dataframe_api_compat/utils.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/dataframe_api_compat/pandas_standard/__init__.py` & `dataframe_api_compat-0.2.7/dataframe_api_compat/pandas_standard/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,20 +100,24 @@
         return Namespace.Float64()
     if dtype == "Float64":
         return Namespace.Float64()
     if dtype == "float32":
         return Namespace.Float32()
     if dtype == "Float32":
         return Namespace.Float32()
-    if dtype == "bool":
+    if dtype in ("bool", "boolean"):
+        # Also for `pandas.core.arrays.boolean.BooleanDtype`
         return Namespace.Bool()
     if dtype == "object":
         return Namespace.String()
     if dtype == "string":
         return Namespace.String()
+    if hasattr(dtype, "name"):
+        # For types like `numpy.dtypes.DateTime64DType`
+        dtype = dtype.name
     if dtype.startswith("datetime64["):
         match = re.search(r"datetime64\[(\w{1,2})", dtype)
         assert match is not None
         time_unit = cast(Literal["ms", "us"], match.group(1))
         return Namespace.Datetime(time_unit)
     if dtype.startswith("timedelta64["):
         match = re.search(r"timedelta64\[(\w{1,2})", dtype)
```

### Comparing `dataframe_api_compat-0.2.6/dataframe_api_compat/pandas_standard/column_object.py` & `dataframe_api_compat-0.2.7/dataframe_api_compat/pandas_standard/column_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     "Int16": "int16",
     "Int8": "int8",
     "UInt64": "uint64",
     "UInt32": "uint32",
     "UInt16": "uint16",
     "UInt8": "uint8",
     "boolean": "bool",
+    "Float64": "float64",
+    "Float32": "float32",
 }
 
 
 class Column(ColumnT):
     def __init__(
         self,
         series: pd.Series[Any],
```

### Comparing `dataframe_api_compat-0.2.6/dataframe_api_compat/pandas_standard/dataframe_object.py` & `dataframe_api_compat-0.2.7/dataframe_api_compat/pandas_standard/dataframe_object.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/dataframe_api_compat/pandas_standard/group_by_object.py` & `dataframe_api_compat-0.2.7/dataframe_api_compat/pandas_standard/group_by_object.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/dataframe_api_compat/pandas_standard/scalar_object.py` & `dataframe_api_compat-0.2.7/dataframe_api_compat/pandas_standard/scalar_object.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/dataframe_api_compat/polars_standard/__init__.py` & `dataframe_api_compat-0.2.7/dataframe_api_compat/polars_standard/__init__.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/dataframe_api_compat/polars_standard/column_object.py` & `dataframe_api_compat-0.2.7/dataframe_api_compat/polars_standard/column_object.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/dataframe_api_compat/polars_standard/dataframe_object.py` & `dataframe_api_compat-0.2.7/dataframe_api_compat/polars_standard/dataframe_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,43 +233,43 @@
     # Binary operations
 
     def __eq__(  # type: ignore[override]
         self,
         other: AnyScalar,
     ) -> DataFrame:
         return self._from_dataframe(
-            self.dataframe.with_columns(pl.col("*").__eq__(other)),
+            self.dataframe.with_columns(pl.col("*").__eq__(other)),  # type: ignore[operator]
         )
 
     def __ne__(  # type: ignore[override]
         self,
         other: AnyScalar,
     ) -> DataFrame:
         return self._from_dataframe(
-            self.dataframe.with_columns(pl.col("*").__ne__(other)),
+            self.dataframe.with_columns(pl.col("*").__ne__(other)),  # type: ignore[operator]
         )
 
     def __ge__(self, other: AnyScalar) -> DataFrame:
         return self._from_dataframe(
-            self.dataframe.with_columns(pl.col("*").__ge__(other)),
+            self.dataframe.with_columns(pl.col("*").__ge__(other)),  # type: ignore[operator]
         )
 
     def __gt__(self, other: AnyScalar) -> DataFrame:
         return self._from_dataframe(
-            self.dataframe.with_columns(pl.col("*").__gt__(other)),
+            self.dataframe.with_columns(pl.col("*").__gt__(other)),  # type: ignore[operator]
         )
 
     def __le__(self, other: AnyScalar) -> DataFrame:
         return self._from_dataframe(
-            self.dataframe.with_columns(pl.col("*").__le__(other)),
+            self.dataframe.with_columns(pl.col("*").__le__(other)),  # type: ignore[operator]
         )
 
     def __lt__(self, other: AnyScalar) -> DataFrame:
         return self._from_dataframe(
-            self.dataframe.with_columns(pl.col("*").__lt__(other)),
+            self.dataframe.with_columns(pl.col("*").__lt__(other)),  # type: ignore[operator]
         )
 
     def __and__(self, other: AnyScalar) -> DataFrame:
         _other = validate_comparand(self, other)
         return self._from_dataframe(
             self.dataframe.with_columns(pl.col("*") & _other),
         )
```

### Comparing `dataframe_api_compat-0.2.6/dataframe_api_compat/polars_standard/group_by_object.py` & `dataframe_api_compat-0.2.7/dataframe_api_compat/polars_standard/group_by_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import cast
 
 import polars as pl
+from packaging.version import Version
+from packaging.version import parse
 
 from dataframe_api_compat.polars_standard import Namespace
 from dataframe_api_compat.polars_standard.dataframe_object import DataFrame
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
@@ -15,14 +17,16 @@
     from dataframe_api.groupby_object import Aggregation as AggregationT
     from dataframe_api.typing import NullType
     from dataframe_api.typing import Scalar
 
 else:
     GroupByT = object
 
+POLARS_VERSION = parse(pl.__version__)
+
 
 class GroupBy(GroupByT):
     def __init__(
         self,
         df: DataFrame,
         keys: Sequence[str],
         api_version: str,
@@ -54,15 +58,18 @@
         return DataFrame(
             result,
             api_version=self._api_version,
             is_persisted=self._is_persisted,
         )
 
     def size(self) -> DataFrame:
-        result = self._grouped.count().rename({"count": "size"})
+        if Version("0.20.5") > POLARS_VERSION:
+            result = self._grouped.count().rename({"count": "size"})
+        else:
+            result = self._grouped.len().rename({"len": "size"})
         return self._to_dataframe(result)
 
     def any(self, *, skip_nulls: bool | Scalar = True) -> DataFrame:
         self._validate_booleanness()
         result = self._grouped.agg(pl.col("*").any())
         return self._to_dataframe(result)
 
@@ -123,14 +130,15 @@
             ),
         )
 
 
 def resolve_aggregation(aggregation: AggregationT) -> pl.Expr:
     aggregation = cast(Namespace.Aggregation, aggregation)
     if aggregation.aggregation == "count":
-        return pl.count().alias(aggregation.output_name)
+        result = pl.len() if Version("0.20.5") <= POLARS_VERSION else pl.count()
+        return result.alias(aggregation.output_name)
     return getattr(  # type: ignore[no-any-return]
         pl.col(aggregation.column_name),
         aggregation.aggregation,
     )().alias(
         aggregation.output_name,
     )
```

### Comparing `dataframe_api_compat-0.2.6/dataframe_api_compat/polars_standard/scalar_object.py` & `dataframe_api_compat-0.2.7/dataframe_api_compat/polars_standard/scalar_object.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/docs/pandas-column.md` & `dataframe_api_compat-0.2.7/docs/pandas-column.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
       - __gt__
       - __hash__
       - __init__
       - __init_subclass__
       - __invert__
       - __iter__
       - __le__
-      - __len__
       - __lt__
       - __mod__
       - __module__
       - __mul__
       - __ne__
       - __new__
       - __or__
@@ -51,55 +50,55 @@
       - __str__
       - __sub__
       - __subclasshook__
       - __truediv__
       - __weakref__
       - all
       - any
-      - api_version
+      - cast
       - column
       - cumulative_max
       - cumulative_min
       - cumulative_prod
       - cumulative_sum
       - day
-      - df
       - dtype
       - fill_nan
       - fill_null
       - filter
       - floor
-      - take
       - get_value
       - hour
       - is_in
       - is_nan
       - is_null
       - iso_weekday
-      - materialise
+      - len
       - max
       - mean
       - median
       - microsecond
       - min
       - minute
       - month
+      - n_unique
       - name
       - nanosecond
       - parent_dataframe
       - persist
       - prod
       - rename
       - second
       - shift
       - slice_rows
       - sort
       - sorted_indices
       - std
       - sum
+      - take
       - to_array
       - unique_indices
       - unix_timestamp
       - var
       - year
       show_signature_annotations: true
       show_bases: false
```

### Comparing `dataframe_api_compat-0.2.6/docs/pandas-dataframe.md` & `dataframe_api_compat-0.2.7/docs/pandas-dataframe.md`

 * *Files 11% similar despite different names*

```diff
@@ -49,47 +49,42 @@
       - __sizeof__
       - __str__
       - __sub__
       - __subclasshook__
       - __truediv__
       - __weakref__
       - all
-      - all_horizontal
       - any
-      - any_horizontal
-      - api_version
       - assign
+      - cast
       - col
       - column_names
       - dataframe
       - drop
       - drop_nulls
       - fill_nan
       - fill_null
       - filter
       - get_column_names
-      - take
       - group_by
       - is_nan
       - is_null
-      - is_persisted
+      - iter_columns
       - join
       - max
       - mean
       - median
       - min
       - persist
       - prod
       - rename
       - schema
       - select
       - shape
       - slice_rows
       - sort
-      - sorted_indices
       - std
       - sum
+      - take
       - to_array
-      - unique_indices
-      - validate_is_persisted
       - var
       show_signature_annotations: true
```

### Comparing `dataframe_api_compat-0.2.6/docs/pandas-namespace.md` & `dataframe_api_compat-0.2.7/docs/pandas-scalar.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Pandas Namespace
-::: dataframe_api_compat.pandas_standard.Namespace
+# Pandas Scalar
+::: dataframe_api_compat.pandas_standard.Scalar
     handler: python
     paths: []
     options:
       members:
       - __abs__
       - __add__
       - __bool__
@@ -38,20 +38,20 @@
       - __repr__
       - __rfloordiv__
       - __rmod__
       - __rmul__
       - __rpow__
       - __rsub__
       - __rtruediv__
+      - __scalar_namespace__
       - __setattr__
       - __sizeof__
       - __str__
       - __sub__
       - __subclasshook__
       - __truediv__
       - __weakref__
-      - df
       - dtype
-      - is_persisted
+      - parent_dataframe
       - persist
-      - value
+      - scalar
       show_signature_annotations: true
```

### Comparing `dataframe_api_compat-0.2.6/docs/pandas-scalar.md` & `dataframe_api_compat-0.2.7/docs/polars-scalar.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Pandas Scalar
-::: dataframe_api_compat.pandas_standard.Scalar
+# Polars Namespace
+::: dataframe_api_compat.polars_standard.Namespace
     handler: python
     paths: []
     options:
       members:
       - __abs__
       - __add__
       - __bool__
@@ -38,20 +38,20 @@
       - __repr__
       - __rfloordiv__
       - __rmod__
       - __rmul__
       - __rpow__
       - __rsub__
       - __rtruediv__
+      - __scalar_namespace__
       - __setattr__
       - __sizeof__
       - __str__
       - __sub__
       - __subclasshook__
       - __truediv__
       - __weakref__
-      - df
       - dtype
-      - is_persisted
+      - parent_dataframe
       - persist
-      - value
+      - scalar
       show_signature_annotations: true
```

### Comparing `dataframe_api_compat-0.2.6/docs/polars-column.md` & `dataframe_api_compat-0.2.7/docs/polars-column.md`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,14 @@
       - __gt__
       - __hash__
       - __init__
       - __init_subclass__
       - __invert__
       - __iter__
       - __le__
-      - __len__
       - __lt__
       - __mod__
       - __module__
       - __mul__
       - __ne__
       - __new__
       - __or__
@@ -51,55 +50,54 @@
       - __str__
       - __sub__
       - __subclasshook__
       - __truediv__
       - __weakref__
       - all
       - any
-      - api_version
+      - cast
       - column
       - cumulative_max
       - cumulative_min
       - cumulative_prod
       - cumulative_sum
       - day
-      - df
       - dtype
-      - expr
       - fill_nan
       - fill_null
       - filter
       - floor
-      - take
       - get_value
       - hour
       - is_in
       - is_nan
       - is_null
       - iso_weekday
-      - materialise
+      - len
       - max
       - mean
       - median
       - microsecond
       - min
       - minute
       - month
+      - n_unique
       - name
       - nanosecond
       - parent_dataframe
       - persist
       - prod
       - rename
       - second
       - shift
       - slice_rows
       - sort
       - sorted_indices
       - std
       - sum
+      - take
       - to_array
       - unique_indices
       - unix_timestamp
       - var
       - year
       show_signature_annotations: true
```

### Comparing `dataframe_api_compat-0.2.6/docs/polars-dataframe.md` & `dataframe_api_compat-0.2.7/docs/polars-dataframe.md`

 * *Files 12% similar despite different names*

```diff
@@ -49,49 +49,42 @@
       - __sizeof__
       - __str__
       - __sub__
       - __subclasshook__
       - __truediv__
       - __weakref__
       - all
-      - all_horizontal
       - any
-      - any_horizontal
-      - api_version
       - assign
+      - cast
       - col
       - column_names
       - dataframe
-      - df
       - drop
       - drop_nulls
       - fill_nan
       - fill_null
       - filter
       - get_column_names
-      - take
       - group_by
       - is_nan
       - is_null
-      - is_persisted
+      - iter_columns
       - join
-      - materialise_expression
       - max
       - mean
       - median
       - min
       - persist
       - prod
       - rename
       - schema
       - select
       - shape
       - slice_rows
       - sort
-      - sorted_indices
       - std
       - sum
+      - take
       - to_array
-      - unique_indices
-      - validate_is_persisted
       - var
       show_signature_annotations: true
```

### Comparing `dataframe_api_compat-0.2.6/docs/polars-namespace.md` & `dataframe_api_compat-0.2.7/docs/modin-scalar.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Pandas Namespace
-::: dataframe_api_compat.pandas_standard.Namespace
+# Modin Scalar
+::: dataframe_api_compat.modin_standard.Scalar
     handler: python
     paths: []
     options:
       members:
       - __abs__
       - __add__
       - __bool__
@@ -38,21 +38,20 @@
       - __repr__
       - __rfloordiv__
       - __rmod__
       - __rmul__
       - __rpow__
       - __rsub__
       - __rtruediv__
+      - __scalar_namespace__
       - __setattr__
       - __sizeof__
       - __str__
       - __sub__
       - __subclasshook__
       - __truediv__
       - __weakref__
-      - df
       - dtype
-      - is_persisted
-      - materialise
+      - parent_dataframe
       - persist
-      - value
+      - scalar
       show_signature_annotations: true
```

### Comparing `dataframe_api_compat-0.2.6/docs/polars-scalar.md` & `dataframe_api_compat-0.2.7/docs/modin-namespace.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,64 @@
-# Polars Namespace
-::: dataframe_api_compat.polars_standard.Namespace
+# Modin Namespace
+::: dataframe_api_compat.modin_standard.Namespace
     handler: python
     paths: []
     options:
       members:
-      - __abs__
-      - __add__
-      - __bool__
+      - Aggregation
+      - Bool
+      - Date
+      - Datetime
+      - Duration
+      - Float32
+      - Float64
+      - Int16
+      - Int32
+      - Int64
+      - Int8
+      - NullType
+      - String
+      - UInt16
+      - UInt32
+      - UInt64
+      - UInt8
       - __class__
+      - __dataframe_api_version__
       - __delattr__
       - __dict__
       - __dir__
       - __doc__
       - __eq__
-      - __float__
-      - __floordiv__
       - __format__
       - __ge__
       - __getattribute__
       - __gt__
       - __hash__
       - __init__
       - __init_subclass__
-      - __int__
       - __le__
       - __lt__
-      - __mod__
       - __module__
-      - __mul__
       - __ne__
-      - __neg__
       - __new__
-      - __pow__
-      - __radd__
       - __reduce__
       - __reduce_ex__
       - __repr__
-      - __rfloordiv__
-      - __rmod__
-      - __rmul__
-      - __rpow__
-      - __rsub__
-      - __rtruediv__
       - __setattr__
       - __sizeof__
       - __str__
-      - __sub__
       - __subclasshook__
-      - __truediv__
       - __weakref__
-      - df
-      - dtype
-      - is_persisted
-      - materialise
-      - persist
-      - value
+      - all_horizontal
+      - any_horizontal
+      - column_from_1d_array
+      - column_from_sequence
+      - concat
+      - dataframe_from_2d_array
+      - dataframe_from_columns
+      - date
+      - is_dtype
+      - is_null
+      - null
+      - sorted_indices
+      - unique_indices
       show_signature_annotations: true
```

### Comparing `dataframe_api_compat-0.2.6/docs/quick_start.md` & `dataframe_api_compat-0.2.7/docs/quick_start.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # Quick start
 
 ## Prerequisites
 
 Please start by following the [installation instructions](installation.md)
 
-Then, please install the following:
+Then, please install any two libraries from the following list:
 
 - [pandas](https://pandas.pydata.org/docs/getting_started/install.html)
 - [Polars](https://pola-rs.github.io/polars/user-guide/installation/)
+- [Modin](https://modin.readthedocs.io/en/latest/?badge=latest#installation-and-choosing-your-compute-engine)
+
+> [!TIP]
+> The Modin interface is compatible with the pandas interface, so if you want
+> to try Modin in the following examples - just change the following import:
+> `import pandas as pd` -> `import modin.pandas as pd`.
 
 ## Simple example
 
 Create a Python file `t.py` with the following content:
 
 ```python
 import pandas as pd
```

### Comparing `dataframe_api_compat-0.2.6/docs/reference.md` & `dataframe_api_compat-0.2.7/docs/reference.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Reference
 
 ## API Reference
 
 Please refer to the [Dataframe API Spec](https://data-apis.org/dataframe-api/draft/API_specification/index.html).
 
-Note that the spec is not specific to pandas and Polars - if you follow it, then your code will also be compatible
+Note that the spec is not specific to pandas, Polars and Modin - if you follow it, then your code will also be compatible
 with any other packages which implements the spec.
 
 ## Dataframe Interchange Protocol
 
 Standardised way of interchanging data between libraries, see
 [here](https://data-apis.org/dataframe-protocol/latest/index.html).
 
 ## Array API
 
-Array counterpart to the DataFrame API, see [here](https://data-apis.org/array-api/2022.12/index.html).
+Array counterpart to the DataFrame API, see [here](https://data-apis.org/array-api/2023.12/index.html).
```

### Comparing `dataframe_api_compat-0.2.6/docs/basics/column.md` & `dataframe_api_compat-0.2.7/docs/basics/column.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 You might expect a function like the following to just work:
 
 ```python exec="1" source="above" session="ex3"
 def my_func(df1, df2):
     df1_s = df1.__dataframe_consortium_standard__(api_version='2023.11-beta')
     df2_s = df2.__dataframe_consortium_standard__(api_version='2023.11-beta')
     df1_s.filter(df2_s.col('a') > 0)
-    return df_s.dataframe
+    return df1_s.dataframe
 ```
 
 However, if you tried passing two different dataframes to this function, you'd get
 a message saying something like:
 ```python
 cannot compare columns from different dataframes
 ```
```

### Comparing `dataframe_api_compat-0.2.6/docs/basics/complete_example.md` & `dataframe_api_compat-0.2.7/docs/basics/complete_example.md`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/docs/basics/dataframe.md` & `dataframe_api_compat-0.2.7/docs/basics/dataframe.md`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/docs/basics/persist.md` & `dataframe_api_compat-0.2.7/docs/basics/persist.md`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/docs/basics/scalar.md` & `dataframe_api_compat-0.2.7/docs/basics/scalar.md`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/tests/column/any_all_test.py` & `dataframe_api_compat-0.2.7/tests/column/any_all_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 import pytest
 
+from tests.utils import BaseHandler
 from tests.utils import bool_dataframe_1
 
 
-def test_expr_any(library: str) -> None:
+def test_expr_any(library: BaseHandler) -> None:
     df = bool_dataframe_1(library)
     with pytest.raises(RuntimeError):
         bool(df.col("a").any())
     df = df.persist()
     result = df.col("a").any()
     with pytest.warns(UserWarning):
         assert bool(result.persist())
 
 
-def test_expr_all(library: str) -> None:
+def test_expr_all(library: BaseHandler) -> None:
     df = bool_dataframe_1(library).persist()
     result = df.col("a").all()
     assert not bool(result)
```

### Comparing `dataframe_api_compat-0.2.6/tests/column/col_sorted_indices_test.py` & `dataframe_api_compat-0.2.7/tests/column/col_sorted_indices_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,43 @@
 from __future__ import annotations
 
-import pandas as pd
-
-from tests.utils import convert_dataframe_to_pandas_numpy
+from tests.utils import BaseHandler
+from tests.utils import compare_dataframe_with_reference
 from tests.utils import integer_dataframe_6
-from tests.utils import interchange_to_pandas
 
 
-def test_expression_sorted_indices_ascending(library: str) -> None:
+def test_expression_sorted_indices_ascending(library: BaseHandler) -> None:
     df = integer_dataframe_6(library)
-    df.__dataframe_namespace__()
+    ns = df.__dataframe_namespace__()
     col = df.col
     sorted_indices = col("b").sorted_indices()
     result = df.take(sorted_indices)
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected = pd.DataFrame(
-        {
-            "a": [2, 2, 1, 1, 1],
-            "b": [1, 2, 3, 4, 4],
-        },
-    )
-    pd.testing.assert_frame_equal(result_pd, expected)
+    expected = {"a": [2, 2, 1, 1, 1], "b": [1, 2, 3, 4, 4]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Int64)
 
 
-def test_expression_sorted_indices_descending(library: str) -> None:
+def test_expression_sorted_indices_descending(library: BaseHandler) -> None:
     df = integer_dataframe_6(library)
-    df.__dataframe_namespace__()
+    ns = df.__dataframe_namespace__()
     col = df.col
     sorted_indices = col("b").sorted_indices(ascending=False)
     result = df.take(sorted_indices)
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected = pd.DataFrame(
-        {
-            "a": [1, 1, 1, 2, 2],
-            "b": [4, 4, 3, 2, 1],
-        },
-    )
-    pd.testing.assert_frame_equal(result_pd, expected)
+    expected = {"a": [1, 1, 1, 2, 2], "b": [4, 4, 3, 2, 1]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Int64)
 
 
-def test_column_sorted_indices_ascending(library: str) -> None:
-    df = integer_dataframe_6(library).persist()
+def test_column_sorted_indices_ascending(library: BaseHandler) -> None:
+    df = integer_dataframe_6(library)
+    ns = df.__dataframe_namespace__()
     sorted_indices = df.col("b").sorted_indices()
     result = df.take(sorted_indices)
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected = pd.DataFrame(
-        {
-            "a": [2, 2, 1, 1, 1],
-            "b": [1, 2, 3, 4, 4],
-        },
-    )
-    pd.testing.assert_frame_equal(result_pd, expected)
+    expected = {"a": [2, 2, 1, 1, 1], "b": [1, 2, 3, 4, 4]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Int64)
 
 
-def test_column_sorted_indices_descending(library: str) -> None:
-    df = integer_dataframe_6(library).persist()
+def test_column_sorted_indices_descending(library: BaseHandler) -> None:
+    df = integer_dataframe_6(library)
+    ns = df.__dataframe_namespace__()
     sorted_indices = df.col("b").sorted_indices(ascending=False)
     result = df.take(sorted_indices)
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected = pd.DataFrame(
-        {
-            "a": [1, 1, 1, 2, 2],
-            "b": [4, 4, 3, 2, 1],
-        },
-    )
-    pd.testing.assert_frame_equal(result_pd, expected)
+    expected = {"a": [1, 1, 1, 2, 2], "b": [4, 4, 3, 2, 1]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Int64)
```

### Comparing `dataframe_api_compat-0.2.6/tests/column/col_to_array_object_test.py` & `dataframe_api_compat-0.2.7/tests/column/col_to_array_object_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import numpy as np
 import pytest
 
+from tests.utils import BaseHandler
 from tests.utils import bool_dataframe_1
 from tests.utils import integer_dataframe_1
 
 
 @pytest.mark.parametrize(
     "dtype",
     [
@@ -18,25 +19,25 @@
         "uint16",
         "uint32",
         "uint64",
         "float32",
         "float64",
     ],
 )
-def test_column_to_array_object(library: str, dtype: str) -> None:  # noqa: ARG001
+def test_column_to_array_object(library: BaseHandler, dtype: str) -> None:  # noqa: ARG001
     ser = integer_dataframe_1(library).col("a").persist()
     result = np.asarray(ser.to_array())
     expected = np.array([1, 2, 3], dtype=np.int64)
     np.testing.assert_array_equal(result, expected)
 
 
-def test_column_to_array_object_bool(library: str) -> None:
+def test_column_to_array_object_bool(library: BaseHandler) -> None:
     df = bool_dataframe_1(library).persist().col("a")
     result = np.asarray(df.to_array())
     expected = np.array([True, True, False], dtype="bool")
     np.testing.assert_array_equal(result, expected)
 
 
-def test_column_to_array_object_invalid(library: str) -> None:
+def test_column_to_array_object_invalid(library: BaseHandler) -> None:
     df = bool_dataframe_1(library).col("a")
     with pytest.raises(RuntimeError):
         _ = np.asarray(df.to_array())
```

### Comparing `dataframe_api_compat-0.2.6/tests/column/cross_df_comparisons_test.py` & `dataframe_api_compat-0.2.7/tests/column/cross_df_comparisons_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import pytest
 
+from tests.utils import BaseHandler
 from tests.utils import integer_dataframe_1
 from tests.utils import integer_dataframe_2
 
 
-def test_invalid_comparisons(library: str) -> None:
+def test_invalid_comparisons(library: BaseHandler) -> None:
     with pytest.raises(ValueError):
         _ = integer_dataframe_1(library).col("a") > integer_dataframe_2(library).col("a")
 
 
-def test_invalid_comparisons_scalar(library: str) -> None:
+def test_invalid_comparisons_scalar(library: BaseHandler) -> None:
     with pytest.raises(ValueError):
         _ = (
             integer_dataframe_1(library).col("a")
             > integer_dataframe_2(library).col("a").mean()
         )
```

### Comparing `dataframe_api_compat-0.2.6/tests/column/fill_null_test.py` & `dataframe_api_compat-0.2.7/tests/column/fill_null_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from __future__ import annotations
 
+from tests.utils import BaseHandler
 from tests.utils import nan_dataframe_1
 from tests.utils import null_dataframe_2
 
 
-def test_fill_null_column(library: str) -> None:
+def test_fill_null_column(library: BaseHandler) -> None:
     df = null_dataframe_2(library)
     ser = df.col("a")
     result = df.assign(ser.fill_null(0).rename("result")).col("result")
-    assert float(result.get_value(2).persist()) == 0.0  # type:ignore[arg-type]
-    assert float(result.get_value(1).persist()) != 0.0  # type:ignore[arg-type]
-    assert float(result.get_value(0).persist()) != 0.0  # type:ignore[arg-type]
+    assert float(result.get_value(2).persist()) == 0.0  # type: ignore[arg-type]
+    assert float(result.get_value(1).persist()) != 0.0  # type: ignore[arg-type]
+    assert float(result.get_value(0).persist()) != 0.0  # type: ignore[arg-type]
 
 
-def test_fill_null_noop_column(library: str) -> None:
+def test_fill_null_noop_column(library: BaseHandler) -> None:
     df = nan_dataframe_1(library)
     ser = df.col("a")
     result = df.assign(ser.fill_null(0).rename("result")).persist().col("result")
-    if library != "pandas-numpy":
+    if library.name not in ("pandas-numpy", "modin"):
         # nan should not have changed!
         assert float(result.get_value(2)) != float(  # type: ignore[arg-type]
             result.get_value(2),  # type: ignore[arg-type]
         )
     else:
         # nan was filled with 0
         assert float(result.get_value(2)) == 0  # type: ignore[arg-type]
```

### Comparing `dataframe_api_compat-0.2.6/tests/column/get_rows_by_mask_test.py` & `dataframe_api_compat-0.2.7/tests/column/get_rows_by_mask_test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from __future__ import annotations
 
 import pandas as pd
 
+from tests.utils import BaseHandler
+from tests.utils import compare_column_with_reference
 from tests.utils import integer_dataframe_1
-from tests.utils import interchange_to_pandas
 
 
-def test_column_filter(library: str) -> None:
+def test_column_filter(library: BaseHandler) -> None:
     df = integer_dataframe_1(library)
     ser = df.col("a")
     mask = ser > 1
     ser = ser.filter(mask).persist()
     result_pd = pd.Series(ser.to_array(), name="result")
     expected = pd.Series([2, 3], name="result")
     pd.testing.assert_series_equal(result_pd, expected)
 
 
-def test_column_take_by_mask_noop(library: str) -> None:
+def test_column_take_by_mask_noop(library: BaseHandler) -> None:
     df = integer_dataframe_1(library)
-    df.__dataframe_namespace__()
+    ns = df.__dataframe_namespace__()
     ser = df.col("a")
     mask = ser > 0
     ser = ser.filter(mask)
     result = df.assign(ser.rename("result"))
-    result_pd = interchange_to_pandas(result)["result"]
-    expected = pd.Series([1, 2, 3], name="result")
-    pd.testing.assert_series_equal(result_pd, expected)
+    compare_column_with_reference(result.col("result"), [1, 2, 3], dtype=ns.Int64)
```

### Comparing `dataframe_api_compat-0.2.6/tests/column/is_in_test.py` & `dataframe_api_compat-0.2.7/tests/column/is_in_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from typing import Any
 
-import pandas as pd
 import pytest
 
+from tests.utils import BaseHandler
+from tests.utils import compare_column_with_reference
 from tests.utils import float_dataframe_1
 from tests.utils import float_dataframe_2
 from tests.utils import float_dataframe_3
-from tests.utils import interchange_to_pandas
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
 
 @pytest.mark.parametrize(
     ("df_factory", "expected_values"),
@@ -21,42 +21,40 @@
         (float_dataframe_1, [False, True]),
         (float_dataframe_2, [True, False]),
         (float_dataframe_3, [True, False]),
     ],
 )
 @pytest.mark.filterwarnings("ignore:np.find_common_type is deprecated")
 def test_is_in(
-    library: str,
-    df_factory: Callable[[str], Any],
+    library: BaseHandler,
+    df_factory: Callable[[BaseHandler], Any],
     expected_values: list[bool],
 ) -> None:
-    df = df_factory(library).persist()
+    df = df_factory(library)
+    ns = df.__dataframe_namespace__()
     ser = df.col("a")
     other = ser + 1
     result = df.assign(ser.is_in(other).rename("result"))
-    result_pd = interchange_to_pandas(result)["result"]
-    expected = pd.Series(expected_values, name="result")
-    pd.testing.assert_series_equal(result_pd, expected)
+    compare_column_with_reference(result.col("result"), expected_values, dtype=ns.Bool)
 
 
 @pytest.mark.parametrize(
     ("df_factory", "expected_values"),
     [
         (float_dataframe_1, [False, True]),
         (float_dataframe_2, [True, False]),
         (float_dataframe_3, [True, False]),
     ],
 )
 @pytest.mark.filterwarnings("ignore:np.find_common_type is deprecated")
 def test_expr_is_in(
-    library: str,
-    df_factory: Callable[[str], Any],
+    library: BaseHandler,
+    df_factory: Callable[[BaseHandler], Any],
     expected_values: list[bool],
 ) -> None:
     df = df_factory(library)
+    ns = df.__dataframe_namespace__()
     col = df.col
     ser = col("a")
     other = ser + 1
     result = df.assign(ser.is_in(other).rename("result"))
-    result_pd = interchange_to_pandas(result)["result"]
-    expected = pd.Series(expected_values, name="result")
-    pd.testing.assert_series_equal(result_pd, expected)
+    compare_column_with_reference(result.col("result"), expected_values, dtype=ns.Bool)
```

### Comparing `dataframe_api_compat-0.2.6/tests/column/reductions_test.py` & `dataframe_api_compat-0.2.7/tests/dataframe/any_all_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 from __future__ import annotations
 
-import pandas as pd
 import pytest
 
-from tests.utils import integer_dataframe_1
-from tests.utils import interchange_to_pandas
+from tests.utils import BaseHandler
+from tests.utils import bool_dataframe_1
+from tests.utils import bool_dataframe_3
+from tests.utils import compare_dataframe_with_reference
 
 
 @pytest.mark.parametrize(
-    ("reduction", "expected"),
+    ("reduction", "expected_data"),
     [
-        ("min", 1),
-        ("max", 3),
-        ("sum", 6),
-        ("prod", 6),
-        ("median", 2.0),
-        ("mean", 2.0),
-        ("std", 1.0),
-        ("var", 1.0),
+        ("any", {"a": [True], "b": [True]}),
+        ("all", {"a": [False], "b": [True]}),
     ],
 )
-def test_expression_reductions(
-    library: str,
+def test_reductions(
+    library: BaseHandler,
     reduction: str,
-    expected: float,
+    expected_data: dict[str, object],
 ) -> None:
-    df = integer_dataframe_1(library)
-    df.__dataframe_namespace__()
-    ser = df.col("a")
-    ser = ser - getattr(ser, reduction)()
-    result = df.assign(ser.rename("result"))
-    result_pd = interchange_to_pandas(result)["result"]
-    ser_pd = interchange_to_pandas(df)["a"].rename("result")
-    expected_pd = ser_pd - expected
-    pd.testing.assert_series_equal(result_pd, expected_pd)
+    df = bool_dataframe_1(library)
+    ns = df.__dataframe_namespace__()
+    result = getattr(df, reduction)()
+    compare_dataframe_with_reference(result, expected_data, dtype=ns.Bool)  # type: ignore[arg-type]
+
+
+def test_any(library: BaseHandler) -> None:
+    df = bool_dataframe_3(library)
+    ns = df.__dataframe_namespace__()
+    result = df.any()
+    expected = {"a": [False], "b": [True], "c": [True]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Bool)
+
+
+def test_all(library: BaseHandler) -> None:
+    df = bool_dataframe_3(library)
+    ns = df.__dataframe_namespace__()
+    result = df.all()
+    expected = {"a": [False], "b": [False], "c": [True]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Bool)
```

### Comparing `dataframe_api_compat-0.2.6/tests/column/shift_test.py` & `dataframe_api_compat-0.2.7/tests/column/pow_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,53 @@
-import pandas as pd
-import polars as pl
-from polars.testing import assert_frame_equal
+from __future__ import annotations
 
-from tests.utils import float_dataframe_1
+from tests.utils import BaseHandler
+from tests.utils import compare_dataframe_with_reference
 from tests.utils import integer_dataframe_1
-from tests.utils import interchange_to_pandas
 
 
-def test_shift_with_fill_value(library: str) -> None:
+def test_float_powers_column(library: BaseHandler) -> None:
     df = integer_dataframe_1(library)
-    result = df.assign(df.col("a").shift(1).fill_null(999))
-    expected = pd.DataFrame(
-        {
-            "a": [999, 1, 2],
-            "b": [4, 5, 6],
-        },
-    )
-    result_pd = interchange_to_pandas(result)
-    if library == "pandas-numpy":
-        result_pd = result_pd.astype("int64")
-    pd.testing.assert_frame_equal(result_pd, expected)
-
-
-def test_shift_without_fill_value(library: str) -> None:
-    df = float_dataframe_1(library)
-    result = df.assign(df.col("a").shift(-1))
-    if library == "pandas-numpy":
-        expected = pd.DataFrame({"a": [3.0, float("nan")]})
-        pd.testing.assert_frame_equal(result.dataframe, expected)
-    elif library == "pandas-nullable":
-        expected = pd.DataFrame({"a": [3.0, None]}, dtype="Float64")
-        pd.testing.assert_frame_equal(result.dataframe, expected)
-    elif library == "polars-lazy":
-        expected = pl.DataFrame({"a": [3.0, None]})
-        assert_frame_equal(result.dataframe.collect(), expected)  # type: ignore[attr-defined]
-    else:  # pragma: no cover
-        msg = "unexpected library"
-        raise AssertionError(msg)
+    ns = df.__dataframe_namespace__()
+    ser = df.col("a")
+    other = df.col("b") * 1.0
+    result = df.assign(ser.__pow__(other).rename("result"))
+    expected = {"a": [1, 2, 3], "b": [4, 5, 6], "result": [1.0, 32.0, 729.0]}
+    expected_dtype = {"a": ns.Int64, "b": ns.Int64, "result": ns.Float64}
+    compare_dataframe_with_reference(result, expected, expected_dtype)  # type: ignore[arg-type]
 
 
-def test_shift_with_fill_value_complicated(library: str) -> None:
+def test_float_powers_scalar_column(library: BaseHandler) -> None:
     df = integer_dataframe_1(library)
-    result = df.assign(df.col("a").shift(1).fill_null(df.col("a").mean()))
-    expected = pd.DataFrame(
-        {
-            "a": [2.0, 1, 2],
-            "b": [4, 5, 6],
-        },
-    )
-    result_pd = interchange_to_pandas(result)
-    if library == "pandas-nullable":
-        result_pd = result_pd.astype({"a": "float64"})
-    pd.testing.assert_frame_equal(result_pd, expected)
+    ns = df.__dataframe_namespace__()
+    ser = df.col("a")
+    other = 1.0
+    result = df.assign(ser.__pow__(other).rename("result"))
+    expected = {"a": [1, 2, 3], "b": [4, 5, 6], "result": [1.0, 2.0, 3.0]}
+    expected_dtype = {"a": ns.Int64, "b": ns.Int64, "result": ns.Float64}
+    compare_dataframe_with_reference(result, expected, expected_dtype)  # type: ignore[arg-type]
+
+
+def test_int_powers_column(library: BaseHandler) -> None:
+    df = integer_dataframe_1(library)
+    ns = df.__dataframe_namespace__()
+    ser = df.col("a")
+    other = df.col("b") * 1
+    result = df.assign(ser.__pow__(other).rename("result"))
+    if library.name == "polars-lazy":
+        result = result.cast({name: ns.Int64() for name in ("a", "b", "result")})
+    expected = {"a": [1, 2, 3], "b": [4, 5, 6], "result": [1, 32, 729]}
+    expected_dtype = {name: ns.Int64 for name in ("a", "b", "result")}
+    compare_dataframe_with_reference(result, expected, expected_dtype)
+
+
+def test_int_powers_scalar_column(library: BaseHandler) -> None:
+    df = integer_dataframe_1(library)
+    ns = df.__dataframe_namespace__()
+    ser = df.col("a")
+    other = 1
+    result = df.assign(ser.__pow__(other).rename("result"))
+    if library.name == "polars-lazy":
+        result = result.cast({name: ns.Int64() for name in ("a", "b", "result")})
+    expected = {"a": [1, 2, 3], "b": [4, 5, 6], "result": [1, 2, 3]}
+    expected_dtype = {name: ns.Int64 for name in ("a", "b", "result")}
+    compare_dataframe_with_reference(result, expected, expected_dtype)
```

### Comparing `dataframe_api_compat-0.2.6/tests/column/slice_rows_test.py` & `dataframe_api_compat-0.2.7/tests/column/slice_rows_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from __future__ import annotations
 
 from typing import Any
 
 import pandas as pd
 import pytest
 
+from tests.utils import BaseHandler
 from tests.utils import integer_dataframe_3
 
 
 @pytest.mark.parametrize(
     ("start", "stop", "step", "expected"),
     [
         (2, 7, 2, pd.Series([3, 5, 7], name="result")),
         (None, 7, 2, pd.Series([1, 3, 5, 7], name="result")),
         (2, None, 2, pd.Series([3, 5, 7], name="result")),
         (2, None, None, pd.Series([3, 4, 5, 6, 7], name="result")),
     ],
 )
 def test_column_slice_rows(
-    library: str,
+    library: BaseHandler,
     start: int | None,
     stop: int | None,
     step: int | None,
     expected: pd.Series[Any],
 ) -> None:
     ser = integer_dataframe_3(library).col("a")
     result = ser.slice_rows(start, stop, step).persist()
```

### Comparing `dataframe_api_compat-0.2.6/tests/column/temporal/components_test.py` & `dataframe_api_compat-0.2.7/tests/column/temporal/components_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Literal
 
-import pandas as pd
 import pytest
 
-from tests.utils import interchange_to_pandas
+from tests.utils import BaseHandler
+from tests.utils import compare_column_with_reference
 from tests.utils import temporal_dataframe_1
 
 
 @pytest.mark.parametrize(
     ("attr", "expected"),
     [
         ("year", [2020, 2020, 2020]),
@@ -18,77 +18,93 @@
         ("hour", [1, 3, 5]),
         ("minute", [2, 1, 4]),
         ("second", [1, 2, 9]),
         ("iso_weekday", [3, 4, 5]),
         ("unix_timestamp", [1577840521, 1577934062, 1578027849]),
     ],
 )
-def test_col_components(library: str, attr: str, expected: list[int]) -> None:
-    df = temporal_dataframe_1(library).persist()
+def test_col_components(library: BaseHandler, attr: str, expected: list[int]) -> None:
+    df = temporal_dataframe_1(library)
+    ns = df.__dataframe_namespace__()
     for col_name in ("a", "c", "e"):
-        result = df.assign(getattr(df.col(col_name), attr)().rename("result")).select(
-            "result",
+        result = (
+            df.assign(getattr(df.col(col_name), attr)().rename("result"))
+            .select(
+                "result",
+            )
+            .cast({"result": ns.Int64()})
         )
-        result = interchange_to_pandas(result)["result"].astype("int64")
-        expected = pd.Series(expected, name="result")
-        pd.testing.assert_series_equal(result, expected)
+        compare_column_with_reference(result.col("result"), expected, dtype=ns.Int64)
 
 
 @pytest.mark.parametrize(
     ("col_name", "expected"),
     [
         ("a", [123000, 321000, 987000]),
         ("c", [123543, 321654, 987321]),
         ("e", [123543, 321654, 987321]),
     ],
 )
-def test_col_microsecond(library: str, col_name: str, expected: list[int]) -> None:
-    df = temporal_dataframe_1(library).persist()
-    result = df.assign(df.col(col_name).microsecond().rename("result")).select(
-        "result",
+def test_col_microsecond(
+    library: BaseHandler,
+    col_name: str,
+    expected: list[int],
+) -> None:
+    df = temporal_dataframe_1(library)
+    ns = df.__dataframe_namespace__()
+    result = (
+        df.assign(df.col(col_name).microsecond().rename("result"))
+        .select(
+            "result",
+        )
+        .cast({"result": ns.Int64()})
     )
-    result = interchange_to_pandas(result)["result"].astype("int64")
-    expected = pd.Series(expected, name="result")
-    pd.testing.assert_series_equal(result, expected)
+    compare_column_with_reference(result.col("result"), expected, dtype=ns.Int64)
 
 
 @pytest.mark.parametrize(
     ("col_name", "expected"),
     [
         ("a", [123000000, 321000000, 987000000]),
         ("c", [123543000, 321654000, 987321000]),
         ("e", [123543000, 321654000, 987321000]),
     ],
 )
-def test_col_nanosecond(library: str, col_name: str, expected: list[int]) -> None:
-    df = temporal_dataframe_1(library).persist()
-    result = df.assign(df.col(col_name).nanosecond().rename("result")).select(  # type: ignore[attr-defined]
-        "result",
+def test_col_nanosecond(library: BaseHandler, col_name: str, expected: list[int]) -> None:
+    df = temporal_dataframe_1(library)
+    ns = df.__dataframe_namespace__()
+    result = (
+        df.assign(df.col(col_name).nanosecond().rename("result"))  # type: ignore[attr-defined]
+        .select(
+            "result",
+        )
+        .cast({"result": ns.Int64()})
     )
-    result = interchange_to_pandas(result)["result"].astype("int64")
-    expected = pd.Series(expected, name="result")
-    pd.testing.assert_series_equal(result, expected)
+    compare_column_with_reference(result.col("result"), expected, dtype=ns.Int64)
 
 
 @pytest.mark.parametrize(
     ("time_unit", "expected"),
     [
         ("s", [1577840521, 1577934062, 1578027849]),
         ("ms", [1577840521123, 1577934062321, 1578027849987]),
         ("us", [1577840521123543, 1577934062321654, 1578027849987321]),
         ("ns", [1577840521123543000, 1577934062321654000, 1578027849987321000]),
     ],
 )
 def test_col_unix_timestamp_time_units(
-    library: str,
+    library: BaseHandler,
     time_unit: Literal["s", "ms", "us", "ns"],
     expected: list[int],
 ) -> None:
     df = temporal_dataframe_1(library)
-    result = df.assign(
-        df.col("e").unix_timestamp(time_unit=time_unit).rename("result"),
-    ).select(
-        "result",
+    ns = df.__dataframe_namespace__()
+    result = (
+        df.assign(
+            df.col("e").unix_timestamp(time_unit=time_unit).rename("result"),
+        )
+        .select(
+            "result",
+        )
+        .cast({"result": ns.Int64()})
     )
-    result = interchange_to_pandas(result)["result"].astype("int64")
-    expected = pd.Series(expected, name="result")
-    pd.testing.assert_series_equal(result, expected, check_exact=True)
+    compare_column_with_reference(result.col("result"), expected, dtype=ns.Int64)
```

### Comparing `dataframe_api_compat-0.2.6/tests/dataframe/and_test.py` & `dataframe_api_compat-0.2.7/tests/dataframe/and_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from __future__ import annotations
 
-import pandas as pd
-
+from tests.utils import BaseHandler
 from tests.utils import bool_dataframe_1
-from tests.utils import convert_dataframe_to_pandas_numpy
-from tests.utils import interchange_to_pandas
+from tests.utils import compare_dataframe_with_reference
 
 
-def test_and_with_scalar(library: str) -> None:
+def test_and_with_scalar(library: BaseHandler) -> None:
     df = bool_dataframe_1(library)
+    ns = df.__dataframe_namespace__()
     other = True
     result = df & other
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected = pd.DataFrame({"a": [True, True, False], "b": [True, True, True]})
-    pd.testing.assert_frame_equal(result_pd, expected)
+    expected = {"a": [True, True, False], "b": [True, True, True]}
+    compare_dataframe_with_reference(result, expected, ns.Bool)
 
 
-def test_rand_with_scalar(library: str) -> None:
+def test_rand_with_scalar(library: BaseHandler) -> None:
     df = bool_dataframe_1(library)
+    ns = df.__dataframe_namespace__()
     other = True
     result = other & df
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected = pd.DataFrame({"a": [True, True, False], "b": [True, True, True]})
-    pd.testing.assert_frame_equal(result_pd, expected)
+    expected = {"a": [True, True, False], "b": [True, True, True]}
+    compare_dataframe_with_reference(result, expected, ns.Bool)
```

### Comparing `dataframe_api_compat-0.2.6/tests/dataframe/fill_nan_test.py` & `dataframe_api_compat-0.2.7/tests/dataframe/fill_nan_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 from __future__ import annotations
 
-import pandas as pd
 import pytest
 
-from tests.utils import interchange_to_pandas
+from tests.utils import BaseHandler
+from tests.utils import compare_dataframe_with_reference
 from tests.utils import nan_dataframe_1
 
 
-def test_fill_nan(library: str) -> None:
+def test_fill_nan(library: BaseHandler) -> None:
     df = nan_dataframe_1(library)
+    ns = df.__dataframe_namespace__()
     result = df.fill_nan(-1)
-    result_pd = interchange_to_pandas(result)
-    result_pd = result_pd.astype("float64")
-    expected = pd.DataFrame({"a": [1.0, 2.0, -1.0]})
-    pd.testing.assert_frame_equal(result_pd, expected)
+    result = result.cast({"a": ns.Float64()})
+    expected = {"a": [1.0, 2.0, -1.0]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Float64)
 
 
-def test_fill_nan_with_scalar(library: str) -> None:
+def test_fill_nan_with_scalar(library: BaseHandler) -> None:
     df = nan_dataframe_1(library)
+    ns = df.__dataframe_namespace__()
     result = df.fill_nan(df.col("a").get_value(0))
-    result_pd = interchange_to_pandas(result)
-    result_pd = result_pd.astype("float64")
-    expected = pd.DataFrame({"a": [1.0, 2.0, 1.0]})
-    pd.testing.assert_frame_equal(result_pd, expected)
+    result = result.cast({"a": ns.Float64()})
+    expected = {"a": [1.0, 2.0, 1.0]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Float64)
 
 
-def test_fill_nan_with_scalar_invalid(library: str) -> None:
+def test_fill_nan_with_scalar_invalid(library: BaseHandler) -> None:
     df = nan_dataframe_1(library)
     other = df + 1
     with pytest.raises(ValueError):
         _ = df.fill_nan(other.col("a").get_value(0))
 
 
-def test_fill_nan_with_null(library: str) -> None:
+def test_fill_nan_with_null(library: BaseHandler) -> None:
     df = nan_dataframe_1(library)
-    namespace = df.__dataframe_namespace__()
-    result = df.fill_nan(namespace.null)
+    ns = df.__dataframe_namespace__()
+    result = df.fill_nan(ns.null)
     n_nans = result.is_nan().sum()
-    n_nans = interchange_to_pandas(n_nans)
-    if library == "pandas-numpy":
+    result = n_nans.col("a").persist().get_value(0).scalar
+    if library.name in ("pandas-numpy", "modin"):
         # null is nan for pandas-numpy
-        assert n_nans["a"][0] == 1  # type: ignore[index]
+        assert result == 1
     else:
-        assert n_nans["a"][0] == 0  # type: ignore[index]
+        assert result == 0
```

### Comparing `dataframe_api_compat-0.2.6/tests/dataframe/fill_null_test.py` & `dataframe_api_compat-0.2.7/tests/dataframe/fill_null_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from __future__ import annotations
 
 import pytest
 
-from tests.utils import interchange_to_pandas
+from tests.utils import BaseHandler
 from tests.utils import nan_dataframe_1
 from tests.utils import null_dataframe_2
 
 
 @pytest.mark.parametrize(
     "column_names",
     [
         ["a", "b"],
         None,
         ["a"],
         ["b"],
     ],
 )
-def test_fill_null(library: str, column_names: list[str] | None) -> None:
+def test_fill_null(library: BaseHandler, column_names: list[str] | None) -> None:
     df = null_dataframe_2(library)
     df.__dataframe_namespace__()
     result = df.fill_null(0, column_names=column_names)
 
     if column_names is None or "a" in column_names:
         res1 = result.filter(result.col("a").is_null()).persist()
         # check there no nulls left in the column
         assert res1.shape()[0] == 0
         # check the last element was filled with 0
-        assert interchange_to_pandas(result)["a"].iloc[2] == 0
+        assert result.col("a").persist().get_value(2).scalar == 0
     if column_names is None or "b" in column_names:
         res1 = result.filter(result.col("b").is_null()).persist()
         assert res1.shape()[0] == 0
-        assert interchange_to_pandas(result)["b"].iloc[2] == 0
+        assert result.col("b").persist().get_value(2).scalar == 0
 
 
-def test_fill_null_noop(library: str) -> None:
+def test_fill_null_noop(library: BaseHandler) -> None:
     df = nan_dataframe_1(library)
     result_raw = df.fill_null(0)
     if hasattr(result_raw.dataframe, "collect"):
         result = result_raw.dataframe.collect()
     else:
         result = result_raw.dataframe
-    if library != "pandas-numpy":
+    if library.name not in ("pandas-numpy", "modin"):
         # nan should not have changed!
         assert result["a"][2] != result["a"][2]
     else:
         # in pandas-numpy, null is nan, so it gets filled
         assert result["a"][2] == 0
```

### Comparing `dataframe_api_compat-0.2.6/tests/dataframe/get_rows_test.py` & `dataframe_api_compat-0.2.7/tests/dataframe/get_rows_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from __future__ import annotations
 
-import pandas as pd
-
-from tests.utils import convert_dataframe_to_pandas_numpy
+from tests.utils import BaseHandler
+from tests.utils import compare_dataframe_with_reference
 from tests.utils import integer_dataframe_1
-from tests.utils import interchange_to_pandas
 
 
-def test_take(library: str) -> None:
+def test_take(library: BaseHandler) -> None:
     df = integer_dataframe_1(library)
-    df.__dataframe_namespace__()
+    ns = df.__dataframe_namespace__()
     df = df.assign((df.col("a") - 1).sort(ascending=False).rename("result"))
-    df.__dataframe_namespace__()
     result = df.take(df.col("result"))
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected = pd.DataFrame({"a": [3, 2, 1], "b": [6, 5, 4], "result": [0, 1, 2]})
-    pd.testing.assert_frame_equal(result_pd, expected)
+    expected = {"a": [3, 2, 1], "b": [6, 5, 4], "result": [0, 1, 2]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Int64)
```

### Comparing `dataframe_api_compat-0.2.6/tests/dataframe/is_null_test.py` & `dataframe_api_compat-0.2.7/tests/dataframe/is_null_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from __future__ import annotations
 
-import pandas as pd
-
-from tests.utils import interchange_to_pandas
+from tests.utils import BaseHandler
+from tests.utils import compare_dataframe_with_reference
 from tests.utils import nan_dataframe_2
 from tests.utils import null_dataframe_1
 
 
-def test_is_null_1(library: str) -> None:
+def test_is_null_1(library: BaseHandler) -> None:
     df = nan_dataframe_2(library)
+    ns = df.__dataframe_namespace__()
     result = df.is_null()
-    result_pd = interchange_to_pandas(result)
-    if library == "pandas-numpy":
+    if library.name == "pandas-numpy":
         # nan and null are the same in pandas-numpy
-        expected = pd.DataFrame({"a": [False, False, True]})
+        expected = {"a": [False, False, True]}
     else:
-        expected = pd.DataFrame({"a": [False, False, False]})
-    pd.testing.assert_frame_equal(result_pd, expected)
+        expected = {"a": [False, False, False]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Bool)
 
 
-def test_is_null_2(library: str) -> None:
+def test_is_null_2(library: BaseHandler) -> None:
     df = null_dataframe_1(library)
+    ns = df.__dataframe_namespace__()
     result = df.is_null()
-    result_pd = interchange_to_pandas(result)
-    expected = pd.DataFrame({"a": [False, False, True]})
-    pd.testing.assert_frame_equal(result_pd, expected)
+    expected = {"a": [False, False, True]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Bool)
```

### Comparing `dataframe_api_compat-0.2.6/tests/dataframe/or_test.py` & `dataframe_api_compat-0.2.7/tests/dataframe/all_rowwise_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 from __future__ import annotations
 
-import pandas as pd
+import pytest
 
+from tests.utils import BaseHandler
 from tests.utils import bool_dataframe_1
-from tests.utils import convert_dataframe_to_pandas_numpy
-from tests.utils import interchange_to_pandas
+from tests.utils import compare_dataframe_with_reference
 
 
-def test_or_with_scalar(library: str) -> None:
+def test_all_horizontal(library: BaseHandler) -> None:
     df = bool_dataframe_1(library)
-    other = True
-    result = df | other
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected = pd.DataFrame({"a": [True, True, True], "b": [True, True, True]})
-    pd.testing.assert_frame_equal(result_pd, expected)
+    ns = df.__dataframe_namespace__()
+    mask = ns.all_horizontal(*[df.col(col_name) for col_name in df.column_names])
+    result = df.filter(mask)
+    expected = {"a": [True, True], "b": [True, True]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Bool)
 
 
-def test_ror_with_scalar(library: str) -> None:
+def test_all_horizontal_invalid(library: BaseHandler) -> None:
     df = bool_dataframe_1(library)
-    other = True
-    result = other | df
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected = pd.DataFrame({"a": [True, True, True], "b": [True, True, True]})
-    pd.testing.assert_frame_equal(result_pd, expected)
+    namespace = df.__dataframe_namespace__()
+    with pytest.raises(ValueError):
+        _ = namespace.all_horizontal(df.col("a"), (df + 1).col("b"))
```

### Comparing `dataframe_api_compat-0.2.6/tests/dataframe/rename_columns_test.py` & `dataframe_api_compat-0.2.7/tests/dataframe/divmod_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,16 @@
 from __future__ import annotations
 
-import pandas as pd
-import pytest
-
-from tests.utils import convert_dataframe_to_pandas_numpy
+from tests.utils import BaseHandler
+from tests.utils import compare_dataframe_with_reference
 from tests.utils import integer_dataframe_1
-from tests.utils import interchange_to_pandas
-
-
-def test_rename(library: str) -> None:
-    df = integer_dataframe_1(library)
-    result = df.rename({"a": "c", "b": "e"})
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected = pd.DataFrame({"c": [1, 2, 3], "e": [4, 5, 6]})
-    pd.testing.assert_frame_equal(result_pd, expected)
 
 
-def test_rename_invalid(library: str) -> None:
+def test_divmod_with_scalar(library: BaseHandler) -> None:
     df = integer_dataframe_1(library)
-    with pytest.raises(
-        TypeError,
-        match="Expected Mapping, got: <class 'function'>",
-    ):  # pragma: no cover
-        # why is this not covered? bug in coverage?
-        df.rename(lambda x: x.upper())  # type: ignore  # noqa: PGH003
+    ns = df.__dataframe_namespace__()
+    other = 2
+    result_quotient, result_remainder = df.__divmod__(other)
+    expected_quotient = {"a": [0, 1, 1], "b": [2, 2, 3]}
+    expected_remainder = {"a": [1, 0, 1], "b": [0, 1, 0]}
+    compare_dataframe_with_reference(result_quotient, expected_quotient, dtype=ns.Int64)
+    compare_dataframe_with_reference(result_remainder, expected_remainder, dtype=ns.Int64)
```

### Comparing `dataframe_api_compat-0.2.6/tests/dataframe/schema_test.py` & `dataframe_api_compat-0.2.7/tests/dataframe/schema_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
-import pandas as pd
 import pytest
 from packaging.version import Version
 
-from tests.utils import PANDAS_VERSION
+from tests.utils import BaseHandler
 from tests.utils import mixed_dataframe_1
+from tests.utils import pandas_version
 
 
-@pytest.mark.skipif(
-    Version("2.0.0") > PANDAS_VERSION,
-    reason="no pyarrow support",
-)
-def test_schema(library: str) -> None:
+def test_schema(library: BaseHandler) -> None:
+    if library.name in ("pandas-numpy", "pandas-nullable") and pandas_version() < Version(
+        "2.0.0",
+    ):  # pragma: no cover
+        pytest.skip(reason="no pyarrow support")
     df = mixed_dataframe_1(library)
     namespace = df.__dataframe_namespace__()
     result = df.schema
     assert list(result.keys()) == [
         "a",
         "b",
         "c",
@@ -46,35 +46,35 @@
     assert isinstance(result["i"], namespace.Float64)
     assert isinstance(result["j"], namespace.Float32)
     assert isinstance(result["k"], namespace.Bool)
     assert isinstance(result["l"], namespace.String)
     assert isinstance(result["m"], namespace.Datetime)
     assert isinstance(result["n"], namespace.Datetime)
     if not (
-        library.startswith("pandas")
-        and tuple(int(v) for v in pd.__version__.split(".")) < (2, 0, 0)
+        library.name in ("pandas-numpy", "pandas-nullable")
+        and pandas_version() < Version("2.0.0")
     ):  # pragma: no cover (coverage bug?)
         # pandas non-nanosecond support only came in 2.0
         assert result["n"].time_unit == "ms"
     else:  # pragma: no cover
         pass
     assert result["n"].time_zone is None
     assert isinstance(result["o"], namespace.Datetime)
     if not (
-        library.startswith("pandas")
-        and tuple(int(v) for v in pd.__version__.split(".")) < (2, 0, 0)
+        library.name in ("pandas-numpy", "pandas-nullable")
+        and pandas_version() < Version("2.0.0")
     ):  # pragma: no cover (coverage bug?)
         # pandas non-nanosecond support only came in 2.0
         assert result["o"].time_unit == "us"
     else:  # pragma: no cover
         pass
     assert result["o"].time_zone is None
     if not (
-        library.startswith("pandas")
-        and tuple(int(v) for v in pd.__version__.split(".")) < (2, 0, 0)
+        library.name in ("pandas-numpy", "pandas-nullable")
+        and pandas_version() < Version("2.0.0")
     ):
         # pandas non-nanosecond support only came in 2.0 - before that, these would be 'float'
         assert isinstance(result["p"], namespace.Duration)
         assert result["p"].time_unit == "ms"
         assert isinstance(result["q"], namespace.Duration)
         assert result["q"].time_unit == "us"
     else:  # pragma: no cover
```

### Comparing `dataframe_api_compat-0.2.6/tests/dataframe/update_columns_test.py` & `dataframe_api_compat-0.2.7/tests/dataframe/update_columns_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from __future__ import annotations
 
-import pandas as pd
-
+from tests.utils import BaseHandler
+from tests.utils import compare_dataframe_with_reference
 from tests.utils import integer_dataframe_1
-from tests.utils import interchange_to_pandas
 
 
-def test_update_columns(library: str) -> None:
+def test_update_columns(library: BaseHandler) -> None:
     df = integer_dataframe_1(library)
-    df.__dataframe_namespace__()
+    ns = df.__dataframe_namespace__()
     col = df.col
     result = df.assign(col("a") + 1)
-    result_pd = interchange_to_pandas(result)
-    expected = pd.DataFrame({"a": [2, 3, 4], "b": [4, 5, 6]})
-    pd.testing.assert_frame_equal(result_pd, expected)
+    expected = {"a": [2, 3, 4], "b": [4, 5, 6]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Int64)
 
 
-def test_update_multiple_columns(library: str) -> None:
+def test_update_multiple_columns(library: BaseHandler) -> None:
     df = integer_dataframe_1(library)
-    df.__dataframe_namespace__()
+    ns = df.__dataframe_namespace__()
     col = df.col
     result = df.assign(col("a") + 1, col("b") + 2)
-    result_pd = interchange_to_pandas(result)
-    expected = pd.DataFrame({"a": [2, 3, 4], "b": [6, 7, 8]})
-    pd.testing.assert_frame_equal(result_pd, expected)
+    expected = {"a": [2, 3, 4], "b": [6, 7, 8]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Int64)
```

### Comparing `dataframe_api_compat-0.2.6/tests/groupby/size_test.py` & `dataframe_api_compat-0.2.7/tests/groupby/size_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from __future__ import annotations
 
-import pandas as pd
-
-from tests.utils import convert_dataframe_to_pandas_numpy
+from tests.utils import BaseHandler
+from tests.utils import compare_dataframe_with_reference
 from tests.utils import integer_dataframe_4
-from tests.utils import interchange_to_pandas
 
 
-def test_group_by_size(library: str) -> None:
+def test_group_by_size(library: BaseHandler) -> None:
     df = integer_dataframe_4(library)
+    ns = df.__dataframe_namespace__()
     result = df.group_by("key").size()
     result = result.sort("key")
-    result_pd = interchange_to_pandas(result)
-    expected = pd.DataFrame({"key": [1, 2], "size": [2, 2]})
+    expected = {"key": [1, 2], "size": [2, 2]}
     # TODO polars returns uint32. what do we standardise to?
-    result_pd["size"] = result_pd["size"].astype("int64")
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    pd.testing.assert_frame_equal(result_pd, expected)
+    result = result.cast({"size": ns.Int64()})
+    compare_dataframe_with_reference(result, expected, dtype=ns.Int64)
```

### Comparing `dataframe_api_compat-0.2.6/tests/integration/persistedness_test.py` & `dataframe_api_compat-0.2.7/tests/integration/persistedness_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import pandas as pd
 import pytest
 
-from tests.utils import convert_dataframe_to_pandas_numpy
+from tests.utils import BaseHandler
+from tests.utils import compare_dataframe_with_reference
 from tests.utils import integer_dataframe_1
 from tests.utils import integer_dataframe_2
-from tests.utils import interchange_to_pandas
 
 
-def test_within_df_propagation(library: str) -> None:
+def test_within_df_propagation(library: BaseHandler) -> None:
     df1 = integer_dataframe_1(library)
-    df1 = df1
     df1 = df1 + 1
     with pytest.raises(RuntimeError):
         _ = int(df1.col("a").get_value(0))  # type: ignore[call-overload]
 
     df1 = integer_dataframe_1(library)
     df1 = df1.persist()
     df1 = df1 + 1
@@ -45,39 +43,45 @@
     # ...but not if you modify the scalar
     df1 = integer_dataframe_1(library)
     df1 = df1 + 1
     scalar = df1.col("a").get_value(0).persist()
     assert int(scalar + 1) == 3  # type: ignore[call-overload]
 
 
-def test_within_df_within_col_propagation(library: str) -> None:
+def test_within_df_within_col_propagation(library: BaseHandler) -> None:
     df1 = integer_dataframe_1(library)
     df1 = df1 + 1
     df1 = df1.persist()
     assert int((df1.col("a") + 1).mean()) == 4  # type: ignore[call-overload]
 
 
-def test_cross_df_propagation(library: str) -> None:
+def test_cross_df_propagation(library: BaseHandler) -> None:
     df1 = integer_dataframe_1(library)
     df2 = integer_dataframe_2(library)
-    df1 = (df1 + 1).persist()
-    df2 = df2.rename({"b": "c"}).persist()
+    ns = df1.__dataframe_namespace__()
+    df1 = df1 + 1
+    df2 = df2.rename({"b": "c"})
     result = df1.join(df2, how="left", left_on="a", right_on="a")
-    result_pd = convert_dataframe_to_pandas_numpy(interchange_to_pandas(result))
-    expected = pd.DataFrame(
-        {
-            "a": [2, 3, 4],
-            "b": [5, 6, 7],
-            "c": [2.0, float("nan"), 6.0],
-        },
-    )
-    pd.testing.assert_frame_equal(result_pd, expected)
+    ns = result.__dataframe_namespace__()
+    expected = {
+        "a": [2, 3, 4],
+        "b": [5, 6, 7],
+        "c": [2.0, float("nan"), 6.0],
+    }
+    expected_dtype = {
+        "a": ns.Int64,
+        "b": ns.Int64,
+        "c": ns.Int64
+        if library.name in ["pandas-nullable", "polars-lazy"]
+        else ns.Float64,
+    }
+    compare_dataframe_with_reference(result, expected, dtype=expected_dtype)  # type: ignore[arg-type]
 
 
-def test_multiple_propagations(library: str) -> None:
+def test_multiple_propagations(library: BaseHandler) -> None:
     # This is a bit "ugly", as the user is "required" to call `persist`
     # multiple times to do things optimally
     df = integer_dataframe_1(library)
     df = df.persist()
     with pytest.warns(UserWarning):
         df1 = df.filter(df.col("a") > 1).persist()
         df2 = df.filter(df.col("a") <= 1).persist()
@@ -92,15 +96,15 @@
 
     df1 = df1 + 1
     # without this persist, `df1 + 1` will be computed twice
     int(df1.col("a").mean())  # type: ignore[call-overload]
     int(df1.col("a").mean())  # type: ignore[call-overload]
 
 
-def test_parent_propagations(library: str) -> None:
+def test_parent_propagations(library: BaseHandler) -> None:
     # Set up something like this:
     #
     #         df
     #     df1    df2
     #
     # If I persist df1, then that triggers df.
     # If I then want call some scalar on df2, that will have to trigger
```

### Comparing `dataframe_api_compat-0.2.6/tests/integration/upstream_test.py` & `dataframe_api_compat-0.2.7/tests/integration/upstream_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 import sys
 
 import pytest
+from packaging.version import Version
+from packaging.version import parse
 
 
 class TestPolars:
     def test_dataframe(self) -> None:
-        import polars as pl
+        pl = pytest.importorskip("polars")
 
-        if tuple(int(v) for v in pl.__version__.split(".")) < (
-            0,
-            19,
-            0,
-        ):  # pragma: no cover
+        if parse(pl.__version__) < Version("0.19.0"):  # pragma: no cover
             # before consortium standard in polars
             return
 
         df_pl = pl.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
         df = df_pl.__dataframe_consortium_standard__()
         result = df.get_column_names()
         expected = ["a", "b"]
         assert result == expected
 
     def test_lazyframe(self) -> None:
-        import polars as pl
+        pl = pytest.importorskip("polars")
 
-        if tuple(int(v) for v in pl.__version__.split(".")) < (
-            0,
-            19,
-            0,
-        ):  # pragma: no cover
+        if parse(pl.__version__) < Version("0.19.0"):  # pragma: no cover
             # before consortium standard in polars
             return
 
         df_pl = pl.LazyFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
         df = df_pl.__dataframe_consortium_standard__()
         result = df.get_column_names()
         expected_1 = ["a", "b"]
@@ -53,23 +47,39 @@
         Test some basic methods of the dataframe consortium standard.
 
         Full testing is done at https://github.com/data-apis/dataframe-api-compat,
         this is just to check that the entry point works as expected.
         """
         import pandas as pd
 
-        if tuple(int(v) for v in pd.__version__.split(".")) < (
-            2,
-            1,
-            0,
-        ):  # pragma: no cover
+        if parse(pd.__version__) < Version("2.1.0"):  # pragma: no cover
             # before consortium standard in pandas
             return
 
         df_pd = pd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
         df = df_pd.__dataframe_consortium_standard__()
         result_1 = df.get_column_names()
         expected_1 = ["a", "b"]
         assert result_1 == expected_1
 
+        ser = pd.Series([1, 2, 3], name="a")
+        assert ser.name == "a"
+
+
+class TestModin:
+    def test_pandas(self) -> None:
+        """
+        Test some basic methods of the dataframe consortium standard.
+
+        Full testing is done at https://github.com/data-apis/dataframe-api-compat,
+        this is just to check that the entry point works as expected.
+        """
+        pd = pytest.importorskip("modin.pandas")
+
+        df_pd = pd.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
+        df = df_pd.__dataframe_consortium_standard__()
+        result_1 = df.get_column_names()
+        expected_1 = ["a", "b"]
+        assert result_1 == expected_1
+
         ser = pd.Series([1, 2, 3], name="a")
         assert ser.name == "a"
```

### Comparing `dataframe_api_compat-0.2.6/tests/namespace/column_from_1d_array_test.py` & `dataframe_api_compat-0.2.7/tests/namespace/column_from_1d_array_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,134 +1,124 @@
 from __future__ import annotations
 
 from datetime import date
 from datetime import datetime
 from datetime import timedelta
 
 import numpy as np
-import pandas as pd
 import pytest
 from packaging.version import Version
 
-from tests.utils import PANDAS_VERSION
-from tests.utils import POLARS_VERSION
+from tests.utils import BaseHandler
+from tests.utils import compare_column_with_reference
 from tests.utils import integer_dataframe_1
-from tests.utils import interchange_to_pandas
+from tests.utils import pandas_version
+from tests.utils import polars_version
 
 
 @pytest.mark.parametrize(
-    "pandas_dtype",
+    ("pandas_dtype", "column_dtype"),
     [
-        "float64",
-        "float32",
-        "int64",
-        "int32",
-        "int16",
-        "int8",
-        "uint64",
-        "uint32",
-        "uint16",
-        "uint8",
+        ("float64", "Float64"),
+        ("float32", "Float32"),
+        ("int64", "Int64"),
+        ("int32", "Int32"),
+        ("int16", "Int16"),
+        ("int8", "Int8"),
+        ("uint64", "UInt64"),
+        ("uint32", "UInt32"),
+        ("uint16", "UInt16"),
+        ("uint8", "UInt8"),
     ],
 )
 def test_column_from_1d_array(
-    library: str,
+    library: BaseHandler,
     pandas_dtype: str,
+    column_dtype: str,
 ) -> None:
     ser = integer_dataframe_1(library).col("a").persist()
-    namespace = ser.__column_namespace__()
+    ns = ser.__column_namespace__()
     arr = np.array([1, 2, 3], dtype=pandas_dtype)
-    result = namespace.dataframe_from_columns(
-        namespace.column_from_1d_array(  # type: ignore[call-arg]
+    result = ns.dataframe_from_columns(
+        ns.column_from_1d_array(  # type: ignore[call-arg]
             arr,
             name="result",
         ),
     )
-    result_pd = interchange_to_pandas(result)["result"]
-    expected = pd.Series([1, 2, 3], name="result", dtype=pandas_dtype)
-    pd.testing.assert_series_equal(result_pd, expected)
+    expected = [1, 2, 3]
+    compare_column_with_reference(
+        result.col("result"),
+        expected,
+        dtype=getattr(ns, column_dtype),
+    )
 
 
 def test_column_from_1d_array_string(
-    library: str,
+    library: BaseHandler,
 ) -> None:
     ser = integer_dataframe_1(library).persist().col("a")
-    namespace = ser.__column_namespace__()
+    ns = ser.__column_namespace__()
     arr = np.array(["a", "b", "c"])
-    result = namespace.dataframe_from_columns(
-        namespace.column_from_1d_array(  # type: ignore[call-arg]
+    result = ns.dataframe_from_columns(
+        ns.column_from_1d_array(  # type: ignore[call-arg]
             arr,
             name="result",
         ),
     )
-    result_pd = interchange_to_pandas(result)["result"]
-    expected = pd.Series(["a", "b", "c"], name="result", dtype="object")
-    pd.testing.assert_series_equal(result_pd, expected)
+    expected = ["a", "b", "c"]
+    compare_column_with_reference(result.col("result"), expected, dtype=ns.String)
 
 
 def test_column_from_1d_array_bool(
-    library: str,
+    library: BaseHandler,
 ) -> None:
     ser = integer_dataframe_1(library).persist().col("a")
-    namespace = ser.__column_namespace__()
+    ns = ser.__column_namespace__()
     arr = np.array([True, False, True])
-    result = namespace.dataframe_from_columns(
-        namespace.column_from_1d_array(  # type: ignore[call-arg]
+    result = ns.dataframe_from_columns(
+        ns.column_from_1d_array(  # type: ignore[call-arg]
             arr,
             name="result",
         ),
     )
-    result_pd = interchange_to_pandas(result)["result"]
-    expected = pd.Series([True, False, True], name="result")
-    pd.testing.assert_series_equal(result_pd, expected)
+    expected = [True, False, True]
+    compare_column_with_reference(result.col("result"), expected, dtype=ns.Bool)
 
 
-def test_datetime_from_1d_array(library: str) -> None:
+def test_datetime_from_1d_array(library: BaseHandler) -> None:
     ser = integer_dataframe_1(library).persist().col("a")
-    namespace = ser.__column_namespace__()
+    ns = ser.__column_namespace__()
     arr = np.array([date(2020, 1, 1), date(2020, 1, 2)], dtype="datetime64[ms]")
-    result = namespace.dataframe_from_columns(
-        namespace.column_from_1d_array(  # type: ignore[call-arg]
+    result = ns.dataframe_from_columns(
+        ns.column_from_1d_array(  # type: ignore[call-arg]
             arr,
             name="result",
         ),
     )
-    result_pd = interchange_to_pandas(result)["result"]
-    expected = pd.Series(
-        [datetime(2020, 1, 1), datetime(2020, 1, 2)],
-        name="result",
-        dtype="datetime64[ms]",
-    )
-    pd.testing.assert_series_equal(result_pd, expected)
+    expected = [datetime(2020, 1, 1), datetime(2020, 1, 2)]
+    compare_column_with_reference(result.col("result"), expected, dtype=ns.Datetime)
 
 
-@pytest.mark.skipif(
-    Version("0.19.9") > POLARS_VERSION,
-    reason="upstream bug",
-)
-@pytest.mark.skipif(
-    Version("2.0.0") > PANDAS_VERSION,
-    reason="pandas before non-nano",
-)
-def test_duration_from_1d_array(library: str) -> None:
+def test_duration_from_1d_array(library: BaseHandler) -> None:
+    if library.name in ("pandas-numpy", "pandas-nullable") and pandas_version() < Version(
+        "2.0.0",
+    ):  # pragma: no cover
+        pytest.skip(reason="pandas before non-nano")
+    if library.name == "polars-lazy" and polars_version() < Version(
+        "0.19.9",
+    ):  # pragma: no cover
+        pytest.skip(reason="upstream bug")
+
     ser = integer_dataframe_1(library).persist().col("a")
-    namespace = ser.__column_namespace__()
+    ns = ser.__column_namespace__()
     arr = np.array([timedelta(1), timedelta(2)], dtype="timedelta64[ms]")
-    result = namespace.dataframe_from_columns(
-        namespace.column_from_1d_array(  # type: ignore[call-arg]
+    result = ns.dataframe_from_columns(
+        ns.column_from_1d_array(  # type: ignore[call-arg]
             arr,
             name="result",
         ),
     )
-    if library == "polars-lazy":
+    if library.name == "polars-lazy":
         # https://github.com/data-apis/dataframe-api/issues/329
-        result_pd = (
-            result.dataframe.collect().to_pandas()["result"].astype("timedelta64[ms]")  # type: ignore[attr-defined]
-        )
-    else:
-        result_pd = result.dataframe["result"]  # type: ignore[index]
-    expected = pd.Series(
-        [timedelta(1), timedelta(2)],
-        name="result",
-        dtype="timedelta64[ms]",
-    )
-    pd.testing.assert_series_equal(result_pd, expected)
+        result = result.cast({"result": ns.Duration("ms")})
+    expected = [timedelta(1), timedelta(2)]
+    compare_column_with_reference(result.col("result"), expected, dtype=ns.Duration)
```

### Comparing `dataframe_api_compat-0.2.6/tests/namespace/concat_test.py` & `dataframe_api_compat-0.2.7/tests/namespace/concat_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from __future__ import annotations
 
-import pandas as pd
-import polars as pl
+from typing import Any
+
 import pytest
 
-from tests.utils import convert_dataframe_to_pandas_numpy
+from tests.utils import BaseHandler
+from tests.utils import compare_dataframe_with_reference
 from tests.utils import integer_dataframe_1
 from tests.utils import integer_dataframe_2
 from tests.utils import integer_dataframe_4
-from tests.utils import interchange_to_pandas
 
 
-def test_concat(library: str) -> None:
+def test_concat(library: BaseHandler) -> None:
     df1 = integer_dataframe_1(library)
     df2 = integer_dataframe_2(library)
-    namespace = df1.__dataframe_namespace__()
-    result = namespace.concat([df1, df2])
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected = pd.DataFrame({"a": [1, 2, 3, 1, 2, 4], "b": [4, 5, 6, 4, 2, 6]})
-    pd.testing.assert_frame_equal(result_pd, expected)
+    ns = df1.__dataframe_namespace__()
+    result = ns.concat([df1, df2])
+    expected = {"a": [1, 2, 3, 1, 2, 4], "b": [4, 5, 6, 4, 2, 6]}
+    compare_dataframe_with_reference(result, expected, dtype=ns.Int64)
 
 
-def test_concat_mismatch(library: str) -> None:
+def test_concat_mismatch(library: BaseHandler) -> None:
     df1 = integer_dataframe_1(library).persist()
     df2 = integer_dataframe_4(library).persist()
-    namespace = df1.__dataframe_namespace__()
+    ns = df1.__dataframe_namespace__()
+    exceptions: tuple[Any, ...] = (ValueError,)
+    if library.name == "polars-lazy":
+        import polars as pl
+
+        exceptions = (ValueError, pl.exceptions.ShapeError)
     # TODO check the error
-    with pytest.raises((ValueError, pl.exceptions.ShapeError)):
-        _ = namespace.concat([df1, df2]).persist()
+    with pytest.raises(exceptions):
+        _ = ns.concat([df1, df2]).persist()
```

### Comparing `dataframe_api_compat-0.2.6/tests/namespace/is_dtype_test.py` & `dataframe_api_compat-0.2.7/tests/namespace/is_dtype_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import pytest
 from packaging.version import Version
 
-from tests.utils import PANDAS_VERSION
+from tests.utils import BaseHandler
 from tests.utils import mixed_dataframe_1
+from tests.utils import pandas_version
 
 
 @pytest.mark.parametrize(
     ("dtype", "expected"),
     [
         ("integral", ["a", "b", "c", "d", "e", "f", "g", "h"]),
         ("signed integer", ["a", "b", "c", "d"]),
@@ -16,16 +17,16 @@
         ("floating", ["i", "j"]),
         ("bool", ["k"]),
         ("string", ["l"]),
         (("string", "integral"), ["a", "b", "c", "d", "e", "f", "g", "h", "l"]),
         (("string", "unsigned integer"), ["e", "f", "g", "h", "l"]),
     ],
 )
-@pytest.mark.skipif(
-    Version("2.0.0") > PANDAS_VERSION,
-    reason="before pandas got non-nano support",
-)
-def test_is_dtype(library: str, dtype: str, expected: list[str]) -> None:
+def test_is_dtype(library: BaseHandler, dtype: str, expected: list[str]) -> None:
+    if library.name in ("pandas-numpy", "pandas-nullable") and pandas_version() < Version(
+        "2.0.0",
+    ):  # pragma: no cover
+        pytest.skip(reason="pandas before non-nano")
     df = mixed_dataframe_1(library).persist()
     namespace = df.__dataframe_namespace__()
     result = [i for i in df.column_names if namespace.is_dtype(df.schema[i], dtype)]
     assert result == expected
```

### Comparing `dataframe_api_compat-0.2.6/tests/namespace/namespace_is_null_test.py` & `dataframe_api_compat-0.2.7/tests/namespace/namespace_is_null_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
+from tests.utils import BaseHandler
 from tests.utils import integer_dataframe_1
 from tests.utils import integer_dataframe_2
 
 
-def test_is_null(library: str) -> None:
+def test_is_null(library: BaseHandler) -> None:
     df = integer_dataframe_1(library)
     other = integer_dataframe_2(library)
     # use scalar namespace just for coverage purposes
     namespace = df.col("a").get_value(0).__scalar_namespace__()
     namespace_other = other.__dataframe_namespace__()
     null = namespace.null
     assert namespace_other.is_null(null)
```

### Comparing `dataframe_api_compat-0.2.6/tests/namespace/sorted_indices_test.py` & `dataframe_api_compat-0.2.7/tests/namespace/sorted_indices_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,53 @@
 from __future__ import annotations
 
-import pandas as pd
-
-from tests.utils import convert_dataframe_to_pandas_numpy
+from tests.utils import BaseHandler
+from tests.utils import compare_dataframe_with_reference
 from tests.utils import integer_dataframe_6
-from tests.utils import interchange_to_pandas
 
 
-def test_column_sorted_indices_ascending(library: str) -> None:
+def test_column_sorted_indices_ascending(library: BaseHandler) -> None:
     df = integer_dataframe_6(library)
+    ns = df.__dataframe_namespace__()
     sorted_indices = df.col("b").sorted_indices()
     result = df.assign(sorted_indices.rename("result"))
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected_1 = pd.DataFrame(
-        {
-            "a": [1, 1, 1, 2, 2],
-            "b": [4, 4, 3, 1, 2],
-            "result": [3, 4, 2, 0, 1],
-        },
-    )
-    expected_2 = pd.DataFrame(
-        {
-            "a": [1, 1, 1, 2, 2],
-            "b": [4, 4, 3, 1, 2],
-            "result": [3, 4, 2, 1, 0],
-        },
-    )
-    if library in ("polars", "polars-lazy"):
-        result_pd["result"] = result_pd["result"].astype("int64")
+    expected_1 = {
+        "a": [1, 1, 1, 2, 2],
+        "b": [4, 4, 3, 1, 2],
+        "result": [3, 4, 2, 0, 1],
+    }
+    expected_2 = {
+        "a": [1, 1, 1, 2, 2],
+        "b": [4, 4, 3, 1, 2],
+        "result": [3, 4, 2, 1, 0],
+    }
+    if library.name == "polars-lazy":
+        result = result.cast({"result": ns.Int64()})
     try:
-        pd.testing.assert_frame_equal(result_pd, expected_1)
+        compare_dataframe_with_reference(result, expected_1, dtype=ns.Int64)
     except AssertionError:  # pragma: no cover
         # order isn't determinist, so try both
-        pd.testing.assert_frame_equal(result_pd, expected_2)
+        compare_dataframe_with_reference(result, expected_2, dtype=ns.Int64)
 
 
-def test_column_sorted_indices_descending(library: str) -> None:
+def test_column_sorted_indices_descending(library: BaseHandler) -> None:
     df = integer_dataframe_6(library)
+    ns = df.__dataframe_namespace__()
     sorted_indices = df.col("b").sorted_indices(ascending=False)
     result = df.assign(sorted_indices.rename("result"))
-    result_pd = interchange_to_pandas(result)
-    result_pd = convert_dataframe_to_pandas_numpy(result_pd)
-    expected_1 = pd.DataFrame(
-        {
-            "a": [1, 1, 1, 2, 2],
-            "b": [4, 4, 3, 1, 2],
-            "result": [1, 0, 2, 4, 3],
-        },
-    )
-    expected_2 = pd.DataFrame(
-        {
-            "a": [1, 1, 1, 2, 2],
-            "b": [4, 4, 3, 1, 2],
-            "result": [0, 1, 2, 4, 3],
-        },
-    )
-    if library in ("polars", "polars-lazy"):
-        result_pd["result"] = result_pd["result"].astype("int64")
+    expected_1 = {
+        "a": [1, 1, 1, 2, 2],
+        "b": [4, 4, 3, 1, 2],
+        "result": [1, 0, 2, 4, 3],
+    }
+    expected_2 = {
+        "a": [1, 1, 1, 2, 2],
+        "b": [4, 4, 3, 1, 2],
+        "result": [0, 1, 2, 4, 3],
+    }
+    if library.name == "polars-lazy":
+        result = result.cast({"result": ns.Int64()})
     try:
-        pd.testing.assert_frame_equal(result_pd, expected_1)
+        compare_dataframe_with_reference(result, expected_1, dtype=ns.Int64)
     except AssertionError:
         # order isn't determinist, so try both
-        pd.testing.assert_frame_equal(result_pd, expected_2)
+        compare_dataframe_with_reference(result, expected_2, dtype=ns.Int64)
```

### Comparing `dataframe_api_compat-0.2.6/tests/namespace/to_array_object_test.py` & `dataframe_api_compat-0.2.7/tests/namespace/to_array_object_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import numpy as np
 
+from tests.utils import BaseHandler
 from tests.utils import integer_dataframe_1
 
 
-def test_to_array_object(library: str) -> None:
+def test_to_array_object(library: BaseHandler) -> None:
     df = integer_dataframe_1(library).persist()
     result = np.asarray(df.to_array(dtype="int64"))  # type: ignore  # noqa: PGH003
     expected = np.array([[1, 4], [2, 5], [3, 6]], dtype=np.int64)
     np.testing.assert_array_equal(result, expected)
 
 
-def test_column_to_array_object(library: str) -> None:
+def test_column_to_array_object(library: BaseHandler) -> None:
     col = integer_dataframe_1(library).col("a")
     result = np.asarray(col.persist().to_array())
     result = np.asarray(col.persist().to_array())
     expected = np.array([1, 2, 3], dtype=np.int64)
     np.testing.assert_array_equal(result, expected)
```

### Comparing `dataframe_api_compat-0.2.6/tests/scalars/float_test.py` & `dataframe_api_compat-0.2.7/tests/scalars/float_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
-import pandas as pd
 import pytest
 
+from tests.utils import BaseHandler
+from tests.utils import compare_dataframe_with_reference
 from tests.utils import integer_dataframe_1
 from tests.utils import integer_dataframe_2
-from tests.utils import interchange_to_pandas
 
 
 @pytest.mark.parametrize(
     "attr",
     [
         "__lt__",
         "__le__",
@@ -28,45 +28,45 @@
         "__rpow__",
         "__floordiv__",
         "__rfloordiv__",
         "__truediv__",
         "__rtruediv__",
     ],
 )
-def test_float_binary(library: str, attr: str) -> None:
+def test_float_binary(library: BaseHandler, attr: str) -> None:
     other = 0.5
     df = integer_dataframe_2(library).persist()
     scalar = df.col("a").mean()
     float_scalar = float(scalar)  # type: ignore[arg-type]
     assert getattr(scalar, attr)(other) == getattr(float_scalar, attr)(other)
 
 
-def test_float_binary_invalid(library: str) -> None:
+def test_float_binary_invalid(library: BaseHandler) -> None:
     lhs = integer_dataframe_2(library).col("a").mean()
     rhs = integer_dataframe_1(library).col("b").mean()
     with pytest.raises(ValueError):
         _ = lhs > rhs
 
 
-def test_float_binary_lazy_valid(library: str) -> None:
+def test_float_binary_lazy_valid(library: BaseHandler) -> None:
     df = integer_dataframe_2(library).persist()
     lhs = df.col("a").mean()
     rhs = df.col("b").mean()
     result = lhs > rhs
     assert not bool(result)
 
 
 @pytest.mark.parametrize(
     "attr",
     [
         "__abs__",
         "__neg__",
     ],
 )
-def test_float_unary(library: str, attr: str) -> None:
+def test_float_unary(library: BaseHandler, attr: str) -> None:
     df = integer_dataframe_2(library).persist()
     with pytest.warns(UserWarning):
         scalar = df.col("a").persist().mean()
     float_scalar = float(scalar)  # type: ignore[arg-type]
     assert getattr(scalar, attr)() == getattr(float_scalar, attr)()
 
 
@@ -74,40 +74,38 @@
     "attr",
     [
         "__int__",
         "__float__",
         "__bool__",
     ],
 )
-def test_float_unary_invalid(library: str, attr: str) -> None:
+def test_float_unary_invalid(library: BaseHandler, attr: str) -> None:
     df = integer_dataframe_2(library)
     scalar = df.col("a").mean()
     float_scalar = float(scalar.persist())  # type: ignore[arg-type]
     with pytest.raises(RuntimeError):
         assert getattr(scalar, attr)() == getattr(float_scalar, attr)()
 
 
-def test_free_standing(library: str) -> None:
+def test_free_standing(library: BaseHandler) -> None:
     df = integer_dataframe_1(library)
     namespace = df.__dataframe_namespace__()
     ser = namespace.column_from_1d_array(  # type: ignore[call-arg]
         np.array([1, 2, 3]),
         name="a",
     )
     result = float(ser.mean() + 1)  # type: ignore[arg-type]
     assert result == 3.0
 
 
-def test_right_comparand(library: str) -> None:
+def test_right_comparand(library: BaseHandler) -> None:
     df = integer_dataframe_1(library)
+    ns = df.__dataframe_namespace__()
     col = df.col("a")  # [1, 2, 3]
     scalar = df.col("b").get_value(0)  # 4
     result = df.assign((scalar - col).rename("c"))
-    result_pd = interchange_to_pandas(result)
-    expected = pd.DataFrame(
-        {
-            "a": [1, 2, 3],
-            "b": [4, 5, 6],
-            "c": [3, 2, 1],
-        },
-    )
-    pd.testing.assert_frame_equal(result_pd, expected)
+    expected = {
+        "a": [1, 2, 3],
+        "b": [4, 5, 6],
+        "c": [3, 2, 1],
+    }
+    compare_dataframe_with_reference(result, expected, ns.Int64)
```

### Comparing `dataframe_api_compat-0.2.6/utils/bump_version.py` & `dataframe_api_compat-0.2.7/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/utils/generate_random_versions.py` & `dataframe_api_compat-0.2.7/utils/generate_random_versions.py`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/utils/pandas_versions.txt` & `dataframe_api_compat-0.2.7/utils/pandas_versions.txt`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/utils/polars_versions.txt` & `dataframe_api_compat-0.2.7/utils/polars_versions.txt`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/LICENSE` & `dataframe_api_compat-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dataframe_api_compat-0.2.6/README.md` & `dataframe_api_compat-0.2.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 [![Build Status](https://github.com/data-apis/dataframe-api-compat/workflows/tox/badge.svg)](https://github.com/data-apis/dataframe-api-compat/actions?workflow=tox)
 [![Coverage](https://codecov.io/gh/MarcoGorelli/cython-lint/branch/main/graph/badge.svg)](https://codecov.io/gh/data-apis/dataframe-api-compat)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/MarcoGorelli/dataframe-api-compat/main.svg)](https://results.pre-commit.ci/latest/github/MarcoGorelli/dataframe-api-compat/main)
 
 # Dataframe API Compat
 
-Extremely lightweight compatibility layer between pandas and Polars:
+Extremely lightweight compatibility layer between pandas, Polars, Modin and any other project which implements the [Python Dataframe API Standard](https://data-apis.org/dataframe-api/).
 
 - ✅ No dependencies.
-- ✅ Lightweight: wheel is smaller than 30 kB.
+- ✅ Lightweight: wheel is smaller than 50 kB.
 - ✅ Simple, minimal, and predictable.
 
-No need to choose - support both with ease!
-
 Documentation, including installation instructions and tutorial, are here: https://data-apis.org/dataframe-api-compat.
```

### Comparing `dataframe_api_compat-0.2.6/pyproject.toml` & `dataframe_api_compat-0.2.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dataframe_api_compat"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Implementation of the DataFrame Standard for pandas and Polars"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -71,18 +71,28 @@
   'TD',
   'TRY004'
 ]
 
 [tool.ruff.isort]
 force-single-line = true
 
+[tool.black]
+line-length = 90
+
 [tool.pytest.ini_options]
 filterwarnings = [
   "error",
   'ignore:distutils Version classes are deprecated:DeprecationWarning',
+  # modin specific
+  'ignore:.*pkg_resources:DeprecationWarning',
+  'ignore:Ray execution environment not yet initialized:UserWarning',
+  "ignore:Distributing <class '.*'> object.:UserWarning",
+  'ignore:.*ray:ResourceWarning',
+  'ignore:.*is not currently supported by PandasOnRay:UserWarning',
+  'ignore:.*implementation has mismatches with pandas:UserWarning',
 ]
 xfail_strict = true
 
 [tool.coverage.run]
 plugins = ["covdefaults"]
 
 [tool.coverage.report]
```

### Comparing `dataframe_api_compat-0.2.6/PKG-INFO` & `dataframe_api_compat-0.2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dataframe_api_compat
-Version: 0.2.6
+Version: 0.2.7
 Summary: Implementation of the DataFrame Standard for pandas and Polars
 Project-URL: Homepage, https://github.com/data-apis/dataframe-api-compat
 Project-URL: Bug Tracker, https://github.com/data-apis/dataframe-api-compat
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,16 +15,14 @@
 
 [![Build Status](https://github.com/data-apis/dataframe-api-compat/workflows/tox/badge.svg)](https://github.com/data-apis/dataframe-api-compat/actions?workflow=tox)
 [![Coverage](https://codecov.io/gh/MarcoGorelli/cython-lint/branch/main/graph/badge.svg)](https://codecov.io/gh/data-apis/dataframe-api-compat)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/MarcoGorelli/dataframe-api-compat/main.svg)](https://results.pre-commit.ci/latest/github/MarcoGorelli/dataframe-api-compat/main)
 
 # Dataframe API Compat
 
-Extremely lightweight compatibility layer between pandas and Polars:
+Extremely lightweight compatibility layer between pandas, Polars, Modin and any other project which implements the [Python Dataframe API Standard](https://data-apis.org/dataframe-api/).
 
 - ✅ No dependencies.
-- ✅ Lightweight: wheel is smaller than 30 kB.
+- ✅ Lightweight: wheel is smaller than 50 kB.
 - ✅ Simple, minimal, and predictable.
 
-No need to choose - support both with ease!
-
 Documentation, including installation instructions and tutorial, are here: https://data-apis.org/dataframe-api-compat.
```

