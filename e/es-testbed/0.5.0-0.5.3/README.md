# Comparing `tmp/es_testbed-0.5.0.tar.gz` & `tmp/es_testbed-0.5.3.tar.gz`

## Comparing `es_testbed-0.5.0.tar` & `es_testbed-0.5.3.tar`

### file list

```diff
@@ -1,124 +1,123 @@
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 es_testbed-0.5.0/pytest.ini
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/.gitignore
--rw-r--r--   0        0        0    38627 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/class_index.html
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/coverage_html.js
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_17bd492d087794b9___init___py.html
--rw-r--r--   0        0        0    15958 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_17bd492d087794b9_test_cls_ilm_py.html
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_17bd492d087794b9_test_cls_tracker_py.html
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_17bd492d087794b9_test_defaults_py.html
--rw-r--r--   0        0        0    42035 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_17bd492d087794b9_test_utils_py.html
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20___init___py.html
--rw-r--r--   0        0        0    23419 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20_args_py.html
--rw-r--r--   0        0        0    28433 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20_base_py.html
--rw-r--r--   0        0        0    68567 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20_ilm_py.html
--rw-r--r--   0        0        0    54039 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20_plan_py.html
--rw-r--r--   0        0        0    47154 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20_testplan_py.html
--rw-r--r--   0        0        0    19157 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20_tracker_py.html
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_72ef0405fdf841ab___init___py.html
--rw-r--r--   0        0        0    30376 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_72ef0405fdf841ab_config_py.html
--rw-r--r--   0        0        0   136101 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_72ef0405fdf841ab_es_api_py.html
--rw-r--r--   0        0        0    62980 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_72ef0405fdf841ab_utils_py.html
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_9e00aab3b961c475___init___py.html
--rw-r--r--   0        0        0    16252 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_9e00aab3b961c475_alias_py.html
--rw-r--r--   0        0        0    14137 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_9e00aab3b961c475_data_stream_py.html
--rw-r--r--   0        0        0    15073 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_9e00aab3b961c475_entity_py.html
--rw-r--r--   0        0        0    51367 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_9e00aab3b961c475_index_py.html
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_a40f6d277e0496df___init___py.html
--rw-r--r--   0        0        0    21647 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_basic_data_streams_py.html
--rw-r--r--   0        0        0    22256 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_basic_frozen_py.html
--rw-r--r--   0        0        0    23130 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_basic_indices_py.html
--rw-r--r--   0        0        0    23441 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_basic_rollover_py.html
--rw-r--r--   0        0        0    24175 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_cold_ds_py.html
--rw-r--r--   0        0        0    26080 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_cold_indices_py.html
--rw-r--r--   0        0        0    24187 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_frozen_ds_py.html
--rw-r--r--   0        0        0    25949 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_frozen_indices_py.html
--rw-r--r--   0        0        0    24387 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_rollover_frozen_py.html
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0    27321 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_a44f0ac069e85531_conftest_py.html
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902___init___py.html
--rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_componentmgr_py.html
--rw-r--r--   0        0        0    29730 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_data_streammgr_py.html
--rw-r--r--   0        0        0    54006 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_entitymgr_py.html
--rw-r--r--   0        0        0    20808 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_ilmmgr_py.html
--rw-r--r--   0        0        0    45506 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_indexmgr_py.html
--rw-r--r--   0        0        0    22746 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_snapshotmgr_py.html
--rw-r--r--   0        0        0    21276 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_templatemgr_py.html
--rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_f43263c25e31810d___init___py.html
--rw-r--r--   0        0        0    37655 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_f43263c25e31810d_defaults_py.html
--rw-r--r--   0        0        0    13071 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_f43263c25e31810d_exceptions_py.html
--rw-r--r--   0        0        0    57008 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_f43263c25e31810d_testbed_creator_py.html
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/d_f43263c25e31810d_version_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/favicon_32.png
--rw-r--r--   0        0        0   126290 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/function_index.html
--rw-r--r--   0        0        0    21307 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/keybd_open.png
--rw-r--r--   0        0        0    11597 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/status.json
--rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/style.css
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_17bd492d087794b9___init___py.html
--rw-r--r--   0        0        0    25098 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_17bd492d087794b9_test_cls_ilm_py.html
--rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_17bd492d087794b9_test_cls_tracker_py.html
--rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_17bd492d087794b9_test_defaults_py.html
--rw-r--r--   0        0        0    31639 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_17bd492d087794b9_test_utils_py.html
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_396c7038a91d0266___init___py.html
--rw-r--r--   0        0        0    19689 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_396c7038a91d0266_componentmgr_py.html
--rw-r--r--   0        0        0    30906 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_396c7038a91d0266_data_streammgr_py.html
--rw-r--r--   0        0        0    47374 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_396c7038a91d0266_entitymgr_py.html
--rw-r--r--   0        0        0    22588 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_396c7038a91d0266_ilmmgr_py.html
--rw-r--r--   0        0        0    44234 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_396c7038a91d0266_indexmgr_py.html
--rw-r--r--   0        0        0    21132 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_396c7038a91d0266_snapshotmgr_py.html
--rw-r--r--   0        0        0    21787 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_396c7038a91d0266_templatemgr_py.html
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_549446c4d0fe5c90___init___py.html
--rw-r--r--   0        0        0   135505 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_549446c4d0fe5c90_es_api_py.html
--rw-r--r--   0        0        0    63456 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_549446c4d0fe5c90_utils_py.html
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_6c086c3223cbe98b___init___py.html
--rw-r--r--   0        0        0    23267 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_6c086c3223cbe98b_args_py.html
--rw-r--r--   0        0        0    20211 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_6c086c3223cbe98b_base_py.html
--rw-r--r--   0        0        0    86740 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_6c086c3223cbe98b_ilm_py.html
--rw-r--r--   0        0        0    46898 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_6c086c3223cbe98b_testplan_py.html
--rw-r--r--   0        0        0    26560 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_6c086c3223cbe98b_tracker_py.html
--rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_712229651729ba66___init___py.html
--rw-r--r--   0        0        0    16100 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_712229651729ba66_alias_py.html
--rw-r--r--   0        0        0    13985 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_712229651729ba66_data_stream_py.html
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_712229651729ba66_entity_py.html
--rw-r--r--   0        0        0    50130 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_712229651729ba66_index_py.html
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_95d9102b3aa62d65___init___py.html
--rw-r--r--   0        0        0    36249 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_95d9102b3aa62d65_defaults_py.html
--rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_95d9102b3aa62d65_exceptions_py.html
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_95d9102b3aa62d65_version_py.html
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_a40f6d277e0496df___init___py.html
--rw-r--r--   0        0        0    21360 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_a40f6d277e0496df_test_basic_data_streams_py.html
--rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_a40f6d277e0496df_test_basic_indices_py.html
--rw-r--r--   0        0        0    23263 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_a40f6d277e0496df_test_testbed_py.html
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_a44f0ac069e85531___init___py.html
--rw-r--r--   0        0        0    15373 2020-02-02 00:00:00.000000 es_testbed-0.5.0/cov_html/z_a44f0ac069e85531_conftest_py.html
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/__init__.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/defaults.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/exceptions.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/version.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/__init__.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/base.py
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/ilm.py
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/plan.py
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/tracker.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entities/__init__.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entities/alias.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entities/data_stream.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entities/entity.py
--rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entities/index.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/__init__.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/componentmgr.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/data_streammgr.py
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/entitymgr.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/ilmmgr.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/indexmgr.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/snapshotmgr.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/templatemgr.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/helpers/__init__.py
--rw-r--r--   0        0        0    15204 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/helpers/es_api.py
--rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 es_testbed-0.5.0/src/es_testbed/helpers/utils.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 es_testbed-0.5.0/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_testbed-0.5.0/LICENSE
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 es_testbed-0.5.0/README.md
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 es_testbed-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 es_testbed-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 es_testbed-0.5.3/pytest.ini
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/.gitignore
+-rw-r--r--   0        0        0    38627 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/class_index.html
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/coverage_html.js
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_17bd492d087794b9___init___py.html
+-rw-r--r--   0        0        0    15958 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_17bd492d087794b9_test_cls_ilm_py.html
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_17bd492d087794b9_test_cls_tracker_py.html
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_17bd492d087794b9_test_defaults_py.html
+-rw-r--r--   0        0        0    42035 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_17bd492d087794b9_test_utils_py.html
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20___init___py.html
+-rw-r--r--   0        0        0    23419 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20_args_py.html
+-rw-r--r--   0        0        0    28433 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20_base_py.html
+-rw-r--r--   0        0        0    68567 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20_ilm_py.html
+-rw-r--r--   0        0        0    54039 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20_plan_py.html
+-rw-r--r--   0        0        0    47154 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20_testplan_py.html
+-rw-r--r--   0        0        0    19157 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20_tracker_py.html
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_72ef0405fdf841ab___init___py.html
+-rw-r--r--   0        0        0    30376 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_72ef0405fdf841ab_config_py.html
+-rw-r--r--   0        0        0   136119 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_72ef0405fdf841ab_es_api_py.html
+-rw-r--r--   0        0        0    62980 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_72ef0405fdf841ab_utils_py.html
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_9e00aab3b961c475___init___py.html
+-rw-r--r--   0        0        0    16252 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_9e00aab3b961c475_alias_py.html
+-rw-r--r--   0        0        0    14137 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_9e00aab3b961c475_data_stream_py.html
+-rw-r--r--   0        0        0    15073 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_9e00aab3b961c475_entity_py.html
+-rw-r--r--   0        0        0    51367 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_9e00aab3b961c475_index_py.html
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_a40f6d277e0496df___init___py.html
+-rw-r--r--   0        0        0    21647 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_basic_data_streams_py.html
+-rw-r--r--   0        0        0    22256 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_basic_frozen_py.html
+-rw-r--r--   0        0        0    23130 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_basic_indices_py.html
+-rw-r--r--   0        0        0    23441 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_basic_rollover_py.html
+-rw-r--r--   0        0        0    24175 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_cold_ds_py.html
+-rw-r--r--   0        0        0    26080 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_cold_indices_py.html
+-rw-r--r--   0        0        0    24187 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_frozen_ds_py.html
+-rw-r--r--   0        0        0    25949 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_frozen_indices_py.html
+-rw-r--r--   0        0        0    24387 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_rollover_frozen_py.html
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    27321 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_a44f0ac069e85531_conftest_py.html
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902___init___py.html
+-rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_componentmgr_py.html
+-rw-r--r--   0        0        0    29730 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_data_streammgr_py.html
+-rw-r--r--   0        0        0    54006 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_entitymgr_py.html
+-rw-r--r--   0        0        0    20808 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_ilmmgr_py.html
+-rw-r--r--   0        0        0    45506 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_indexmgr_py.html
+-rw-r--r--   0        0        0    22746 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_snapshotmgr_py.html
+-rw-r--r--   0        0        0    21276 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_templatemgr_py.html
+-rw-r--r--   0        0        0     5695 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_f43263c25e31810d___init___py.html
+-rw-r--r--   0        0        0    37655 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_f43263c25e31810d_defaults_py.html
+-rw-r--r--   0        0        0    13071 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_f43263c25e31810d_exceptions_py.html
+-rw-r--r--   0        0        0    57008 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_f43263c25e31810d_testbed_creator_py.html
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/d_f43263c25e31810d_version_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/favicon_32.png
+-rw-r--r--   0        0        0   126290 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/function_index.html
+-rw-r--r--   0        0        0    21307 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/keybd_open.png
+-rw-r--r--   0        0        0    11597 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/status.json
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/style.css
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_17bd492d087794b9___init___py.html
+-rw-r--r--   0        0        0    25098 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_17bd492d087794b9_test_cls_ilm_py.html
+-rw-r--r--   0        0        0     5953 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_17bd492d087794b9_test_cls_tracker_py.html
+-rw-r--r--   0        0        0    11768 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_17bd492d087794b9_test_defaults_py.html
+-rw-r--r--   0        0        0    31639 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_17bd492d087794b9_test_utils_py.html
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_396c7038a91d0266___init___py.html
+-rw-r--r--   0        0        0    19689 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_396c7038a91d0266_componentmgr_py.html
+-rw-r--r--   0        0        0    30906 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_396c7038a91d0266_data_streammgr_py.html
+-rw-r--r--   0        0        0    47374 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_396c7038a91d0266_entitymgr_py.html
+-rw-r--r--   0        0        0    22588 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_396c7038a91d0266_ilmmgr_py.html
+-rw-r--r--   0        0        0    44234 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_396c7038a91d0266_indexmgr_py.html
+-rw-r--r--   0        0        0    21132 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_396c7038a91d0266_snapshotmgr_py.html
+-rw-r--r--   0        0        0    21787 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_396c7038a91d0266_templatemgr_py.html
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_549446c4d0fe5c90___init___py.html
+-rw-r--r--   0        0        0   135505 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_549446c4d0fe5c90_es_api_py.html
+-rw-r--r--   0        0        0    63456 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_549446c4d0fe5c90_utils_py.html
+-rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_6c086c3223cbe98b___init___py.html
+-rw-r--r--   0        0        0    23267 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_6c086c3223cbe98b_args_py.html
+-rw-r--r--   0        0        0    20211 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_6c086c3223cbe98b_base_py.html
+-rw-r--r--   0        0        0    86740 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_6c086c3223cbe98b_ilm_py.html
+-rw-r--r--   0        0        0    46898 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_6c086c3223cbe98b_testplan_py.html
+-rw-r--r--   0        0        0    26560 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_6c086c3223cbe98b_tracker_py.html
+-rw-r--r--   0        0        0     6038 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_712229651729ba66___init___py.html
+-rw-r--r--   0        0        0    16100 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_712229651729ba66_alias_py.html
+-rw-r--r--   0        0        0    13985 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_712229651729ba66_data_stream_py.html
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_712229651729ba66_entity_py.html
+-rw-r--r--   0        0        0    50130 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_712229651729ba66_index_py.html
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_95d9102b3aa62d65___init___py.html
+-rw-r--r--   0        0        0    36249 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_95d9102b3aa62d65_defaults_py.html
+-rw-r--r--   0        0        0    12919 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_95d9102b3aa62d65_exceptions_py.html
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_95d9102b3aa62d65_version_py.html
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_a40f6d277e0496df___init___py.html
+-rw-r--r--   0        0        0    21360 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_a40f6d277e0496df_test_basic_data_streams_py.html
+-rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_a40f6d277e0496df_test_basic_indices_py.html
+-rw-r--r--   0        0        0    23263 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_a40f6d277e0496df_test_testbed_py.html
+-rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    15373 2020-02-02 00:00:00.000000 es_testbed-0.5.3/cov_html/z_a44f0ac069e85531_conftest_py.html
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/__init__.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/defaults.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/exceptions.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/__init__.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/base.py
+-rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/ilm.py
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/plan.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/tracker.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entities/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entities/alias.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entities/data_stream.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entities/entity.py
+-rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entities/index.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/__init__.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/componentmgr.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/data_streammgr.py
+-rw-r--r--   0        0        0     5609 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/entitymgr.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/ilmmgr.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/indexmgr.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/snapshotmgr.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/templatemgr.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/helpers/__init__.py
+-rw-r--r--   0        0        0    15320 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/helpers/es_api.py
+-rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 es_testbed-0.5.3/src/es_testbed/helpers/utils.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 es_testbed-0.5.3/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_testbed-0.5.3/LICENSE
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 es_testbed-0.5.3/README.md
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 es_testbed-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 es_testbed-0.5.3/PKG-INFO
```

### Comparing `es_testbed-0.5.0/cov_html/class_index.html` & `es_testbed-0.5.3/cov_html/class_index.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/coverage_html.js` & `es_testbed-0.5.3/cov_html/coverage_html.js`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/d_17bd492d087794b9___init___py.html` & `es_testbed-0.5.3/cov_html/d_17bd492d087794b9___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_rollover_frozen_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_17bd492d087794b9_test_cls_ilm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -87,13 +87,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_rollover_frozen_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_17bd492d087794b9_test_cls_ilm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_17bd492d087794b9_test_cls_ilm_py.html` & `es_testbed-0.5.3/cov_html/d_17bd492d087794b9_test_cls_ilm_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_17bd492d087794b9___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_17bd492d087794b9_test_cls_tracker_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -148,13 +148,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_17bd492d087794b9___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_17bd492d087794b9_test_cls_tracker_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Test functions in es_testbed.defaults""" 
 _2# pylint: disable=missing-function-docstring,redefined-outer-name 
 _3# import pytest 
 _4# from es_testbed.defaults import TESTPLAN 
 _5 
 _6 
 _7# @pytest.fixture 
@@ -71,8 +71,8 @@
 _5_6 
 _5_7# def test_cls_ilm_cold(ilm, hot, cold): 
 _5_8# expected = {'phases': {'hot': hot, 'cold': cold}} 
 _5_9# ilm.tiers = ['hot', 'cold'] 
 _6_0# ilm.repository = 'repo' 
 _6_1# assert ilm.policy['phases'].keys() == expected['phases'].keys() 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_17bd492d087794b9_test_cls_tracker_py.html` & `es_testbed-0.5.3/cov_html/d_17bd492d087794b9_test_cls_tracker_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_17bd492d087794b9_test_cls_ilm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_17bd492d087794b9_test_defaults_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -93,13 +93,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_17bd492d087794b9_test_cls_ilm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_17bd492d087794b9_test_defaults_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,16 +6,16 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Test functions in es_testbed.defaults""" 
 _2# pylint: disable=protected-access, import-error 
 _3# add import-error here ^^^ to avoid false-positives for the local import 
 _4# from unittest import TestCase 
 _5# from es_testbed.defaults import NAMEMAPPER 
 _6# from es_testbed.classes.tracker import Tracker 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_17bd492d087794b9_test_defaults_py.html` & `es_testbed-0.5.3/cov_html/d_17bd492d087794b9_test_defaults_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_17bd492d087794b9_test_cls_tracker_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_17bd492d087794b9_test_utils_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -112,13 +112,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_17bd492d087794b9_test_cls_tracker_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_17bd492d087794b9_test_utils_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 1188 ssttaatteemmeennttss ?  1188 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Test functions in es_testbed.defaults""" 
 _2# pylint: disable=missing-function-docstring,redefined-outer-name 
 _3import pytest 
 _4from es_testbed.defaults import ilmcold, ilmwarm, ilm_force_merge, ilm_phase 
 _5 
 _6@pytest.fixture 
 _7def forcemerge(): 
@@ -33,8 +33,8 @@
 _2_0 tier = 'warm' 
 _2_1 assert ilm_phase(tier) == {tier: ilmwarm()} 
 _2_2 
 _2_3def test_default_ilm_cold(): 
 _2_4 tier = 'cold' 
 _2_5 assert ilm_phase(tier) == {tier: ilmcold()} 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_17bd492d087794b9_test_utils_py.html` & `es_testbed-0.5.3/cov_html/d_17bd492d087794b9_test_utils_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_17bd492d087794b9_test_defaults_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -191,13 +191,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_17bd492d087794b9_test_defaults_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 7700 ssttaatteemmeennttss ?  7700 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Test functions in es_testbed.helpers.utils""" 
 _2# pylint: disable=missing-function-docstring,redefined-outer-name 
 _3import typing as t 
 _4import pytest 
 _5from dotmap import DotMap 
 _6from es_testbed import defaults as dft 
 _7from es_testbed import exceptions as ex 
@@ -123,8 +123,8 @@
 _1_0_0 tests = [(doc.message, 'message'), (doc.nested.key, 'nested'),
 (doc.deep.l1.l2.l3, 'deep')] 
 _1_0_1 for test in tests: 
 _1_0_2 dm, val = test 
 _1_0_3 assert dm == fieldmatch(val, i) 
 _1_0_4 i += 1 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20___init___py.html` & `es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_f43263c25e31810d___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5d92fa905a1d3e20_base_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -88,13 +88,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_f43263c25e31810d___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5d92fa905a1d3e20_base_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,11 +7,11 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""__init__""" 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20_args_py.html` & `es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20_args_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20_base_py.html` & `es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20_base_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_5d92fa905a1d3e20___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9e00aab3b961c475___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -156,13 +156,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_5d92fa905a1d3e20___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9e00aab3b961c475___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 4466 ssttaatteemmeennttss ?  3344 rruunn 1122 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Base TestBed Class""" 
 _2import typing as t 
 _3from datetime import datetime, timezone 
 _4from dotmap import DotMap 
 _5from elasticsearch8 import Elasticsearch 
 _6from es_testbed.helpers.es_api import delete 
 _7from es_testbed.helpers.utils import getlogger 
@@ -87,8 +87,8 @@
 (interval=None)) 
 _6_7 self.client.cluster.put_settings(persistent=self.ilm_polling
 (interval=None)) 
 _6_8 end = datetime.now(timezone.utc) 
 _6_9 self.logger.info('Testbed teardown elapsed time: %s', (end -
 start).total_seconds()) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20_ilm_py.html` & `es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20_ilm_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_templatemgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5d92fa905a1d3e20_plan_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -281,13 +281,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_templatemgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5d92fa905a1d3e20_plan_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 112299 ssttaatteemmeennttss ?  9900 rruunn 3399 mmiissssiinngg 00 eexxcclluuddeedd 1111 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""ILM Defining Class""" 
 _2import typing as t 
 _3from os import getenv 
 _4from time import sleep 
 _5from dotmap import DotMap 
 _6from elasticsearch8 import Elasticsearch 
 _7from es_testbed.defaults import PAUSE_ENVVAR, PAUSE_DEFAULT 
@@ -221,8 +221,8 @@
 _1_8_9 raise ResultNotExpected from err 
 _1_9_0 try: 
 _1_9_1 self.update() 
 _1_9_2 except NameChanged as err: 
 _1_9_3 self.logger.debug('Passing along upstream exception...') 
 _1_9_4 raise NameChanged from err 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20_plan_py.html` & `es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20_plan_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_5d92fa905a1d3e20_ilm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5d92fa905a1d3e20_tracker_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -250,13 +250,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_5d92fa905a1d3e20_ilm_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5d92fa905a1d3e20_tracker_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 8833 ssttaatteemmeennttss ?  7766 rruunn 77 mmiissssiinngg 00 eexxcclluuddeedd 99 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""TestPlan Class Definition""" 
 _2import typing as t 
 _3from dotmap import DotMap 
 _4from es_testbed.defaults import TESTPLAN 
 _5from es_testbed.helpers.utils import build_ilm_policy, getlogger, randomstr 
 _6# pylint: disable=missing-docstring 
 _7 
@@ -189,8 +189,8 @@
 _1_5_8 
 _1_5_9 def update_rollover_alias(self) -> None: 
 _1_6_0 if self._plan.rollover_alias: 
 _1_6_1 self._plan.rollover_alias = f'{self._plan.prefix}-idx-{self._plan.uniq}' 
 _1_6_2 else: 
 _1_6_3 self._plan.rollover_alias = None 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20_testplan_py.html` & `es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20_testplan_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/d_5d92fa905a1d3e20_tracker_py.html` & `es_testbed-0.5.3/cov_html/d_5d92fa905a1d3e20_tracker_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_5d92fa905a1d3e20_plan_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_f43263c25e31810d_defaults_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -135,13 +135,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_5d92fa905a1d3e20_plan_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_f43263c25e31810d_defaults_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3322 ssttaatteemmeennttss ?  3311 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Tracker Class Definition""" 
 _2import typing as t 
 _3from dotmap import DotMap 
 _4from elasticsearch8 import Elasticsearch 
 _5from es_testbed.helpers.utils import getlogger 
 _6from .entitymgrs import ( 
 _7 ComponentMgr, DataStreamMgr, IlmMgr, IndexMgr, SnapshotMgr, TemplateMgr) 
