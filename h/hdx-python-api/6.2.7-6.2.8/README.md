# Comparing `tmp/hdx_python_api-6.2.7.tar.gz` & `tmp/hdx_python_api-6.2.8.tar.gz`

## Comparing `hdx_python_api-6.2.7.tar` & `hdx_python_api-6.2.8.tar`

### file list

```diff
@@ -1,128 +1,129 @@
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     4896 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.config/coveragerc
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.config/pytest.ini
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/documentation/.readthedocs.yaml
--rwxr-xr-x   0        0        0    45219 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/documentation/main.md
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/documentation/pydoc-markdown.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/api/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/api/_version.py
--rwxr-xr-x   0        0        0    24570 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/api/configuration.py
--rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/api/hdx_base_configuration.yaml
--rwxr-xr-x   0        0        0     4541 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/api/locations.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/api/remotehdx.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/__init__.py
--rwxr-xr-x   0        0        0   118959 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/dataset.py
--rwxr-xr-x   0        0        0     9438 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/dataset_title_helper.py
--rwxr-xr-x   0        0        0     6706 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/date_helper.py
--rwxr-xr-x   0        0        0     3575 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/filestore_helper.py
--rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/hdx_datasource_topline.yaml
--rwxr-xr-x   0        0        0    28529 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/hdxobject.py
--rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/indicator_resource_view_template.yaml
--rwxr-xr-x   0        0        0    11087 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/organization.py
--rwxr-xr-x   0        0        0    29270 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/resource.py
--rwxr-xr-x   0        0        0     4524 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/resource_matcher.py
--rwxr-xr-x   0        0        0     7672 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/resource_view.py
--rwxr-xr-x   0        0        0    15012 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/showcase.py
--rwxr-xr-x   0        0        0     9663 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/user.py
--rwxr-xr-x   0        0        0    22462 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/data/vocabulary.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/facades/__init__.py
--rwxr-xr-x   0        0        0     3860 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/facades/infer_arguments.py
--rwxr-xr-x   0        0        0     1113 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/facades/keyword_arguments.py
--rwxr-xr-x   0        0        0     1057 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/src/hdx/facades/simple.py
--rwxr-xr-x   0        0        0     6148 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/Accepted_Tags.csv
--rwxr-xr-x   0        0        0   169337 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/Tag_Mapping.csv
--rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/Tag_Mapping_ChainRuleError.csv
--rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/dataset_search_results.yaml
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/empty.csv
--rwxr-xr-x   0        0        0    13843 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/organization_show_results.yaml
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/resource_formats.json
--rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/showcase_all_search_results.yaml
--rwxr-xr-x   0        0        0     1548 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/test_data.csv
--rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/test_data.zip
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/CKAN/hdx_dataset_static.yaml
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/empty.yaml
--rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_base_config.json
--rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_base_config.yaml
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_config.yaml
--rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_dataset_static.json
--rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_dataset_static.yaml
--rwxr-xr-x   0        0        0      561 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_datasource_topline.json
--rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_datasource_topline.yaml
--rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_email_configuration.yaml
--rwxr-xr-x   0        0        0       76 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_missing_site_config.json
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_organization_static.json
--rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_organization_static.yaml
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_resource_static.json
--rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_resource_static.yaml
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_resource_view_static.json
--rwxr-xr-x   0        0        0     1175 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_resource_view_static.yaml
--rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_showcase_static.json
--rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_showcase_static.yaml
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_user_static.json
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_user_static.yaml
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_vocabulary_static.json
--rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/hdx_vocabulary_static.yaml
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/project_configuration.yaml
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/user_agent_config.yaml
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/user_agent_config2.yaml
--rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/user_agent_config3.yaml
--rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/config/user_agent_config_wrong.yaml
--rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
--rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/gen_resource/conflict_data_alg.csv
--rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/gen_resource/test_data_no_data.csv
--rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/gen_resource/test_data_no_years.csv
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
--rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
--rw-r--r--   0        0        0    37596 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/expected_resources_to_update.json
--rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
--rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
--rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
--rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
--rw-r--r--   0        0        0   842237 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
--rw-r--r--   0        0        0    48524 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/unesco_dataset.json
--rw-r--r--   0        0        0    38435 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
--rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_logic/update_logic_resources.yaml
--rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/fixtures/update_logic/update_logic_resources_new.yaml
--rwxr-xr-x   0        0        0    45086 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/conftest.py
--rw-r--r--   0        0        0    10613 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/api/test_ckan.py
--rwxr-xr-x   0        0        0    36252 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/api/test_configuration.py
--rwxr-xr-x   0        0        0     3009 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/api/test_locations.py
--rwxr-xr-x   0        0        0     9940 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/__init__.py
--rwxr-xr-x   0        0        0    49910 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_dataset_core.py
--rwxr-xr-x   0        0        0    77175 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_dataset_noncore.py
--rwxr-xr-x   0        0        0    11850 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_dataset_title_helper.py
--rwxr-xr-x   0        0        0    19579 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_organization.py
--rwxr-xr-x   0        0        0    48267 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_resource.py
--rwxr-xr-x   0        0        0    19115 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_resource_view.py
--rwxr-xr-x   0        0        0    23052 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_showcase.py
--rw-r--r--   0        0        0    10361 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_update_dataset_resources.py
--rw-r--r--   0        0        0    56414 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_update_logic.py
--rwxr-xr-x   0        0        0    21178 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_user.py
--rwxr-xr-x   0        0        0   116053 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/data/test_vocabulary.py
--rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/facades/__init__.py
--rwxr-xr-x   0        0        0     3184 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/facades/test_infer_arguments.py
--rwxr-xr-x   0        0        0     5962 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/facades/test_keyword_arguments.py
--rwxr-xr-x   0        0        0     5656 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/tests/hdx/facades/test_simple.py
--rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/workingexample/my_code.py
--rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/workingexample/my_resource.csv
--rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/workingexample/my_resource.xlsx
--rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/workingexample/run.py
--rwxr-xr-x   0        0        0     1203 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/.gitignore
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/LICENSE
--rwxr-xr-x   0        0        0     1207 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/README.md
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/pyproject.toml
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 hdx_python_api-6.2.7/PKG-INFO
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     4892 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/.config/coveragerc
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/.config/pytest.ini
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/documentation/.readthedocs.yaml
+-rwxr-xr-x   0        0        0    45406 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/documentation/main.md
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/api/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/api/_version.py
+-rwxr-xr-x   0        0        0    24570 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/api/configuration.py
+-rwxr-xr-x   0        0        0     2023 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/api/hdx_base_configuration.yaml
+-rwxr-xr-x   0        0        0     4541 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/api/locations.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/api/remotehdx.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0   118934 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/dataset.py
+-rwxr-xr-x   0        0        0     9438 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/dataset_title_helper.py
+-rwxr-xr-x   0        0        0     6706 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/date_helper.py
+-rwxr-xr-x   0        0        0     3626 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/filestore_helper.py
+-rwxr-xr-x   0        0        0      366 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0    28529 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/hdxobject.py
+-rwxr-xr-x   0        0        0     2915 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/indicator_resource_view_template.yaml
+-rwxr-xr-x   0        0        0    11087 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/organization.py
+-rwxr-xr-x   0        0        0    29313 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/resource.py
+-rwxr-xr-x   0        0        0     4524 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/resource_matcher.py
+-rwxr-xr-x   0        0        0     7672 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/resource_view.py
+-rwxr-xr-x   0        0        0    15012 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/showcase.py
+-rwxr-xr-x   0        0        0     9663 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/user.py
+-rwxr-xr-x   0        0        0    22462 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/data/vocabulary.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3860 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/facades/infer_arguments.py
+-rwxr-xr-x   0        0        0     1113 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/facades/keyword_arguments.py
+-rwxr-xr-x   0        0        0     1057 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/src/hdx/facades/simple.py
+-rwxr-xr-x   0        0        0     6148 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/Accepted_Tags.csv
+-rwxr-xr-x   0        0        0   169337 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/Tag_Mapping.csv
+-rwxr-xr-x   0        0        0      234 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/Tag_Mapping_ChainRuleError.csv
+-rwxr-xr-x   0        0        0    25870 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/dataset_search_results.yaml
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/empty.csv
+-rwxr-xr-x   0        0        0    13843 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/organization_show_results.yaml
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/resource_formats.json
+-rwxr-xr-x   0        0        0    14465 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/showcase_all_search_results.yaml
+-rwxr-xr-x   0        0        0     1548 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/test_data.csv
+-rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/test_data.zip
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/CKAN/hdx_dataset_static.yaml
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/empty.yaml
+-rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_base_config.json
+-rwxr-xr-x   0        0        0      373 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_base_config.yaml
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_config.yaml
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_dataset_static.json
+-rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_dataset_static.yaml
+-rwxr-xr-x   0        0        0      561 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_datasource_topline.json
+-rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_datasource_topline.yaml
+-rwxr-xr-x   0        0        0      173 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_email_configuration.yaml
+-rwxr-xr-x   0        0        0       76 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_missing_site_config.json
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_organization_static.json
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_organization_static.yaml
+-rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_resource_static.json
+-rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_resource_static.yaml
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_resource_view_static.json
+-rwxr-xr-x   0        0        0     1175 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_resource_view_static.yaml
+-rwxr-xr-x   0        0        0      222 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_showcase_static.json
+-rwxr-xr-x   0        0        0      188 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_showcase_static.yaml
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_user_static.json
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_user_static.yaml
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_vocabulary_static.json
+-rwxr-xr-x   0        0        0       39 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/hdx_vocabulary_static.yaml
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0        0        0      420 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/project_configuration.yaml
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/user_agent_config.yaml
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/user_agent_config2.yaml
+-rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/user_agent_config3.yaml
+-rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/config/user_agent_config_wrong.yaml
+-rwxr-xr-x   0        0        0    23724 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
+-rwxr-xr-x   0        0        0     1788 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/gen_resource/conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/gen_resource/test_data_no_data.csv
+-rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/gen_resource/test_data_no_years.csv
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
+-rw-r--r--   0        0        0    50900 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0    37596 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/expected_resources_to_update.json
+-rw-r--r--   0        0        0   319924 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
+-rw-r--r--   0        0        0    92805 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   290790 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
+-rw-r--r--   0        0        0   230593 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
+-rw-r--r--   0        0        0   216041 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
+-rw-r--r--   0        0        0   842237 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
+-rw-r--r--   0        0        0    48524 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/unesco_dataset.json
+-rw-r--r--   0        0        0    38435 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
+-rw-r--r--   0        0        0    24658 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_logic/update_logic_resources.yaml
+-rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/fixtures/update_logic/update_logic_resources_new.yaml
+-rwxr-xr-x   0        0        0    45086 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/conftest.py
+-rw-r--r--   0        0        0    10613 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/api/test_ckan.py
+-rwxr-xr-x   0        0        0    36252 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/api/test_configuration.py
+-rwxr-xr-x   0        0        0     3009 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/api/test_locations.py
+-rwxr-xr-x   0        0        0    10196 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/__init__.py
+-rwxr-xr-x   0        0        0    49910 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/test_dataset_core.py
+-rwxr-xr-x   0        0        0    77175 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/test_dataset_noncore.py
+-rwxr-xr-x   0        0        0    11850 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/test_dataset_title_helper.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/test_filestore_helper.py
+-rwxr-xr-x   0        0        0    19579 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/test_organization.py
+-rwxr-xr-x   0        0        0    48001 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/test_resource.py
+-rwxr-xr-x   0        0        0    19115 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/test_resource_view.py
+-rwxr-xr-x   0        0        0    23052 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/test_showcase.py
+-rw-r--r--   0        0        0    10495 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/test_update_dataset_resources.py
+-rw-r--r--   0        0        0    56414 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/test_update_logic.py
+-rwxr-xr-x   0        0        0    21178 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/test_user.py
+-rwxr-xr-x   0        0        0   116053 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/data/test_vocabulary.py
+-rwxr-xr-x   0        0        0     1489 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/facades/__init__.py
+-rwxr-xr-x   0        0        0     3184 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/facades/test_infer_arguments.py
+-rwxr-xr-x   0        0        0     5962 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/facades/test_keyword_arguments.py
+-rwxr-xr-x   0        0        0     5656 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/tests/hdx/facades/test_simple.py
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/workingexample/my_code.py
+-rwxr-xr-x   0        0        0       12 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/workingexample/my_resource.csv
+-rwxr-xr-x   0        0        0     4755 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/workingexample/my_resource.xlsx
+-rwxr-xr-x   0        0        0      393 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/workingexample/run.py
+-rwxr-xr-x   0        0        0     1203 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/.gitignore
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/LICENSE
+-rwxr-xr-x   0        0        0     1207 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/README.md
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 hdx_python_api-6.2.8/PKG-INFO
```