@@ -58,8 +58,8 @@
 _4_3 # These are ordered this way on purpose 
 _4_4 self.entities.teardown() 
 _4_5 self.snapshots.teardown() 
 _4_6 self.templates.teardown() 
 _4_7 self.components.teardown() 
 _4_8 self.ilm_policies.teardown() 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_72ef0405fdf841ab___init___py.html` & `es_testbed-0.5.3/cov_html/d_72ef0405fdf841ab___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_f43263c25e31810d_exceptions_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_72ef0405fdf841ab_es_api_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -87,13 +87,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_f43263c25e31810d_exceptions_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_72ef0405fdf841ab_es_api_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,10 +7,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_72ef0405fdf841ab_config_py.html` & `es_testbed-0.5.3/cov_html/d_72ef0405fdf841ab_config_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/d_72ef0405fdf841ab_es_api_py.html` & `es_testbed-0.5.3/cov_html/d_72ef0405fdf841ab_es_api_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for /Users/buh/.pyenv/versions/3.12.2/envs/es-testbed/lib/python3.12/site-packages/es_testbed/helpers/es_api.py: 75%</title>
+    <title>Coverage for /Users/buh/.pyenv/versions/3.12.2/envs/es-testbed/lib/python3.12/site-packages/es_testbed/helpers/es_api.py: 74%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>/Users/buh/.pyenv/versions/3.12.2/envs/es-testbed/lib/python3.12/site-packages/es_testbed/helpers/es_api.py</b>:
-            <span class="pc_cov">75%</span>
+            <span class="pc_cov">74%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -52,26 +52,26 @@
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
             <span class="text">213 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">161<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">52<span class="text"> missing</span></button>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">159<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">54<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
             <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">12<span class="text"> partial</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_72ef0405fdf841ab___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_72ef0405fdf841ab_utils_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -384,16 +384,16 @@
     <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">    <span class="nam">response</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">indices</span><span class="op">.</span><span class="nam">get_alias</span><span class="op">(</span><span class="nam">index</span><span class="op">=</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">    <span class="nam">retval</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
     <p class="par run show_par"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">    <span class="key">for</span> <span class="nam">index</span> <span class="key">in</span> <span class="nam">list</span><span class="op">(</span><span class="nam">response</span><span class="op">.</span><span class="nam">keys</span><span class="op">(</span><span class="op">)</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">302&#x202F;&#x219B;&#x202F;309</span><span class="annotate long">line 302 didn't jump to line 309, because the loop on line 302 didn't complete</span></span></p>
     <p class="run"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">        <span class="key">try</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">            <span class="key">if</span> <span class="nam">response</span><span class="op">[</span><span class="nam">index</span><span class="op">]</span><span class="op">[</span><span class="str">'aliases'</span><span class="op">]</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span><span class="op">[</span><span class="str">'is_write_index'</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">                <span class="nam">retval</span> <span class="op">=</span> <span class="nam">index</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">                <span class="key">break</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">        <span class="key">except</span> <span class="nam">KeyError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">        <span class="key">except</span> <span class="nam">KeyError</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">            <span class="key">continue</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">    <span class="key">return</span> <span class="nam">retval</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t"><span class="key">def</span> <span class="nam">snapshot_name</span><span class="op">(</span><span class="nam">client</span><span class="op">:</span> <span class="nam">Elasticsearch</span><span class="op">,</span> <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="nam">t</span><span class="op">.</span><span class="nam">Union</span><span class="op">[</span><span class="nam">t</span><span class="op">.</span><span class="nam">AnyStr</span><span class="op">,</span> <span class="key">None</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">    <span class="str">"""Get the name of the snapshot behind the mounted index data"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">    <span class="nam">res</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="par run show_par"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">    <span class="key">if</span> <span class="nam">exists</span><span class="op">(</span><span class="nam">client</span><span class="op">,</span> <span class="str">'index'</span><span class="op">,</span> <span class="nam">name</span><span class="op">)</span><span class="op">:</span> <span class="com"># Can jump straight to nested keys if it exists</span>&nbsp;</span><span class="r"><span class="annotate short">314&#x202F;&#x219B;&#x202F;316</span><span class="annotate long">line 314 didn't jump to line 316, because the condition on line 314 was never false</span></span></p>
     <p class="run"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">        <span class="nam">res</span> <span class="op">=</span> <span class="nam">client</span><span class="op">.</span><span class="nam">indices</span><span class="op">.</span><span class="nam">get</span><span class="op">(</span><span class="nam">index</span><span class="op">=</span><span class="nam">name</span><span class="op">)</span><span class="op">[</span><span class="nam">name</span><span class="op">]</span><span class="op">[</span><span class="str">'settings'</span><span class="op">]</span><span class="op">[</span><span class="str">'index'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
@@ -486,13 +486,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_72ef0405fdf841ab___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_72ef0405fdf841ab_utils_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 ************ CCoovveerraaggee ffoorr //UUsseerrss//bbuuhh//..ppyyeennvv//vveerrssiioonnss//33..1122..22//eennvvss//eess--tteessttbbeedd//lliibb//
-ppyytthhoonn33..1122//ssiittee--ppaacckkaaggeess//eess__tteessttbbeedd//hheellppeerrss//eess__aappii..ppyy:: 7755%% ************
+ppyytthhoonn33..1122//ssiittee--ppaacckkaaggeess//eess__tteessttbbeedd//hheellppeerrss//eess__aappii..ppyy:: 7744%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 221133 ssttaatteemmeennttss ?  116611 rruunn 5522 mmiissssiinngg 00 eexxcclluuddeedd 1122 ppaarrttiiaall **********
+********** 221133 ssttaatteemmeennttss ?  115599 rruunn 5544 mmiissssiinngg 00 eexxcclluuddeedd 1122 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Functions that make Elasticsearch API Calls""" 
 _2import typing as t 
 _3from os import getenv 
 _4from elasticsearch8 import Elasticsearch, exceptions as esx 
 _5from es_wait import Exists, Snapshot 
 _6from es_testbed.defaults import MAPPING, PAUSE_DEFAULT, PAUSE_ENVVAR 
 _7from es_testbed import exceptions as exc 
@@ -442,8 +442,8 @@
 _3_9_5 return client.indices.resolve_index(name=name, expand_wildcards=['open',
 'closed']) 
 _3_9_6 
 _3_9_7def rollover(client: Elasticsearch, name: str) -> None: 
 _3_9_8 """Rollover alias or datastream identified by name""" 
 _3_9_9 client.indices.rollover(alias=name, wait_for_active_shards='all') 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_72ef0405fdf841ab_utils_py.html` & `es_testbed-0.5.3/cov_html/d_72ef0405fdf841ab_utils_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_72ef0405fdf841ab_es_api_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_f43263c25e31810d_version_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -282,13 +282,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_72ef0405fdf841ab_es_api_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_f43263c25e31810d_version_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 110022 ssttaatteemmeennttss ?  9911 rruunn 1111 mmiissssiinngg 00 eexxcclluuddeedd 55 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Utility helper functions""" 
 _2import typing as t 
 _3import random 
 _4import string 
 _5import logging 
 _6from copy import deepcopy 
 _7from datetime import datetime, timezone 
@@ -228,8 +228,8 @@
 _1_9_0 logger = getlogger(__name__) 
 _1_9_1 # Use deepcopy of compare so we don't change the original 
 _1_9_2 uniq = remove_by_index(original, deepcopy(compare)) 
 _1_9_3 if uniq: 
 _1_9_4 logger.debug('Values found only in compare: %s', uniq) 
 _1_9_5 return uniq 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_9e00aab3b961c475___init___py.html` & `es_testbed-0.5.3/cov_html/d_9e00aab3b961c475___init___py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_5d92fa905a1d3e20_base_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9e00aab3b961c475_alias_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -92,13 +92,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_5d92fa905a1d3e20_base_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9e00aab3b961c475_alias_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 44 ssttaatteemmeennttss ?  44 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Entities Init File""" 
 _2from .entity import Entity 
 _3from .alias import Alias 
 _4from .index import Index 
 _5from .data_stream import DataStream 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_9e00aab3b961c475_alias_py.html` & `es_testbed-0.5.3/cov_html/d_9e00aab3b961c475_alias_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_9e00aab3b961c475___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9e00aab3b961c475_data_stream_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -122,13 +122,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_9e00aab3b961c475___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9e00aab3b961c475_data_stream_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 2233 ssttaatteemmeennttss ?  2222 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 33 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Alias Entity Class""" 
 _2import typing as t 
 _3from elasticsearch8 import Elasticsearch 
 _4from es_testbed.helpers.utils import getlogger 
 _5from es_testbed.helpers import es_api 
 _6from .entity import Entity 
 _7 
@@ -47,8 +47,8 @@
 _3_1 if alias['indices'] == index_list: 31 ↛ 26line 31 didn't jump to line 26,
 because the condition on line 31 was never false
 _3_2 self.logger.debug('Confirm match of indices backed by alias %s', self.name) 
 _3_3 retval = True 
 _3_4 break 
 _3_5 return retval 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_9e00aab3b961c475_data_stream_py.html` & `es_testbed-0.5.3/cov_html/d_9e00aab3b961c475_data_stream_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_9e00aab3b961c475_alias_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9e00aab3b961c475_entity_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -118,13 +118,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_9e00aab3b961c475_alias_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9e00aab3b961c475_entity_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 2200 ssttaatteemmeennttss ?  2200 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Index Entity Class""" 
 _2import typing as t 
 _3from elasticsearch8 import Elasticsearch 
 _4from es_testbed.helpers import es_api 
 _5from es_testbed.helpers.utils import getlogger 
 _6from . import Alias 
 _7 
@@ -42,8 +42,8 @@
 _2_8 if self.backing_indices == index_list: 28 ↛ 31line 28 didn't jump to line
 31, because the condition on line 28 was never false
 _2_9 self.logger.debug('Confirm match of data_stream "%s" backing indices',
 self.name) 
 _3_0 retval = True 
 _3_1 return retval 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_9e00aab3b961c475_entity_py.html` & `es_testbed-0.5.3/cov_html/d_9e00aab3b961c475_entity_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_9e00aab3b961c475_data_stream_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9e00aab3b961c475_index_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -121,13 +121,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_9e00aab3b961c475_data_stream_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_9e00aab3b961c475_index_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 2222 ssttaatteemmeennttss ?  2211 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Base Entity Class""" 
 _2import typing as t 
 _3from elasticsearch8 import Elasticsearch 
 _4from es_testbed.helpers import es_api 
 _5from es_testbed.helpers.utils import getlogger 
 _6 
 _7# pylint: disable=missing-docstring,too-many-arguments 
@@ -44,8 +44,8 @@
 _2_9 
 _3_0 def setup(self): 
 _3_1 pass 
 _3_2 
 _3_3 def teardown(self): 
 _3_4 pass 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_9e00aab3b961c475_index_py.html` & `es_testbed-0.5.3/cov_html/d_9e00aab3b961c475_index_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_9e00aab3b961c475_entity_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -219,13 +219,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_9e00aab3b961c475_entity_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 110022 ssttaatteemmeennttss ?  7766 rruunn 2266 mmiissssiinngg 00 eexxcclluuddeedd 44 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Index Entity Class""" 
 _2import typing as t 
 _3from os import getenv 
 _4from elasticsearch8 import Elasticsearch 
 _5from es_wait import Exists 
 _6from es_testbed.defaults import PAUSE_DEFAULT, PAUSE_ENVVAR, TIMEOUT_DEFAULT,
 TIMEOUT_ENVVAR 
@@ -159,8 +159,8 @@
 _1_2_7 Get ILM phase information and put it in self.ilm_tracker 
 _1_2_8 Name as an arg makes it configurable 
 _1_2_9 """ 
 _1_3_0 if self.policy_name: 
 _1_3_1 self.ilm_tracker = IlmTracker(self.client, name) 
 _1_3_2 self.ilm_tracker.update() 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_a40f6d277e0496df___init___py.html` & `es_testbed-0.5.3/cov_html/d_a40f6d277e0496df___init___py.html`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a44f0ac069e85531_conftest_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_basic_data_streams_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -87,13 +87,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a44f0ac069e85531_conftest_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_basic_data_streams_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,10 +6,10 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_basic_data_streams_py.html` & `es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_basic_data_streams_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_basic_frozen_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -134,13 +134,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_basic_frozen_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3333 ssttaatteemmeennttss ?  3333 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Test functions in es_testbed.TestBed""" 
 _2# pylint: disable=redefined-outer-name,missing-function-docstring,missing-
 class-docstring 
 _3import pytest 
 _4from es_testbed import PlanBuilder, TestBed 
 _5from es_testbed.defaults import NAMEMAPPER 
 _6from es_testbed.helpers.es_api import get_ds_current 
@@ -57,8 +57,8 @@
 _4_3 template = f'{prefix}-{NAMEMAPPER['template']}-{uniq}-000001' 
 _4_4 assert tb.tracker.templates.last == template 
 _4_5 result = tb.client.indices.get_index_template(name=template)
 ['index_templates'] 
 _4_6 assert len(result) == 1 
 _4_7 assert result[0]['index_template']['composed_of'] == components 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_basic_frozen_py.html` & `es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_basic_frozen_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_basic_data_streams_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_basic_rollover_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -140,13 +140,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_basic_data_streams_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_basic_rollover_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3333 ssttaatteemmeennttss ?  3322 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Test functions in es_testbed.TestBed""" 
 _2# pylint: disable=redefined-outer-name,missing-function-docstring,missing-
 class-docstring 
 _3import pytest 
 _4from es_testbed import PlanBuilder, TestBed 
 _5 
 _6@pytest.fixture(scope='module') 
@@ -64,8 +64,8 @@
 _4_9 template = f'{namecore('template')}-000001' 
 _5_0 assert tb.tracker.templates.last == template 
 _5_1 result = tb.client.indices.get_index_template(name=template)
 ['index_templates'] 
 _5_2 assert len(result) == 1 
 _5_3 assert result[0]['index_template']['composed_of'] == components 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_basic_indices_py.html` & `es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_basic_indices_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_basic_rollover_py.html` & `es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_basic_rollover_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_basic_frozen_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_cold_ds_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -138,13 +138,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_basic_frozen_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_cold_ds_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3366 ssttaatteemmeennttss ?  3366 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Test functions in es_testbed.TestBed""" 
 _2# pylint: disable=redefined-outer-name,missing-function-docstring,missing-
 class-docstring 
 _3import pytest 
 _4from es_testbed import PlanBuilder, TestBed 
 _5from es_testbed.defaults import NAMEMAPPER 
 _6from es_testbed.helpers.es_api import get_write_index 
@@ -61,8 +61,8 @@
 _4_7 template = f'{prefix}-{NAMEMAPPER['template']}-{uniq}-000001' 
 _4_8 assert tb.tracker.templates.last == template 
 _4_9 result = tb.client.indices.get_index_template(name=template)
 ['index_templates'] 
 _5_0 assert len(result) == 1 
 _5_1 assert result[0]['index_template']['composed_of'] == components 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_cold_ds_py.html` & `es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_cold_ds_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_basic_rollover_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_cold_indices_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -144,13 +144,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_basic_rollover_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_cold_indices_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3377 ssttaatteemmeennttss ?  3366 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Test functions in es_testbed.TestBed""" 
 _2# pylint: disable=redefined-outer-name,missing-function-docstring,missing-
 class-docstring 
 _3import pytest 
 _4from es_testbed import PlanBuilder, TestBed 
 _5from es_testbed.helpers.es_api import get_ds_current 
 _6 
@@ -68,8 +68,8 @@
 _5_3 template = f'{namecore('template')}-000001' 
 _5_4 assert tb.tracker.templates.last == template 
 _5_5 result = tb.client.indices.get_index_template(name=template)
 ['index_templates'] 
 _5_6 assert len(result) == 1 
 _5_7 assert result[0]['index_template']['composed_of'] == components 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_cold_indices_py.html` & `es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_frozen_indices_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for tests/integration/test_cold_indices.py: 95%</title>
+    <title>Coverage for tests/integration/test_frozen_indices.py: 95%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>tests/integration/test_cold_indices.py</b>:
+            <span class="text">Coverage for </span><b>tests/integration/test_frozen_indices.py</b>:
             <span class="pc_cov">95%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -58,20 +58,20 @@
             <span class="text">38 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">37<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">1<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
             <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">1<span class="text"> partial</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_cold_ds_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_frozen_ds_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_frozen_ds_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_rollover_frozen_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -95,36 +95,36 @@
     <p class="mis show_mis"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">        <span class="nam">pytest</span><span class="op">.</span><span class="nam">skip</span><span class="op">(</span><span class="str">'No snapshot repository'</span><span class="op">,</span> <span class="nam">allow_module_level</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">        <span class="str">'type'</span><span class="op">:</span> <span class="str">'indices'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">        <span class="str">'prefix'</span><span class="op">:</span> <span class="nam">prefix</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">        <span class="str">'rollover_alias'</span><span class="op">:</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">        <span class="str">'uniq'</span><span class="op">:</span> <span class="nam">uniq</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="str">'repository'</span><span class="op">:</span> <span class="nam">repo</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="str">'ilm'</span><span class="op">:</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">            <span class="str">'enabled'</span><span class="op">:</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">            <span class="str">'tiers'</span><span class="op">:</span> <span class="op">[</span><span class="str">'hot'</span><span class="op">,</span> <span class="str">'cold'</span><span class="op">,</span> <span class="str">'delete'</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">            <span class="str">'forcemerge'</span><span class="op">:</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">            <span class="str">'max_num_segments'</span><span class="op">:</span> <span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="str">'defaults'</span><span class="op">:</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">            <span class="str">'entity_count'</span><span class="op">:</span> <span class="num">3</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">            <span class="str">'docs'</span><span class="op">:</span> <span class="num">10</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">            <span class="str">'match'</span><span class="op">:</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">            <span class="str">'searchable'</span><span class="op">:</span> <span class="str">'frozen'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="key">class</span> <span class="nam">TestFrozenIndices</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="key">class</span> <span class="nam">TestFrozenRolloverNoILMIndices</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="op">@</span><span class="nam">pytest</span><span class="op">.</span><span class="nam">fixture</span><span class="op">(</span><span class="nam">scope</span><span class="op">=</span><span class="str">"class"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="key">def</span> <span class="nam">tb</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">client</span><span class="op">,</span> <span class="nam">settings</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="nam">theplan</span> <span class="op">=</span> <span class="nam">PlanBuilder</span><span class="op">(</span><span class="nam">settings</span><span class="op">=</span><span class="nam">settings</span><span class="op">)</span><span class="op">.</span><span class="nam">plan</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">teebee</span> <span class="op">=</span> <span class="nam">TestBed</span><span class="op">(</span><span class="nam">client</span><span class="op">,</span> <span class="nam">plan</span><span class="op">=</span><span class="nam">theplan</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">teebee</span><span class="op">.</span><span class="nam">setup</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="key">yield</span> <span class="nam">teebee</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">teebee</span><span class="op">.</span><span class="nam">teardown</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_entity_count</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">tb</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="key">assert</span> <span class="nam">len</span><span class="op">(</span><span class="nam">tb</span><span class="op">.</span><span class="nam">tracker</span><span class="op">.</span><span class="nam">entities</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">)</span> <span class="op">==</span> <span class="num">3</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_first_index</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">tb</span><span class="op">,</span> <span class="nam">cold</span><span class="op">,</span> <span class="nam">prefix</span><span class="op">,</span> <span class="nam">uniq</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="nam">value</span> <span class="op">=</span> <span class="fst">f'</span><span class="op">{</span><span class="nam">cold</span><span class="op">}</span><span class="op">{</span><span class="nam">prefix</span><span class="op">}</span><span class="fst">-</span><span class="op">{</span><span class="nam">NAMEMAPPER</span><span class="op">[</span><span class="str">'index'</span><span class="op">]</span><span class="op">}</span><span class="fst">-</span><span class="op">{</span><span class="nam">uniq</span><span class="op">}</span><span class="fst">-000001</span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_first_index</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">tb</span><span class="op">,</span> <span class="nam">frozen</span><span class="op">,</span> <span class="nam">prefix</span><span class="op">,</span> <span class="nam">uniq</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="nam">value</span> <span class="op">=</span> <span class="fst">f'</span><span class="op">{</span><span class="nam">frozen</span><span class="op">}</span><span class="op">{</span><span class="nam">prefix</span><span class="op">}</span><span class="fst">-</span><span class="op">{</span><span class="nam">NAMEMAPPER</span><span class="op">[</span><span class="str">'index'</span><span class="op">]</span><span class="op">}</span><span class="fst">-</span><span class="op">{</span><span class="nam">uniq</span><span class="op">}</span><span class="fst">-000001</span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="key">assert</span> <span class="nam">tb</span><span class="op">.</span><span class="nam">tracker</span><span class="op">.</span><span class="nam">entities</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">.</span><span class="nam">name</span> <span class="op">==</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_last_index</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">tb</span><span class="op">,</span> <span class="nam">prefix</span><span class="op">,</span> <span class="nam">uniq</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">value</span> <span class="op">=</span> <span class="fst">f'</span><span class="op">{</span><span class="nam">prefix</span><span class="op">}</span><span class="fst">-</span><span class="op">{</span><span class="nam">NAMEMAPPER</span><span class="op">[</span><span class="str">'index'</span><span class="op">]</span><span class="op">}</span><span class="fst">-</span><span class="op">{</span><span class="nam">uniq</span><span class="op">}</span><span class="fst">-000003</span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="key">assert</span> <span class="nam">tb</span><span class="op">.</span><span class="nam">tracker</span><span class="op">.</span><span class="nam">entities</span><span class="op">.</span><span class="nam">last</span><span class="op">.</span><span class="nam">name</span> <span class="op">==</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_write_index</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">tb</span><span class="op">,</span> <span class="nam">prefix</span><span class="op">,</span> <span class="nam">uniq</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
@@ -141,18 +141,18 @@
     <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">tb</span><span class="op">.</span><span class="nam">client</span><span class="op">.</span><span class="nam">indices</span><span class="op">.</span><span class="nam">get_index_template</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">template</span><span class="op">)</span><span class="op">[</span><span class="str">'index_templates'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="key">assert</span> <span class="nam">len</span><span class="op">(</span><span class="nam">result</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">assert</span> <span class="nam">result</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">[</span><span class="str">'index_template'</span><span class="op">]</span><span class="op">[</span><span class="str">'composed_of'</span><span class="op">]</span> <span class="op">==</span> <span class="nam">components</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_cold_ds_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_frozen_ds_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_frozen_ds_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_rollover_frozen_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-************ CCoovveerraaggee ffoorr tteessttss//iinntteeggrraattiioonn//tteesstt__ccoolldd__iinnddiicceess..ppyy:: 9955%% ************
+************ CCoovveerraaggee ffoorr tteessttss//iinntteeggrraattiioonn//tteesstt__ffrroozzeenn__iinnddiicceess..ppyy:: 9955%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3388 ssttaatteemmeennttss ?  3377 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Test functions in es_testbed.TestBed""" 
 _2# pylint: disable=redefined-outer-name,missing-function-docstring,missing-
 class-docstring 
 _3import pytest 
 _4from es_testbed import PlanBuilder, TestBed 
 _5from es_testbed.defaults import NAMEMAPPER 
 _6from es_testbed.helpers.es_api import get_write_index 
@@ -26,36 +26,36 @@
 _1_1 pytest.skip('No snapshot repository', allow_module_level=True) 
 _1_2 return { 
 _1_3 'type': 'indices', 
 _1_4 'prefix': prefix, 
 _1_5 'rollover_alias': True, 
 _1_6 'uniq': uniq, 
 _1_7 'repository': repo, 
-_1_8 'ilm': { 
-_1_9 'enabled': True, 
-_2_0 'tiers': ['hot', 'cold', 'delete'], 
-_2_1 'forcemerge': False, 
-_2_2 'max_num_segments': 1, 
+_1_8 'defaults': { 
+_1_9 'entity_count': 3, 
+_2_0 'docs': 10, 
+_2_1 'match': True, 
+_2_2 'searchable': 'frozen', 
 _2_3 } 
 _2_4 } 
 _2_5 
-_2_6class TestFrozenIndices: 
+_2_6class TestFrozenRolloverNoILMIndices: 
 _2_7 @pytest.fixture(scope="class") 
 _2_8 def tb(self, client, settings): 
 _2_9 theplan = PlanBuilder(settings=settings).plan 
 _3_0 teebee = TestBed(client, plan=theplan) 
 _3_1 teebee.setup() 
 _3_2 yield teebee 
 _3_3 teebee.teardown() 
 _3_4 
 _3_5 def test_entity_count(self, tb): 
 _3_6 assert len(tb.tracker.entities.entity_list) == 3 
 _3_7 
-_3_8 def test_first_index(self, tb, cold, prefix, uniq): 
-_3_9 value = f'{cold}{prefix}-{NAMEMAPPER['index']}-{uniq}-000001' 
+_3_8 def test_first_index(self, tb, frozen, prefix, uniq): 
+_3_9 value = f'{frozen}{prefix}-{NAMEMAPPER['index']}-{uniq}-000001' 
 _4_0 assert tb.tracker.entities.entity_list[0].name == value 
 _4_1 
 _4_2 def test_last_index(self, tb, prefix, uniq): 
 _4_3 value = f'{prefix}-{NAMEMAPPER['index']}-{uniq}-000003' 
 _4_4 assert tb.tracker.entities.last.name == value 
 _4_5 
 _4_6 def test_write_index(self, tb, prefix, uniq): 
@@ -70,8 +70,8 @@
 _5_5 template = f'{prefix}-{NAMEMAPPER['template']}-{uniq}-000001' 
 _5_6 assert tb.tracker.templates.last == template 
 _5_7 result = tb.client.indices.get_index_template(name=template)
 ['index_templates'] 
 _5_8 assert len(result) == 1 
 _5_9 assert result[0]['index_template']['composed_of'] == components 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_frozen_ds_py.html` & `es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_frozen_ds_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_cold_indices_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_frozen_indices_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -144,13 +144,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_cold_indices_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_frozen_indices_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3377 ssttaatteemmeennttss ?  3366 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Test functions in es_testbed.TestBed""" 
 _2# pylint: disable=redefined-outer-name,missing-function-docstring,missing-
 class-docstring 
 _3import pytest 
 _4from es_testbed import PlanBuilder, TestBed 
 _5from es_testbed.helpers.es_api import get_ds_current 
 _6 
@@ -68,8 +68,8 @@
 _5_3 template = f'{namecore('template')}-000001' 
 _5_4 assert tb.tracker.templates.last == template 
 _5_5 result = tb.client.indices.get_index_template(name=template)
 ['index_templates'] 
 _5_6 assert len(result) == 1 
 _5_7 assert result[0]['index_template']['composed_of'] == components 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_frozen_indices_py.html` & `es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_cold_indices_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for tests/integration/test_frozen_indices.py: 95%</title>
+    <title>Coverage for tests/integration/test_cold_indices.py: 95%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>tests/integration/test_frozen_indices.py</b>:
+            <span class="text">Coverage for </span><b>tests/integration/test_cold_indices.py</b>:
             <span class="pc_cov">95%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -58,20 +58,20 @@
             <span class="text">38 statements &nbsp;</span>
             <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">37<span class="text"> run</span></button>
             <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">1<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
             <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">1<span class="text"> partial</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_frozen_ds_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_cold_ds_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_rollover_frozen_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_frozen_ds_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -95,36 +95,36 @@
     <p class="mis show_mis"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t">        <span class="nam">pytest</span><span class="op">.</span><span class="nam">skip</span><span class="op">(</span><span class="str">'No snapshot repository'</span><span class="op">,</span> <span class="nam">allow_module_level</span><span class="op">=</span><span class="key">True</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">return</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">        <span class="str">'type'</span><span class="op">:</span> <span class="str">'indices'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">        <span class="str">'prefix'</span><span class="op">:</span> <span class="nam">prefix</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">        <span class="str">'rollover_alias'</span><span class="op">:</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">        <span class="str">'uniq'</span><span class="op">:</span> <span class="nam">uniq</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="str">'repository'</span><span class="op">:</span> <span class="nam">repo</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="str">'defaults'</span><span class="op">:</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">            <span class="str">'entity_count'</span><span class="op">:</span> <span class="num">3</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">            <span class="str">'docs'</span><span class="op">:</span> <span class="num">10</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">            <span class="str">'match'</span><span class="op">:</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">            <span class="str">'searchable'</span><span class="op">:</span> <span class="str">'frozen'</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="str">'ilm'</span><span class="op">:</span> <span class="op">{</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">            <span class="str">'enabled'</span><span class="op">:</span> <span class="key">True</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">            <span class="str">'tiers'</span><span class="op">:</span> <span class="op">[</span><span class="str">'hot'</span><span class="op">,</span> <span class="str">'cold'</span><span class="op">,</span> <span class="str">'delete'</span><span class="op">]</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">            <span class="str">'forcemerge'</span><span class="op">:</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">            <span class="str">'max_num_segments'</span><span class="op">:</span> <span class="num">1</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">        <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="op">}</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="key">class</span> <span class="nam">TestFrozenRolloverNoILMIndices</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="key">class</span> <span class="nam">TestFrozenIndices</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">    <span class="op">@</span><span class="nam">pytest</span><span class="op">.</span><span class="nam">fixture</span><span class="op">(</span><span class="nam">scope</span><span class="op">=</span><span class="str">"class"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="key">def</span> <span class="nam">tb</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">client</span><span class="op">,</span> <span class="nam">settings</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="nam">theplan</span> <span class="op">=</span> <span class="nam">PlanBuilder</span><span class="op">(</span><span class="nam">settings</span><span class="op">=</span><span class="nam">settings</span><span class="op">)</span><span class="op">.</span><span class="nam">plan</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">teebee</span> <span class="op">=</span> <span class="nam">TestBed</span><span class="op">(</span><span class="nam">client</span><span class="op">,</span> <span class="nam">plan</span><span class="op">=</span><span class="nam">theplan</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">teebee</span><span class="op">.</span><span class="nam">setup</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="key">yield</span> <span class="nam">teebee</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">teebee</span><span class="op">.</span><span class="nam">teardown</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_entity_count</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">tb</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="key">assert</span> <span class="nam">len</span><span class="op">(</span><span class="nam">tb</span><span class="op">.</span><span class="nam">tracker</span><span class="op">.</span><span class="nam">entities</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">)</span> <span class="op">==</span> <span class="num">3</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_first_index</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">tb</span><span class="op">,</span> <span class="nam">frozen</span><span class="op">,</span> <span class="nam">prefix</span><span class="op">,</span> <span class="nam">uniq</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="nam">value</span> <span class="op">=</span> <span class="fst">f'</span><span class="op">{</span><span class="nam">frozen</span><span class="op">}</span><span class="op">{</span><span class="nam">prefix</span><span class="op">}</span><span class="fst">-</span><span class="op">{</span><span class="nam">NAMEMAPPER</span><span class="op">[</span><span class="str">'index'</span><span class="op">]</span><span class="op">}</span><span class="fst">-</span><span class="op">{</span><span class="nam">uniq</span><span class="op">}</span><span class="fst">-000001</span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_first_index</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">tb</span><span class="op">,</span> <span class="nam">cold</span><span class="op">,</span> <span class="nam">prefix</span><span class="op">,</span> <span class="nam">uniq</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="nam">value</span> <span class="op">=</span> <span class="fst">f'</span><span class="op">{</span><span class="nam">cold</span><span class="op">}</span><span class="op">{</span><span class="nam">prefix</span><span class="op">}</span><span class="fst">-</span><span class="op">{</span><span class="nam">NAMEMAPPER</span><span class="op">[</span><span class="str">'index'</span><span class="op">]</span><span class="op">}</span><span class="fst">-</span><span class="op">{</span><span class="nam">uniq</span><span class="op">}</span><span class="fst">-000001</span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="key">assert</span> <span class="nam">tb</span><span class="op">.</span><span class="nam">tracker</span><span class="op">.</span><span class="nam">entities</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">.</span><span class="nam">name</span> <span class="op">==</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_last_index</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">tb</span><span class="op">,</span> <span class="nam">prefix</span><span class="op">,</span> <span class="nam">uniq</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">        <span class="nam">value</span> <span class="op">=</span> <span class="fst">f'</span><span class="op">{</span><span class="nam">prefix</span><span class="op">}</span><span class="fst">-</span><span class="op">{</span><span class="nam">NAMEMAPPER</span><span class="op">[</span><span class="str">'index'</span><span class="op">]</span><span class="op">}</span><span class="fst">-</span><span class="op">{</span><span class="nam">uniq</span><span class="op">}</span><span class="fst">-000003</span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="key">assert</span> <span class="nam">tb</span><span class="op">.</span><span class="nam">tracker</span><span class="op">.</span><span class="nam">entities</span><span class="op">.</span><span class="nam">last</span><span class="op">.</span><span class="nam">name</span> <span class="op">==</span> <span class="nam">value</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">def</span> <span class="nam">test_write_index</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">tb</span><span class="op">,</span> <span class="nam">prefix</span><span class="op">,</span> <span class="nam">uniq</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
@@ -141,18 +141,18 @@
     <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">        <span class="nam">result</span> <span class="op">=</span> <span class="nam">tb</span><span class="op">.</span><span class="nam">client</span><span class="op">.</span><span class="nam">indices</span><span class="op">.</span><span class="nam">get_index_template</span><span class="op">(</span><span class="nam">name</span><span class="op">=</span><span class="nam">template</span><span class="op">)</span><span class="op">[</span><span class="str">'index_templates'</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">        <span class="key">assert</span> <span class="nam">len</span><span class="op">(</span><span class="nam">result</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">        <span class="key">assert</span> <span class="nam">result</span><span class="op">[</span><span class="num">0</span><span class="op">]</span><span class="op">[</span><span class="str">'index_template'</span><span class="op">]</span><span class="op">[</span><span class="str">'composed_of'</span><span class="op">]</span> <span class="op">==</span> <span class="nam">components</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_frozen_ds_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_cold_ds_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_rollover_frozen_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df_test_frozen_ds_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-************ CCoovveerraaggee ffoorr tteessttss//iinntteeggrraattiioonn//tteesstt__ffrroozzeenn__iinnddiicceess..ppyy:: 9955%% ************
+************ CCoovveerraaggee ffoorr tteessttss//iinntteeggrraattiioonn//tteesstt__ccoolldd__iinnddiicceess..ppyy:: 9955%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3388 ssttaatteemmeennttss ?  3377 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Test functions in es_testbed.TestBed""" 
 _2# pylint: disable=redefined-outer-name,missing-function-docstring,missing-
 class-docstring 
 _3import pytest 
 _4from es_testbed import PlanBuilder, TestBed 
 _5from es_testbed.defaults import NAMEMAPPER 
 _6from es_testbed.helpers.es_api import get_write_index 
@@ -26,36 +26,36 @@
 _1_1 pytest.skip('No snapshot repository', allow_module_level=True) 
 _1_2 return { 
 _1_3 'type': 'indices', 
 _1_4 'prefix': prefix, 
 _1_5 'rollover_alias': True, 
 _1_6 'uniq': uniq, 
 _1_7 'repository': repo, 
-_1_8 'defaults': { 
-_1_9 'entity_count': 3, 
-_2_0 'docs': 10, 
-_2_1 'match': True, 
-_2_2 'searchable': 'frozen', 
+_1_8 'ilm': { 
+_1_9 'enabled': True, 
+_2_0 'tiers': ['hot', 'cold', 'delete'], 
+_2_1 'forcemerge': False, 
+_2_2 'max_num_segments': 1, 
 _2_3 } 
 _2_4 } 
 _2_5 
-_2_6class TestFrozenRolloverNoILMIndices: 
+_2_6class TestFrozenIndices: 
 _2_7 @pytest.fixture(scope="class") 
 _2_8 def tb(self, client, settings): 
 _2_9 theplan = PlanBuilder(settings=settings).plan 
 _3_0 teebee = TestBed(client, plan=theplan) 
 _3_1 teebee.setup() 
 _3_2 yield teebee 
 _3_3 teebee.teardown() 
 _3_4 
 _3_5 def test_entity_count(self, tb): 
 _3_6 assert len(tb.tracker.entities.entity_list) == 3 
 _3_7 
-_3_8 def test_first_index(self, tb, frozen, prefix, uniq): 
-_3_9 value = f'{frozen}{prefix}-{NAMEMAPPER['index']}-{uniq}-000001' 
+_3_8 def test_first_index(self, tb, cold, prefix, uniq): 
+_3_9 value = f'{cold}{prefix}-{NAMEMAPPER['index']}-{uniq}-000001' 
 _4_0 assert tb.tracker.entities.entity_list[0].name == value 
 _4_1 
 _4_2 def test_last_index(self, tb, prefix, uniq): 
 _4_3 value = f'{prefix}-{NAMEMAPPER['index']}-{uniq}-000003' 
 _4_4 assert tb.tracker.entities.last.name == value 
 _4_5 
 _4_6 def test_write_index(self, tb, prefix, uniq): 
@@ -70,8 +70,8 @@
 _5_5 template = f'{prefix}-{NAMEMAPPER['template']}-{uniq}-000001' 
 _5_6 assert tb.tracker.templates.last == template 
 _5_7 result = tb.client.indices.get_index_template(name=template)
 ['index_templates'] 
 _5_8 assert len(result) == 1 
 _5_9 assert result[0]['index_template']['composed_of'] == components 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_a40f6d277e0496df_test_rollover_frozen_py.html` & `es_testbed-0.5.3/cov_html/d_a40f6d277e0496df_test_rollover_frozen_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_frozen_indices_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_17bd492d087794b9___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -146,13 +146,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a40f6d277e0496df_test_frozen_indices_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_17bd492d087794b9___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3377 ssttaatteemmeennttss ?  3366 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Test functions in es_testbed.TestBed""" 
 _2# pylint: disable=redefined-outer-name,missing-function-docstring,missing-
 class-docstring 
 _3import pytest 
 _4from es_testbed import PlanBuilder, TestBed 
 _5from es_testbed.helpers.es_api import get_write_index 
 _6 
@@ -70,8 +70,8 @@
 _5_5 template = f'{namecore('template')}-000001' 
 _5_6 assert tb.tracker.templates.last == template 
 _5_7 result = tb.client.indices.get_index_template(name=template)
 ['index_templates'] 
 _5_8 assert len(result) == 1 
 _5_9 assert result[0]['index_template']['composed_of'] == components 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_a44f0ac069e85531___init___py.html` & `es_testbed-0.5.3/cov_html/d_a44f0ac069e85531___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_f43263c25e31810d_version_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a44f0ac069e85531_conftest_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -88,13 +88,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_f43263c25e31810d_version_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a44f0ac069e85531_conftest_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,11 +6,11 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 00 ssttaatteemmeennttss ?  00 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Tests base __init__""" 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_a44f0ac069e85531_conftest_py.html` & `es_testbed-0.5.3/cov_html/d_a44f0ac069e85531_conftest_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a44f0ac069e85531___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -163,13 +163,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a44f0ac069e85531___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a40f6d277e0496df___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 5566 ssttaatteemmeennttss ?  5522 rruunn 44 mmiissssiinngg 00 eexxcclluuddeedd 33 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Top-level conftest.py""" 
 _2# pylint: disable=missing-function-docstring,redefined-outer-name 
 _3from os import environ 
 _4from datetime import datetime, timezone 
 _5import random 
 _6import string 
 _7import pytest 
@@ -89,8 +89,8 @@
 _7_1 return name # Return the repo name if it's online 
 _7_2 
 _7_3@pytest.fixture(scope='module') 
 _7_4def uniq(): 
 _7_5 """Return a random uniq value""" 
 _7_6 return randomstr(length=8, lowercase=True) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902___init___py.html` & `es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902___init___py.html`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_9e00aab3b961c475_index_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_componentmgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -95,13 +95,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_9e00aab3b961c475_index_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_componentmgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,18 +7,18 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 77 ssttaatteemmeennttss ?  77 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Make class import nicer""" 
 _2from .componentmgr import ComponentMgr 
 _3from .data_streammgr import DataStreamMgr 
 _4from .entitymgr import EntityMgr 
 _5from .ilmmgr import IlmMgr 
 _6from .indexmgr import IndexMgr 
 _7from .snapshotmgr import SnapshotMgr 
 _8from .templatemgr import TemplateMgr 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_componentmgr_py.html` & `es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_componentmgr_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_data_streammgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -132,13 +132,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_data_streammgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3322 ssttaatteemmeennttss ?  3311 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Component Template Entity Manager Class""" 
 _2import typing as t 
 _3from dotmap import DotMap 
 _4from elasticsearch8 import Elasticsearch 
 _5from es_testbed.exceptions import ResultNotExpected 
 _6from es_testbed.helpers import es_api 
 _7from es_testbed.helpers.utils import getlogger, mapping_component,
@@ -58,8 +58,8 @@
 _4_0 raise ResultNotExpected( 
 _4_1 f'Unable to verify creation of component template {self.name}') 
 _4_2 self.appender(self.name) 
 _4_3 self.logger.info('Created component template: "%s"', self.last) 
 _4_4 self.logger.info('Successfully created all component templates.') 
 _4_5 self.success = True 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_data_streammgr_py.html` & `es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_data_streammgr_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_componentmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_entitymgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -165,13 +165,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_componentmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_entitymgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 5544 ssttaatteemmeennttss ?  5544 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""data_stream Entity Manager Class""" 
 _2import typing as t 
 _3from dotmap import DotMap 
 _4from elasticsearch8 import Elasticsearch 
 _5from es_testbed.helpers import es_api 
 _6from es_testbed.helpers.utils import getlogger 
 _7from .indexmgr import IndexMgr 
@@ -93,8 +93,8 @@
 _7_3 client=self.client, 
 _7_4 name=name, 
 _7_5 snapmgr=self.snapmgr, 
 _7_6 policy_name=self.policy_name 
 _7_7 ) 
 _7_8 self.index_trackers.append(entity) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_entitymgr_py.html` & `es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_entitymgr_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_data_streammgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_ilmmgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -237,13 +237,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_data_streammgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_ilmmgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 112255 ssttaatteemmeennttss ?  110088 rruunn 1177 mmiissssiinngg 00 eexxcclluuddeedd 55 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Entity Class Definition""" 
 _2import typing as t 
 _3from dotmap import DotMap 
 _4from elasticsearch8 import Elasticsearch 
 _5from es_testbed.defaults import NAMEMAPPER, PLURALMAP 
 _6from es_testbed.helpers.es_api import delete, get 
 _7from es_testbed.helpers.utils import getlogger, uniq_values 
@@ -171,8 +171,8 @@
 _1_4_6 self.entity_list = curr 
 _1_4_7 else: 
 _1_4_8 self.logger.warning('Not correcting entity_list! Values should be: %s',
 curr) 
 _1_4_9 retval = curr 
 _1_5_0 return retval 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_ilmmgr_py.html` & `es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_ilmmgr_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_entitymgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_indexmgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -139,13 +139,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_entitymgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_indexmgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3311 ssttaatteemmeennttss ?  3300 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""ILM Policy Entity Manager Class""" 
 _2import typing as t 
 _3from dotmap import DotMap 
 _4from elasticsearch8 import Elasticsearch 
 _5from es_testbed.exceptions import ResultNotExpected 
 _6from es_testbed.helpers import es_api 
 _7from es_testbed.helpers.utils import build_ilm_policy, getlogger 
@@ -62,8 +62,8 @@
 _4_7 self.appender(self.name) 
 _4_8 self.logger.info('Successfully created ILM policy: %s', self.last) 
 _4_9 else: 
 _5_0 self.appender(None) # This covers self.plan.ilm_policies[-1] 
 _5_1 self.logger.info('No ILM policy created.') 
 _5_2 self.success = True 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_indexmgr_py.html` & `es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_indexmgr_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_ilmmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_snapshotmgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -209,13 +209,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_ilmmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_snapshotmgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 8811 ssttaatteemmeennttss ?  7799 rruunn 22 mmiissssiinngg 00 eexxcclluuddeedd 33 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Index Entity Manager Class""" 
 _2import typing as t 
 _3from dotmap import DotMap 
 _4from elasticsearch8 import Elasticsearch 
 _5from es_testbed.helpers import es_api 
 _6from es_testbed.helpers.utils import getlogger, setting_component 
 _7from .entitymgr import EntityMgr 
@@ -137,8 +137,8 @@
 _1_1_7 name=name, 
 _1_1_8 snapmgr=self.snapmgr, 
 _1_1_9 policy_name=self.policy_name 
 _1_2_0 ) 
 _1_2_1 self.failsafe.append(name) 
 _1_2_2 self.entity_list.append(entity) 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_snapshotmgr_py.html` & `es_testbed-0.5.3/cov_html/z_396c7038a91d0266_snapshotmgr_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html>
+<html lang="en">
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for /Users/buh/.pyenv/versions/3.12.2/envs/es-testbed/lib/python3.12/site-packages/es_testbed/classes/entitymgrs/snapshotmgr.py: 90%</title>
+    <title>Coverage for src/es_testbed/classes/entitymgrs/snapshotmgr.py: 53%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script type="text/javascript" src="coverage_html.js" defer></script>
+    <script src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>/Users/buh/.pyenv/versions/3.12.2/envs/es-testbed/lib/python3.12/site-packages/es_testbed/classes/entitymgrs/snapshotmgr.py</b>:
-            <span class="pc_cov">90%</span>
+            <span class="text">Coverage for </span><b>src/es_testbed/classes/entitymgrs/snapshotmgr.py</b>:
+            <span class="pc_cov">53%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -51,108 +51,102 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">35 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">32<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">3<span class="text"> missing</span></button>
+            <span class="text">32 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">18<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">14<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
             <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">1<span class="text"> partial</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_indexmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="z_396c7038a91d0266_indexmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_templatemgr_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="z_396c7038a91d0266_templatemgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
+            created at 2024-04-23 13:14 -0600
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"/>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
-            <button type="button" class="button_top_of_page" data-shortcut="0"/>
-            <button type="button" class="button_first_chunk" data-shortcut="1"/>
-            <button type="button" class="button_prev_file" data-shortcut="["/>
-            <button type="button" class="button_next_file" data-shortcut="]"/>
-            <button type="button" class="button_to_index" data-shortcut="u"/>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
+            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
+            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
+            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
+            <button type="button" class="button_prev_file" data-shortcut="["></button>
+            <button type="button" class="button_next_file" data-shortcut="]"></button>
+            <button type="button" class="button_to_index" data-shortcut="u"></button>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Snapshot Entity Manager Class"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span> <span class="key">as</span> <span class="nam">t</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">dotmap</span> <span class="key">import</span> <span class="nam">DotMap</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">elasticsearch8</span> <span class="key">import</span> <span class="nam">Elasticsearch</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">es_testbed</span><span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">es_api</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">es_testbed</span><span class="op">.</span><span class="nam">helpers</span><span class="op">.</span><span class="nam">utils</span> <span class="key">import</span> <span class="nam">getlogger</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">entitymgr</span> <span class="key">import</span> <span class="nam">EntityMgr</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">elasticsearch8</span> <span class="key">import</span> <span class="nam">Elasticsearch</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">es_testbed</span><span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">es_api</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">es_testbed</span><span class="op">.</span><span class="nam">helpers</span><span class="op">.</span><span class="nam">utils</span> <span class="key">import</span> <span class="nam">getlogger</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">entitymgr</span> <span class="key">import</span> <span class="nam">EntityMgr</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="op">.</span><span class="nam">testplan</span> <span class="key">import</span> <span class="nam">TestPlan</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="com"># pylint: disable=missing-docstring</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">class</span> <span class="nam">SnapshotMgr</span><span class="op">(</span><span class="nam">EntityMgr</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="nam">kind</span> <span class="op">=</span> <span class="str">'snapshot'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="nam">listname</span> <span class="op">=</span> <span class="str">'snapshots'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">            <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">            <span class="nam">client</span><span class="op">:</span> <span class="nam">Elasticsearch</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">            <span class="nam">plan</span><span class="op">:</span> <span class="nam">DotMap</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">            <span class="nam">autobuild</span><span class="op">:</span> <span class="nam">t</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">bool</span><span class="op">]</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__init__</span><span class="op">(</span><span class="nam">client</span><span class="op">=</span><span class="nam">client</span><span class="op">,</span> <span class="nam">plan</span><span class="op">=</span><span class="nam">plan</span><span class="op">,</span> <span class="nam">autobuild</span><span class="op">=</span><span class="nam">autobuild</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span> <span class="op">=</span> <span class="nam">getlogger</span><span class="op">(</span><span class="str">'es_testbed.SnapshotMgr'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">            <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">            <span class="nam">client</span><span class="op">:</span> <span class="nam">Elasticsearch</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">            <span class="nam">plan</span><span class="op">:</span> <span class="nam">TestPlan</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">            <span class="nam">autobuild</span><span class="op">:</span> <span class="nam">t</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">bool</span><span class="op">]</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__init__</span><span class="op">(</span><span class="nam">client</span><span class="op">=</span><span class="nam">client</span><span class="op">,</span> <span class="nam">plan</span><span class="op">=</span><span class="nam">plan</span><span class="op">,</span> <span class="nam">autobuild</span><span class="op">=</span><span class="nam">autobuild</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">kind</span> <span class="op">=</span> <span class="str">'snapshot'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span> <span class="op">=</span> <span class="nam">getlogger</span><span class="op">(</span><span class="str">'es_testbed.SnapshotMgr'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="com"># We do not autobuild in this class</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="key">def</span> <span class="nam">add</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">index</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">tier</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">        <span class="nam">msg</span> <span class="op">=</span> <span class="fst">f'</span><span class="fst">Creating snapshot of index </span><span class="op">{</span><span class="nam">index</span><span class="op">}</span><span class="fst"> and mounting in the </span><span class="op">{</span><span class="nam">tier</span><span class="op">}</span><span class="fst"> tier...</span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="nam">msg</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="nam">es_api</span><span class="op">.</span><span class="nam">do_snap</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">        <span class="nam">msg</span> <span class="op">=</span> <span class="fst">f'</span><span class="fst">Creating snapshot of index </span><span class="op">{</span><span class="nam">index</span><span class="op">}</span><span class="fst"> and mounting in the </span><span class="op">{</span><span class="nam">tier</span><span class="op">}</span><span class="fst"> tier...</span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="nam">msg</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="nam">es_api</span><span class="op">.</span><span class="nam">do_snap</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">client</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">plan</span><span class="op">.</span><span class="nam">repository</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">plan</span><span class="op">.</span><span class="nam">ilm</span><span class="op">.</span><span class="nam">repository</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">            <span class="nam">index</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">            <span class="nam">tier</span><span class="op">=</span><span class="nam">tier</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">appender</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Successfully created snapshot "%s"'</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">last</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">success</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Successfully created snapshot "%s"'</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">last</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">success</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_existing</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="str">"""Add a snapshot that's already been created, e.g. by ILM promotion"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Adding snapshot %s to list...'</span><span class="op">,</span> <span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">appender</span><span class="op">(</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">success</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Adding snapshot %s to list...'</span><span class="op">,</span> <span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">success</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="key">def</span> <span class="nam">setup</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">def</span> <span class="nam">teardown</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span> <span class="com"># We override the parent method here to speed things up.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">self</span><span class="op">.</span><span class="nam">success</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">48&#x202F;&#x219B;&#x202F;49</span><span class="annotate long">line 48 didn't jump to line 49</span></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">                <span class="nam">msg</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">                    <span class="fst">f'</span><span class="fst">Setup did not complete successfully. </span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">                    <span class="fst">f'</span><span class="fst">Manual cleanup of </span><span class="op">{</span><span class="nam">self</span><span class="op">.</span><span class="nam">kind</span><span class="op">}</span><span class="fst">s may be necessary.</span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="nam">msg</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Cleaning up any existing snapshots...'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">            <span class="nam">es_api</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">client</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kind</span><span class="op">,</span> <span class="str">','</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">)</span><span class="op">,</span> <span class="nam">repository</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">plan</span><span class="op">.</span><span class="nam">repository</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Cleanup of snapshots completed.'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">entity_list</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">failsafe</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">def</span> <span class="nam">teardown</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">self</span><span class="op">.</span><span class="nam">success</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">47&#x202F;&#x219B;&#x202F;50</span><span class="annotate long">line 47 didn't jump to line 50, because the condition on line 47 was never false</span></span></p>
+    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'No snapshots to clean up.'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">            <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Cleaning up any existing snapshots...'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="key">for</span> <span class="nam">snapshot</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">            <span class="nam">es_api</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">client</span><span class="op">,</span> <span class="str">'snapshot'</span><span class="op">,</span> <span class="nam">snapshot</span><span class="op">,</span> <span class="nam">repository</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">plan</span><span class="op">.</span><span class="nam">ilm</span><span class="op">.</span><span class="nam">repository</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Cleanup of snapshots completed.'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_indexmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_templatemgr_py.html">&#xbb; next</a>
+            <a class="nav" href="z_396c7038a91d0266_indexmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a class="nav" href="z_396c7038a91d0266_templatemgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
+            created at 2024-04-23 13:14 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,79 +1,72 @@
-************ CCoovveerraaggee ffoorr //UUsseerrss//bbuuhh//..ppyyeennvv//vveerrssiioonnss//33..1122..22//eennvvss//eess--tteessttbbeedd//lliibb//
-ppyytthhoonn33..1122//ssiittee--ppaacckkaaggeess//eess__tteessttbbeedd//ccllaasssseess//eennttiittyymmggrrss//ssnnaappsshhoottmmggrr..ppyy:: 9900%%
+************ CCoovveerraaggee ffoorr ssrrcc//eess__tteessttbbeedd//ccllaasssseess//eennttiittyymmggrrss//ssnnaappsshhoottmmggrr..ppyy:: 5533%%
 ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 3355 ssttaatteemmeennttss ?  3322 rruunn 33 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+********** 3322 ssttaatteemmeennttss ?  1188 rruunn 1144 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
+23 13:14 -0600
 _1"""Snapshot Entity Manager Class""" 
 _2import typing as t 
-_3from dotmap import DotMap 
-_4from elasticsearch8 import Elasticsearch 
-_5from es_testbed.helpers import es_api 
-_6from es_testbed.helpers.utils import getlogger 
-_7from .entitymgr import EntityMgr 
+_3from elasticsearch8 import Elasticsearch 
+_4from es_testbed.helpers import es_api 
+_5from es_testbed.helpers.utils import getlogger 
+_6from .entitymgr import EntityMgr 
+_7from ..testplan import TestPlan 
 _8 
 _9# pylint: disable=missing-docstring 
 _1_0 
 _1_1class SnapshotMgr(EntityMgr): 
-_1_2 kind = 'snapshot' 
-_1_3 listname = 'snapshots' 
-_1_4 def __init__( 
-_1_5 self, 
-_1_6 client: Elasticsearch = None, 
-_1_7 plan: DotMap = None, 
-_1_8 autobuild: t.Optional[bool] = False, 
-_1_9 ): 
-_2_0 super().__init__(client=client, plan=plan, autobuild=autobuild) 
-_2_1 self.logger = getlogger('es_testbed.SnapshotMgr') 
+_1_2 def __init__( 
+_1_3 self, 
+_1_4 client: Elasticsearch = None, 
+_1_5 plan: TestPlan = None, 
+_1_6 autobuild: t.Optional[bool] = False, 
+_1_7 ): 
+_1_8 super().__init__(client=client, plan=plan, autobuild=autobuild) 
+_1_9 self.kind = 'snapshot' 
+_2_0 self.logger = getlogger('es_testbed.SnapshotMgr') 
+_2_1 # We do not autobuild in this class 
 _2_2 
 _2_3 def add(self, index: str, tier: str) -> None: 
 _2_4 msg = f'Creating snapshot of index {index} and mounting in the {tier}
 tier...' 
 _2_5 self.logger.info(msg) 
 _2_6 es_api.do_snap( 
 _2_7 self.client, 
-_2_8 self.plan.repository, 
+_2_8 self.plan.ilm.repository, 
 _2_9 self.name, 
 _3_0 index, 
 _3_1 tier=tier 
 _3_2 ) 
-_3_3 self.appender(self.name) 
+_3_3 self.entity_list.append(self.name) 
 _3_4 self.logger.info('Successfully created snapshot "%s"', self.last) 
 _3_5 self.success = True 
 _3_6 
 _3_7 def add_existing(self, name: str) -> None: 
 _3_8 """Add a snapshot that's already been created, e.g. by ILM promotion""" 
 _3_9 self.logger.info('Adding snapshot %s to list...', name) 
-_4_0 self.appender(name) 
+_4_0 self.entity_list.append(name) 
 _4_1 self.success = True 
 _4_2 
 _4_3 def setup(self): 
 _4_4 pass 
 _4_5 
-_4_6 def teardown(self): # We override the parent method here to speed things
-up. 
-_4_7 if self.entity_list: 
-_4_8 if not self.success: 48 ↛ 49line 48 didn't jump to line 49
-_4_9 msg = ( 
-_5_0 f'Setup did not complete successfully. ' 
-_5_1 f'Manual cleanup of {self.kind}s may be necessary.' 
-_5_2 ) 
-_5_3 self.logger.warning(msg) 
-_5_4 self.logger.info('Cleaning up any existing snapshots...') 
-_5_5 es_api.delete( 
-_5_6 self.client, self.kind, ','.join(self.entity_list),
-repository=self.plan.repository) 
-_5_7 self.logger.info('Cleanup of snapshots completed.') 
-_5_8 self.entity_list = [] 
-_5_9 self.failsafe = [] 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+_4_6 def teardown(self): 
+_4_7 if not self.success: 47 ↛ 50line 47 didn't jump to line 50, because the
+condition on line 47 was never false
+_4_8 self.logger.info('No snapshots to clean up.') 
+_4_9 return 
+_5_0 self.logger.info('Cleaning up any existing snapshots...') 
+_5_1 for snapshot in self.entity_list: 
+_5_2 es_api.delete(self.client, 'snapshot', snapshot,
+repository=self.plan.ilm.repository) 
+_5_3 self.logger.info('Cleanup of snapshots completed.') 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
+23 13:14 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_e41b34ddf7b70902_templatemgr_py.html` & `es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_templatemgr_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_snapshotmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5d92fa905a1d3e20_ilm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -139,13 +139,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_snapshotmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5d92fa905a1d3e20_ilm_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3322 ssttaatteemmeennttss ?  3311 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Index Template Entity Manager Class""" 
 _2import typing as t 
 _3from dotmap import DotMap 
 _4from elasticsearch8 import Elasticsearch 
 _5from es_testbed.exceptions import ResultNotExpected 
 _6from es_testbed.helpers import es_api 
 _7from es_testbed.helpers.utils import getlogger 
@@ -63,8 +63,8 @@
 didn't jump to line 48, because the condition on line 47 was never true
 _4_8 raise ResultNotExpected( 
 _4_9 f'Unable to verify creation of index template {self.name}') 
 _5_0 self.appender(self.name) 
 _5_1 self.logger.debug('Successfully created index template: %s', self.last) 
 _5_2 self.success = True 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_f43263c25e31810d___init___py.html` & `es_testbed-0.5.3/cov_html/d_f43263c25e31810d___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5d92fa905a1d3e20___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -90,13 +90,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_5d92fa905a1d3e20___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,13 +7,13 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Make classes easier to import here""" 
 _2from .classes.base import TestBed 
 _3from .classes.plan import PlanBuilder 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_f43263c25e31810d_defaults_py.html` & `es_testbed-0.5.3/cov_html/d_f43263c25e31810d_defaults_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_5d92fa905a1d3e20_tracker_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_f43263c25e31810d_exceptions_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -209,13 +209,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_5d92fa905a1d3e20_tracker_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_f43263c25e31810d_exceptions_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3322 ssttaatteemmeennttss ?  3322 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""Default values and constants""" 
 _2import typing as t 
 _3# pylint: disable=missing-function-docstring 
 _4 
 _5EPILOG: str = 'Learn more at https://github.com/untergeek/es-testbed' 
 _6 
 _7HELP_OPTIONS: dict = {'help_option_names': ['-h', '--help']} 
@@ -132,8 +132,8 @@
 _1_1_7 } 
 _1_1_8 return {tier: phase_map[tier]} 
 _1_1_9 
 _1_2_0def ilm_force_merge(max_num_segments=1): 
 _1_2_1 """Return an ILM policy force merge action block using max_num_segments""" 
 _1_2_2 return {'forcemerge': {'max_num_segments': max_num_segments}} 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_f43263c25e31810d_exceptions_py.html` & `es_testbed-0.5.3/cov_html/d_f43263c25e31810d_exceptions_py.html`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_f43263c25e31810d_defaults_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_72ef0405fdf841ab___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -129,13 +129,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_f43263c25e31810d_defaults_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_72ef0405fdf841ab___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 88 ssttaatteemmeennttss ?  88 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""es-testbed Exceptions""" 
 _2### Parent exception 
 _3class TestbedException(Exception): 
 _4 """ 
 _5 Base class for all exceptions raised by the tool which are not Elasticsearch 
 _6 or es_client exceptions. 
 _7 """ 
@@ -51,8 +51,8 @@
 _3_7 """ 
 _3_8 
 _3_9class TimeoutException(TestbedException): 
 _4_0 """ 
 _4_1 An process took too long to complete 
 _4_2 """ 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/d_f43263c25e31810d_testbed_creator_py.html` & `es_testbed-0.5.3/cov_html/d_f43263c25e31810d_testbed_creator_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/d_f43263c25e31810d_version_py.html` & `es_testbed-0.5.3/cov_html/d_f43263c25e31810d_version_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_72ef0405fdf841ab_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a44f0ac069e85531___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -89,13 +89,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_72ef0405fdf841ab_utils_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a44f0ac069e85531___init___py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -7,12 +7,12 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 11 ssttaatteemmeennttss ?  00 rruunn 11 mmiissssiinngg 00 eexxcclluuddeedd 00 ppaarrttiiaall **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
 _1"""es-testbed Version""" 
 _2__version__ = '0.5.0' 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-24 22:41 -0600
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/favicon_32.png` & `es_testbed-0.5.3/cov_html/favicon_32.png`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/function_index.html` & `es_testbed-0.5.3/cov_html/function_index.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/index.html` & `es_testbed-0.5.3/cov_html/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -262,19 +262,19 @@
                 <td>0</td>
                 <td>0</td>
                 <td class="right" data-ratio="0 0">100%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_72ef0405fdf841ab_es_api_py.html">/Users/buh/.pyenv/versions/3.12.2/envs/es-testbed/lib/python3.12/site-packages/es_testbed/helpers/es_api.py</a></td>
                 <td>213</td>
-                <td>52</td>
+                <td>54</td>
                 <td>0</td>
                 <td>48</td>
                 <td>12</td>
-                <td class="right" data-ratio="195 261">75%</td>
+                <td class="right" data-ratio="193 261">74%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_72ef0405fdf841ab_utils_py.html">/Users/buh/.pyenv/versions/3.12.2/envs/es-testbed/lib/python3.12/site-packages/es_testbed/helpers/utils.py</a></td>
                 <td>102</td>
                 <td>11</td>
                 <td>0</td>
                 <td>46</td>
@@ -435,31 +435,31 @@
                 <td class="right" data-ratio="96 96">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td>1649</td>
-                <td>186</td>
+                <td>188</td>
                 <td>0</td>
                 <td>436</td>
                 <td>69</td>
-                <td class="right" data-ratio="1800 2085">86%</td>
+                <td class="right" data-ratio="1798 2085">86%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-24 22:41 -0600
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_17bd492d087794b9_test_utils_py.html"/>
         <a id="nextFileLink" class="nav" href="d_f43263c25e31810d___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 ************ CCoovveerraaggee rreeppoorrtt:: 8866%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x b p c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-24 22:41 -0600
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-25 19:21 -0600
 MMoodduullee                     ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd bbrraanncchheess ppaarrttiiaall ccoovveerraaggee
 _/_U_s_e_r_s_/_b_u_h_/_._p_y_e_n_v_/
 _v_e_r_s_i_o_n_s_/_3_._1_2_._2_/_e_n_v_s_/_e_s_-
 _t_e_s_t_b_e_d_/_l_i_b_/_p_y_t_h_o_n_3_._1_2_/    2          0       0        0        0       100%
 _s_i_t_e_-_p_a_c_k_a_g_e_s_/_e_s___t_e_s_t_b_e_d_/
 _____i_n_i_t_____._p_y
 _/_U_s_e_r_s_/_b_u_h_/_._p_y_e_n_v_/
@@ -125,15 +125,15 @@
 _/_U_s_e_r_s_/_b_u_h_/_._p_y_e_n_v_/
 _v_e_r_s_i_o_n_s_/_3_._1_2_._2_/_e_n_v_s_/_e_s_-
 _t_e_s_t_b_e_d_/_l_i_b_/_p_y_t_h_o_n_3_._1_2_/    0          0       0        0        0       100%
 _s_i_t_e_-_p_a_c_k_a_g_e_s_/_e_s___t_e_s_t_b_e_d_/
 _h_e_l_p_e_r_s_/_____i_n_i_t_____._p_y
 _/_U_s_e_r_s_/_b_u_h_/_._p_y_e_n_v_/
 _v_e_r_s_i_o_n_s_/_3_._1_2_._2_/_e_n_v_s_/_e_s_-
-_t_e_s_t_b_e_d_/_l_i_b_/_p_y_t_h_o_n_3_._1_2_/    213        52      0        48       12      75%
+_t_e_s_t_b_e_d_/_l_i_b_/_p_y_t_h_o_n_3_._1_2_/    213        54      0        48       12      74%
 _s_i_t_e_-_p_a_c_k_a_g_e_s_/_e_s___t_e_s_t_b_e_d_/
 _h_e_l_p_e_r_s_/_e_s___a_p_i_._p_y
 _/_U_s_e_r_s_/_b_u_h_/_._p_y_e_n_v_/
 _v_e_r_s_i_o_n_s_/_3_._1_2_._2_/_e_n_v_s_/_e_s_-
 _t_e_s_t_b_e_d_/_l_i_b_/_p_y_t_h_o_n_3_._1_2_/    102        11      0        46       5       86%
 _s_i_t_e_-_p_a_c_k_a_g_e_s_/_e_s___t_e_s_t_b_e_d_/
 _h_e_l_p_e_r_s_/_u_t_i_l_s_._p_y
@@ -165,10 +165,10 @@
 _t_e_s_t_s_/_u_n_i_t_/_____i_n_i_t_____._p_y     0          0       0        0        0       100%
 _t_e_s_t_s_/_u_n_i_t_/_t_e_s_t___c_l_s___i_l_m_._p_y 0          0       0        0        0       100%
 _t_e_s_t_s_/_u_n_i_t_/                0          0       0        0        0       100%
 _t_e_s_t___c_l_s___t_r_a_c_k_e_r_._p_y
 _t_e_s_t_s_/_u_n_i_t_/                18         0       0        2        0       100%
 _t_e_s_t___d_e_f_a_u_l_t_s_._p_y
 _t_e_s_t_s_/_u_n_i_t_/_t_e_s_t___u_t_i_l_s_._p_y   70         0       0        26       0       100%
-Total                      1649       186     0        436      69      86%
+Total                      1649       188     0        436      69      86%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-24 22:41 -0600
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/keybd_closed.png` & `es_testbed-0.5.3/cov_html/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/keybd_open.png` & `es_testbed-0.5.3/cov_html/keybd_open.png`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/status.json` & `es_testbed-0.5.3/cov_html/status.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899683830171635%*

 * *Differences: {"'files'": "{'d_72ef0405fdf841ab_es_api_py': {'hash': '1d69a62e4df68299f2c394321ade39af', "*

 * *            "'index': {'nums': {insert: [(4, 54)], delete: [4]}}}}",*

 * * "'globals'": "'9045ecaa451a4a7c3ab69dbf4ada66ae'"}*

```diff
@@ -184,23 +184,23 @@
                     0,
                     0
                 ],
                 "relative_filename": "/Users/buh/.pyenv/versions/3.12.2/envs/es-testbed/lib/python3.12/site-packages/es_testbed/helpers/__init__.py"
             }
         },
         "d_72ef0405fdf841ab_es_api_py": {
-            "hash": "dc8bc42c8531b242872ea3957464a8f8",
+            "hash": "1d69a62e4df68299f2c394321ade39af",
             "index": {
                 "html_filename": "d_72ef0405fdf841ab_es_api_py.html",
                 "nums": [
                     0,
                     1,
                     213,
                     0,
-                    52,
+                    54,
                     48,
                     12,
                     14
                 ],
                 "relative_filename": "/Users/buh/.pyenv/versions/3.12.2/envs/es-testbed/lib/python3.12/site-packages/es_testbed/helpers/es_api.py"
             }
         },
@@ -695,11 +695,11 @@
                     0
                 ],
                 "relative_filename": "/Users/buh/.pyenv/versions/3.12.2/envs/es-testbed/lib/python3.12/site-packages/es_testbed/version.py"
             }
         }
     },
     "format": 2,
-    "globals": "1c457a5997d38e02eaaee9cd2740a6e2",
+    "globals": "9045ecaa451a4a7c3ab69dbf4ada66ae",
     "note": "This file is an internal implementation detail to speed up HTML report generation. Its format can change at any time. You might be looking for the JSON report: https://coverage.rtfd.io/cmd.html#cmd-json",
     "version": "7.4.4"
 }
```

### Comparing `es_testbed-0.5.0/cov_html/style.css` & `es_testbed-0.5.3/cov_html/style.css`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_17bd492d087794b9___init___py.html` & `es_testbed-0.5.3/cov_html/z_17bd492d087794b9___init___py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_17bd492d087794b9_test_cls_ilm_py.html` & `es_testbed-0.5.3/cov_html/z_17bd492d087794b9_test_cls_ilm_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_17bd492d087794b9_test_cls_tracker_py.html` & `es_testbed-0.5.3/cov_html/z_17bd492d087794b9_test_cls_tracker_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_17bd492d087794b9_test_defaults_py.html` & `es_testbed-0.5.3/cov_html/z_17bd492d087794b9_test_defaults_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_17bd492d087794b9_test_utils_py.html` & `es_testbed-0.5.3/cov_html/z_17bd492d087794b9_test_utils_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_396c7038a91d0266___init___py.html` & `es_testbed-0.5.3/cov_html/z_396c7038a91d0266___init___py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_396c7038a91d0266_componentmgr_py.html` & `es_testbed-0.5.3/cov_html/z_396c7038a91d0266_componentmgr_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_396c7038a91d0266_data_streammgr_py.html` & `es_testbed-0.5.3/cov_html/z_396c7038a91d0266_data_streammgr_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_396c7038a91d0266_entitymgr_py.html` & `es_testbed-0.5.3/cov_html/z_396c7038a91d0266_entitymgr_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_396c7038a91d0266_ilmmgr_py.html` & `es_testbed-0.5.3/cov_html/z_396c7038a91d0266_ilmmgr_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_396c7038a91d0266_indexmgr_py.html` & `es_testbed-0.5.3/cov_html/z_396c7038a91d0266_indexmgr_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_396c7038a91d0266_snapshotmgr_py.html` & `es_testbed-0.5.3/cov_html/d_e41b34ddf7b70902_snapshotmgr_py.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
-<html lang="en">
+<html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/es_testbed/classes/entitymgrs/snapshotmgr.py: 53%</title>
+    <title>Coverage for /Users/buh/.pyenv/versions/3.12.2/envs/es-testbed/lib/python3.12/site-packages/es_testbed/classes/entitymgrs/snapshotmgr.py: 90%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
-    <script src="coverage_html.js" defer></script>
+    <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/es_testbed/classes/entitymgrs/snapshotmgr.py</b>:
-            <span class="pc_cov">53%</span>
+            <span class="text">Coverage for </span><b>/Users/buh/.pyenv/versions/3.12.2/envs/es-testbed/lib/python3.12/site-packages/es_testbed/classes/entitymgrs/snapshotmgr.py</b>:
+            <span class="pc_cov">90%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
-                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts">
+                <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
                 <p class="legend">Shortcuts on this page</p>
                 <div class="keyhelp">
                     <p>
                         <kbd>r</kbd>
                         <kbd>m</kbd>
@@ -51,102 +51,108 @@
                     <p>
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
-            <span class="text">32 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">18<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">14<span class="text"> missing</span></button>
+            <span class="text">35 statements &nbsp;</span>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">32<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">3<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
             <button type="button" class="par run show_par button_toggle_par" value="par" data-shortcut="p" title="Toggle lines partially run">1<span class="text"> partial</span></button>
         </h2>
         <p class="text">
-            <a id="prevFileLink" class="nav" href="z_396c7038a91d0266_indexmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_indexmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a id="nextFileLink" class="nav" href="z_396c7038a91d0266_templatemgr_py.html">&#xbb; next</a>
+            <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_templatemgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-23 13:14 -0600
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-25 19:21 -0600
         </p>
         <aside class="hidden">
-            <button type="button" class="button_next_chunk" data-shortcut="j"></button>
-            <button type="button" class="button_prev_chunk" data-shortcut="k"></button>
-            <button type="button" class="button_top_of_page" data-shortcut="0"></button>
-            <button type="button" class="button_first_chunk" data-shortcut="1"></button>
-            <button type="button" class="button_prev_file" data-shortcut="["></button>
-            <button type="button" class="button_next_file" data-shortcut="]"></button>
-            <button type="button" class="button_to_index" data-shortcut="u"></button>
-            <button type="button" class="button_show_hide_help" data-shortcut="?"></button>
+            <button type="button" class="button_next_chunk" data-shortcut="j"/>
+            <button type="button" class="button_prev_chunk" data-shortcut="k"/>
+            <button type="button" class="button_top_of_page" data-shortcut="0"/>
+            <button type="button" class="button_first_chunk" data-shortcut="1"/>
+            <button type="button" class="button_prev_file" data-shortcut="["/>
+            <button type="button" class="button_next_file" data-shortcut="]"/>
+            <button type="button" class="button_to_index" data-shortcut="u"/>
+            <button type="button" class="button_show_hide_help" data-shortcut="?"/>
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="str">"""Snapshot Entity Manager Class"""</span>&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t"><span class="key">import</span> <span class="nam">typing</span> <span class="key">as</span> <span class="nam">t</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">elasticsearch8</span> <span class="key">import</span> <span class="nam">Elasticsearch</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">es_testbed</span><span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">es_api</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">es_testbed</span><span class="op">.</span><span class="nam">helpers</span><span class="op">.</span><span class="nam">utils</span> <span class="key">import</span> <span class="nam">getlogger</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">entitymgr</span> <span class="key">import</span> <span class="nam">EntityMgr</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="op">.</span><span class="nam">testplan</span> <span class="key">import</span> <span class="nam">TestPlan</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="key">from</span> <span class="nam">dotmap</span> <span class="key">import</span> <span class="nam">DotMap</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">elasticsearch8</span> <span class="key">import</span> <span class="nam">Elasticsearch</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="key">from</span> <span class="nam">es_testbed</span><span class="op">.</span><span class="nam">helpers</span> <span class="key">import</span> <span class="nam">es_api</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="key">from</span> <span class="nam">es_testbed</span><span class="op">.</span><span class="nam">helpers</span><span class="op">.</span><span class="nam">utils</span> <span class="key">import</span> <span class="nam">getlogger</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="op">.</span><span class="nam">entitymgr</span> <span class="key">import</span> <span class="nam">EntityMgr</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="com"># pylint: disable=missing-docstring</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="key">class</span> <span class="nam">SnapshotMgr</span><span class="op">(</span><span class="nam">EntityMgr</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">            <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">            <span class="nam">client</span><span class="op">:</span> <span class="nam">Elasticsearch</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">            <span class="nam">plan</span><span class="op">:</span> <span class="nam">TestPlan</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">            <span class="nam">autobuild</span><span class="op">:</span> <span class="nam">t</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">bool</span><span class="op">]</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__init__</span><span class="op">(</span><span class="nam">client</span><span class="op">=</span><span class="nam">client</span><span class="op">,</span> <span class="nam">plan</span><span class="op">=</span><span class="nam">plan</span><span class="op">,</span> <span class="nam">autobuild</span><span class="op">=</span><span class="nam">autobuild</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">kind</span> <span class="op">=</span> <span class="str">'snapshot'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span> <span class="op">=</span> <span class="nam">getlogger</span><span class="op">(</span><span class="str">'es_testbed.SnapshotMgr'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="com"># We do not autobuild in this class</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">    <span class="nam">kind</span> <span class="op">=</span> <span class="str">'snapshot'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="nam">listname</span> <span class="op">=</span> <span class="str">'snapshots'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">            <span class="nam">self</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">            <span class="nam">client</span><span class="op">:</span> <span class="nam">Elasticsearch</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">            <span class="nam">plan</span><span class="op">:</span> <span class="nam">DotMap</span> <span class="op">=</span> <span class="key">None</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">            <span class="nam">autobuild</span><span class="op">:</span> <span class="nam">t</span><span class="op">.</span><span class="nam">Optional</span><span class="op">[</span><span class="nam">bool</span><span class="op">]</span> <span class="op">=</span> <span class="key">False</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">        <span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="nam">super</span><span class="op">(</span><span class="op">)</span><span class="op">.</span><span class="nam">__init__</span><span class="op">(</span><span class="nam">client</span><span class="op">=</span><span class="nam">client</span><span class="op">,</span> <span class="nam">plan</span><span class="op">=</span><span class="nam">plan</span><span class="op">,</span> <span class="nam">autobuild</span><span class="op">=</span><span class="nam">autobuild</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span> <span class="op">=</span> <span class="nam">getlogger</span><span class="op">(</span><span class="str">'es_testbed.SnapshotMgr'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">    <span class="key">def</span> <span class="nam">add</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">index</span><span class="op">:</span> <span class="nam">str</span><span class="op">,</span> <span class="nam">tier</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">        <span class="nam">msg</span> <span class="op">=</span> <span class="fst">f'</span><span class="fst">Creating snapshot of index </span><span class="op">{</span><span class="nam">index</span><span class="op">}</span><span class="fst"> and mounting in the </span><span class="op">{</span><span class="nam">tier</span><span class="op">}</span><span class="fst"> tier...</span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="nam">msg</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="nam">es_api</span><span class="op">.</span><span class="nam">do_snap</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">        <span class="nam">msg</span> <span class="op">=</span> <span class="fst">f'</span><span class="fst">Creating snapshot of index </span><span class="op">{</span><span class="nam">index</span><span class="op">}</span><span class="fst"> and mounting in the </span><span class="op">{</span><span class="nam">tier</span><span class="op">}</span><span class="fst"> tier...</span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="nam">msg</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t">        <span class="nam">es_api</span><span class="op">.</span><span class="nam">do_snap</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">client</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">plan</span><span class="op">.</span><span class="nam">ilm</span><span class="op">.</span><span class="nam">repository</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">plan</span><span class="op">.</span><span class="nam">repository</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">name</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">            <span class="nam">index</span><span class="op">,</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">            <span class="nam">tier</span><span class="op">=</span><span class="nam">tier</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Successfully created snapshot "%s"'</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">last</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">success</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">appender</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Successfully created snapshot "%s"'</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">last</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">success</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">    <span class="key">def</span> <span class="nam">add_existing</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">name</span><span class="op">:</span> <span class="nam">str</span><span class="op">)</span> <span class="op">-></span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">        <span class="str">"""Add a snapshot that's already been created, e.g. by ILM promotion"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Adding snapshot %s to list...'</span><span class="op">,</span> <span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">.</span><span class="nam">append</span><span class="op">(</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">success</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Adding snapshot %s to list...'</span><span class="op">,</span> <span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">appender</span><span class="op">(</span><span class="nam">name</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">success</span> <span class="op">=</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="run"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">    <span class="key">def</span> <span class="nam">setup</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
     <p class="mis show_mis"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">        <span class="key">pass</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">def</span> <span class="nam">teardown</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="par run show_par"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">self</span><span class="op">.</span><span class="nam">success</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">47&#x202F;&#x219B;&#x202F;50</span><span class="annotate long">line 47 didn't jump to line 50, because the condition on line 47 was never false</span></span></p>
-    <p class="run"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'No snapshots to clean up.'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">            <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Cleaning up any existing snapshots...'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="key">for</span> <span class="nam">snapshot</span> <span class="key">in</span> <span class="nam">self</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">            <span class="nam">es_api</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">client</span><span class="op">,</span> <span class="str">'snapshot'</span><span class="op">,</span> <span class="nam">snapshot</span><span class="op">,</span> <span class="nam">repository</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">plan</span><span class="op">.</span><span class="nam">ilm</span><span class="op">.</span><span class="nam">repository</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Cleanup of snapshots completed.'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t">    <span class="key">def</span> <span class="nam">teardown</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span> <span class="com"># We override the parent method here to speed things up.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="par run show_par"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">self</span><span class="op">.</span><span class="nam">success</span><span class="op">:</span>&nbsp;</span><span class="r"><span class="annotate short">48&#x202F;&#x219B;&#x202F;49</span><span class="annotate long">line 48 didn't jump to line 49</span></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">                <span class="nam">msg</span> <span class="op">=</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">                    <span class="fst">f'</span><span class="fst">Setup did not complete successfully. </span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">                    <span class="fst">f'</span><span class="fst">Manual cleanup of </span><span class="op">{</span><span class="nam">self</span><span class="op">.</span><span class="nam">kind</span><span class="op">}</span><span class="fst">s may be necessary.</span><span class="fst">'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">                <span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="mis show_mis"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="nam">msg</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Cleaning up any existing snapshots...'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">            <span class="nam">es_api</span><span class="op">.</span><span class="nam">delete</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">client</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">kind</span><span class="op">,</span> <span class="str">','</span><span class="op">.</span><span class="nam">join</span><span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">entity_list</span><span class="op">)</span><span class="op">,</span> <span class="nam">repository</span><span class="op">=</span><span class="nam">self</span><span class="op">.</span><span class="nam">plan</span><span class="op">.</span><span class="nam">repository</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">'Cleanup of snapshots completed.'</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">entity_list</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">failsafe</span> <span class="op">=</span> <span class="op">[</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
-            <a class="nav" href="z_396c7038a91d0266_indexmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
-            <a class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
-            <a class="nav" href="z_396c7038a91d0266_templatemgr_py.html">&#xbb; next</a>
+            <a id="prevFileLink" class="nav" href="d_e41b34ddf7b70902_indexmgr_py.html">&#xab; prev</a> &nbsp; &nbsp;
+            <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
+            <a id="nextFileLink" class="nav" href="d_e41b34ddf7b70902_templatemgr_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
-            <a class="nav" href="https://coverage.readthedocs.io/en/7.5.0">coverage.py v7.5.0</a>,
-            created at 2024-04-23 13:14 -0600
+            <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
+            created at 2024-04-25 19:21 -0600
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,72 +1,79 @@
-************ CCoovveerraaggee ffoorr ssrrcc//eess__tteessttbbeedd//ccllaasssseess//eennttiittyymmggrrss//ssnnaappsshhoottmmggrr..ppyy:: 5533%%
+************ CCoovveerraaggee ffoorr //UUsseerrss//bbuuhh//..ppyyeennvv//vveerrssiioonnss//33..1122..22//eennvvss//eess--tteessttbbeedd//lliibb//
+ppyytthhoonn33..1122//ssiittee--ppaacckkaaggeess//eess__tteessttbbeedd//ccllaasssseess//eennttiittyymmggrrss//ssnnaappsshhoottmmggrr..ppyy:: 9900%%
 ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x p   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 3322 ssttaatteemmeennttss ?  1188 rruunn 1144 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-23 13:14 -0600
+********** 3355 ssttaatteemmeennttss ?  3322 rruunn 33 mmiissssiinngg 00 eexxcclluuddeedd 11 ppaarrttiiaall **********
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+25 19:21 -0600
 _1"""Snapshot Entity Manager Class""" 
 _2import typing as t 
-_3from elasticsearch8 import Elasticsearch 
-_4from es_testbed.helpers import es_api 
-_5from es_testbed.helpers.utils import getlogger 
-_6from .entitymgr import EntityMgr 
-_7from ..testplan import TestPlan 
+_3from dotmap import DotMap 
+_4from elasticsearch8 import Elasticsearch 
+_5from es_testbed.helpers import es_api 
+_6from es_testbed.helpers.utils import getlogger 
+_7from .entitymgr import EntityMgr 
 _8 
 _9# pylint: disable=missing-docstring 
 _1_0 
 _1_1class SnapshotMgr(EntityMgr): 
-_1_2 def __init__( 
-_1_3 self, 
-_1_4 client: Elasticsearch = None, 
-_1_5 plan: TestPlan = None, 
-_1_6 autobuild: t.Optional[bool] = False, 
-_1_7 ): 
-_1_8 super().__init__(client=client, plan=plan, autobuild=autobuild) 
-_1_9 self.kind = 'snapshot' 
-_2_0 self.logger = getlogger('es_testbed.SnapshotMgr') 
-_2_1 # We do not autobuild in this class 
+_1_2 kind = 'snapshot' 
+_1_3 listname = 'snapshots' 
+_1_4 def __init__( 
+_1_5 self, 
+_1_6 client: Elasticsearch = None, 
+_1_7 plan: DotMap = None, 
+_1_8 autobuild: t.Optional[bool] = False, 
+_1_9 ): 
+_2_0 super().__init__(client=client, plan=plan, autobuild=autobuild) 
+_2_1 self.logger = getlogger('es_testbed.SnapshotMgr') 
 _2_2 
 _2_3 def add(self, index: str, tier: str) -> None: 
 _2_4 msg = f'Creating snapshot of index {index} and mounting in the {tier}
 tier...' 
 _2_5 self.logger.info(msg) 
 _2_6 es_api.do_snap( 
 _2_7 self.client, 
-_2_8 self.plan.ilm.repository, 
+_2_8 self.plan.repository, 
 _2_9 self.name, 
 _3_0 index, 
 _3_1 tier=tier 
 _3_2 ) 
-_3_3 self.entity_list.append(self.name) 
+_3_3 self.appender(self.name) 
 _3_4 self.logger.info('Successfully created snapshot "%s"', self.last) 
 _3_5 self.success = True 
 _3_6 
 _3_7 def add_existing(self, name: str) -> None: 
 _3_8 """Add a snapshot that's already been created, e.g. by ILM promotion""" 
 _3_9 self.logger.info('Adding snapshot %s to list...', name) 
-_4_0 self.entity_list.append(name) 
+_4_0 self.appender(name) 
 _4_1 self.success = True 
 _4_2 
 _4_3 def setup(self): 
 _4_4 pass 
 _4_5 
-_4_6 def teardown(self): 
-_4_7 if not self.success: 47 ↛ 50line 47 didn't jump to line 50, because the
-condition on line 47 was never false
-_4_8 self.logger.info('No snapshots to clean up.') 
-_4_9 return 
-_5_0 self.logger.info('Cleaning up any existing snapshots...') 
-_5_1 for snapshot in self.entity_list: 
-_5_2 es_api.delete(self.client, 'snapshot', snapshot,
-repository=self.plan.ilm.repository) 
-_5_3 self.logger.info('Cleanup of snapshots completed.') 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._5_._0, created at 2024-04-
-23 13:14 -0600
+_4_6 def teardown(self): # We override the parent method here to speed things
+up. 
+_4_7 if self.entity_list: 
+_4_8 if not self.success: 48 ↛ 49line 48 didn't jump to line 49
+_4_9 msg = ( 
+_5_0 f'Setup did not complete successfully. ' 
+_5_1 f'Manual cleanup of {self.kind}s may be necessary.' 
+_5_2 ) 
+_5_3 self.logger.warning(msg) 
+_5_4 self.logger.info('Cleaning up any existing snapshots...') 
+_5_5 es_api.delete( 
+_5_6 self.client, self.kind, ','.join(self.entity_list),
+repository=self.plan.repository) 
+_5_7 self.logger.info('Cleanup of snapshots completed.') 
+_5_8 self.entity_list = [] 
+_5_9 self.failsafe = [] 
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+25 19:21 -0600
```

### Comparing `es_testbed-0.5.0/cov_html/z_396c7038a91d0266_templatemgr_py.html` & `es_testbed-0.5.3/cov_html/z_396c7038a91d0266_templatemgr_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_549446c4d0fe5c90___init___py.html` & `es_testbed-0.5.3/cov_html/z_549446c4d0fe5c90___init___py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_549446c4d0fe5c90_es_api_py.html` & `es_testbed-0.5.3/cov_html/z_549446c4d0fe5c90_es_api_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_549446c4d0fe5c90_utils_py.html` & `es_testbed-0.5.3/cov_html/z_549446c4d0fe5c90_utils_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_6c086c3223cbe98b___init___py.html` & `es_testbed-0.5.3/cov_html/z_6c086c3223cbe98b___init___py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_6c086c3223cbe98b_args_py.html` & `es_testbed-0.5.3/cov_html/z_6c086c3223cbe98b_args_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_6c086c3223cbe98b_base_py.html` & `es_testbed-0.5.3/cov_html/z_6c086c3223cbe98b_base_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_6c086c3223cbe98b_ilm_py.html` & `es_testbed-0.5.3/cov_html/z_6c086c3223cbe98b_ilm_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_6c086c3223cbe98b_testplan_py.html` & `es_testbed-0.5.3/cov_html/z_6c086c3223cbe98b_testplan_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_6c086c3223cbe98b_tracker_py.html` & `es_testbed-0.5.3/cov_html/z_6c086c3223cbe98b_tracker_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_712229651729ba66___init___py.html` & `es_testbed-0.5.3/cov_html/z_712229651729ba66___init___py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_712229651729ba66_alias_py.html` & `es_testbed-0.5.3/cov_html/z_712229651729ba66_alias_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_712229651729ba66_data_stream_py.html` & `es_testbed-0.5.3/cov_html/z_712229651729ba66_data_stream_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_712229651729ba66_entity_py.html` & `es_testbed-0.5.3/cov_html/z_712229651729ba66_entity_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_712229651729ba66_index_py.html` & `es_testbed-0.5.3/cov_html/z_712229651729ba66_index_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_95d9102b3aa62d65___init___py.html` & `es_testbed-0.5.3/cov_html/z_95d9102b3aa62d65___init___py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_95d9102b3aa62d65_defaults_py.html` & `es_testbed-0.5.3/cov_html/z_95d9102b3aa62d65_defaults_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_95d9102b3aa62d65_exceptions_py.html` & `es_testbed-0.5.3/cov_html/z_95d9102b3aa62d65_exceptions_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_95d9102b3aa62d65_version_py.html` & `es_testbed-0.5.3/cov_html/z_95d9102b3aa62d65_version_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_a40f6d277e0496df___init___py.html` & `es_testbed-0.5.3/cov_html/z_a40f6d277e0496df___init___py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_a40f6d277e0496df_test_basic_data_streams_py.html` & `es_testbed-0.5.3/cov_html/z_a40f6d277e0496df_test_basic_data_streams_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_a40f6d277e0496df_test_basic_indices_py.html` & `es_testbed-0.5.3/cov_html/z_a40f6d277e0496df_test_basic_indices_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_a40f6d277e0496df_test_testbed_py.html` & `es_testbed-0.5.3/cov_html/z_a40f6d277e0496df_test_testbed_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_a44f0ac069e85531___init___py.html` & `es_testbed-0.5.3/cov_html/z_a44f0ac069e85531___init___py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/cov_html/z_a44f0ac069e85531_conftest_py.html` & `es_testbed-0.5.3/cov_html/z_a44f0ac069e85531_conftest_py.html`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/src/es_testbed/defaults.py` & `es_testbed-0.5.3/src/es_testbed/defaults.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Default values and constants"""
+
 import typing as t
+
 # pylint: disable=missing-function-docstring
 
 EPILOG: str = 'Learn more at https://github.com/untergeek/es-testbed'
 
 HELP_OPTIONS: dict = {'help_option_names': ['-h', '--help']}
 
 ARGSCLASSES: list = ['IlmBuilder', 'IlmExplain', 'TestPlan']
@@ -15,17 +17,15 @@
 
 MAPPING: dict = {
     'properties': {
         '@timestamp': {'type': 'date'},
         'message': {'type': 'keyword'},
         'number': {'type': 'long'},
         'nested': {'properties': {'key': {'type': 'keyword'}}},
-        'deep': {'properties': {'l1': {'properties': {'l2': {
-            'properties': {'l3': {'type': 'keyword'}}}}}}
-        }
+        'deep': {'properties': {'l1': {'properties': {'l2': {'properties': {'l3': {'type': 'keyword'}}}}}}},
     }
 }
 
 NAMEMAPPER: t.Dict[str, str] = {
     'index': 'idx',
     'data_stream': 'ds',
     'component': 'cmp',
@@ -43,80 +43,73 @@
 }
 
 TESTPLAN: dict = {
     'type': 'indices',
     'prefix': 'es-testbed',
     'repository': None,
     'rollover_alias': None,
-    'ilm': {
-        'enabled': False,
-        'tiers': ['hot', 'delete'],
-        'forcemerge': False,
-        'max_num_segments': 1
-    },
+    'ilm': {'enabled': False, 'tiers': ['hot', 'delete'], 'forcemerge': False, 'max_num_segments': 1},
     'defaults': {
         'entity_count': 3,
         'docs': 10,
         'match': True,
         'searchable': None,
     },
     'entities': [],
 }
 
 TIER: dict = {
-    'hot': {
-        'pref': 'data_hot,data_content'
-    },
-    'warm': {
-        'pref': 'data_warm,data_hot,data_content'
-    },
+    'hot': {'pref': 'data_hot,data_content'},
+    'warm': {'pref': 'data_warm,data_hot,data_content'},
     'cold': {
         'pref': 'data_cold,data_warm,data_hot,data_content',
         'prefix': 'restored',
         'storage': 'full_copy',
     },
     'frozen': {
         'pref': 'data_frozen',
         'prefix': 'partial',
         'storage': 'shared_cache',
-    }
+    },
 }
 
 TIMEOUT_DEFAULT: str = '30'
 TIMEOUT_ENVVAR: str = 'ES_TESTBED_TIMEOUT'
 
-IlmPhase: t.TypeAlias = (
-    t.Dict[str, t.Union[str, t.Dict[str, str], t.Dict[str, t.Dict[str, t.Dict[str, str]]]]]
-)
+IlmPhase: t.TypeAlias = t.Dict[str, t.Union[str, t.Dict[str, str], t.Dict[str, t.Dict[str, t.Dict[str, str]]]]]
+
 
 def ilmhot() -> IlmPhase:
-    return {
-        'actions': {
-            'rollover': {
-                'max_primary_shard_size': '1gb',
-                'max_age': '1d'
-            }
-        }
-    }
+    return {'actions': {'rollover': {'max_primary_shard_size': '1gb', 'max_age': '1d'}}}
+
+
 def ilmwarm() -> IlmPhase:
     return {'min_age': '2d', 'actions': {}}
+
+
 def ilmcold() -> IlmPhase:
-    return  {'min_age': '3d', 'actions': {}}
+    return {'min_age': '3d', 'actions': {}}
+
+
 def ilmfrozen() -> IlmPhase:
     return {'min_age': '4d', 'actions': {}}
+
+
 def ilmdelete() -> IlmPhase:
     return {'min_age': '5d', 'actions': {'delete': {}}}
 
+
 def ilm_phase(tier):
     """Return the default phase step based on 'tier'"""
     phase_map = {
         'hot': ilmhot(),
         'warm': ilmwarm(),
         'cold': ilmcold(),
         'frozen': ilmfrozen(),
         'delete': ilmdelete(),
     }
     return {tier: phase_map[tier]}
 
+
 def ilm_force_merge(max_num_segments=1):
     """Return an ILM policy force merge action block using max_num_segments"""
     return {'forcemerge': {'max_num_segments': max_num_segments}}
```

### Comparing `es_testbed-0.5.0/src/es_testbed/exceptions.py` & `es_testbed-0.5.3/src/es_testbed/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 """es-testbed Exceptions"""
-### Parent exception
-class TestbedException(Exception):
+
+
+class TestbedException(Exception):  # parent exception
     """
     Base class for all exceptions raised by the tool which are not Elasticsearch
     or es_client exceptions.
     """
-###
+
+
 class MissingArgument(TestbedException):
     """
     An expected argument was missing
     """
 
+
 class NameChanged(TestbedException):
     """
     An index name changed, likely due to an ILM promotion to cold or frozen
     """
 
+
 class ResultNotExpected(TestbedException):
     """
     The result we got is not what we expected
     """
 
+
 class TestbedFailure(TestbedException):
     """
     Whatever we were trying to do failed.
     """
 
+
 class TestbedMisconfig(TestbedException):
     """
     There was a misconfiguration encountered.
     """
 
+
 class TestPlanMisconfig(TestbedMisconfig):
     """
     There was a misconfiguration in a TestPlan.
     """
 
+
 class TimeoutException(TestbedException):
     """
     An process took too long to complete
     """
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/base.py` & `es_testbed-0.5.3/src/es_testbed/classes/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 """Base TestBed Class"""
+
 import typing as t
 from datetime import datetime, timezone
 from dotmap import DotMap
 from elasticsearch8 import Elasticsearch
 from es_testbed.helpers.es_api import delete
 from es_testbed.helpers.utils import getlogger
 from .plan import PlanBuilder
 from .tracker import Tracker
 
 # pylint: disable=broad-exception-caught
 
+
 class TestBed:
     """Base TestBed Class"""
+
     __test__ = False
-    def __init__(
-            self,
-            client: Elasticsearch = None,
-            plan: DotMap = None,
-            autobuild: t.Optional[bool] = False,
-        ):
+
+    def __init__(self, client: Elasticsearch = None, plan: DotMap = None, autobuild: t.Optional[bool] = False):
         """Initialize"""
         self.logger = getlogger('es_testbed.TestBed')
         self.client = client
         if plan is None:
-            plan = PlanBuilder() # Use defaults
+            plan = PlanBuilder().plan  # Use defaults
         self.plan = plan
-        self.tracker = Tracker(
-            client=client, plan=plan, autobuild=autobuild)
+        self.tracker = Tracker(client=client, plan=plan, autobuild=autobuild)
 
     def failsafe_teardown(self):
         """Fallback method to delete things still remaining"""
         items = ['index', 'data_stream', 'snapshot', 'template', 'component', 'ilm']
         for i in items:
             if i == 'snapshot':
                 snaps = ','.join(self.plan.failsafes[i])
@@ -57,13 +55,19 @@
         self.tracker.setup()
         end = datetime.now(timezone.utc)
         self.logger.info('Testbed setup elapsed time: %s', (end - start).total_seconds())
 
     def teardown(self):
         """Tear down anything we created"""
         start = datetime.now(timezone.utc)
-        self.tracker.teardown()
+        try:
+            self.tracker.teardown()
+        except Exception as err:
+            self.logger.error('An exception occurred during teardown: %s', err)
+            self.logger.info('Remaining entities: %s', self.plan)
+            self.logger.info('Attempting failsafe cleanup...')
+            self.failsafe_teardown()
         # Do we clean up the failsafes in the plan?
         self.logger.info('Restoring ILM polling to default: %s', self.ilm_polling(interval=None))
         self.client.cluster.put_settings(persistent=self.ilm_polling(interval=None))
         end = datetime.now(timezone.utc)
         self.logger.info('Testbed teardown elapsed time: %s', (end - start).total_seconds())
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/ilm.py` & `es_testbed-0.5.3/src/es_testbed/classes/ilm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """ILM Defining Class"""
+
 import typing as t
 from os import getenv
 from time import sleep
 from dotmap import DotMap
 from elasticsearch8 import Elasticsearch
 from es_testbed.defaults import PAUSE_ENVVAR, PAUSE_DEFAULT
 from es_testbed.exceptions import NameChanged, ResultNotExpected, TestbedMisconfig
 from es_testbed.helpers import es_api
 from es_testbed.helpers.utils import getlogger
+
 PAUSE_VALUE = float(getenv(PAUSE_ENVVAR, default=PAUSE_DEFAULT))
 
 # pylint: disable=missing-docstring
 
-### Example ILM explain output
+# ## Example ILM explain output
 # {
 #     'action': 'complete',
 #     'action_time_millis': 0,
 #     'age': '5.65m',
 #     'index': 'INDEX_NAME',
 #     'index_creation_date_millis': 0,
 #     'lifecycle_date_millis': 0,
@@ -41,19 +43,21 @@
 #     'phase_time_millis': 0,
 #     'policy': 'POLICY_NAME',
 #     'step': 'complete',
 #     'step_time_millis': 0,
 #     'time_since_index_creation': '5.65m'
 # }
 
+
 class IlmTracker:
+
     def __init__(self, client: Elasticsearch, name: str):
         self.logger = getlogger('es_testbed.IlmTracker')
         self.client = client
-        self.name = self.resolve(name) # A single index name
+        self.name = self.resolve(name)  # A single index name
         self._explain = DotMap(self.get_explain_data())
         self._phases = es_api.get_ilm_phases(self.client, self._explain.policy)
 
     @property
     def current_step(self) -> dict:
         return {
             'phase': self._explain.phase,
@@ -67,30 +71,32 @@
 
     @property
     def next_phase(self) -> str:
         retval = None
         if self._explain.phase == 'delete':
             self.logger.warning('Already on "delete" phase. No more phases to advance')
         else:
-            curr = self.pnum(self._explain.phase) # A numeric representation of the current phase
+            curr = self.pnum(self._explain.phase)  # A numeric representation of the current phase
             # A list of any remaining phases in the policy with a higher number than the current
             remaining = [self.pnum(x) for x in self.policy_phases if self.pnum(x) > curr]
-            if remaining: # If any:
+            if remaining:  # If any:
                 retval = self.pname(remaining[0])
                 # Get the phase name from the number stored in the first element
         return retval
 
     @property
     def policy_phases(self) -> t.Sequence[str]:
         return list(self._phases.keys())
 
-    def advance(self, phase: str=None, action: str=None, name: str=None) -> None:
+    def advance(
+        self, phase: t.Union[str, None] = None, action: t.Union[str, None] = None, name: t.Union[str, None] = None
+    ) -> None:
         def wait(phase: str) -> None:
             counter = 0
-            sleep(1.5) # Initial wait since we set ILM to poll every second
+            sleep(1.5)  # Initial wait since we set ILM to poll every second
             while self._explain.phase != phase:
                 sleep(PAUSE_VALUE)
                 self.update()
                 counter += 1
                 self.count_logging(counter)
 
         if self._explain.phase == 'delete':
@@ -123,15 +129,17 @@
             self.logger.debug('Passing along upstream exception...')
             raise NameChanged from err
         except ResultNotExpected as err:
             msg = f'Unable to get ilm_explain API call results. Error: {err}'
             self.logger.critical(msg)
             raise ResultNotExpected(msg) from err
 
-    def next_step(self, phase: str=None, action: str=None, name: str=None) -> t.Dict:
+    def next_step(
+        self, phase: t.Union[str, None] = None, action: t.Union[str, None] = None, name: t.Union[str, None] = None
+    ) -> t.Dict:
         err1 = bool((action is not None) and (name is None))
         err2 = bool((action is None) and (name is not None))
         if err1 or err2:
             msg = 'If either action or name is specified, both must be'
             self.logger.critical(msg)
             raise TestbedMisconfig(msg)
         if not phase:
@@ -170,22 +178,19 @@
             self.logger.debug('Passing along upstream exception...')
             raise NameChanged from err
 
     def wait4complete(self) -> None:
         counter = 0
         self.logger.debug('Waiting for current action and step to complete')
         self.logger.debug('Action: %s --- Step: %s', self._explain.action, self._explain.step)
-        while not bool(
-                    self._explain.action == 'complete' and
-                    self._explain.step == 'complete'):
+        while not bool(self._explain.action == 'complete' and self._explain.step == 'complete'):
             counter += 1
             sleep(PAUSE_VALUE)
             if counter % 10 == 0:
-                self.logger.debug(
-                    'Action: %s --- Step: %s', self._explain.action, self._explain.step)
+                self.logger.debug('Action: %s --- Step: %s', self._explain.action, self._explain.step)
             try:
                 self.count_logging(counter)
             except ResultNotExpected as err:
                 self.logger.critical('Breaking the loop. Explain: %s', self._explain.toDict())
                 raise ResultNotExpected from err
             try:
                 self.update()
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/plan.py` & `es_testbed-0.5.3/src/es_testbed/classes/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """TestPlan Class Definition"""
+
 import typing as t
 from dotmap import DotMap
 from es_testbed.defaults import TESTPLAN
 from es_testbed.helpers.utils import build_ilm_policy, getlogger, randomstr
+
 # pylint: disable=missing-docstring
 
+
 class PlanBuilder:
-    def __init__(
-            self,
-            settings: t.Dict = None,
-            default_entities: bool = True,
-            autobuild: t.Optional[bool] = True,
-        ):
+
+    def __init__(self, settings: t.Dict = None, default_entities: bool = True, autobuild: t.Optional[bool] = True):
         self.logger = getlogger('es_testbed.PlanBuilder')
         self.default_entities = default_entities
         if settings is None:
             settings = TESTPLAN
         self.settings = settings
         self._plan = DotMap(TESTPLAN)
         if autobuild:
             self.setup()
 
-        ### Example settings
+        # ## Example settings
         # settings={
         #   'type': 'indices',       # Default is indices? Or should it be data_streams?
         #   'prefix': 'es-testbed',  # Provide this value as a default
         #   'rollover_alias': False, # Only respected if 'type' == 'indices'.
         #                            # Will rollover after creation and filling 1st index
         #                            # If True, will be overridden to value of alias name
         #                            # If False, will be overridden with None
@@ -34,26 +33,26 @@
         #   'ilm': {                 # All of these ILM values are defaults
         #     'enabled': False,
         #     'tiers': ['hot', 'delete'],
         #     'forcemerge': False,
         #     'max_num_segments': 1,
         #   }
         #
-        ## If these keys aren't specified per entity, then all entities will get this treatment
-        ## EXCEPT for the is_write_index for aliases and data_streams
+        # # If these keys aren't specified per entity, then all entities will get this treatment
+        # # EXCEPT for the is_write_index for aliases and data_streams
         #
         #   'defaults': {
         #     'entity_count': 3,
         #     'docs': 10,
         #     'match': True,
         #     'searchable': tier...
         #   }
         #
-        ## Manually specifying entities makes sense for individual indices, but not so much for
-        ## alias-backed indices or data_streams
+        # # Manually specifying entities makes sense for individual indices, but not so much for
+        # # alias-backed indices or data_streams
         #   'entities': [
         #    {
         #      'docs': 10,
         #      'match': True,
         #      'searchable': 'frozen'
         #    },
         #    {
@@ -77,45 +76,47 @@
         self._plan.failsafes = DotMap()
         items = ['index', 'data_stream', 'snapshot', 'ilm', 'template', 'component', 'entity_type']
         for i in items:
             self._plan.failsafes[i] = []
 
     def _create_lists(self):
         names = [
-            'indices', 'data_stream', 'snapshots', 'ilm_policies', 'index_templates',
-            'component_templates', 'entity_mgrs'
+            'indices',
+            'data_stream',
+            'snapshots',
+            'ilm_policies',
+            'index_templates',
+            'component_templates',
+            'entity_mgrs',
         ]
         for name in names:
             self._plan[name] = []
 
     def add_entity(
-            self,
-            docs: t.Optional[int] = 10,
-            match: t.Optional[bool] = True,
-            searchable: t.Optional[str] = None
-        ) -> None:
+        self, docs: t.Optional[int] = 10, match: t.Optional[bool] = True, searchable: t.Optional[str] = None
+    ) -> None:
         entity = {'docs': docs, 'match': match}
         if searchable:
             entity['searchable'] = searchable
         self._plan.entities.append(entity)
 
     def make_default_entities(self) -> None:
-        defs = TESTPLAN['defaults'] # Start with defaults
+        defs = TESTPLAN['defaults']  # Start with defaults
         if 'defaults' in self._plan:
             defs = self._plan.defaults
         kwargs = {'docs': defs['docs'], 'match': defs['match'], 'searchable': defs['searchable']}
         for _ in range(0, defs['entity_count']):
             self.add_entity(**kwargs)
         self.logger.debug('Plan will create %s (backing) indices', len(self._plan.entities))
 
     def setup(self) -> None:
         self._plan.uniq = randomstr(length=8, lowercase=True)
         self._create_lists()
         self._create_failsafes()
-        self.update(self.settings) # Override with settings.
+        self.update(self.settings)  # Override with settings.
         self.update_rollover_alias()
         self.update_ilm()
         if not self._plan.entities:
             if self.default_entities:
                 self.make_default_entities()
         self.logger.debug('Test Plan: %s', self._plan.pprint())
 
@@ -146,15 +147,15 @@
         ilm = self._plan.ilm
         for entity in self._plan.entities:
             if 'searchable' in entity and entity['searchable'] is not None:
                 if not entity['searchable'] in ilm.tiers:
                     ilm.tiers.append(entity['searchable'])
         kwargs = {
             'tiers': ilm.tiers,
-            'forcemerge': ilm.forcemerge, 
+            'forcemerge': ilm.forcemerge,
             'max_num_segments': ilm.max_num_segments,
             'repository': self._plan.repository,
         }
         self._plan.ilm.policy = build_ilm_policy(**kwargs)
 
     def update_rollover_alias(self) -> None:
         if self._plan.rollover_alias:
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/tracker.py` & `es_testbed-0.5.3/src/es_testbed/classes/tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 """Tracker Class Definition"""
+
 import typing as t
 from dotmap import DotMap
 from elasticsearch8 import Elasticsearch
 from es_testbed.helpers.utils import getlogger
-from .entitymgrs import (
-    ComponentMgr, DataStreamMgr, IlmMgr, IndexMgr, SnapshotMgr, TemplateMgr)
+from .entitymgrs import ComponentMgr, DataStreamMgr, IlmMgr, IndexMgr, SnapshotMgr, TemplateMgr
 
 # pylint: disable=missing-docstring,too-many-instance-attributes
 
 TYPEMAP = {'indices': IndexMgr, 'data_stream': DataStreamMgr}
 
+
 class Tracker:
     """Object for tracking entities created in TestBed"""
-    def __init__(
-            self,
-            client: Elasticsearch = None,
-            plan: DotMap = None,
-            autobuild: t.Optional[bool] = False,
-        ):
+
+    def __init__(self, client: Elasticsearch = None, plan: DotMap = None, autobuild: t.Optional[bool] = False):
         """Initialize"""
         self.logger = getlogger('es_testbed.Tracker')
         self.client = client
         self.plan = plan
         self.ilm_policies = None
         self.components = None
         self.templates = None
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/entities/alias.py` & `es_testbed-0.5.3/src/es_testbed/classes/entities/alias.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Alias Entity Class"""
+
 import typing as t
 from elasticsearch8 import Elasticsearch
 from es_testbed.helpers.utils import getlogger
 from es_testbed.helpers import es_api
 from .entity import Entity
 
 # pylint: disable=missing-docstring,too-many-arguments
 
+
 class Alias(Entity):
-    def __init__(
-            self,
-            client: Elasticsearch,
-            name: str = None,
-            autobuild: t.Optional[bool] = True,
-        ):
+
+    def __init__(self, client: Elasticsearch, name: str = None, autobuild: t.Optional[bool] = True):
         super().__init__(client=client, name=name, autobuild=autobuild)
         self.logger = getlogger('es_testbed.Alias')
 
     def rollover(self) -> None:
         es_api.rollover(self.client, self.name)
 
     def verify(self, index_list: t.Sequence[str]) -> bool:
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/entities/data_stream.py` & `es_testbed-0.5.3/src/es_testbed/classes/entities/data_stream.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Index Entity Class"""
+
 import typing as t
 from elasticsearch8 import Elasticsearch
 from es_testbed.helpers import es_api
 from es_testbed.helpers.utils import getlogger
 from . import Alias
 
 # pylint: disable=missing-docstring,too-many-arguments
 
+
 class DataStream(Alias):
-    def __init__(
-            self,
-            client: Elasticsearch = None,
-            name: str = None,
-            autobuild: t.Optional[bool] = True,
-        ):
+
+    def __init__(self, client: Elasticsearch = None, name: str = None, autobuild: t.Optional[bool] = True):
         super().__init__(client=client, name=name, autobuild=autobuild)
         self.logger = getlogger('es_testbed.Data_Stream')
         self.index_tracker = []
         self.alias = None
 
     @property
     def backing_indices(self):
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/entities/index.py` & `es_testbed-0.5.3/src/es_testbed/classes/entities/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 """Index Entity Class"""
+
 import typing as t
 from os import getenv
 from elasticsearch8 import Elasticsearch
 from es_wait import Exists
 from es_testbed.defaults import PAUSE_DEFAULT, PAUSE_ENVVAR, TIMEOUT_DEFAULT, TIMEOUT_ENVVAR
 from es_testbed.exceptions import NameChanged, ResultNotExpected
 from es_testbed.helpers import es_api
 from es_testbed.helpers.utils import getlogger, mounted_name
 from .entity import Entity
 from ..ilm import IlmTracker
+
 PAUSE_VALUE = float(getenv(PAUSE_ENVVAR, default=PAUSE_DEFAULT))
 TIMEOUT_VALUE = float(getenv(TIMEOUT_ENVVAR, default=TIMEOUT_DEFAULT))
 
 # pylint: disable=missing-docstring,too-many-arguments
 
+
 class Index(Entity):
+
     def __init__(
-            self,
-            client: Elasticsearch = None,
-            name: str = None,
-            autobuild: t.Optional[bool] = True,
-            snapmgr = None,
-            policy_name: str = None,
-        ):
+        self,
+        client: Elasticsearch = None,
+        name: str = None,
+        autobuild: t.Optional[bool] = True,
+        snapmgr=None,
+        policy_name: str = None,
+    ):
         super().__init__(client=client, name=name, autobuild=autobuild)
         self.logger = getlogger('es_testbed.Index')
         self.policy_name = policy_name
         self.ilm_tracker = None
         self.snapmgr = snapmgr
         self.track_ilm(self.name)
 
     @property
     def _get_target(self) -> str:
         target = None
         phases = self.ilm_tracker.policy_phases
         curr = self.ilm_tracker.explain.phase
         if not bool(('cold' in phases) or ('frozen' in phases)):
             self.logger.info('ILM Policy for "%s" has no cold/frozen phases', self.name)
-            target = curr # Keep the same
+            target = curr  # Keep the same
         if bool(('cold' in phases) and ('frozen' in phases)):
             if self.ilm_tracker.pname(curr) < self.ilm_tracker.pname('cold'):
                 target = 'cold'
             elif curr == 'cold':
                 target = 'frozen'
             elif self.ilm_tracker.pname(curr) >= self.ilm_tracker.pname('frozen'):
                 target = curr
@@ -60,52 +64,49 @@
         current, target = self.phase_tuple
         while current != target:
             self.logger.debug('Attempting to move %s to ILM phase %s', self.name, target)
             self.ilm_tracker.advance(phase=target)
             # At this point, it's "in" a searchable tier, but the index name hasn't changed yet
             newidx = mounted_name(self.name, target)
             self.logger.debug('Waiting for ILM phase change to complete. New index: %s', newidx)
-            kwargs = {
-                'name': newidx, 'kind': 'index', 'pause': PAUSE_VALUE, 'timeout': TIMEOUT_VALUE}
+            kwargs = {'name': newidx, 'kind': 'index', 'pause': PAUSE_VALUE, 'timeout': TIMEOUT_VALUE}
             test = Exists(self.client, **kwargs)
             test.wait_for_it()
             self.logger.info('ILM advance to phase %s completed', target)
-            self.aka.append(self.name) # Append the old name to the AKA list
+            self.aka.append(self.name)  # Append the old name to the AKA list
             self.name = newidx
-            self.track_ilm(self.name) # Refresh the ilm_tracker with the new index name
+            self.track_ilm(self.name)  # Refresh the ilm_tracker with the new index name
             current, target = self.phase_tuple
 
     def manual_ss(self, scheme) -> None:
         """If we are NOT using ILM but have specified searchable snapshots in the plan entities"""
         if 'searchable' in scheme and scheme['searchable'] is not None:
             self.snapmgr.add(self.name, scheme['searchable'])
             # Replace self.name with the renamed name
             self.name = mounted_name(self.name, scheme['searchable'])
 
     def mount_ss(self, scheme: dict) -> None:
         """If the index is planned to become a searchable snapshot, we do that now"""
         self.logger.debug('Checking if %s should be a searchable snapshot', self.name)
         if self.am_i_write_idx:
-            self.logger.info(
-                '%s is the write_index. Cannot mount as searchable snapshot', self.name)
+            self.logger.info('%s is the write_index. Cannot mount as searchable snapshot', self.name)
             return
-        if not self.policy_name: # If we have this, chances are we have a policy
+        if not self.policy_name:  # If we have this, chances are we have a policy
             self.logger.debug('No ILM policy found. Switching to manual mode')
             self.manual_ss(scheme)
             return
         current = self.ilm_tracker.explain.phase
         target = self._get_target
         if current != target:
             self.logger.debug('Attempting to move %s to ILM phase %s', self.name, target)
             self.ilm_tracker.advance(phase=target)
             # At this point, it's "in" a searchable tier, but the index name hasn't changed yet
             newidx = mounted_name(self.name, target)
             self.logger.debug('Waiting for ILM phase change to complete. New index: %s', newidx)
-            kwargs = {
-                'name': newidx, 'kind': 'index', 'pause': PAUSE_VALUE, 'timeout': TIMEOUT_VALUE}
+            kwargs = {'name': newidx, 'kind': 'index', 'pause': PAUSE_VALUE, 'timeout': TIMEOUT_VALUE}
             test = Exists(self.client, **kwargs)
             test.wait_for_it()
             try:
                 self.ilm_tracker.wait4complete()
             except NameChanged:
                 try:
                     self.track_ilm(newidx)
@@ -114,17 +115,17 @@
                     self.logger.critical('Index name mismatch. Cannot continue')
                     raise ResultNotExpected from err
             self.logger.info('ILM advance to phase %s completed', target)
             self.logger.debug('Getting snapshot name for tracking...')
             snapname = es_api.snapshot_name(self.client, newidx)
             self.logger.debug('Snapshot %s backs %s', snapname, newidx)
             self.snapmgr.add_existing(snapname)
-            self.aka.append(self.name) # Append the old name to the AKA list
+            self.aka.append(self.name)  # Append the old name to the AKA list
             self.name = newidx
-            self.track_ilm(self.name) # Refresh the ilm_tracker with the new index name
+            self.track_ilm(self.name)  # Refresh the ilm_tracker with the new index name
 
     def track_ilm(self, name: str) -> None:
         """
         Get ILM phase information and put it in self.ilm_tracker
         Name as an arg makes it configurable
         """
         if self.policy_name:
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/componentmgr.py` & `es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/componentmgr.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """Component Template Entity Manager Class"""
+
 import typing as t
 from dotmap import DotMap
 from elasticsearch8 import Elasticsearch
 from es_testbed.exceptions import ResultNotExpected
 from es_testbed.helpers import es_api
 from es_testbed.helpers.utils import getlogger, mapping_component, setting_component
 from .entitymgr import EntityMgr
 
 # pylint: disable=missing-docstring,too-many-arguments
 
+
 class ComponentMgr(EntityMgr):
     kind = 'component'
     listname = 'component_templates'
-    def __init__(
-            self,
-            client: Elasticsearch = None,
-            plan: DotMap = None,
-            autobuild: t.Optional[bool] = True,
-        ):
+
+    def __init__(self, client: Elasticsearch = None, plan: DotMap = None, autobuild: t.Optional[bool] = True):
         super().__init__(client=client, plan=plan, autobuild=autobuild)
         self.logger = getlogger('es_testbed.ComponentMgr')
 
     @property
     def components(self):
         retval = []
         kw = {'ilm_policy': self.plan.ilm_policies[-1], 'rollover_alias': self.plan.rollover_alias}
@@ -33,13 +31,12 @@
     def logdisplay(self) -> str:
         return 'component template'
 
     def setup(self):
         for component in self.components:
             es_api.put_comp_tmpl(self.client, self.name, component)
             if not es_api.exists(self.client, self.kind, self.name):
-                raise ResultNotExpected(
-                    f'Unable to verify creation of component template {self.name}')
+                raise ResultNotExpected(f'Unable to verify creation of component template {self.name}')
             self.appender(self.name)
             self.logger.info('Created component template: "%s"', self.last)
         self.logger.info('Successfully created all component templates.')
         self.success = True
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/data_streammgr.py` & `es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/data_streammgr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """data_stream Entity Manager Class"""
+
 import typing as t
 from dotmap import DotMap
 from elasticsearch8 import Elasticsearch
 from es_testbed.helpers import es_api
 from es_testbed.helpers.utils import getlogger
 from .indexmgr import IndexMgr
 from .snapshotmgr import SnapshotMgr
 from ..entities import DataStream, Index
 
 # pylint: disable=missing-docstring,too-many-arguments,broad-exception-caught
 
+
 class DataStreamMgr(IndexMgr):
     kind = 'data_stream'
     listname = 'data_stream'
+
     def __init__(
-            self,
-            client: Elasticsearch = None,
-            plan: DotMap = None,
-            autobuild: t.Optional[bool] = True,
-            snapmgr: SnapshotMgr = None,
-        ):
+        self,
+        client: Elasticsearch = None,
+        plan: DotMap = None,
+        autobuild: t.Optional[bool] = True,
+        snapmgr: SnapshotMgr = None,
+    ):
         self.ds = None
         self.index_trackers = []
         super().__init__(client=client, plan=plan, autobuild=autobuild, snapmgr=snapmgr)
         self.logger = getlogger('es_testbed.DataStreamMgr')
 
     @property
-    def suffix(self): # Remapping this to send no suffix for data_streams
+    def suffix(self):  # Remapping this to send no suffix for data_streams
         return ''
 
     @property
     def indexlist(self) -> t.Sequence[str]:
         return [x.name for x in self.index_trackers]
 
     def add(self, value):
@@ -41,15 +44,15 @@
         """If the indices were marked as searchable snapshots, we do that now"""
         for idx, scheme in enumerate(self.plan.entities):
             self.index_trackers[idx].mount_ss(scheme)
         self.logger.info('Completed backing index promotion to searchable snapshots.')
         self.logger.info('data_stream backing indices: %s', self.ds.backing_indices)
 
     def setup(self) -> bool:
-        self.index_trackers = [] # Inheritance oddity requires redeclaration here
+        self.index_trackers = []  # Inheritance oddity requires redeclaration here
         for scheme in self.plan.entities:
             if not self.entity_list:
                 self.add(self.name)
             else:
                 self.ds.rollover()
             self.filler(scheme)
         self.logger.debug('Created data_stream: %s', self.ds.name)
@@ -65,14 +68,9 @@
     def track_data_stream(self) -> None:
         self.logger.debug('Tracking data_stream: %s', self.name)
         self.ds = DataStream(client=self.client, name=self.name)
         self.appender(self.name)
 
     def track_index(self, name: str) -> None:
         self.logger.debug('Tracking index: %s', name)