### Comparing `hdx_python_api-6.2.7/CONTRIBUTING.md` & `hdx_python_api-6.2.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/requirements.txt` & `hdx_python_api-6.2.8/requirements.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 chardet==5.2.0
     # via frictionless
 charset-normalizer==3.3.2
     # via requests
 ckanapi==4.8
 click==8.1.7
     # via typer
-coverage==7.4.4
+coverage==7.5.0
     # via pytest-cov
 cryptography==42.0.5
     # via pyopenssl
 defopt==6.4.0
 distlib==0.3.8
     # via virtualenv
 dnspython==2.6.1
     # via email-validator
 docopt==0.6.2
     # via
     #   ckanapi
     #   num2words
-docutils==0.21.post1
+docutils==0.21.2
     # via defopt
 email-validator==2.1.1
 et-xmlfile==1.1.0
     # via openpyxl
 filelock==3.13.4
     # via virtualenv
 frictionless==5.16.1
@@ -48,27 +48,27 @@
     # via
     #   google-auth-oauthlib
     #   gspread
 google-auth-oauthlib==1.2.0
     # via gspread
 gspread==6.1.0
 hdx-python-country==3.7.0
-hdx-python-utilities==3.6.7
+hdx-python-utilities==3.6.8
     # via hdx-python-country
 humanize==4.9.0
     # via frictionless