-        entity = Index(
-            client=self.client,
-            name=name,
-            snapmgr=self.snapmgr,
-            policy_name=self.policy_name
-        )
+        entity = Index(client=self.client, name=name, snapmgr=self.snapmgr, policy_name=self.policy_name)
         self.index_trackers.append(entity)
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/entitymgr.py` & `es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/entitymgr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,97 +1,107 @@
 """Entity Class Definition"""
+
 import typing as t
 from dotmap import DotMap
 from elasticsearch8 import Elasticsearch
 from es_testbed.defaults import NAMEMAPPER, PLURALMAP
 from es_testbed.helpers.es_api import delete, get
 from es_testbed.helpers.utils import getlogger, uniq_values
 
 # pylint: disable=missing-docstring,broad-exception-caught,too-many-instance-attributes
 
+
 class EntityMgr:
     kind = 'entity_type'
     listname = 'entity_mgrs'
+
     def __init__(
-            self,
-            client: Elasticsearch = None,
-            plan: DotMap = None,
-            autobuild: t.Optional[bool] = True,
-        ):
+        self, client: t.Union[Elasticsearch, None] = None, plan: DotMap = None, autobuild: t.Optional[bool] = True
+    ):
         self.logger = getlogger('es_testbed.EntityMgr')
         self.client = client
         self.plan = plan
         self.success = False
         if autobuild:
             self.setup()
 
     @property
     def entity_list(self):
         return self.plan[self.listname]