-identify==2.5.35
+identify==2.5.36
     # via pre-commit
-idna==3.6
+idna==3.7
     # via
     #   email-validator
     #   requests
 ijson==3.2.3
     # via hdx-python-utilities
-inflect==7.2.0
+inflect==7.2.1
     # via quantulum3
 iniconfig==2.0.0
     # via pytest
 isodate==0.6.1
     # via frictionless
 jinja2==3.1.3
     # via frictionless
@@ -104,17 +104,17 @@
     # via requests-oauthlib
 openpyxl==3.1.2
     # via hdx-python-utilities
 packaging==24.0
     # via pytest
 petl==1.7.15
     # via frictionless
-platformdirs==4.2.0
+platformdirs==4.2.1
     # via virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 ply==3.11
     # via
     #   jsonpath-ng
     #   libhxl
 pockets==0.9.1
     # via sphinxcontrib-napoleon
@@ -124,17 +124,17 @@
     #   ndg-httpsclient
     #   pyasn1-modules
     #   rsa
 pyasn1-modules==0.4.0
     # via google-auth
 pycparser==2.22
     # via cffi
-pydantic==2.6.4
+pydantic==2.7.1
     # via frictionless
-pydantic-core==2.16.3
+pydantic-core==2.18.2
     # via pydantic
 pygments==2.17.2
     # via rich
 pyopenssl==24.1.0
     # via ndg-httpsclient
 pyphonetics==0.5.3
     # via hdx-python-country
@@ -155,15 +155,15 @@
     #   ckanapi
     #   frictionless
 pyyaml==6.0.1
     # via
     #   frictionless
     #   pre-commit
     #   tableschema-to-template
-quantulum3==0.9.0
+quantulum3==0.9.1
 ratelimit==2.2.1
     # via hdx-python-utilities
 requests==2.31.0
     # via
     #   ckanapi
     #   frictionless
     #   libhxl
@@ -179,15 +179,15 @@
     # via typer
 rsa==4.9
     # via google-auth
 ruamel-yaml==0.18.6
     # via hdx-python-utilities
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-setuptools==69.2.0
+setuptools==69.5.1
     # via
     #   ckanapi
     #   nodeenv
 shellingham==1.5.4
     # via typer
 simpleeval==0.9.13
     # via frictionless
@@ -230,17 +230,17 @@
     # via
     #   libhxl
     #   pyphonetics
 urllib3==2.2.1
     # via
     #   libhxl
     #   requests
-validators==0.28.0
+validators==0.28.1
     # via frictionless
-virtualenv==20.25.1
+virtualenv==20.26.0
     # via pre-commit
 wheel==0.43.0
     # via libhxl
 xlrd==2.0.1
     # via hdx-python-utilities
 xlrd3==1.1.0
     # via libhxl
```

### Comparing `hdx_python_api-6.2.7/.config/pre-commit-config.yaml` & `hdx_python_api-6.2.8/.config/pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     rev: v4.5.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
         exclude: test_scraper_.*\.json
       - id: check-ast
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.2
+    rev: v0.4.2
     hooks:
       # Run the linter.
       - id: ruff
         args: [--config, .config/ruff.toml, --fix]
       # Run the formatter.
       - id: ruff-format
         args: [--config, .config/ruff.toml]
   - repo: https://github.com/astral-sh/uv-pre-commit
-    rev: v0.1.24
+    rev: 0.1.38
     hooks:
       # Run the pip compile
       - id: pip-compile
         name: pip-compile requirements.txt
         files: pyproject.toml
         args: [ pyproject.toml, --resolver=backtracking, --all-extras, --upgrade, -q, -o, requirements.txt ]