+
     @entity_list.setter
     def entity_list(self, value: t.Sequence) -> None:
         self.plan[self.listname] = value
+
     @property
     def entity_root(self) -> str:
         return f'{self.plan.prefix}-{self.ident()}-{self.plan.uniq}'
+
     @property
     def failsafe(self):
         return self.plan.failsafes[self.kind]
+
     @failsafe.setter
     def failsafe(self, value: t.Sequence) -> None:
         self.plan.failsafes[self.kind] = value
+
     @property
     def indexlist(self) -> t.Sequence[str]:
-        return [] # Empty attribute/property waiting to be overridden
+        return []  # Empty attribute/property waiting to be overridden
+
     @property
     def last(self) -> str:
-        return self.entity_list[-1] # Return the most recently appended item
+        return self.entity_list[-1]  # Return the most recently appended item
+
     @property
     def logdisplay(self) -> str:
         return self.kind
+
     @property
     def name(self) -> str:
         return f'{self.entity_root}{self.suffix}'
+
     @property
     def pattern(self) -> str:
         return f'*{self.entity_root}*'
+
     @property
     def suffix(self) -> str:
         return f'-{len(self.entity_list) + 1:06}'
 
     def appender(self, name: str) -> None:
         self.failsafe.append(name)
         self.entity_list.append(name)
 
     def ident(self, dkey=None):
         if not dkey:
-            dkey=self.kind
+            dkey = self.kind
         return NAMEMAPPER[dkey]
 
-    def iterate_clean(self) -> None:
+    def iterate_clean(self) -> bool:
         succeed = True
         positions = []
-        for idx, entity in enumerate(self.entity_list): # There should only be one, but we cover it
+        for idx, entity in enumerate(self.entity_list):  # There should only be one, but we cover it
             value = entity
             if self.kind == 'index':
                 value = entity.name
             self.logger.debug('Deleting %s %s', self.logdisplay, value)
             try:
                 delete(self.client, self.kind, value)
             except Exception as err:
                 succeed = False
                 msg = f'Unable to delete {self.logdisplay}: {value}. Error: {err}'
                 self.logger.error(msg)
                 continue
             self.logger.debug('Deleted %s %s', self.logdisplay, value)
             positions.append(idx)
-        positions.sort() # Sort first to ensure lowest to highest order
-        for idx in reversed(positions): # Reverse the list and iterate
-            del self.entity_list[idx] # Delete the value at position idx
-            del self.plan.failsafes[self.kind][idx] # Delete the value at position idx
+        positions.sort()  # Sort first to ensure lowest to highest order
+        for idx in reversed(positions):  # Reverse the list and iterate
+            del self.entity_list[idx]  # Delete the value at position idx
+            del self.plan.failsafes[self.kind][idx]  # Delete the value at position idx
         return succeed
 
     def scan(self) -> t.Sequence[str]:
         """Find all entities matching our pattern"""
         entities = get(self.client, self.kind, self.pattern)
         msg = f'{self.kind} entities found matching pattern "{self.pattern}": {entities}'
         self.logger.debug(msg)