```

### Comparing `hdx_python_api-6.2.7/.github/workflows/publish.yaml` & `hdx_python_api-6.2.8/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/.github/workflows/run-python-tests.yaml` & `hdx_python_api-6.2.8/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/documentation/main.md` & `hdx_python_api-6.2.8/documentation/main.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,18 @@
 HDX.
 
 The code for the library is [here](https://github.com/OCHA-DAP/hdx-python-api).
 The library has detailed API documentation which can be found in the menu at the top.
 
 
 ## Breaking Changes
+From 6.2.8, fix mark_data_updated which was broken due to an error in 
+dataset_update_filestore_resource in which timezone information was 
+incorrectly added to the iso formatted string
+
 From 6.2.7, generate_resource_from_iterator renamed to
 generate_resource_from_iterable with requirement of iterable rather iterator
 
 From 6.2.6, kwargs take preference over environment variables which take
 preference over configuration files
 
 From 6.2.5, environment variables take preference over kwargs which take
```

### Comparing `hdx_python_api-6.2.7/documentation/pydoc-markdown.yaml` & `hdx_python_api-6.2.8/documentation/pydoc-markdown.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/api/configuration.py` & `hdx_python_api-6.2.8/src/hdx/api/configuration.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/api/hdx_base_configuration.yaml` & `hdx_python_api-6.2.8/src/hdx/api/hdx_base_configuration.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/api/locations.py` & `hdx_python_api-6.2.8/src/hdx/api/locations.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/api/remotehdx.py` & `hdx_python_api-6.2.8/src/hdx/api/remotehdx.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/data/dataset.py` & `hdx_python_api-6.2.8/src/hdx/data/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Dataset class containing all logic for creating, checking, and updating datasets and associated resources."""
 
 import json
 import logging
 import sys
 import warnings
 from copy import deepcopy
-from datetime import datetime, timezone
+from datetime import datetime
 from os.path import isfile, join
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Iterable,
@@ -37,14 +37,15 @@
 from hdx.data.resource_matcher import ResourceMatcher
 from hdx.location.country import Country
 from hdx.utilities.base_downloader import BaseDownload
 from hdx.utilities.dateparse import (
     default_date,
     default_enddate,
     now_utc,
+    now_utc_notz,
     parse_date,
     parse_date_range,
 )
 from hdx.utilities.dictandlist import merge_two_dictionaries, write_list_to_csv
 from hdx.utilities.downloader import Download
 from hdx.utilities.loader import load_json
 from hdx.utilities.path import script_dir_plus_file
@@ -594,17 +595,17 @@
         """
         self.clean_tags()
         scriptinfo = kwargs.get("updated_by_script")
         if scriptinfo:
             del kwargs["updated_by_script"]
         else:
             scriptinfo = self.configuration.get_user_agent()
-        # No need to output timezone info here
+        # Should not output timezone info here
         data["updated_by_script"] = (
-            f"{scriptinfo} ({datetime.now(timezone.utc).replace(tzinfo=None).isoformat(timespec='microseconds')})"
+            f"{scriptinfo} ({now_utc_notz().isoformat(timespec='microseconds')})"
         )
         batch = kwargs.get("batch")
         if batch:
             if not is_valid_uuid(batch):
                 raise HDXError(f"{batch} is not a valid UUID!")
             data["batch"] = batch
             del kwargs["batch"]
```

### Comparing `hdx_python_api-6.2.7/src/hdx/data/dataset_title_helper.py` & `hdx_python_api-6.2.8/src/hdx/data/dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/data/date_helper.py` & `hdx_python_api-6.2.8/src/hdx/data/date_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/data/filestore_helper.py` & `hdx_python_api-6.2.8/src/hdx/data/filestore_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Helper to the Dataset class for handling resources with filestores."""
 
-from datetime import datetime, timezone
 from typing import TYPE_CHECKING, Any, Dict
 
+from hdx.utilities.dateparse import now_utc_notz
+
 if TYPE_CHECKING:
     from hdx.data.resource import Resource
 
 
 class FilestoreHelper:
     temporary_url = "updated_by_file_upload_step"
 
@@ -86,11 +87,12 @@
         file_to_upload = resource_data_to_update.get_file_to_upload()
         if file_to_upload:
             filestore_resources[resource_index] = file_to_upload
             resource_data_to_update["url"] = cls.temporary_url
 
         data_updated = resource_data_to_update.is_marked_data_updated()
         if data_updated:
-            resource_data_to_update["last_modified"] = datetime.now(
-                timezone.utc
-            ).isoformat(timespec="microseconds")
+            # Should not output timezone info here
+            resource_data_to_update["last_modified"] = (
+                now_utc_notz().isoformat(timespec="microseconds")
+            )
             resource_data_to_update.data_updated = False
```

### Comparing `hdx_python_api-6.2.7/src/hdx/data/hdxobject.py` & `hdx_python_api-6.2.8/src/hdx/data/hdxobject.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/data/indicator_resource_view_template.yaml` & `hdx_python_api-6.2.8/src/hdx/data/indicator_resource_view_template.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/data/organization.py` & `hdx_python_api-6.2.8/src/hdx/data/organization.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/data/resource.py` & `hdx_python_api-6.2.8/src/hdx/data/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Resource class containing all logic for creating, checking, and updating resources."""
 
 import logging
 import warnings
-from datetime import datetime, timezone
+from datetime import datetime
 from os.path import join
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import hdx.data.dataset
 import hdx.data.filestore_helper as filestore_helper
 from hdx.api.configuration import Configuration
 from hdx.data.date_helper import DateHelper
 from hdx.data.hdxobject import HDXError, HDXObject
 from hdx.data.resource_view import ResourceView
-from hdx.utilities.dateparse import now_utc, parse_date
+from hdx.utilities.dateparse import now_utc, now_utc_notz, parse_date
 from hdx.utilities.downloader import Download
 from hdx.utilities.typehint import ListTuple
 from hdx.utilities.uuid import is_valid_uuid
 
 logger = logging.getLogger(__name__)
 
 
@@ -389,17 +389,18 @@
             data_updated (bool): If True, set last_modified to now. Defaults to False.
 
         Returns:
             None
         """
         data_updated = kwargs.pop("data_updated", self.data_updated)
         if data_updated and not self.file_to_upload:
-            self.old_data["last_modified"] = datetime.now(
-                timezone.utc
-            ).isoformat(timespec="microseconds")
+            # Should not output timezone info here
+            self.old_data["last_modified"] = now_utc_notz().isoformat(
+                timespec="microseconds"
+            )
             self.data_updated = False
             # old_data will be merged into data in the next step
         self._merge_hdx_update(
             "resource", "id", self._get_files(), True, **kwargs
         )
 
     def update_in_hdx(self, **kwargs: Any) -> None:
```

### Comparing `hdx_python_api-6.2.7/src/hdx/data/resource_matcher.py` & `hdx_python_api-6.2.8/src/hdx/data/resource_matcher.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/data/resource_view.py` & `hdx_python_api-6.2.8/src/hdx/data/resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/data/showcase.py` & `hdx_python_api-6.2.8/src/hdx/data/showcase.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/data/user.py` & `hdx_python_api-6.2.8/src/hdx/data/user.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/data/vocabulary.py` & `hdx_python_api-6.2.8/src/hdx/data/vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/facades/infer_arguments.py` & `hdx_python_api-6.2.8/src/hdx/facades/infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/facades/keyword_arguments.py` & `hdx_python_api-6.2.8/src/hdx/facades/keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/src/hdx/facades/simple.py` & `hdx_python_api-6.2.8/src/hdx/facades/simple.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/Accepted_Tags.csv` & `hdx_python_api-6.2.8/tests/fixtures/Accepted_Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/Tag_Mapping.csv` & `hdx_python_api-6.2.8/tests/fixtures/Tag_Mapping.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/dataset_search_results.yaml` & `hdx_python_api-6.2.8/tests/fixtures/dataset_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/organization_show_results.yaml` & `hdx_python_api-6.2.8/tests/fixtures/organization_show_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/resource_formats.json` & `hdx_python_api-6.2.8/tests/fixtures/resource_formats.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/showcase_all_search_results.yaml` & `hdx_python_api-6.2.8/tests/fixtures/showcase_all_search_results.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/test_data.csv` & `hdx_python_api-6.2.8/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/test_data.zip` & `hdx_python_api-6.2.8/tests/fixtures/test_data.zip`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/config/hdx_dataset_static.json` & `hdx_python_api-6.2.8/tests/fixtures/config/hdx_dataset_static.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/config/hdx_dataset_static.yaml` & `hdx_python_api-6.2.8/tests/fixtures/config/hdx_dataset_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/config/hdx_datasource_topline.json` & `hdx_python_api-6.2.8/tests/fixtures/config/hdx_datasource_topline.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/config/hdx_resource_view_static.yaml` & `hdx_python_api-6.2.8/tests/fixtures/config/hdx_resource_view_static.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx` & `hdx_python_api-6.2.8/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/gen_resource/conflict_data_alg.csv` & `hdx_python_api-6.2.8/tests/fixtures/gen_resource/conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/gen_resource/qc_conflict_data_alg.csv` & `hdx_python_api-6.2.8/tests/fixtures/gen_resource/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/gen_resource/test_data_no_years.csv` & `hdx_python_api-6.2.8/tests/fixtures/gen_resource/test_data_no_years.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv` & `hdx_python_api-6.2.8/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/dem_data_zwe.csv` & `hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/dem_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv` & `hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/expected_resources_to_update.json` & `hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/expected_resources_to_update.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/opri_data_zwe.csv` & `hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/opri_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv` & `hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv` & `hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv` & `hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv` & `hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv` & `hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv` & `hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/unesco_dataset.json` & `hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/unesco_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_dataset_resources/unesco_update_dataset.json` & `hdx_python_api-6.2.8/tests/fixtures/update_dataset_resources/unesco_update_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_logic/update_logic_resources.yaml` & `hdx_python_api-6.2.8/tests/fixtures/update_logic/update_logic_resources.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/fixtures/update_logic/update_logic_resources_new.yaml` & `hdx_python_api-6.2.8/tests/fixtures/update_logic/update_logic_resources_new.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/conftest.py` & `hdx_python_api-6.2.8/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/api/test_ckan.py` & `hdx_python_api-6.2.8/tests/hdx/api/test_ckan.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/api/test_configuration.py` & `hdx_python_api-6.2.8/tests/hdx/api/test_configuration.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/api/test_locations.py` & `hdx_python_api-6.2.8/tests/hdx/api/test_locations.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/data/__init__.py` & `hdx_python_api-6.2.8/tests/hdx/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,24 @@
         "description": "Resource2",
         "name": "Resource2",
         "url": "http://resource2.xls",
         "format": "xls",
     },
 ]
 
+resource_data = {
+    "name": "MyResource1",
+    "package_id": "6f36a41c-f126-4b18-aaaf-6c2ddfbc5d4d",
+    "format": "xlsx",
+    "url": "http://test/spreadsheet.xlsx",
+    "description": "My Resource",
+    "api_type": "api",
+    "resource_type": "api",
+}
+
 organization_data = {
     "name": "MyOrganization1",
     "title": "Humanitarian Organization",
     "description": "We do humanitarian work",
 }
 
 user_data = {
```

### Comparing `hdx_python_api-6.2.7/tests/hdx/data/test_dataset_core.py` & `hdx_python_api-6.2.8/tests/hdx/data/test_dataset_core.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/data/test_dataset_noncore.py` & `hdx_python_api-6.2.8/tests/hdx/data/test_dataset_noncore.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/data/test_dataset_title_helper.py` & `hdx_python_api-6.2.8/tests/hdx/data/test_dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/data/test_organization.py` & `hdx_python_api-6.2.8/tests/hdx/data/test_organization.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/data/test_resource.py` & `hdx_python_api-6.2.8/tests/hdx/data/test_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from datetime import datetime, timezone
 from os import remove
 from os.path import basename, join
 
 import pytest
 
-from . import MockResponse, dataset_resultdict
+from . import MockResponse, dataset_resultdict, resource_data
 from .test_resource_view import resource_view_list, resource_view_mocklist
 from hdx.api.configuration import Configuration
 from hdx.data.hdxobject import HDXError
 from hdx.data.resource import Resource
 from hdx.utilities.dateparse import parse_date
 from hdx.utilities.dictandlist import merge_two_dictionaries
 from hdx.utilities.downloader import DownloadError
@@ -314,24 +314,14 @@
     return MockResponse(
         404,
         '{"success": false, "error": {"message": "TEST ERROR: Not show", "__type": "TEST ERROR: Not Show Error"}, "help": "http://test-data.humdata.org/api/3/action/help_show?name=resource_view_show"}',
     )
 
 
 class TestResource:
-    resource_data = {
-        "name": "MyResource1",
-        "package_id": "6f36a41c-f126-4b18-aaaf-6c2ddfbc5d4d",
-        "format": "xlsx",
-        "url": "http://test/spreadsheet.xlsx",
-        "description": "My Resource",
-        "api_type": "api",
-        "resource_type": "api",
-    }
-
     datastore = None
 
     @pytest.fixture(scope="class")
     def static_yaml(self):
         return join("tests", "fixtures", "config", "hdx_resource_static.yaml")
 
     @pytest.fixture(scope="class")
@@ -681,23 +671,23 @@
             "74b74ae1-df0c-4716-829f-4f939a046813"
         )
         assert resource is None
         with pytest.raises(HDXError):
             Resource.read_from_hdx("ABC")
 
     def test_check_url_filetoupload(self, configuration):
-        resource_data = copy.deepcopy(TestResource.resource_data)
-        resource = Resource(resource_data)
+        resource_data_copy = copy.deepcopy(resource_data)
+        resource = Resource(resource_data_copy)
         resource.check_url_filetoupload()
         resource.set_file_to_upload("abc")
         resource.check_url_filetoupload()
         resource["url"] = "lala"
         with pytest.raises(HDXError):
             resource.check_url_filetoupload()
-        resource = Resource(resource_data)
+        resource = Resource(resource_data_copy)
         resource["format"] = "NOTEXIST"
         with pytest.raises(HDXError):
             resource.check_url_filetoupload()
         with pytest.raises(HDXError):
             resource.set_format("NOTEXIST")
         del resource["format"]
         with pytest.raises(HDXError):
@@ -722,41 +712,41 @@
             "enddate": datetime(2020, 10, 20, 23, 59, 59, tzinfo=timezone.utc),
             "startdate_str": "09/02/2020",
             "enddate_str": "20/10/2020",
             "ongoing": False,
         }
 
     def test_check_required_fields(self, configuration):
-        resource_data = copy.deepcopy(TestResource.resource_data)
-        resource = Resource(resource_data)
+        resource_data_copy = copy.deepcopy(resource_data)
+        resource = Resource(resource_data_copy)
         resource.check_url_filetoupload()
         resource.check_required_fields()
 
     def test_create_in_hdx(self, configuration, date_pattern, post_create):
         resource = Resource()
         with pytest.raises(HDXError):
             resource.create_in_hdx()
         resource["id"] = "74b74ae1-df0c-4716-829f-4f939a046811"
         resource["name"] = "LALA"
         with pytest.raises(HDXError):
             resource.create_in_hdx()
 
-        resource_data = copy.deepcopy(TestResource.resource_data)
-        resource = Resource(resource_data)
+        resource_data_copy = copy.deepcopy(resource_data)
+        resource = Resource(resource_data_copy)
         resource.create_in_hdx()
         assert resource["id"] == "de6549d8-268b-4dfe-adaf-a4ae5c8510d5"
         assert resource["url_type"] == "api"
         assert resource["resource_type"] == "api"
         assert (
             resource["url"]
             == "https://raw.githubusercontent.com/OCHA-DAP/hdx-python-api/main/tests/fixtures/test_data.csv"
         )
 
-        resource_data = copy.deepcopy(TestResource.resource_data)
-        resource = Resource(resource_data)
+        resource_data_copy = copy.deepcopy(resource_data)
+        resource = Resource(resource_data_copy)
         filetoupload = join("tests", "fixtures", "test_data.csv")
         resource.set_file_to_upload(filetoupload)
         assert resource.get_file_to_upload() == filetoupload
         resource.create_in_hdx()
         assert resource["url_type"] == "upload"
         assert resource["resource_type"] == "file.upload"
         assert (
@@ -766,21 +756,21 @@
         assert resource["state"] == "active"
         resource.set_file_to_upload(filetoupload)
         resource.create_in_hdx()
         assert (
             resource["url"]
             == "http://test-data.humdata.org/dataset/6f36a41c-f126-4b18-aaaf-6c2ddfbc5d4d/resource/de6549d8-268b-4dfe-adaf-a4ae5c8510d5/download/test_data.csv"
         )
-        resource_data["name"] = "MyResource2"
-        resource = Resource(resource_data)
+        resource_data_copy["name"] = "MyResource2"
+        resource = Resource(resource_data_copy)
         with pytest.raises(HDXError):
             resource.create_in_hdx()
 
-        resource_data["name"] = "MyResource3"
-        resource = Resource(resource_data)
+        resource_data_copy["name"] = "MyResource3"
+        resource = Resource(resource_data_copy)
         with pytest.raises(HDXError):
             resource.create_in_hdx()
 
     def test_update_in_hdx(self, configuration, date_pattern, post_update):
         resource = Resource()
         resource["id"] = "NOTEXIST"
         with pytest.raises(HDXError):
@@ -837,18 +827,18 @@
         with pytest.raises(HDXError):
             resource.update_in_hdx()
 
         resource.data = {}
         with pytest.raises(HDXError):
             resource.update_in_hdx()
 
-        resource_data = copy.deepcopy(TestResource.resource_data)
-        resource_data["name"] = "MyResource1"
-        resource_data["id"] = "74b74ae1-df0c-4716-829f-4f939a046811"
-        resource = Resource(resource_data)
+        resource_data_copy = copy.deepcopy(resource_data)
+        resource_data_copy["name"] = "MyResource1"
+        resource_data_copy["id"] = "74b74ae1-df0c-4716-829f-4f939a046811"
+        resource = Resource(resource_data_copy)
         resource.mark_data_updated()
         assert resource.data_updated is True
         assert resource.is_marked_data_updated() is True
         resource.create_in_hdx()
         assert resource.is_marked_data_updated() is False
         assert resource["id"] == "74b74ae1-df0c-4716-829f-4f939a046811"
         assert resource.get_format() == "xlsx"
@@ -868,25 +858,25 @@
         )
         resource.delete_from_hdx()
         del resource["id"]
         with pytest.raises(HDXError):
             resource.delete_from_hdx()
 
     def test_update_yaml(self, configuration, static_yaml):
-        resource_data = copy.deepcopy(TestResource.resource_data)
-        resource = Resource(resource_data)
+        resource_data_copy = copy.deepcopy(resource_data)
+        resource = Resource(resource_data_copy)
         assert resource["name"] == "MyResource1"
         assert resource.get_format() == "xlsx"
         resource.update_from_yaml(static_yaml)
         assert resource["name"] == "MyResource1"
         assert resource.get_format() == "csv"
 
     def test_update_json(self, configuration, static_json):
-        resource_data = copy.deepcopy(TestResource.resource_data)
-        resource = Resource(resource_data)
+        resource_data_copy = copy.deepcopy(resource_data)
+        resource = Resource(resource_data_copy)
         assert resource["name"] == "MyResource1"
         assert resource.get_format() == "xlsx"
         resource.update_from_json(static_json)
         assert resource["name"] == "MyResource1"
         assert resource.get_format() == "zipped csv"
 
     def test_patch(self, configuration, post_patch):
@@ -894,16 +884,16 @@
         resource["id"] = "74b74ae1-df0c-4716-829f-4f939a046811"
         resource.update_in_hdx(
             operation="patch", batch_mode="KEEP_OLD", skip_validation=True
         )
         assert resource["id"] == "de6549d8-268b-4dfe-adaf-a4ae5c8510d5"
 
     def test_get_dataset(self, configuration, post_dataset):
-        resource_data = copy.deepcopy(TestResource.resource_data)
-        resource = Resource(resource_data)
+        resource_data_copy = copy.deepcopy(resource_data)
+        resource = Resource(resource_data_copy)
         dataset = resource.get_dataset()
         assert dataset["id"] == "6f36a41c-f126-4b18-aaaf-6c2ddfbc5d4d"
         del resource["package_id"]
         with pytest.raises(HDXError):
             resource.get_dataset()
 
     def test_search_in_hdx(self, configuration, search):
```

### Comparing `hdx_python_api-6.2.7/tests/hdx/data/test_resource_view.py` & `hdx_python_api-6.2.8/tests/hdx/data/test_resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/data/test_showcase.py` & `hdx_python_api-6.2.8/tests/hdx/data/test_showcase.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/data/test_update_dataset_resources.py` & `hdx_python_api-6.2.8/tests/hdx/data/test_update_dataset_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,18 @@
             ("Other Policy Relevant Indicators indicator list", "csv"),
             ("Other Policy Relevant Indicators metadata", "csv"),
             ("Demographic and Socio-economic data", "csv"),
             ("Demographic and Socio-economic indicator list", "csv"),
             ("QuickCharts-SDG 4 Global and Thematic data", "csv"),
         ]
         dataset._prepare_hdx_call(dataset.old_data, {})
+        assert (
+            dataset["updated_by_script"]
+            == "HDX Scraper: UNESCO (2022-12-19T12:51:30.579185)"
+        )
         results = dataset._revise_dataset(
             tuple(),
             resources_to_update,
             resources_to_delete,
             filestore_resources,
             new_resource_order,
             hxl_update=False,
```

### Comparing `hdx_python_api-6.2.7/tests/hdx/data/test_update_logic.py` & `hdx_python_api-6.2.8/tests/hdx/data/test_update_logic.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/data/test_user.py` & `hdx_python_api-6.2.8/tests/hdx/data/test_user.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/data/test_vocabulary.py` & `hdx_python_api-6.2.8/tests/hdx/data/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/facades/__init__.py` & `hdx_python_api-6.2.8/tests/hdx/facades/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/facades/test_infer_arguments.py` & `hdx_python_api-6.2.8/tests/hdx/facades/test_infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/facades/test_keyword_arguments.py` & `hdx_python_api-6.2.8/tests/hdx/facades/test_keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/tests/hdx/facades/test_simple.py` & `hdx_python_api-6.2.8/tests/hdx/facades/test_simple.py`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/workingexample/my_resource.xlsx` & `hdx_python_api-6.2.8/workingexample/my_resource.xlsx`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/.gitignore` & `hdx_python_api-6.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/LICENSE` & `hdx_python_api-6.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/README.md` & `hdx_python_api-6.2.8/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_api-6.2.7/pyproject.toml` & `hdx_python_api-6.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 requires-python = ">=3.8"
 
 dependencies = [
     "ckanapi>=4.8",
     "defopt>=6.4.0",
     "email_validator",
     "hdx-python-country>=3.7.0",
-    "hdx-python-utilities>=3.6.7",
+    "hdx-python-utilities>=3.6.8",
     "libhxl>=5.2.1",
     "makefun",
     "ndg-httpsclient",
     "pyasn1",
     "pyOpenSSL",
     "quantulum3",
     "requests",
```

### Comparing `hdx_python_api-6.2.7/PKG-INFO` & `hdx_python_api-6.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hdx-python-api
-Version: 6.2.7
+Version: 6.2.8
 Summary: HDX Python API for interacting with the Humanitarian Data Exchange
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-api
 Author: Michael Rans
 License: MIT
 License-File: LICENSE
 Keywords: API,CKAN,HDX,humanitarian data exchange
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,15 +25,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: ckanapi>=4.8
 Requires-Dist: defopt>=6.4.0
 Requires-Dist: email-validator
 Requires-Dist: hdx-python-country>=3.7.0
-Requires-Dist: hdx-python-utilities>=3.6.7
+Requires-Dist: hdx-python-utilities>=3.6.8
 Requires-Dist: libhxl>=5.2.1
 Requires-Dist: makefun
 Requires-Dist: ndg-httpsclient
 Requires-Dist: pyasn1
 Requires-Dist: pyopenssl
 Requires-Dist: quantulum3
 Requires-Dist: requests
```