@@ -100,31 +110,28 @@
 
     def setup(self):
         pass
 
     def teardown(self):
         display = PLURALMAP[self.kind] if self.kind in PLURALMAP else self.kind
         if not self.success:
-            msg = (
-                f'Setup did not complete successfully. '
-                f'Manual cleanup of {display}s may be necessary.'
-            )
+            msg = f'Setup did not complete successfully. ' f'Manual cleanup of {display}s may be necessary.'
             self.logger.warning(msg)
-        self.verify(correct=True) # Catch any entities that might exist but not be in entity_list
+        self.verify(correct=True)  # Catch any entities that might exist but not be in entity_list
         if self.entity_list:
             if self.iterate_clean():
                 self.logger.info('Cleanup of %ss completed successfully.', display)
 
     def track_index(self, name: str) -> None:
         pass
 
-    def verify(self, correct: bool=False) -> t.Union[t.Sequence[str], None]:
+    def verify(self, correct: bool = False) -> t.Union[t.Sequence[str], None]:
         retval = None
         diffs = False
-        curr = self.scan() # This is what entity_list _should_ look like.
+        curr = self.scan()  # This is what entity_list _should_ look like.
         if self.kind == 'index':
             entities = self.indexlist
         else:
             entities = self.entity_list
         self.logger.debug('Getting unique values from scan output (not in self.entity_list)')
         scan_diff = uniq_values(entities, curr)
         self.logger.debug('Getting unique values in self.entity_list (not in scan)')
@@ -137,14 +144,14 @@
             self.logger.info('Values in scan not found in entity_list: %s', scan_diff)
         if diffs:
             if correct:
                 self.logger.info('Correcting entity_list with values from scan: %s', curr)
                 if self.kind == 'index':
                     self.entity_list = []
                     for index in curr:
-                        self.track_index(index) # We have to re-create the tracked entities
+                        self.track_index(index)  # We have to re-create the tracked entities
                 else:
                     self.entity_list = curr
             else:
                 self.logger.warning('Not correcting entity_list! Values should be: %s', curr)
                 retval = curr
         return retval
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/ilmmgr.py` & `es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/ilmmgr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 """ILM Policy Entity Manager Class"""
+
 import typing as t
 from dotmap import DotMap
 from elasticsearch8 import Elasticsearch
 from es_testbed.exceptions import ResultNotExpected
 from es_testbed.helpers import es_api
 from es_testbed.helpers.utils import build_ilm_policy, getlogger
 from .entitymgr import EntityMgr
 
 # pylint: disable=missing-docstring
 
+
 class IlmMgr(EntityMgr):
     kind = 'ilm'
     listname = 'ilm_policies'
-    def __init__(
-            self,
-            client: Elasticsearch = None,
-            plan: DotMap = None,
-            autobuild: t.Optional[bool] = True,
-        ):
+
+    def __init__(self, client: Elasticsearch = None, plan: DotMap = None, autobuild: t.Optional[bool] = True):
         super().__init__(client=client, plan=plan, autobuild=autobuild)
         self.logger = getlogger('es_testbed.IlmMgr')
 
     @property
     def logdisplay(self) -> str:
         return 'ILM policy'
 
     def get_policy(self):
         d = self.plan.ilm
         kwargs = {
             'tiers': d.tiers,
-            'forcemerge': d.forcemerge, 
+            'forcemerge': d.forcemerge,
             'max_num_segments': d.max_num_segments,
             'repository': self.plan.repository,
         }
         return build_ilm_policy(**kwargs)
 
     def setup(self):
         if self.plan.ilm.enabled:
             self.plan.ilm.policy = self.get_policy()
             es_api.put_ilm(self.client, self.name, policy=self.plan.ilm.policy)
             # Verify existence
             if not es_api.exists(self.client, 'ilm', self.name):
-                raise ResultNotExpected(
-                    f'Unable to verify creation of ilm policy {self.name}')
+                raise ResultNotExpected(f'Unable to verify creation of ilm policy {self.name}')
             # This goes first because the length of entity_list determines the suffix
             self.appender(self.name)
             self.logger.info('Successfully created ILM policy: %s', self.last)
         else:
-            self.appender(None) # This covers self.plan.ilm_policies[-1]
+            self.appender(None)  # This covers self.plan.ilm_policies[-1]
             self.logger.info('No ILM policy created.')
         self.success = True
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/indexmgr.py` & `es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/indexmgr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 """Index Entity Manager Class"""
+
 import typing as t
 from dotmap import DotMap
 from elasticsearch8 import Elasticsearch
 from es_testbed.helpers import es_api
 from es_testbed.helpers.utils import getlogger, setting_component
 from .entitymgr import EntityMgr
 from .snapshotmgr import SnapshotMgr
 from ..entities import Alias, Index
 
 # pylint: disable=missing-docstring,too-many-arguments,broad-exception-caught,too-many-instance-attributes
 
+
 class IndexMgr(EntityMgr):
     kind = 'index'
     listname = 'indices'
+
     def __init__(
-            self,
-            client: Elasticsearch = None,
-            plan: DotMap = None,
-            autobuild: t.Optional[bool] = True,
-            snapmgr: SnapshotMgr = None,
-        ):
+        self,
+        client: Elasticsearch = None,
+        plan: DotMap = None,
+        autobuild: t.Optional[bool] = True,
+        snapmgr: SnapshotMgr = None,
+    ):
         self.doc_incr = 0
         self.snapmgr = snapmgr
-        self.alias = None # Only used for tracking the rollover alias
+        self.alias = None  # Only used for tracking the rollover alias
         super().__init__(client=client, plan=plan, autobuild=autobuild)
         self.logger = getlogger('es_testbed.IndexMgr')
 
     @property
     def indexlist(self) -> t.Sequence[str]:
         return [x.name for x in self.entity_list]
+
     @property
     def policy_name(self) -> str:
         if len(self.plan.ilm_policies) > 0:
             return self.plan.ilm_policies[-1]
         return None
 
     def _rollover_path(self) -> None:
         if not self.entity_list:
-            kw = {'ilm_policy': self.policy_name,
-                  'rollover_alias': self.plan.rollover_alias}
+            kw = {'ilm_policy': self.policy_name, 'rollover_alias': self.plan.rollover_alias}
             cfg = setting_component(**kw)['settings']
             acfg = {self.plan.rollover_alias: {'is_write_index': True}}
             self.logger.debug('No indices created yet. Starting with a rollover alias index...')
             es_api.create_index(self.client, self.name, aliases=acfg, settings=cfg)
-            self.logger.debug(
-                'Created %s with rollover alias %s', self.name, self.plan.rollover_alias)
+            self.logger.debug('Created %s with rollover alias %s', self.name, self.plan.rollover_alias)
             self.track_alias()
         else:
             self.alias.rollover()
-            if self.policy_name: # We have an ILM policy
+            if self.policy_name:  # We have an ILM policy
                 self.logger.debug('Going to wait now...')
                 self.last.ilm_tracker.wait4complete()
                 self.logger.debug('The wait is over!')
 
     def add(self, value) -> None:
         # In this case, value is a single array element from plan.entities
         self.logger.debug('Creating index: %s', value)
@@ -65,42 +67,36 @@
             else:
                 self.add(self.name)
             self.filler(scheme)
             self.track_index(self.name)
         self.logger.debug('Created indices: %s', self.indexlist)
         if self.plan.rollover_alias:
             if not self.alias.verify(self.indexlist):
-                self.logger.error(
-                    'Unable to confirm rollover of alias "%s" was successfully executed')
+                self.logger.error('Unable to confirm rollover of alias "%s" was successfully executed')
 
     def filler(self, scheme) -> None:
         """If the scheme from the TestPlan says to write docs, do it"""
         # scheme is a single array element from plan.entities
         self.logger.debug('Adding docs to %s', self.name)
         if scheme['docs'] > 0:
             es_api.fill_index(
-                self.client,
-                name=self.name,
-                count=scheme['docs'],
-                start_num=self.doc_incr,
-                match=scheme['match']
+                self.client, name=self.name, count=scheme['docs'], start_num=self.doc_incr, match=scheme['match']
             )
         self.doc_incr += scheme['docs']
 
     def searchable(self) -> None:
         """If the indices were marked as searchable snapshots, we do that now"""
         for idx, scheme in enumerate(self.plan.entities):
             old = self.entity_list[idx].name
             self.entity_list[idx].mount_ss(scheme)
             new = self.entity_list[idx].name
             # Replace the old index name in self.failsafe with the new one at the same list position
             pos = [i for i, value in enumerate(self.failsafe) if value == old]
             self.failsafe[pos[0]] = new
 
-
     def setup(self) -> None:
         self.logger.debug('Beginning setup...')
         if self.plan.rollover_alias:
             self.logger.debug('rollover_alias is True...')
         self.add_indices()
         self.searchable()
         self.logger.info('Successfully created indices: %s', self.indexlist)
@@ -108,15 +104,10 @@
 
     def track_alias(self) -> None:
         self.logger.debug('Tracking alias: %s', self.plan.rollover_alias)
         self.alias = Alias(client=self.client, name=self.plan.rollover_alias)
 
     def track_index(self, name: str) -> None:
         self.logger.debug('Tracking index: %s', name)
-        entity = Index(
-            client=self.client,
-            name=name,
-            snapmgr=self.snapmgr,
-            policy_name=self.policy_name
-        )
+        entity = Index(client=self.client, name=name, snapmgr=self.snapmgr, policy_name=self.policy_name)
         self.failsafe.append(name)
         self.entity_list.append(entity)
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/snapshotmgr.py` & `es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/snapshotmgr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,47 @@
 """Snapshot Entity Manager Class"""
+
 import typing as t
 from dotmap import DotMap
 from elasticsearch8 import Elasticsearch
 from es_testbed.helpers import es_api
 from es_testbed.helpers.utils import getlogger
 from .entitymgr import EntityMgr
 
 # pylint: disable=missing-docstring
 
+
 class SnapshotMgr(EntityMgr):
     kind = 'snapshot'
     listname = 'snapshots'
-    def __init__(
-            self,
-            client: Elasticsearch = None,
-            plan: DotMap = None,
-            autobuild: t.Optional[bool] = False,
-        ):
+
+    def __init__(self, client: Elasticsearch = None, plan: DotMap = None, autobuild: t.Optional[bool] = False):
         super().__init__(client=client, plan=plan, autobuild=autobuild)
         self.logger = getlogger('es_testbed.SnapshotMgr')
 
     def add(self, index: str, tier: str) -> None:
         msg = f'Creating snapshot of index {index} and mounting in the {tier} tier...'
         self.logger.info(msg)
-        es_api.do_snap(
-            self.client,
-            self.plan.repository,
-            self.name,
-            index,
-            tier=tier
-        )
+        es_api.do_snap(self.client, self.plan.repository, self.name, index, tier=tier)
         self.appender(self.name)
         self.logger.info('Successfully created snapshot "%s"', self.last)
         self.success = True
 
     def add_existing(self, name: str) -> None:
         """Add a snapshot that's already been created, e.g. by ILM promotion"""
         self.logger.info('Adding snapshot %s to list...', name)
         self.appender(name)
         self.success = True
 
     def setup(self):
         pass
 
-    def teardown(self): # We override the parent method here to speed things up.
+    def teardown(self):  # We override the parent method here to speed things up.
         if self.entity_list:
             if not self.success:
-                msg = (
-                    f'Setup did not complete successfully. '
-                    f'Manual cleanup of {self.kind}s may be necessary.'
-                )
+                msg = f'Setup did not complete successfully. ' f'Manual cleanup of {self.kind}s may be necessary.'
                 self.logger.warning(msg)
             self.logger.info('Cleaning up any existing snapshots...')
-            es_api.delete(
-                self.client, self.kind, ','.join(self.entity_list), repository=self.plan.repository)
+            es_api.delete(self.client, self.kind, ','.join(self.entity_list), repository=self.plan.repository)
             self.logger.info('Cleanup of snapshots completed.')
             self.entity_list = []
             self.failsafe = []
```

### Comparing `es_testbed-0.5.0/src/es_testbed/classes/entitymgrs/templatemgr.py` & `es_testbed-0.5.3/src/es_testbed/classes/entitymgrs/templatemgr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Index Template Entity Manager Class"""
+
 import typing as t
 from dotmap import DotMap
 from elasticsearch8 import Elasticsearch
 from es_testbed.exceptions import ResultNotExpected
 from es_testbed.helpers import es_api
 from es_testbed.helpers.utils import getlogger
 from .entitymgr import EntityMgr
 
 # pylint: disable=missing-docstring,too-many-arguments
 
+
 class TemplateMgr(EntityMgr):
     kind = 'template'
     listname = 'index_templates'
+
     def __init__(
-            self,
-            client: Elasticsearch = None,
-            plan: DotMap = None,
-            autobuild: t.Optional[bool] = True,
-        ):
+        self, client: t.Union[Elasticsearch, None] = None, plan: DotMap = None, autobuild: t.Optional[bool] = True
+    ):
         super().__init__(client=client, plan=plan, autobuild=autobuild)
         self.logger = getlogger('es_testbed.TemplateMgr')
 
     @property
     def logdisplay(self) -> str:
         return 'index template'
 
@@ -34,19 +34,14 @@
 
     def get_pattern(self, kind: str) -> str:
         return f'{self.plan.prefix}-{self.ident(dkey=kind)}-{self.plan.uniq}'
 
     def setup(self):
         ds = {} if self.plan.type == 'data_stream' else None
         es_api.put_idx_tmpl(
-            self.client,
-            self.name,
-            self.patterns,
-            components=self.plan.component_templates,
-            data_stream=ds
+            self.client, self.name, self.patterns, components=self.plan.component_templates, data_stream=ds
         )
         if not es_api.exists(self.client, self.kind, self.name):
-            raise ResultNotExpected(
-                f'Unable to verify creation of index template {self.name}')
+            raise ResultNotExpected(f'Unable to verify creation of index template {self.name}')
         self.appender(self.name)
         self.logger.debug('Successfully created index template: %s', self.last)
         self.success = True
```

### Comparing `es_testbed-0.5.0/src/es_testbed/helpers/es_api.py` & `es_testbed-0.5.3/src/es_testbed/helpers/es_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,124 +1,125 @@
 """Functions that make Elasticsearch API Calls"""
+
 import typing as t
 from os import getenv
 from elasticsearch8 import Elasticsearch, exceptions as esx
 from es_wait import Exists, Snapshot
 from es_testbed.defaults import MAPPING, PAUSE_DEFAULT, PAUSE_ENVVAR
 from es_testbed import exceptions as exc
 from es_testbed.helpers.utils import doc_gen, get_routing, getlogger, mounted_name, storage_type
+
 LOGGER = getlogger(__name__)
 PAUSE_VALUE = float(getenv(PAUSE_ENVVAR, default=PAUSE_DEFAULT))
 # pylint: disable=broad-except
 
-def emap(kind: str, es: Elasticsearch, value=None):
+
+def emap(kind: str, es: Elasticsearch, value=None) -> t.Dict[str, t.Any]:
     """Return a value from a dictionary"""
     _ = {
         'alias': {
             'delete': es.indices.delete_alias,
             'exists': es.indices.exists_alias,
             'get': es.indices.get_alias,
             'kwargs': {'index': value, 'expand_wildcards': ['open', 'closed']},
-            'plural': 'alias(es)'
+            'plural': 'alias(es)',
         },
         'data_stream': {
             'delete': es.indices.delete_data_stream,
             'exists': es.indices.exists,
             'get': es.indices.get_data_stream,
             'kwargs': {'name': value, 'expand_wildcards': ['open', 'closed']},
             'plural': 'data_stream(s)',
             'key': 'data_streams',
         },
         'index': {
             'delete': es.indices.delete,
             'exists': es.indices.exists,
             'get': es.indices.get,
             'kwargs': {'index': value, 'expand_wildcards': ['open', 'closed']},
-            'plural': 'index(es)'
+            'plural': 'index(es)',
         },
         'template': {
             'delete': es.indices.delete_index_template,
             'exists': es.indices.exists_index_template,
             'get': es.indices.get_index_template,
             'kwargs': {'name': value},
             'plural': 'index template(s)',
             'key': 'index_templates',
         },
         'ilm': {
             'delete': es.ilm.delete_lifecycle,
             'exists': es.ilm.get_lifecycle,
             'get': es.ilm.get_lifecycle,
             'kwargs': {'name': value},
-            'plural': 'ilm policy(ies)'
+            'plural': 'ilm policy(ies)',
         },
         'component': {
             'delete': es.cluster.delete_component_template,
             'exists': es.cluster.exists_component_template,
             'get': es.cluster.get_component_template,
             'kwargs': {'name': value},
             'plural': 'component template(s)',
             'key': 'component_templates',
         },
         'snapshot': {
             'delete': es.snapshot.delete,
             'exists': es.snapshot.get,
             'get': es.snapshot.get,
             'kwargs': {},
-            'plural': 'snapshot(s)'
-        }
+            'plural': 'snapshot(s)',
+        },
     }
     return _[kind]
 
-def change_ds(client: Elasticsearch, actions: dict=None) -> None:
+
+def change_ds(client: Elasticsearch, actions: t.Union[str, None] = None) -> None:
     """Change/Modify/Update a datastream"""
     try:
         client.indices.modify_data_stream(actions=actions, body=None)
     except Exception as err:
         raise exc.ResultNotExpected(f'Unable to modify datastreams. {err}') from err
 
+
 def create_data_stream(client: Elasticsearch, name: str) -> None:
     """Create a datastream"""
     try:
         client.indices.create_data_stream(name=name)
         test = Exists(client, name=name, kind='datastream', pause=PAUSE_VALUE)
         test.wait_for_it()
     except Exception as err:
-        raise exc.TestbedFailure(
-            f'Unable to create datastream {name}. Error: {err}') from err
+        raise exc.TestbedFailure(f'Unable to create datastream {name}. Error: {err}') from err
+
 
 def create_index(
-        client: Elasticsearch,
-        name: str,
-        aliases: dict=None,
-        settings: dict=None,
-        tier: str='hot'
-    ) -> None:
+    client: Elasticsearch,
+    name: str,
+    aliases: t.Union[t.Dict, None] = None,
+    settings: t.Union[t.Dict, None] = None,
+    tier: str = 'hot',
+) -> None:
     """Create named index"""
     if not settings:
         settings = get_routing(tier=tier)
     else:
         settings.update(get_routing(tier=tier))
-    client.indices.create(
-        index=name,
-        aliases=aliases,
-        mappings=MAPPING,
-        settings=settings
-    )
+    client.indices.create(index=name, aliases=aliases, mappings=MAPPING, settings=settings)
     try:
         test = Exists(client, name=name, kind='index', pause=PAUSE_VALUE)
         test.wait_for_it()
     except exc.TimeoutException as err:
         raise exc.ResultNotExpected(f'Failed to create index {name}') from err
     return exists(client, 'index', name)
 
-def delete(client: Elasticsearch, kind: str, name: str, repository: str=None):
+
+def delete(client: Elasticsearch, kind: str, name: str, repository: t.Union[str, None] = None) -> None:
     """Delete the named object of type kind"""
     which = emap(kind, client)
     func = which['delete']
-    if name is None: # Typically only with ilm
+    if name is None:  # Typically only with ilm
         LOGGER.debug('"%s" has a None value for name', kind)
         return
     try:
         if kind == 'snapshot':
             func(snapshot=name, repository=repository)
         elif kind == 'index':
             func(index=name)
@@ -129,29 +130,36 @@
     except Exception as err:
         raise exc.ResultNotExpected(f'Unexpected result: {err}') from err
     if exists(client, kind, name, repository=repository):
         LOGGER.critical('Unable to delete "%s" %s', kind, name)
         raise exc.ResultNotExpected(f'{kind} "{name}" still exists.')
     LOGGER.info('Successfully deleted %s: "%s"', which['plural'], name)
 
-def do_snap(client: Elasticsearch, repo: str, snap: str, idx: str, tier: str='cold') -> None:
+
+def do_snap(client: Elasticsearch, repo: str, snap: str, idx: str, tier: str = 'cold') -> None:
     """Perform a snapshot"""
     client.snapshot.create(repository=repo, snapshot=snap, indices=idx)
     test = Snapshot(client, action='snapshot', snapshot=snap, repository=repo, pause=1, timeout=60)
     test.wait_for_it()
 
     # Mount the index accordingly
     client.searchable_snapshots.mount(
-        repository=repo, snapshot=snap, index=idx, index_settings=get_routing(tier=tier),
-        renamed_index=mounted_name(idx, tier), storage=storage_type(tier),
-        wait_for_completion=True)
+        repository=repo,
+        snapshot=snap,
+        index=idx,
+        index_settings=get_routing(tier=tier),
+        renamed_index=mounted_name(idx, tier),
+        storage=storage_type(tier),
+        wait_for_completion=True,
+    )
     # Fix aliases
     fix_aliases(client, idx, mounted_name(idx, tier))
 
-def exists(client: Elasticsearch, kind: str, name: str, repository: str=None) -> bool:
+
+def exists(client: Elasticsearch, kind: str, name: str, repository: str = None) -> bool:
     """Return boolean existence of the named kind of object"""
     if name is None:
         return False
     retval = True
     func = emap(kind, client)['exists']
     try:
         if kind == 'snapshot':
@@ -164,21 +172,22 @@
             retval = func(name=name)
     except esx.NotFoundError:
         retval = False
     except Exception as err:
         raise exc.ResultNotExpected(f'Unexpected result: {err}') from err
     return retval
 
+
 def fill_index(
-        client: Elasticsearch,
-        name: str=None,
-        count: int=None,
-        start_num: int=None,
-        match: bool=True
-    ) -> None:
+    client: Elasticsearch,
+    name: t.Union[str, None] = None,
+    count: t.Union[int, None] = None,
+    start_num: t.Union[int, None] = None,
+    match: bool = True,
+) -> None:
     """
     Create and fill the named index with mappings and settings as directed
 
     :param client: ES client
     :param name: Index name
     :param count: The number of docs to create
     :param start_number: Where to start the incrementing number
@@ -194,30 +203,33 @@
     :returns: No return value
     """
     for doc in doc_gen(count=count, start_at=start_num, match=match):
         client.index(index=name, document=doc)
     client.indices.flush(index=name)
     client.indices.refresh(index=name)
 
+
 def find_write_index(client: Elasticsearch, name: str) -> t.AnyStr:
     """Find the write_index for an alias by searching any index the alias points to"""
     retval = None
     for alias in get_aliases(client, name):
         retval = get_write_index(client, alias)
         if retval:
             break
     return retval
 
+
 def fix_aliases(client: Elasticsearch, oldidx: str, newidx: str) -> None:
     """Fix aliases using the new and old index names as data"""
     # Delete the original index
     client.indices.delete(index=oldidx)
     # Add the original index name as an alias to the mounted index
     client.indices.put_alias(index=f'{newidx}', name=oldidx)
 
+
 def get(client: Elasticsearch, kind: str, pattern: str) -> t.Sequence[str]:
     """get any/all objects of type kind matching pattern"""
     if pattern is None:
         msg = f'"{kind}" has a None value for pattern'
         LOGGER.error(msg)
         raise exc.TestbedMisconfig(msg)
     which = emap(kind, client, value=pattern)
@@ -230,64 +242,70 @@
     if kind in ['data_stream', 'template', 'component']:
         retval = [x['name'] for x in result[which['key']]]
     else:
         # ['alias', 'ilm', 'index']
         retval = list(result.keys())
     return retval
 
+
 def get_aliases(client: Elasticsearch, name: str) -> t.Sequence[str]:
     """Get aliases from index 'name'"""
     res = client.indices.get(index=name)
     try:
         retval = list(res[name]['aliases'].keys())
     except KeyError:
         retval = None
     return retval
 
+
 def get_backing_indices(client: Elasticsearch, name: str) -> t.Sequence[str]:
     """Get the backing indices from the named data_stream"""
     resp = resolver(client, name)
     data_streams = resp['data_streams']
     retval = []
     if data_streams:
         if len(data_streams) > 1:
             raise exc.ResultNotExpected(f'Expected only a single data_stream matching {name}')
         retval = data_streams[0]['backing_indices']
     return retval
 
+
 def get_ds_current(client: Elasticsearch, name: str) -> str:
     """
     Find which index is the current 'write' index of the datastream
     This is best accomplished by grabbing the last backing_index
     """
     backers = get_backing_indices(client, name)
     retval = None
     if backers:
         retval = backers[-1]
     return retval
 
-def get_ilm(client: Elasticsearch, pattern: str) -> t.Union[t.Dict[str,str], None]:
+
+def get_ilm(client: Elasticsearch, pattern: str) -> t.Union[t.Dict[str, str], None]:
     """Get any ILM entity in ES that matches pattern"""
     try:
         return client.ilm.get_lifecycle(name=pattern)
     except Exception as err:
         msg = f'Unable to get ILM lifecycle matching {pattern}. Error: {err}'
         LOGGER.critical(msg)
         raise exc.ResultNotExpected(msg) from err
 
-def get_ilm_phases(client: Elasticsearch, name: str) -> dict:
+
+def get_ilm_phases(client: Elasticsearch, name: str) -> t.Dict:
     """Return the policy/phases part of the ILM policy identified by 'name'"""
     ilm = get_ilm(client, name)
     try:
         return ilm[name]['policy']['phases']
     except KeyError as err:
         msg = f'Unable to get ILM lifecycle named {name}. Error: {err}'
         LOGGER.critical(msg)
         raise exc.ResultNotExpected(msg) from err
-    
+
+
 def get_write_index(client: Elasticsearch, name: str) -> str:
     """
     Calls :py:meth:`~.elasticsearch.client.IndicesClient.get_alias`
 
     :param client: A client connection object
     :param name: An alias name
 
@@ -304,26 +322,28 @@
             if response[index]['aliases'][name]['is_write_index']:
                 retval = index
                 break
         except KeyError:
             continue
     return retval
 
+
 def snapshot_name(client: Elasticsearch, name: str) -> t.Union[t.AnyStr, None]:
     """Get the name of the snapshot behind the mounted index data"""
     res = {}
-    if exists(client, 'index', name): # Can jump straight to nested keys if it exists
+    if exists(client, 'index', name):  # Can jump straight to nested keys if it exists
         res = client.indices.get(index=name)[name]['settings']['index']
     try:
         retval = res['store']['snapshot']['snapshot_name']
     except KeyError:
         LOGGER.error('%s is not a searchable snapshot')
         retval = None
     return retval
 
+
 def ilm_explain(client: Elasticsearch, name: str) -> t.Union[t.Dict, None]:
     """Return the results from the ILM Explain API call for the named index"""
     try:
         retval = client.ilm.explain_lifecycle(index=name)['indices'][name]
     except KeyError:
         LOGGER.debug('Index name changed')
         new = list(client.ilm.explain_lifecycle(index=name)['indices'].keys())[0]
@@ -333,67 +353,70 @@
         raise exc.NameChanged(f'{name} was not found, likely due to a name change') from err
     except Exception as err:
         msg = f'Unable to get ILM information for index {name}'
         LOGGER.critical(msg)
         raise exc.ResultNotExpected(f'{msg}. Exception: {err}') from err
     return retval
 
-def ilm_move(client: Elasticsearch, name: str, current_step: dict, next_step: dict) -> None:
+
+def ilm_move(client: Elasticsearch, name: str, current_step: t.Dict, next_step: t.Dict) -> None:
     """Move index 'name' from the current step to the next step"""
     try:
         client.ilm.move_to_step(index=name, current_step=current_step, next_step=next_step)
     except Exception as err:
         msg = f'Unable to move index {name} to ILM next step: {next}. Error: {err}'
         LOGGER.critical(msg)
         raise exc.ResultNotExpected(msg)
 
-def put_comp_tmpl(client: Elasticsearch, name: str, component: dict) -> None:
+
+def put_comp_tmpl(client: Elasticsearch, name: str, component: t.Dict) -> None:
     """Publish a component template"""
     try:
         client.cluster.put_component_template(name=name, template=component, create=True)
         test = Exists(client, name=name, kind='component', pause=PAUSE_VALUE)
         test.wait_for_it()
     except Exception as err:
-        raise exc.TestbedFailure(
-            f'Unable to create component template {name}. Error: {err}') from err
+        raise exc.TestbedFailure(f'Unable to create component template {name}. Error: {err}') from err
+
 
 def put_idx_tmpl(
-        client, name: str, index_patterns: list, components: list,
-        data_stream: dict=None) -> None:
+    client, name: str, index_patterns: list, components: list, data_stream: t.Union[t.Dict, None] = None
+) -> None:
     """Publish an index template"""
     try:
         client.indices.put_index_template(
             name=name,
             composed_of=components,
             data_stream=data_stream,
             index_patterns=index_patterns,
             create=True,
         )
         test = Exists(client, name=name, kind='template', pause=PAUSE_VALUE)
         test.wait_for_it()
     except Exception as err:
-        raise exc.TestbedFailure(
-            f'Unable to create index template {name}. Error: {err}') from err
+        raise exc.TestbedFailure(f'Unable to create index template {name}. Error: {err}') from err
 
-def put_ilm(client: Elasticsearch, name: str, policy: dict=None) -> None:
+
+def put_ilm(client: Elasticsearch, name: str, policy: t.Union[t.Dict, None] = None) -> None:
     """Publish an ILM Policy"""
     try:
         client.ilm.put_lifecycle(name=name, policy=policy)
     except Exception as err:
-        raise exc.TestbedFailure(
-            f'Unable to put index lifecycle policy {name}. Error: {err}') from err
+        raise exc.TestbedFailure(f'Unable to put index lifecycle policy {name}. Error: {err}') from err
+
 
 def resolver(client: Elasticsearch, name: str) -> dict:
     """
     Resolve details about the entity, be it an index, alias, or data_stream
-    
+
     Because you can pass search patterns and aliases as name, each element comes back as an array:
-    
+
     {'indices': [], 'aliases': [], 'data_streams': []}
-    
+
     If you only resolve a single index or data stream, you will still have a 1-element list
     """
     return client.indices.resolve_index(name=name, expand_wildcards=['open', 'closed'])
 
+
 def rollover(client: Elasticsearch, name: str) -> None:
     """Rollover alias or datastream identified by name"""
     client.indices.rollover(alias=name, wait_for_active_shards='all')
```

### Comparing `es_testbed-0.5.0/src/es_testbed/helpers/utils.py` & `es_testbed-0.5.3/src/es_testbed/helpers/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 """Utility helper functions"""
+
 import typing as t
 import random
 import string
 import logging
 from copy import deepcopy
 from datetime import datetime, timezone
 from es_testbed.defaults import ilm_force_merge, ilm_phase, MAPPING, TIER
 from es_testbed.exceptions import TestbedMisconfig
 
+
 def build_ilm_phase(tier, actions=None, repository=None):
     """Build a single ILM policy step based on tier"""
     phase = ilm_phase(tier)
     if tier in ['cold', 'frozen']:
         if repository:
             phase[tier]['actions']['searchable_snapshot'] = {'snapshot_repository': repository}
         else:
             msg = f'Unable to build ILM phase for {tier} tier. Value for repository not provided'
             raise TestbedMisconfig(msg)
     if actions:
         phase[tier]['actions'].update(actions)
     return phase
 
-def build_ilm_policy(
-        tiers: list=None,
-        forcemerge: bool=False,
-        max_num_segments: int=1,
-        repository: str=None
-    ):
+
+def build_ilm_policy(tiers: list = None, forcemerge: bool = False, max_num_segments: int = 1, repository: str = None):
     """
     Build a full ILM policy based on the provided tiers.
     Put forcemerge in the last tier before cold or frozen (whichever comes first)
     """
     if not tiers:
         tiers = ['hot', 'delete']
     phases = {}
@@ -38,14 +36,15 @@
         raise TestbedMisconfig('Cannot build cold or frozen phase without repository')
     for tier in tiers:
         phases.update(build_ilm_phase(tier, repository=repository))
     if forcemerge:
         phases['hot']['actions'].update(ilm_force_merge(max_num_segments=max_num_segments))
     return {'phases': phases}
 
+
 def doc_gen(count=10, start_at=0, match=True):
     """Create this doc for each count"""
     keys = ['message', 'nested', 'deep']
     # Start with an empty map
     matchmap = {}
     # Iterate over each key
     for key in keys:
@@ -57,138 +56,141 @@
             # Otherwise matchmap[key] will have a random string value
             matchmap[key] = randomstr()
 
     # This is where count and start_at matter
     for num in range(start_at, start_at + count):
         yield {
             '@timestamp': iso8601_now(),
-            'message': f'{matchmap["message"]}{num}', # message# or randomstr#
-            'number': num if match else random.randint(1001, 32767), # value of num or random int
-            'nested': {
-                'key': f'{matchmap["nested"]}{num}' # nested#
-            },
-            'deep': {
-                'l1': {
-                    'l2': {
-                        'l3': f'{matchmap["deep"]}{num}' # deep#
-                    }
-                }
-            }
+            'message': f'{matchmap["message"]}{num}',  # message# or randomstr#
+            'number': num if match else random.randint(1001, 32767),  # value of num or random int
+            'nested': {'key': f'{matchmap["nested"]}{num}'},  # nested#
+            'deep': {'l1': {'l2': {'l3': f'{matchmap["deep"]}{num}'}}},  # deep#
         }
 
-def ds_action_generator(data_stream: str, index: str, action: str=None):
+
+def ds_action_generator(
+    data_stream: str, index: str, action: t.Union[t.Literal['add'], t.Literal['remove'], None] = None
+) -> t.Dict:
     """Generate a single add or remove backing index action for a data_stream"""
     if not action or action not in ['add', 'remove']:
         raise TestbedMisconfig('action must be "add" or "remove"')
-    return {
-        f'{action}_backing_index': {
-            'data_stream': data_stream,
-            'index': index
-        }
-    }
+    return {f'{action}_backing_index': {'data_stream': data_stream, 'index': index}}
+
 
 def getlogger(name: str) -> logging.getLogger:
     """Return a named logger"""
     return logging.getLogger(name)
 
+
 def get_routing(tier='hot'):
     """Return the routing allocation tier preference"""
     try:
         pref = TIER[tier]['pref']
     except KeyError:
         # Fallback value
         pref = 'data_content'
     return {'index.routing.allocation.include._tier_preference': pref}
 
+
 def iso8601_now() -> str:
     """
     :returns: An ISO8601 timestamp based on now
     :rtype: str
     """
     # Because Python 3.12 now requires non-naive timezone declarations, we must change.
     #
-    ### Example:
-    ### The new way:
-    ###     datetime.now(timezone.utc).isoformat()
-    ###     Result: 2024-04-16T16:00:00+00:00
-    ### End Example
+    # ## Example:
+    # ## The new way:
+    # ##     datetime.now(timezone.utc).isoformat()
+    # ##     Result: 2024-04-16T16:00:00+00:00
+    # ## End Example
     #
     # Note that the +00:00 is appended now where we affirmatively declare the UTC timezone
     #
     # As a result, we will use this function to prune away the timezone if it is +00:00 and replace
     # it with Z, which is shorter Zulu notation for UTC (which Elasticsearch uses)
     #
     # We are MANUALLY, FORCEFULLY declaring timezone.utc, so it should ALWAYS be +00:00, but could
     # in theory sometime show up as a Z, so we test for that.
 
     parts = datetime.now(timezone.utc).isoformat().split('+')
     if len(parts) == 1:
         if parts[0][-1] == 'Z':
-            return parts[0] # Our ISO8601 already ends with a Z for Zulu/UTC time
-        return f'{parts[0]}Z' # It doesn't end with a Z so we put one there
+            return parts[0]  # Our ISO8601 already ends with a Z for Zulu/UTC time
+        return f'{parts[0]}Z'  # It doesn't end with a Z so we put one there
     if parts[1] == '00:00':
-        return f'{parts[0]}Z' # It doesn't end with a Z so we put one there
-    return f'{parts[0]}+{parts[1]}' # Fallback publishes the +TZ, whatever that was
+        return f'{parts[0]}Z'  # It doesn't end with a Z so we put one there
+    return f'{parts[0]}+{parts[1]}'  # Fallback publishes the +TZ, whatever that was
+
 
 def mapping_component():
     """Return a mappings component template"""
     return {'mappings': MAPPING}
 
+
 def mounted_name(index, tier):
     """Return a value for renamed_index for mounting a searchable snapshot index"""
     return f'{TIER[tier]["prefix"]}-{index}'
 
+
 def posmatch(original: t.Sequence[str], compare: t.Sequence[str]) -> t.Sequence[int]:
     """
     Compare the values in compare with original. Return a list of index positions from
     compare of any values that match.
     """
     logger = getlogger(__name__)
     positions = []
     for orig in original:
         for idx, comp in enumerate(compare):
             if comp == orig:
                 logger.debug('Value %s found in both original and compare', comp)
                 positions.append(idx)
     return positions
 
-def randomstr(length: int=16, lowercase: bool=False):
+
+def randomstr(length: int = 16, lowercase: bool = False):
     """Generate a random string"""
     letters = string.ascii_uppercase
     if lowercase:
         letters = string.ascii_lowercase
     return str(''.join(random.choices(letters + string.digits, k=length)))
 
+
 def remove_by_index(original: t.Sequence[str], compare: t.Sequence[str]) -> t.Sequence[str]:
     """By list index position, remove entries from compare which also exist in original"""
     logger = getlogger(__name__)
     positions = posmatch(original, compare)
     if not positions:
         logger.debug('No matching values to remove')
         return compare
     # If you del list[0] first, you get a new list[0]
     # We need to delete from the highest index value to the lowest
-    positions.sort() # Sort first to ensure lowest to highest order
-    for idx in reversed(positions): # Reverse the list and iterate
-        del compare[idx] # Delete the value at position idx
+    positions.sort()  # Sort first to ensure lowest to highest order
+    for idx in reversed(positions):  # Reverse the list and iterate
+        del compare[idx]  # Delete the value at position idx
     return compare
 
-def setting_component(ilm_policy: str=None, rollover_alias: str=None):
+
+def setting_component(
+    ilm_policy: t.Union[str, None] = None, rollover_alias: t.Union[str, None] = None
+) -> t.Dict[str, t.Any]:
     """Return a settings component template"""
-    val = {'settings':{'index.number_of_replicas': 0}}
+    val = {'settings': {'index.number_of_replicas': 0}}
     if ilm_policy:
         val['settings']['index.lifecycle.name'] = ilm_policy
     if rollover_alias:
         val['settings']['index.lifecycle.rollover_alias'] = rollover_alias
     return val
 
-def storage_type(tier):
+
+def storage_type(tier: str) -> t.Dict:
     """Return the storage type of a searchable snapshot by tier"""
     return TIER[tier]["storage"]
 
+
 def uniq_values(original: t.Sequence[str], compare: t.Sequence[str]) -> t.Sequence[str]:
     """Return any values unique to list 'compare'"""
     logger = getlogger(__name__)
     # Use deepcopy of compare so we don't change the original
     uniq = remove_by_index(original, deepcopy(compare))
     if uniq:
         logger.debug('Values found only in compare: %s', uniq)
```

### Comparing `es_testbed-0.5.0/.gitignore` & `es_testbed-0.5.3/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
 
+
+.flake8
+
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
@@ -156,7 +159,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+.vscode
```

### Comparing `es_testbed-0.5.0/LICENSE` & `es_testbed-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/README.md` & `es_testbed-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `es_testbed-0.5.0/pyproject.toml` & `es_testbed-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     'testing',
     'datastream',
     'repository',
     'snapshot',
 ]
 dependencies = [
     'dotmap==1.3.30',
-    'es_client==8.13.1',
+    'es_client==8.13.2',
     'es-wait==0.3.3',
 ]
 
 [project.optional-dependencies]
 test = [
     'mock',
     'requests',
@@ -50,15 +50,15 @@
 
 [project.urls]
 Documentation = 'https://github.com/untergeek/es-testbed#readme'
 Issues = 'https://github.com/untergeek/es-testbed/issues'
 Source = 'https://github.com/untergeek/es-testbed'
 
 [tool.hatch.version]
-path = 'src/es_testbed/version.py'
+path = 'src/es_testbed/__init__.py'
 
 [tool.hatch.envs.default]
 dependencies = [
   'coverage[toml]>=6.5',
   'pytest',
 ]
```

### Comparing `es_testbed-0.5.0/PKG-INFO` & `es_testbed-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-testbed
-Version: 0.5.0
+Version: 0.5.3
 Summary: Library to help with building and tearing down indices, data streams, repositories and snapshots
 Project-URL: Documentation, https://github.com/untergeek/es-testbed#readme
 Project-URL: Issues, https://github.com/untergeek/es-testbed/issues
 Project-URL: Source, https://github.com/untergeek/es-testbed
 Author-email: Elastic <info@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: dotmap==1.3.30
-Requires-Dist: es-client==8.13.1
+Requires-Dist: es-client==8.13.2
 Requires-Dist: es-wait==0.3.3
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == 'doc'
 Requires-Dist: sphinx-rtd-theme; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: mock; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
```

