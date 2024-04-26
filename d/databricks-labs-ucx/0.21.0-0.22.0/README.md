# Comparing `tmp/databricks_labs_ucx-0.21.0.tar.gz` & `tmp/databricks_labs_ucx-0.22.0.tar.gz`

## Comparing `databricks_labs_ucx-0.21.0.tar` & `databricks_labs_ucx-0.22.0.tar`

### file list

```diff
@@ -1,137 +1,158 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/__about__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/__init__.py
--rw-r--r--   0        0        0    11567 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/account.py
--rw-r--r--   0        0        0    24439 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/cli.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/config.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/configure.py
--rw-r--r--   0        0        0    24343 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/install.py
--rw-r--r--   0        0        0    25482 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/runtime.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/__init__.py
--rw-r--r--   0        0        0    14956 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/aws.py
--rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/azure.py
--rw-r--r--   0        0        0     9361 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/clusters.py
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/crawlers.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/init_scripts.py
--rw-r--r--   0        0        0    14915 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/jobs.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/pipelines.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/secrets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/aws/__init__.py
--rw-r--r--   0        0        0    16422 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/aws/access.py
--rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/aws/credentials.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/azure/__init__.py
--rw-r--r--   0        0        0    11252 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/azure/access.py
--rw-r--r--   0        0        0    12609 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/azure/credentials.py
--rw-r--r--   0        0        0    10070 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/azure/locations.py
--rw-r--r--   0        0        0    15280 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/azure/resources.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/framework/__init__.py
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/framework/crawlers.py
--rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/framework/dashboards.py
--rw-r--r--   0        0        0     9855 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/framework/tasks.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/framework/utils.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/__init__.py
--rw-r--r--   0        0        0     5576 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/catalog_schema.py
--rw-r--r--   0        0        0    13904 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/grants.py
--rw-r--r--   0        0        0    16730 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/locations.py
--rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/mapping.py
--rw-r--r--   0        0        0    16840 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/table_migrate.py
--rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/table_move.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/table_size.py
--rw-r--r--   0        0        0    10831 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/tables.py
--rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/tables.scala
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/udfs.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/verification.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/views_sequencer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/installer/__init__.py
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/installer/hms_lineage.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/installer/mixins.py
--rw-r--r--   0        0        0    10332 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/installer/policy.py
--rw-r--r--   0        0        0    23577 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/installer/workflows.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/mixins/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/mixins/__init__.py
--rw-r--r--   0        0        0    42992 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/mixins/fixtures.py
--rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/mixins/redash.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/azure/05_0_azure_service_principals.sql
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/00_2_is_metastore_assigned.sql
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/00_4_is_incompatible_submit_run_detected.sql
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/01_2_group_migration.sql
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/01_5_group_migration_complexity.sql
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/02_2_uc_data_modeling.sql
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/02_5_uc_data_modeling_complexity.sql
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/03_2_data_migration_summary.sql
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/00_0_compatibility.sql
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/00_1_count_total_databases.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/00_2_count_table_failures.sql
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/00_3_count_total_tables.sql
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/00_4_count_external_locations.sql
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/00_5_count_total_views.sql
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/00___assessment_overview.md
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/01_0_count_jobs.sql
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/05_0_object_readiness.sql
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/05_2_assessment_summary.sql
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/05___findings_summary.md
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/10___data_summary.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/15_0_external_locations.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/15_3_mount_points.sql
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/15___storage_summary.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/20_0_cluster_policies.sql
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/20_0_clusters.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/20___compute_summary.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/30_0_job_summary.md
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/30_3_job_details.sql
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/30_3_jobs.sql
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/30_4_submit_runs.sql
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/30_5_submit_runs.sql
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/40_0_pipelines.sql
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/40_3_global_init_scripts.sql
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/40___last_summary.md
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/README.md
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/views/code_patterns.sql
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/views/grant_detail.sql
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/views/misc_patterns.sql
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/views/objects.sql
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/views/table_estimates.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/source_code/__init__.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/source_code/base.py
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/source_code/files.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/source_code/languages.py
--rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/source_code/lsp.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/source_code/notebooks.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/source_code/pyspark.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/source_code/queries.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/source_code/redash.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/upgrades/v0.4.0_added_log_dir.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/__init__.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/base.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/clusters.py
--rw-r--r--   0        0        0    17983 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/generic.py
--rw-r--r--   0        0        0    34284 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/groups.py
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/listing.py
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/manager.py
--rw-r--r--   0        0        0    11805 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/redash.py
--rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/scim.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/secrets.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/tacl.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/LICENSE
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/NOTICE
--rw-r--r--   0        0        0    50404 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/README.md
--rw-r--r--   0        0        0    28378 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/pyproject.toml
--rw-r--r--   0        0        0    52043 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.21.0/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/__about__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/__init__.py
+-rw-r--r--   0        0        0    15778 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/account.py
+-rw-r--r--   0        0        0    17561 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/cli.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/config.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/configure.py
+-rw-r--r--   0        0        0    30383 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/install.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/runtime.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/__init__.py
+-rw-r--r--   0        0        0    15955 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/aws.py
+-rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/azure.py
+-rw-r--r--   0        0        0     9366 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/clusters.py
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/crawlers.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/init_scripts.py
+-rw-r--r--   0        0        0    14899 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/jobs.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/pipelines.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/secrets.py
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/workflows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/aws/__init__.py
+-rw-r--r--   0        0        0    15761 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/aws/access.py
+-rw-r--r--   0        0        0     7240 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/aws/credentials.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/__init__.py
+-rw-r--r--   0        0        0    12115 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/access.py
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/credentials.py
+-rw-r--r--   0        0        0     9045 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/locations.py
+-rw-r--r--   0        0        0    23838 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/resources.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/contexts/__init__.py
+-rw-r--r--   0        0        0    12357 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/contexts/application.py
+-rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/contexts/cli_command.py
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/contexts/workflow_task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/__init__.py
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/crawlers.py
+-rw-r--r--   0        0        0    15609 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/dashboards.py
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/tasks.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/utils.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/__init__.py
+-rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/catalog_schema.py
+-rw-r--r--   0        0        0    27049 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/grants.py
+-rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/locations.py
+-rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/mapping.py
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/migration_status.py
+-rw-r--r--   0        0        0    21146 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/table_migrate.py
+-rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/table_move.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/table_size.py
+-rw-r--r--   0        0        0    17578 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/tables.py
+-rw-r--r--   0        0        0     5796 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/tables.scala
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/udfs.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/verification.py
+-rw-r--r--   0        0        0     7347 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/view_migrate.py
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/workflows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/__init__.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/hms_lineage.py
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/logs.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/mixins.py
+-rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/policy.py
+-rw-r--r--   0        0        0    31795 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/workflows.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/__init__.py
+-rw-r--r--   0        0        0    45618 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/fixtures.py
+-rw-r--r--   0        0        0     6596 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/redash.py
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/wspath.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/azure/05_0_azure_service_principals.sql
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/00_2_is_metastore_assigned.sql
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/00_4_is_incompatible_submit_run_detected.sql
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/01_2_group_migration.sql
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/01_5_group_migration_complexity.sql
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/02_2_uc_data_modeling.sql
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/02_5_uc_data_modeling_complexity.sql
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/03_2_data_migration_summary.sql
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00_0_compatibility.sql
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00_1_count_total_databases.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00_2_count_table_failures.sql
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00_3_count_total_tables.sql
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00_4_count_external_locations.sql
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00_5_count_total_views.sql
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/00___assessment_overview.md
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/01_0_count_jobs.sql
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/05_0_object_readiness.sql
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/05_2_assessment_summary.sql
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/05___findings_summary.md
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/10___data_summary.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/15_0_external_locations.sql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/15_3_mount_points.sql
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/15___storage_summary.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/20_0_cluster_policies.sql
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/20_0_clusters.sql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/20___compute_summary.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/30_0_job_summary.md
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/30_3_job_details.sql
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/30_3_jobs.sql
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/30_4_submit_runs.sql
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/30_5_submit_runs.sql
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/40_0_pipelines.sql
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/40_2_logs.sql
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/40_3_global_init_scripts.sql
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/40___last_summary.md
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/README.md
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/code_patterns.sql
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/grant_detail.sql
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/misc_patterns.sql
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/objects.sql
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/table_estimates.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/__init__.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/base.py
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/dbfs.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/dependencies.py
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/dependency_loaders.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/dependency_resolvers.py
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/files.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/languages.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/lsp.py
+-rw-r--r--   0        0        0    14297 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/notebook.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/notebook_linter.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/notebook_migrator.py
+-rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/pyspark.py
+-rw-r--r--   0        0        0     9613 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/python_linter.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/queries.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/redash.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/site_packages.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/table_creation.py
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/whitelist.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.4.0_added_log_dir.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/__init__.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/base.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/clusters.py
+-rw-r--r--   0        0        0    18659 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/generic.py
+-rw-r--r--   0        0        0    34574 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/groups.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/listing.py
+-rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/manager.py
+-rw-r--r--   0        0        0    12376 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/redash.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/scim.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/secrets.py
+-rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/tacl.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/workflows.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/LICENSE
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/NOTICE
+-rw-r--r--   0        0        0    60336 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/README.md
+-rw-r--r--   0        0        0    28386 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/pyproject.toml
+-rw-r--r--   0        0        0    62011 2020-02-02 00:00:00.000000 databricks_labs_ucx-0.22.0/PKG-INFO
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/account.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/account.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import logging
 from typing import ClassVar
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.tui import Prompts
 from databricks.sdk import AccountClient, WorkspaceClient
-from databricks.sdk.errors import NotFound, ResourceConflict
+from databricks.sdk.errors import NotFound, ResourceConflict, PermissionDenied
 from databricks.sdk.service.iam import ComplexValue, Group, Patch, PatchOp, PatchSchema
 from databricks.sdk.service.provisioning import Workspace
+from databricks.sdk.service.settings import DefaultNamespaceSetting, StringMessage
 
 logger = logging.getLogger(__name__)
 
 
 class AccountWorkspaces:
     _tlds: ClassVar[dict[str, str]] = {
         "aws": "cloud.databricks.com",
         "azure": "azuredatabricks.net",
         "gcp": "gcp.databricks.com",
     }
 
     SYNC_FILE_NAME: ClassVar[str] = "workspaces.json"
 
     def __init__(self, account_client: AccountClient, new_workspace_client=WorkspaceClient):
+        # TODO: new_workspace_client is a design flaw, remove it
         self._new_workspace_client = new_workspace_client
         self._ac = account_client
 
     def _workspaces(self):
         return self._ac.workspaces.list()
 
     def _get_cloud(self) -> str:
@@ -33,37 +35,43 @@
         if self._ac.config.is_gcp:
             return "gcp"
         return "aws"
 
     def client_for(self, workspace: Workspace) -> WorkspaceClient:
         return self._ac.get_workspace_client(workspace)
 
-    def workspace_clients(self) -> list[WorkspaceClient]:
+    def workspace_clients(self, workspaces: list[Workspace] | None) -> list[WorkspaceClient]:
         """
         Return a list of WorkspaceClient for each configured workspace in the account
         :return: list[WorkspaceClient]
         """
+        if workspaces is None:
+            workspaces = self._workspaces()
         clients = []
-        for workspace in self._workspaces():
+        for workspace in workspaces:
             ws = self.client_for(workspace)
             clients.append(ws)
         return clients
 
-    def sync_workspace_info(self):
+    def sync_workspace_info(self, workspaces: list[Workspace] | None = None):
         """
         Create a json dump for each Workspace in account
         For each user that has ucx installed in their workspace,
         upload the json dump of workspace info in the .ucx folder
         """
-        workspaces = []
-        for workspace in self._workspaces():
-            workspaces.append(workspace)
-        for ws in self.workspace_clients():
-            for installation in Installation.existing(ws, "ucx"):
-                installation.save(workspaces, filename=self.SYNC_FILE_NAME)
+        if workspaces is None:
+            workspaces = []
+            for workspace in self._workspaces():
+                workspaces.append(workspace)
+        for ws in self.workspace_clients(workspaces):
+            try:
+                for installation in Installation.existing(ws, "ucx"):
+                    installation.save(workspaces, filename=self.SYNC_FILE_NAME)
+            except (PermissionDenied, NotFound, ValueError):
+                logger.warning(f"Failed to save workspace info for {ws.config.host}")
 
     def create_account_level_groups(self, prompts: Prompts, workspace_ids: list[int] | None = None):
         acc_groups = self._get_account_groups()
         workspace_ids = self._get_valid_workspaces_ids(workspace_ids)
         all_valid_workspace_groups = self._get_valid_workspaces_groups(prompts, workspace_ids)
 
         for group_name, valid_group in all_valid_workspace_groups.items():
@@ -247,7 +255,91 @@
             answer = prompts.question("Next workspace id", valid_number=True, default="stop")
             if answer == "stop":
                 break
             workspace_id = int(answer)
         for installation in Installation.existing(self._ws, 'ucx'):
             installation.save(workspaces, filename=AccountWorkspaces.SYNC_FILE_NAME)
         logger.info("Synchronised workspace id mapping for installations on current workspace")
+
+
+class AccountMetastores:
+    def __init__(
+        self,
+        account_client: AccountClient,
+    ):
+        self._ac = account_client
+
+    def show_all_metastores(self, workspace_id: str | None = None):
+        location = None
+        if workspace_id:
+            logger.info(f"Workspace ID: {workspace_id}")
+            location = self._get_region(int(workspace_id))
+        logger.info("Matching metastores are:")
+        for metastore in self._get_all_metastores(location).keys():
+            logger.info(metastore)
+
+    def assign_metastore(
+        self,
+        prompts: Prompts,
+        str_workspace_id: str | None = None,
+        metastore_id: str | None = None,
+        default_catalog: str | None = None,
+    ):
+        if not str_workspace_id:
+            workspace_choices = self._get_all_workspaces()
+            workspace_id = prompts.choice_from_dict("Please select a workspace:", workspace_choices)
+        else:
+            workspace_id = int(str_workspace_id)
+        if not metastore_id:
+            # search for all matching metastores
+            metastore_choices = self._get_all_metastores(self._get_region(workspace_id))
+            if len(metastore_choices) == 0:
+                raise ValueError(f"No matching metastore found for workspace {workspace_id}")
+            # if there are multiple matches, prompt users to select one
+            if len(metastore_choices) > 1:
+                metastore_id = prompts.choice_from_dict(
+                    "Multiple metastores found, please select one:", metastore_choices
+                )
+            else:
+                metastore_id = list(metastore_choices.values())[0]
+        if metastore_id is not None:
+            self._ac.metastore_assignments.create(workspace_id, metastore_id)
+        # set the default catalog using the default_namespace setting API
+        if default_catalog is not None:
+            self._set_default_catalog(workspace_id, default_catalog)
+
+    def _get_region(self, workspace_id: int) -> str:
+        workspace = self._ac.workspaces.get(workspace_id)
+        if self._ac.config.is_aws:
+            return str(workspace.aws_region)
+        return str(workspace.location)
+
+    def _get_all_workspaces(self) -> dict[str, int]:
+        output = dict[str, int]()
+        for workspace in self._ac.workspaces.list():
+            if workspace.workspace_id:
+                output[f"{workspace.workspace_name} - {workspace.workspace_id}"] = workspace.workspace_id
+        return dict(sorted(output.items()))
+
+    def _get_all_metastores(self, location: str | None = None) -> dict[str, str]:
+        output = dict[str, str]()
+        for metastore in self._ac.metastores.list():
+            if location is None or metastore.region == location:
+                output[f"{metastore.name} - {metastore.metastore_id}"] = str(metastore.metastore_id)
+        return dict(sorted(output.items()))
+
+    def _set_default_catalog(self, workspace_id: int, default_catalog: str):
+        if default_catalog == "":
+            return
+        workspace = self._ac.workspaces.get(int(workspace_id))
+        default_namespace = self._ac.get_workspace_client(workspace).settings.default_namespace
+        # needs to get the etag first, before patching the setting
+        try:
+            etag = default_namespace.get().etag
+        except NotFound as err:
+            # if not found, the etag is returned in the header
+            etag = err.details[0].metadata.get("etag")
+        default_namespace.update(
+            allow_missing=True,
+            field_mask="namespace.value",
+            setting=DefaultNamespaceSetting(etag=etag, namespace=StringMessage(default_catalog)),
+        )
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/cli.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,54 @@
 import json
-import os
-import shutil
 import webbrowser
-from collections.abc import Callable
 from pathlib import Path
 
 from databricks.labs.blueprint.cli import App
 from databricks.labs.blueprint.entrypoint import get_logger
 from databricks.labs.blueprint.installation import Installation, SerdeError
 from databricks.labs.blueprint.tui import Prompts
-from databricks.labs.lsql.backends import StatementExecutionBackend
 from databricks.sdk import AccountClient, WorkspaceClient
 from databricks.sdk.errors import NotFound
 
-from databricks.labs.ucx.account import AccountWorkspaces, WorkspaceInfo
-from databricks.labs.ucx.assessment.aws import AWSResources
-from databricks.labs.ucx.aws.access import AWSResourcePermissions
-from databricks.labs.ucx.aws.credentials import IamRoleMigration
-from databricks.labs.ucx.azure.access import AzureResourcePermissions
-from databricks.labs.ucx.azure.credentials import ServicePrincipalMigration
-from databricks.labs.ucx.azure.locations import ExternalLocationsMigration
+from databricks.labs.ucx.account import AccountWorkspaces
 from databricks.labs.ucx.config import WorkspaceConfig
-from databricks.labs.ucx.hive_metastore import ExternalLocations, TablesCrawler
-from databricks.labs.ucx.hive_metastore.catalog_schema import CatalogSchema
-from databricks.labs.ucx.hive_metastore.mapping import TableMapping
-from databricks.labs.ucx.hive_metastore.table_migrate import TablesMigrator
-from databricks.labs.ucx.hive_metastore.table_move import TableMove
-from databricks.labs.ucx.install import WorkspaceInstallation
-from databricks.labs.ucx.installer.workflows import WorkflowsInstallation
-from databricks.labs.ucx.source_code.files import Files
-from databricks.labs.ucx.workspace_access.clusters import ClusterAccess
-from databricks.labs.ucx.workspace_access.groups import GroupManager
+from databricks.labs.ucx.contexts.cli_command import AccountContext, WorkspaceContext
+from databricks.labs.ucx.hive_metastore.tables import What
 
 ucx = App(__file__)
 logger = get_logger(__file__)
 
 CANT_FIND_UCX_MSG = (
     "Couldn't find UCX configuration in the user's home folder. "
     "Make sure the current user has configured and installed UCX."
 )
 
 
 @ucx.command
 def workflows(w: WorkspaceClient):
     """Show deployed workflows and their state"""
-    installation = WorkflowsInstallation.current(w)
+    ctx = WorkspaceContext(w)
     logger.info("Fetching deployed jobs...")
-    print(json.dumps(installation.latest_job_status()))
+    latest_job_status = ctx.deployed_workflows.latest_job_status()
+    print(json.dumps(latest_job_status))
+
+
+@ucx.command
+def logs(w: WorkspaceClient, workflow: str | None = None):
+    """Show logs of the latest job run"""
+    ctx = WorkspaceContext(w)
+    ctx.deployed_workflows.relay_logs(workflow)
 
 
 @ucx.command
 def open_remote_config(w: WorkspaceClient):
     """Opens remote configuration in the browser"""
-    installation = WorkspaceInstallation.current(w)
-    webbrowser.open(installation.config_file_link())
+    ctx = WorkspaceContext(w)
+    workspace_link = ctx.installation.workspace_link('config.yml')
+    webbrowser.open(workspace_link)
 
 
 @ucx.command
 def installations(w: WorkspaceClient):
     """Show installations by different users on the same workspace"""
     logger.info("Fetching installations...")
     all_users = []
@@ -80,28 +71,27 @@
 
 @ucx.command
 def skip(w: WorkspaceClient, schema: str | None = None, table: str | None = None):
     """Create a skip comment on a schema or a table"""
     logger.info("Running skip command")
     if not schema:
         logger.error("--schema is a required parameter.")
-        return
-    mapping = TableMapping.current(w)
+        return None
+    ctx = WorkspaceContext(w)
     if table:
-        mapping.skip_table(schema, table)
-    else:
-        mapping.skip_schema(schema)
+        return ctx.table_mapping.skip_table(schema, table)
+    return ctx.table_mapping.skip_schema(schema)
 
 
 @ucx.command(is_account=True)
 def sync_workspace_info(a: AccountClient):
     """upload workspace config to all workspaces in the account where ucx is installed"""
     logger.info(f"Account ID: {a.config.account_id}")
-    workspaces = AccountWorkspaces(a)
-    workspaces.sync_workspace_info()
+    ctx = AccountContext(a)
+    ctx.account_workspaces.sync_workspace_info()
 
 
 @ucx.command(is_account=True)
 def create_account_groups(
     a: AccountClient, prompts: Prompts, workspace_ids: str | None = None, new_workspace_client=WorkspaceClient
 ):
     """
@@ -124,95 +114,82 @@
     workspaces = AccountWorkspaces(a, new_workspace_client)
     workspaces.create_account_level_groups(prompts, workspace_id_list)
 
 
 @ucx.command
 def manual_workspace_info(w: WorkspaceClient, prompts: Prompts):
     """only supposed to be run if cannot get admins to run `databricks labs ucx sync-workspace-info`"""
-    installation = Installation.current(w, 'ucx')
-    workspace_info = WorkspaceInfo(installation, w)
-    workspace_info.manual_workspace_info(prompts)
+    ctx = WorkspaceContext(w)
+    ctx.workspace_info.manual_workspace_info(prompts)
 
 
 @ucx.command
 def create_table_mapping(w: WorkspaceClient):
     """create initial table mapping for review"""
-    table_mapping = TableMapping.current(w)
-    installation = Installation.current(w, 'ucx')
-    workspace_info = WorkspaceInfo(installation, w)
-    config = installation.load(WorkspaceConfig)
-    sql_backend = StatementExecutionBackend(w, config.warehouse_id)
-    tables_crawler = TablesCrawler(sql_backend, config.inventory_database)
-    path = table_mapping.save(tables_crawler, workspace_info)
+    ctx = WorkspaceContext(w)
+    path = ctx.table_mapping.save(ctx.tables_crawler, ctx.workspace_info)
     webbrowser.open(f"{w.config.host}/#workspace{path}")
 
 
 @ucx.command
 def validate_external_locations(w: WorkspaceClient, prompts: Prompts):
     """validates and provides mapping to external table to external location and shared generation tf scripts"""
-    installation = Installation.current(w, 'ucx')
-    config = installation.load(WorkspaceConfig)
-    sql_backend = StatementExecutionBackend(w, config.warehouse_id)
-    location_crawler = ExternalLocations(w, sql_backend, config.inventory_database)
-    path = location_crawler.save_as_terraform_definitions_on_workspace(installation)
+    ctx = WorkspaceContext(w)
+    path = ctx.external_locations.save_as_terraform_definitions_on_workspace(ctx.installation)
     if path and prompts.confirm(f"external_locations.tf file written to {path}. Do you want to open it?"):
         webbrowser.open(f"{w.config.host}/#workspace{path}")
 
 
 @ucx.command
 def ensure_assessment_run(w: WorkspaceClient):
     """ensure the assessment job was run on a workspace"""
-    installation = WorkspaceInstallation.current(w)
-    installation.validate_and_run("assessment")
+    ctx = WorkspaceContext(w)
+    deployed_workflows = ctx.deployed_workflows
+    if not deployed_workflows.validate_step("assessment"):
+        deployed_workflows.run_workflow("assessment")
 
 
 @ucx.command
 def repair_run(w: WorkspaceClient, step):
     """Repair Run the Failed Job"""
     if not step:
         raise KeyError("You did not specify --step")
-    installation = WorkflowsInstallation.current(w)
+    ctx = WorkspaceContext(w)
     logger.info(f"Repair Running {step} Job")
-    installation.repair_run(step)
+    ctx.deployed_workflows.repair_run(step)
 
 
 @ucx.command
 def validate_groups_membership(w: WorkspaceClient):
     """Validate the groups to see if the groups at account level and workspace level has different membership"""
-    installation = Installation.current(w, 'ucx')
-    config = installation.load(WorkspaceConfig)
-    sql_backend = StatementExecutionBackend(w, config.warehouse_id)
-    logger.info("Validating Groups which are having different memberships between account and workspace")
-    group_manager = GroupManager(
-        sql_backend=sql_backend,
-        ws=w,
-        inventory_database=config.inventory_database,
-        include_group_names=config.include_group_names,
-        renamed_group_prefix=config.renamed_group_prefix,
-        workspace_group_regex=config.workspace_group_regex,
-        workspace_group_replace=config.workspace_group_replace,
-        account_group_regex=config.account_group_regex,
-    )
-    mismatch_groups = group_manager.validate_group_membership()
+    ctx = WorkspaceContext(w)
+    mismatch_groups = ctx.group_manager.validate_group_membership()
     print(json.dumps(mismatch_groups))
 
 
 @ucx.command
 def revert_migrated_tables(
-    w: WorkspaceClient, prompts: Prompts, schema: str, table: str, *, delete_managed: bool = False
+    w: WorkspaceClient,
+    prompts: Prompts,
+    schema: str,
+    table: str,
+    *,
+    delete_managed: bool = False,
+    ctx: WorkspaceContext | None = None,
 ):
     """remove notation on a migrated table for re-migration"""
     if not schema and not table:
         question = "You haven't specified a schema or a table. All migrated tables will be reverted. Continue?"
         if not prompts.confirm(question, max_attempts=2):
             return
-    tables_migrate = TablesMigrator.for_cli(w)
-    revert = tables_migrate.print_revert_report(delete_managed=delete_managed)
+    if not ctx:
+        ctx = WorkspaceContext(w)
+    revert = ctx.tables_migrator.print_revert_report(delete_managed=delete_managed)
     if revert and prompts.confirm("Would you like to continue?", max_attempts=2):
-        tables_migrate.revert_migrated_tables(schema, table, delete_managed=delete_managed)
+        ctx.tables_migrator.revert_migrated_tables(schema, table, delete_managed=delete_managed)
 
 
 @ucx.command
 def move(
     w: WorkspaceClient,
     prompts: Prompts,
     from_catalog: str,
@@ -228,22 +205,22 @@
         return
     if from_schema == "" or to_schema == "" or from_table == "":
         logger.error("Please enter from_schema, to_schema and from_table (enter * for migrating all tables) details.")
         return
     if from_catalog == to_catalog and from_schema == to_schema:
         logger.error("please select a different schema or catalog to migrate to")
         return
-    tables = TableMove.for_cli(w)
     if not prompts.confirm(f"[WARNING] External tables will be dropped and recreated in the target schema {to_schema}"):
         return
     del_table = prompts.confirm(
         f"should we delete managed tables & views after moving to the new schema" f" {to_catalog}.{to_schema}"
     )
     logger.info(f"migrating tables {from_table} from {from_catalog}.{from_schema} to {to_catalog}.{to_schema}")
-    tables.move(from_catalog, from_schema, from_table, to_catalog, to_schema, del_table=del_table)
+    ctx = WorkspaceContext(w)
+    ctx.table_move.move(from_catalog, from_schema, from_table, to_catalog, to_schema, del_table=del_table)
 
 
 @ucx.command
 def alias(
     w: WorkspaceClient,
     from_catalog: str,
     from_schema: str,
@@ -257,312 +234,192 @@
         return
     if from_schema == "" or to_schema == "" or from_table == "":
         logger.error("Please enter from_schema, to_schema and from_table (enter * for migrating all tables) details.")
         return
     if from_catalog == to_catalog and from_schema == to_schema:
         logger.error("please select a different schema or catalog to migrate to")
         return
-    tables = TableMove.for_cli(w)
     logger.info(f"aliasing table {from_table} from {from_catalog}.{from_schema} to {to_catalog}.{to_schema}")
-    tables.alias_tables(from_catalog, from_schema, from_table, to_catalog, to_schema)
-
-
-def _execute_for_cloud(
-    w: WorkspaceClient,
-    prompts: Prompts,
-    func_azure: Callable,
-    func_aws: Callable,
-    azure_resource_permissions: AzureResourcePermissions | None = None,
-    subscription_id: str | None = None,
-    aws_permissions: AWSResourcePermissions | None = None,
-    aws_profile: str | None = None,
-):
-    if w.config.is_azure:
-        if w.config.auth_type != "azure-cli":
-            logger.error("In order to obtain AAD token, Please run azure cli to authenticate.")
-            return None
-        if not subscription_id:
-            logger.error("Please enter subscription id to scan storage accounts in.")
-            return None
-        return func_azure(
-            w, prompts, subscription_id=subscription_id, azure_resource_permissions=azure_resource_permissions
-        )
-    if w.config.is_aws:
-        if not shutil.which("aws"):
-            logger.error("Couldn't find AWS CLI in path. Please install the CLI from https://aws.amazon.com/cli/")
-            return None
-        if not aws_profile:
-            aws_profile = os.getenv("AWS_DEFAULT_PROFILE")
-        if not aws_profile:
-            logger.error(
-                "AWS Profile is not specified. Use the environment variable [AWS_DEFAULT_PROFILE] "
-                "or use the '--aws-profile=[profile-name]' parameter."
-            )
-            return None
-        return func_aws(w, prompts, aws_profile=aws_profile, aws_permissions=aws_permissions)
-    logger.error("This cmd is only supported for azure and aws workspaces")
-    return None
+    ctx = WorkspaceContext(w)
+    ctx.table_move.alias_tables(from_catalog, from_schema, from_table, to_catalog, to_schema)
 
 
 @ucx.command
 def create_uber_principal(
     w: WorkspaceClient,
     prompts: Prompts,
-    subscription_id: str | None = None,
-    azure_resource_permissions: AzureResourcePermissions | None = None,
-    aws_profile: str | None = None,
-    aws_resource_permissions: AWSResourcePermissions | None = None,
+    ctx: WorkspaceContext | None = None,
+    **named_parameters,
 ):
     """For azure cloud, creates a service principal and gives STORAGE BLOB READER access on all the storage account
     used by tables in the workspace and stores the spn info in the UCX cluster policy. For aws,
     it identifies all s3 buckets used by the Instance Profiles configured in the workspace.
     Pass subscription_id for azure and aws_profile for aws."""
-    return _execute_for_cloud(
-        w,
-        prompts,
-        _azure_setup_uber_principal,
-        _aws_setup_uber_principal,
-        azure_resource_permissions,
-        subscription_id,
-        aws_resource_permissions,
-        aws_profile,
-    )
-
-
-def _azure_setup_uber_principal(
-    w: WorkspaceClient,
-    prompts: Prompts,
-    subscription_id: str,
-    azure_resource_permissions: AzureResourcePermissions | None = None,
-):
-    include_subscriptions = [subscription_id] if subscription_id else None
-    if azure_resource_permissions is None:
-        azure_resource_permissions = AzureResourcePermissions.for_cli(w, include_subscriptions=include_subscriptions)
-    azure_resource_permissions.create_uber_principal(prompts)
-
-
-def _aws_setup_uber_principal(
-    w: WorkspaceClient,
-    prompts: Prompts,
-    aws_profile: str,
-    aws_resource_permissions: AWSResourcePermissions | None = None,
-):
-    installation = Installation.current(w, 'ucx')
-    config = installation.load(WorkspaceConfig)
-    sql_backend = StatementExecutionBackend(w, config.warehouse_id)
-    aws = AWSResources(aws_profile)
-    if aws_resource_permissions is None:
-        aws_resource_permissions = AWSResourcePermissions.for_cli(
-            w, installation, sql_backend, aws, config.inventory_database
-        )
-    aws_resource_permissions.create_uber_principal(prompts)
+    if not ctx:
+        ctx = WorkspaceContext(w, named_parameters)
+    if ctx.is_azure:
+        return ctx.azure_resource_permissions.create_uber_principal(prompts)
+    if ctx.is_aws:
+        return ctx.aws_resource_permissions.create_uber_principal(prompts)
+    raise ValueError("Unsupported cloud provider")
 
 
 @ucx.command
-def principal_prefix_access(
-    w: WorkspaceClient,
-    prompts: Prompts,
-    subscription_id: str | None = None,
-    azure_resource_permissions: AzureResourcePermissions | None = None,
-    aws_profile: str | None = None,
-    aws_resource_permissions: AWSResourcePermissions | None = None,
-):
+def principal_prefix_access(w: WorkspaceClient, ctx: WorkspaceContext | None = None, **named_parameters):
     """For azure cloud, identifies all storage accounts used by tables in the workspace, identify spn and its
     permission on each storage accounts. For aws, identifies all the Instance Profiles configured in the workspace and
     its access to all the S3 buckets, along with AWS roles that are set with UC access and its access to S3 buckets.
     The output is stored in the workspace install folder.
     Pass subscription_id for azure and aws_profile for aws."""
-    return _execute_for_cloud(
-        w,
-        prompts,
-        _azure_principal_prefix_access,
-        _aws_principal_prefix_access,
-        azure_resource_permissions,
-        subscription_id,
-        aws_resource_permissions,
-        aws_profile,
-    )
-
-
-def _azure_principal_prefix_access(
-    w: WorkspaceClient,
-    _: Prompts,
-    *,
-    subscription_id: str,
-    azure_resource_permissions: AzureResourcePermissions | None = None,
-):
-    if w.config.auth_type != "azure-cli":
-        logger.error("In order to obtain AAD token, Please run azure cli to authenticate.")
-        return
-    include_subscriptions = [subscription_id] if subscription_id else None
-    if azure_resource_permissions is None:
-        azure_resource_permissions = AzureResourcePermissions.for_cli(w, include_subscriptions=include_subscriptions)
-    logger.info("Generating azure storage accounts and service principal permission info")
-    path = azure_resource_permissions.save_spn_permissions()
-    if path:
-        logger.info(f"storage and spn info saved under {path}")
-    return
-
-
-def _aws_principal_prefix_access(
-    w: WorkspaceClient,
-    _: Prompts,
-    *,
-    aws_profile: str,
-    aws_permissions: AWSResourcePermissions | None = None,
-):
-    if not shutil.which("aws"):
-        logger.error("Couldn't find AWS CLI in path. Please install the CLI from https://aws.amazon.com/cli/")
-        return
-    logger.info("Generating instance profile and bucket permission info")
-    installation = Installation.current(w, 'ucx')
-    config = installation.load(WorkspaceConfig)
-    sql_backend = StatementExecutionBackend(w, config.warehouse_id)
-    aws = AWSResources(aws_profile)
-    if aws_permissions is None:
-        aws_permissions = AWSResourcePermissions.for_cli(w, installation, sql_backend, aws, config.inventory_database)
-    instance_role_path = aws_permissions.save_instance_profile_permissions()
-    logger.info(f"Instance profile and bucket info saved {instance_role_path}")
-    logger.info("Generating UC roles and bucket permission info")
-    uc_role_path = aws_permissions.save_uc_compatible_roles()
-    logger.info(f"UC roles and bucket info saved {uc_role_path}")
+    if not ctx:
+        ctx = WorkspaceContext(w, named_parameters)
+    if ctx.is_azure:
+        return ctx.azure_resource_permissions.save_spn_permissions()
+    if ctx.is_aws:
+        instance_role_path = ctx.aws_resource_permissions.save_instance_profile_permissions()
+        logger.info(f"Instance profile and bucket info saved {instance_role_path}")
+        logger.info("Generating UC roles and bucket permission info")
+        return ctx.aws_resource_permissions.save_uc_compatible_roles()
+    raise ValueError("Unsupported cloud provider")
 
 
 @ucx.command
-def migrate_credentials(
-    w: WorkspaceClient, prompts: Prompts, aws_profile: str | None = None, aws_resources: AWSResources | None = None
-):
+def migrate_credentials(w: WorkspaceClient, prompts: Prompts, ctx: WorkspaceContext | None = None, **named_parameters):
     """For Azure, this command migrates Azure Service Principals, which have Storage Blob Data Contributor,
     Storage Blob Data Reader, Storage Blob Data Owner roles on ADLS Gen2 locations that are being used in
     Databricks, to UC storage credentials.
     The Azure Service Principals to location mapping are listed in
     {install_folder}/.ucx/azure_storage_account_info.csv which is generated by principal_prefix_access command.
     Please review the file and delete the Service Principals you do not want to be migrated.
     The command will only migrate the Service Principals that have client secret stored in Databricks Secret.
     For AWS, this command migrates AWS Instance Profiles that are being used in Databricks, to UC storage credentials.
     The AWS Instance Profiles to location mapping are listed in
     {install_folder}/.ucx/aws_instance_profile_info.csv which is generated by principal_prefix_access command.
     Please review the file and delete the Instance Profiles you do not want to be migrated.
     Pass aws_profile for aws.
     """
-    installation = Installation.current(w, 'ucx')
-    if w.config.is_azure:
-        logger.info("Running migrate_credentials for Azure")
-        service_principal_migration = ServicePrincipalMigration.for_cli(w, installation, prompts)
-        service_principal_migration.run(prompts)
-        return
-    if w.config.is_aws:
-        if not aws_profile:
-            aws_profile = os.getenv("AWS_DEFAULT_PROFILE")
-        if not aws_profile:
-            logger.error(
-                "AWS Profile is not specified. Use the environment variable [AWS_DEFAULT_PROFILE] "
-                "or use the '--aws-profile=[profile-name]' parameter."
-            )
-            return
-        logger.info("Running migrate_credentials for AWS")
-        if not aws_resources:
-            aws_resources = AWSResources(aws_profile)
-        instance_profile_migration = IamRoleMigration.for_cli(w, installation, aws_resources, prompts)
-        instance_profile_migration.run(prompts)
-        return
-    if w.config.is_gcp:
-        logger.error("migrate_credentials is not yet supported in GCP")
+    if not ctx:
+        ctx = WorkspaceContext(w, named_parameters)
+    if ctx.is_azure:
+        return ctx.service_principal_migration.run(prompts)
+    if ctx.is_aws:
+        return ctx.iam_role_migration.run(prompts)
+    raise ValueError("Unsupported cloud provider")
 
 
 @ucx.command
-def migrate_locations(w: WorkspaceClient, aws_profile: str | None = None):
+def migrate_locations(w: WorkspaceClient, ctx: WorkspaceContext | None = None, **named_parameters):
     """This command creates UC external locations. The candidate locations to be created are extracted from
     guess_external_locations task in the assessment job. You can run validate_external_locations command to check
     the candidate locations. Please make sure the credentials haven migrated before running this command. The command
     will only create the locations that have corresponded UC Storage Credentials.
     """
-    if w.config.is_azure:
-        logger.info("Running migrate_locations for Azure")
-        installation = Installation.current(w, 'ucx')
-        service_principal_migration = ExternalLocationsMigration.for_cli(w, installation)
-        service_principal_migration.run()
-    if w.config.is_aws:
-        logger.error("Migrate_locations for AWS")
-        if not shutil.which("aws"):
-            logger.error("Couldn't find AWS CLI in path. Please install the CLI from https://aws.amazon.com/cli/")
-            return
-        if not aws_profile:
-            aws_profile = os.getenv("AWS_DEFAULT_PROFILE")
-        if not aws_profile:
-            logger.error(
-                "AWS Profile is not specified. Use the environment variable [AWS_DEFAULT_PROFILE] "
-                "or use the '--aws-profile=[profile-name]' parameter."
-            )
-            return
-        installation = Installation.current(w, 'ucx')
-        config = installation.load(WorkspaceConfig)
-        sql_backend = StatementExecutionBackend(w, config.warehouse_id)
-        aws = AWSResources(aws_profile)
-        location = ExternalLocations(w, sql_backend, config.inventory_database)
-        aws_permissions = AWSResourcePermissions(installation, w, sql_backend, aws, location, config.inventory_database)
-        aws_permissions.create_external_locations()
-    if w.config.is_gcp:
-        logger.error("migrate_locations is not yet supported in GCP")
+    if not ctx:
+        ctx = WorkspaceContext(w, named_parameters)
+    if ctx.is_azure:
+        return ctx.azure_external_locations_migration.run()
+    if ctx.is_aws:
+        return ctx.aws_resource_permissions.create_external_locations()
+    raise ValueError("Unsupported cloud provider")
 
 
 @ucx.command
 def create_catalogs_schemas(w: WorkspaceClient, prompts: Prompts):
     """Create UC catalogs and schemas based on the destinations created from create_table_mapping command."""
-    installation = Installation.current(w, 'ucx')
-    catalog_schema = CatalogSchema.for_cli(w, installation)
-    catalog_schema.create_all_catalogs_schemas(prompts)
+    ctx = WorkspaceContext(w)
+    ctx.catalog_schema.create_all_catalogs_schemas(prompts)
 
 
 @ucx.command
 def cluster_remap(w: WorkspaceClient, prompts: Prompts):
     """Re-mapping the cluster to UC"""
     logger.info("Remapping the Clusters to UC")
-    installation = Installation.current(w, 'ucx')
-    cluster = ClusterAccess(installation, w, prompts)
-    cluster_list = cluster.list_cluster()
+    ctx = WorkspaceContext(w)
+    cluster_list = ctx.cluster_access.list_cluster()
     if not cluster_list:
         logger.info("No cluster information present in the workspace")
         return
     print(f"{'Cluster Name':<50}\t{'Cluster Id':<50}")
     for cluster_details in cluster_list:
         print(f"{cluster_details.cluster_name:<50}\t{cluster_details.cluster_id:<50}")
     cluster_ids = prompts.question(
         "Please provide the cluster id's as comma separated value from the above list", default="<ALL>"
     )
-    cluster.map_cluster_to_uc(cluster_ids, cluster_list)
+    ctx.cluster_access.map_cluster_to_uc(cluster_ids, cluster_list)
 
 
 @ucx.command
 def revert_cluster_remap(w: WorkspaceClient, prompts: Prompts):
     """Reverting Re-mapping of  clusters from UC"""
     logger.info("Reverting the Remapping of the Clusters from UC")
-    installation = Installation.current(w, 'ucx')
+    ctx = WorkspaceContext(w)
     cluster_ids = [
         cluster_files.path.split("/")[-1].split(".")[0]
-        for cluster_files in installation.files()
+        for cluster_files in ctx.installation.files()
         if cluster_files.path is not None and cluster_files.path.find("backup/clusters") > 0
     ]
     if not cluster_ids:
         logger.info("There is no cluster files in the backup folder. Skipping the reverting process")
         return
     for cluster in cluster_ids:
         logger.info(cluster)
     cluster_list = prompts.question(
         "Please provide the cluster id's as comma separated value from the above list", default="<ALL>"
     )
-    cluster_details = ClusterAccess(installation, w, prompts)
-    cluster_details.revert_cluster_remap(cluster_list, cluster_ids)
+    ctx.cluster_access.revert_cluster_remap(cluster_list, cluster_ids)
 
 
 @ucx.command
 def migrate_local_code(w: WorkspaceClient, prompts: Prompts):
     """Fix the code files based on their language."""
-    files = Files.for_cli(w)
+    ctx = WorkspaceContext(w)
     working_directory = Path.cwd()
     if not prompts.confirm("Do you want to apply UC migration to all files in the current directory?"):
         return
-    files.apply(working_directory)
+    ctx.local_file_migrator.apply(working_directory)
+
+
+@ucx.command(is_account=True)
+def show_all_metastores(a: AccountClient, workspace_id: str | None = None):
+    """Show all metastores in the account"""
+    logger.info(f"Account ID: {a.config.account_id}")
+    ctx = AccountContext(a)
+    ctx.account_metastores.show_all_metastores(workspace_id)
+
+
+@ucx.command(is_account=True)
+def assign_metastore(
+    a: AccountClient,
+    workspace_id: str | None = None,
+    metastore_id: str | None = None,
+    default_catalog: str | None = None,
+):
+    """Assign metastore to a workspace"""
+    logger.info(f"Account ID: {a.config.account_id}")
+    ctx = AccountContext(a)
+    ctx.account_metastores.assign_metastore(ctx.prompts, workspace_id, metastore_id, default_catalog)
+
+
+@ucx.command
+def migrate_tables(w: WorkspaceClient, prompts: Prompts, *, ctx: WorkspaceContext | None = None):
+    """
+    Trigger the migrate-tables workflow and, optionally, the migrate-external-hiveserde-tables-in-place-experimental
+    workflow.
+    """
+    if ctx is None:
+        ctx = WorkspaceContext(w)
+    deployed_workflows = ctx.deployed_workflows
+    deployed_workflows.run_workflow("migrate-tables")
+
+    tables = ctx.tables_crawler.snapshot()
+    hiveserde_tables = [table for table in tables if table.what == What.EXTERNAL_HIVESERDE]
+    if len(hiveserde_tables) > 0:
+        percentage_hiveserde_tables = len(hiveserde_tables) / len(tables) * 100
+        if prompts.confirm(
+            f"Found {len(hiveserde_tables)} ({percentage_hiveserde_tables:.2f}%) hiveserde tables, do you want to run "
+            f"the migrate-external-hiveserde-tables-in-place-experimental workflow?"
+        ):
+            deployed_workflows.run_workflow("migrate-external-hiveserde-tables-in-place-experimental")
 
 
 if __name__ == "__main__":
     ucx()
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/config.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,17 +44,27 @@
     # Flag to see if terraform has been used for deploying certain entities
     is_terraform_used: bool = False
 
     # Whether the assessment should capture a specific list of databases, if not specified, it will list all databases.
     include_databases: list[str] | None = None
 
     # Whether the tables in mounts crawler should crawl a specific list of mounts.
-    # If not specified, it will list all moubts.
+    # If not specified, it will list all mounts.
     include_mounts: list[str] | None = None
     exclude_paths_in_mount: list[str] | None = None
+    include_paths_in_mount: list[str] | None = None
+
+    # Whether to trigger assessment job after installation
+    trigger_job: bool = False
+
+    # List of workspace ids ucx is installed on, only applied to account-level installation
+    installed_workspace_ids: list[int] | None = None
+
+    # [INTERNAL ONLY] Whether the assessment should capture only specific object permissions.
+    include_object_permissions: list[str] | None = None
 
     def replace_inventory_variable(self, text: str) -> str:
         return text.replace("$inventory", f"hive_metastore.{self.inventory_database}")
 
     @classmethod
     def v1_migrate(cls, raw: dict) -> dict:
         # See https://github.com/databrickslabs/ucx/blob/v0.5.0/src/databricks/labs/ucx/config.py#L16-L32
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/configure.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/configure.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/install.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/install.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,70 @@
+import dataclasses
 import functools
 import logging
 import os
 import re
 import time
 import webbrowser
-from collections.abc import Callable
 from datetime import timedelta
+from functools import cached_property
 from typing import Any
 
 import databricks.sdk.errors
 from databricks.labs.blueprint.entrypoint import get_logger
 from databricks.labs.blueprint.installation import Installation, SerdeError
+from databricks.labs.blueprint.installer import InstallState
 from databricks.labs.blueprint.parallel import ManyError, Threads
 from databricks.labs.blueprint.tui import Prompts
 from databricks.labs.blueprint.upgrades import Upgrades
 from databricks.labs.blueprint.wheels import (
     ProductInfo,
     Version,
-    WheelsV2,
     find_project_root,
 )
 from databricks.labs.lsql.backends import SqlBackend, StatementExecutionBackend
 from databricks.labs.lsql.deployment import SchemaDeployer
-from databricks.sdk import WorkspaceClient
+from databricks.sdk import WorkspaceClient, AccountClient
 from databricks.sdk.errors import (
     AlreadyExists,
     BadRequest,
     InvalidParameterValue,
     NotFound,
+    PermissionDenied,
+    ResourceDoesNotExist,
 )
+from databricks.sdk.service.provisioning import Workspace
 from databricks.sdk.service.sql import (
     CreateWarehouseRequestWarehouseType,
     EndpointInfoWarehouseType,
     SpotInstancePolicy,
 )
 
 from databricks.labs.ucx.__about__ import __version__
 from databricks.labs.ucx.assessment.azure import AzureServicePrincipalInfo
 from databricks.labs.ucx.assessment.clusters import ClusterInfo, PolicyInfo
 from databricks.labs.ucx.assessment.init_scripts import GlobalInitScriptInfo
 from databricks.labs.ucx.assessment.jobs import JobInfo, SubmitRunInfo
 from databricks.labs.ucx.assessment.pipelines import PipelineInfo
 from databricks.labs.ucx.config import WorkspaceConfig
+from databricks.labs.ucx.contexts.cli_command import AccountContext, WorkspaceContext
 from databricks.labs.ucx.framework.dashboards import DashboardFromFiles
+from databricks.labs.ucx.framework.tasks import Task
 from databricks.labs.ucx.hive_metastore.grants import Grant
 from databricks.labs.ucx.hive_metastore.locations import ExternalLocation, Mount
-from databricks.labs.ucx.hive_metastore.table_migrate import MigrationStatus
+from databricks.labs.ucx.hive_metastore.migration_status import MigrationStatus
 from databricks.labs.ucx.hive_metastore.table_size import TableSize
 from databricks.labs.ucx.hive_metastore.tables import Table, TableError
 from databricks.labs.ucx.hive_metastore.udfs import Udf
 from databricks.labs.ucx.installer.hms_lineage import HiveMetastoreLineageEnabler
+from databricks.labs.ucx.installer.logs import LogRecord
 from databricks.labs.ucx.installer.mixins import InstallationMixin
 from databricks.labs.ucx.installer.policy import ClusterPolicyInstaller
-from databricks.labs.ucx.installer.workflows import WorkflowsInstallation
+from databricks.labs.ucx.installer.workflows import WorkflowsDeployment
+from databricks.labs.ucx.runtime import Workflows
 from databricks.labs.ucx.workspace_access.base import Permissions
 from databricks.labs.ucx.workspace_access.generic import WorkspaceObjectInfo
 from databricks.labs.ucx.workspace_access.groups import ConfigureGroups, MigratedGroup
 
 TAG_STEP = "step"
 WAREHOUSE_PREFIX = "Unity Catalog Migration"
 NUM_USER_ATTEMPTS = 10  # number of attempts user gets at answering a question
@@ -64,14 +72,15 @@
 logger = logging.getLogger(__name__)
 
 
 def deploy_schema(sql_backend: SqlBackend, inventory_schema: str):
     # we need to import it like this because we expect a module instance
     from databricks.labs import ucx  # pylint: disable=import-outside-toplevel
 
+    logger.info("Creating ucx schemas...")
     deployer = SchemaDeployer(sql_backend, inventory_schema, ucx)
     deployer.deploy_schema()
     table = functools.partial(deployer.deploy_table)
     Threads.strict(
         "deploy tables",
         [
             functools.partial(table, "azure_service_principals", AzureServicePrincipalInfo),
@@ -88,14 +97,15 @@
             functools.partial(table, "table_failures", TableError),
             functools.partial(table, "workspace_objects", WorkspaceObjectInfo),
             functools.partial(table, "permissions", Permissions),
             functools.partial(table, "submit_runs", SubmitRunInfo),
             functools.partial(table, "policies", PolicyInfo),
             functools.partial(table, "migration_status", MigrationStatus),
             functools.partial(table, "udfs", Udf),
+            functools.partial(table, "logs", LogRecord),
         ],
     )
     deployer.deploy_view("objects", "queries/views/objects.sql")
     deployer.deploy_view("grant_detail", "queries/views/grant_detail.sql")
     deployer.deploy_view("table_estimates", "queries/views/table_estimates.sql")
     deployer.deploy_view("misc_patterns", "queries/views/misc_patterns.sql")
     deployer.deploy_view("code_patterns", "queries/views/code_patterns.sql")
@@ -104,278 +114,369 @@
 def extract_major_minor(version_string):
     match = re.search(r'(\d+\.\d+)', version_string)
     if match:
         return match.group(1)
     return None
 
 
-class WorkspaceInstaller:
+class WorkspaceInstaller(WorkspaceContext):
     def __init__(
         self,
-        prompts: Prompts,
-        installation: Installation,
         ws: WorkspaceClient,
-        product_info: ProductInfo,
         environ: dict[str, str] | None = None,
+        tasks: list[Task] | None = None,
     ):
+        super().__init__(ws)
         if not environ:
             environ = dict(os.environ.items())
+        self._force_install = environ.get("UCX_FORCE_INSTALL")
         if "DATABRICKS_RUNTIME_VERSION" in environ:
             msg = "WorkspaceInstaller is not supposed to be executed in Databricks Runtime"
             raise SystemExit(msg)
-        self._ws = ws
-        self._installation = installation
-        self._prompts = prompts
-        self._policy_installer = ClusterPolicyInstaller(installation, ws, prompts)
-        self._product_info = product_info
-        self._force_install = environ.get("UCX_FORCE_INSTALL")
+
+        self._is_account_install = self._force_install == "account"
+        self._tasks = tasks if tasks else Workflows.all().tasks()
+
+    @cached_property
+    def upgrades(self):
+        return Upgrades(self.product_info, self.installation)
+
+    @cached_property
+    def policy_installer(self):
+        return ClusterPolicyInstaller(self.installation, self.workspace_client, self.prompts)
+
+    @cached_property
+    def installation(self):
+        try:
+            return self.product_info.current_installation(self.workspace_client)
+        except NotFound:
+            if self._force_install == "user":
+                return Installation.assume_user_home(self.workspace_client, self.product_info.product_name())
+            return Installation.assume_global(self.workspace_client, self.product_info.product_name())
 
     def run(
         self,
+        default_config: WorkspaceConfig | None = None,
         verify_timeout=timedelta(minutes=2),
-        sql_backend_factory: Callable[[WorkspaceConfig], SqlBackend] | None = None,
-        wheel_builder_factory: Callable[[], WheelsV2] | None = None,
-    ):
-        logger.info(f"Installing UCX v{self._product_info.version()}")
-        config = self.configure()
-        if not sql_backend_factory:
-            sql_backend_factory = self._new_sql_backend
-        if not wheel_builder_factory:
-            wheel_builder_factory = self._new_wheel_builder
-        wheels = wheel_builder_factory()
-        workflows_installer = WorkflowsInstallation(
-            config, self._installation, self._ws, wheels, self._prompts, self._product_info, verify_timeout
+        config: WorkspaceConfig | None = None,
+    ) -> WorkspaceConfig:
+        logger.info(f"Installing UCX v{self.product_info.version()}")
+        if config is None:
+            config = self.configure(default_config)
+        if self._is_testing():
+            return config
+        workflows_deployment = WorkflowsDeployment(
+            config,
+            self.installation,
+            self.install_state,
+            self.workspace_client,
+            self.wheels,
+            self.product_info,
+            verify_timeout,
+            self._tasks,
         )
         workspace_installation = WorkspaceInstallation(
             config,
-            self._installation,
-            sql_backend_factory(config),
-            self._ws,
-            workflows_installer,
-            self._prompts,
-            self._product_info,
+            self.installation,
+            self.install_state,
+            self.sql_backend,
+            self.workspace_client,
+            workflows_deployment,
+            self.prompts,
+            self.product_info,
         )
         try:
             workspace_installation.run()
         except ManyError as err:
             if len(err.errs) == 1:
                 raise err.errs[0] from None
             raise err
+        return config
+
+    def _is_testing(self):
+        return self.product_info.product_name() != "ucx"
+
+    def _prompt_for_new_installation(self) -> WorkspaceConfig:
+        logger.info("Please answer a couple of questions to configure Unity Catalog migration")
+        inventory_database = self.prompts.question(
+            "Inventory Database stored in hive_metastore", default="ucx", valid_regex=r"^\w+$"
+        )
+        log_level = self.prompts.question("Log level", default="INFO").upper()
+        num_threads = int(self.prompts.question("Number of threads", default="8", valid_number=True))
+        configure_groups = ConfigureGroups(self.prompts)
+        configure_groups.run()
+        # Check if terraform is being used
+        is_terraform_used = self.prompts.confirm("Do you use Terraform to deploy your infrastructure?")
+        include_databases = self._select_databases()
+        trigger_job = self.prompts.confirm("Do you want to trigger assessment job after installation?")
+        return WorkspaceConfig(
+            inventory_database=inventory_database,
+            workspace_group_regex=configure_groups.workspace_group_regex,
+            workspace_group_replace=configure_groups.workspace_group_replace,
+            account_group_regex=configure_groups.account_group_regex,
+            group_match_by_external_id=configure_groups.group_match_by_external_id,  # type: ignore[arg-type]
+            include_group_names=configure_groups.include_group_names,
+            renamed_group_prefix=configure_groups.renamed_group_prefix,
+            log_level=log_level,
+            num_threads=num_threads,
+            is_terraform_used=is_terraform_used,
+            include_databases=include_databases,
+            trigger_job=trigger_job,
+        )
 
     def _compare_remote_local_versions(self):
         try:
-            local_version = self._product_info.released_version()
-            remote_version = self._installation.load(Version).version
+            local_version = self.product_info.released_version()
+            remote_version = self.installation.load(Version).version
             if extract_major_minor(remote_version) == extract_major_minor(local_version):
-                logger.info(f"UCX v{self._product_info.version()} is already installed on this workspace")
+                logger.info(f"UCX v{self.product_info.version()} is already installed on this workspace")
                 msg = "Do you want to update the existing installation?"
-                if not self._prompts.confirm(msg):
+                if not self.prompts.confirm(msg):
                     raise RuntimeWarning(
                         "UCX workspace remote and local install versions are same and no override is requested. Exiting..."
                     )
         except NotFound as err:
             logger.warning(f"UCX workspace remote version not found: {err}")
 
-    def _new_wheel_builder(self):
-        return WheelsV2(self._installation, self._product_info)
-
-    def _new_sql_backend(self, config: WorkspaceConfig) -> SqlBackend:
-        return StatementExecutionBackend(self._ws, config.warehouse_id)
-
     def _confirm_force_install(self) -> bool:
         if not self._force_install:
             return False
         msg = "[ADVANCED] UCX is already installed on this workspace. Do you want to create a new installation?"
-        if not self._prompts.confirm(msg):
+        if not self.prompts.confirm(msg):
             raise RuntimeWarning("UCX is already installed, but no confirmation")
-        if not self._installation.is_global() and self._force_install == "global":
+        if not self.installation.is_global() and self._force_install == "global":
             # TODO:
             # Logic for forced global over user install
             # Migration logic will go here
             # verify complains without full path, asks to raise NotImplementedError builtin
             raise databricks.sdk.errors.NotImplemented("Migration needed. Not implemented yet.")
-        if self._installation.is_global() and self._force_install == "user":
+        if self.installation.is_global() and self._force_install == "user":
             # Logic for forced user install over global install
-            self._installation = Installation.assume_user_home(self._ws, self._product_info.product_name())
+            self.replace(
+                installation=Installation.assume_user_home(self.workspace_client, self.product_info.product_name())
+            )
             return True
         return False
 
-    def configure(self) -> WorkspaceConfig:
+    def configure(self, default_config: WorkspaceConfig | None = None) -> WorkspaceConfig:
         try:
-            config = self._installation.load(WorkspaceConfig)
+            config = self.installation.load(WorkspaceConfig)
             self._compare_remote_local_versions()
             if self._confirm_force_install():
-                return self._configure_new_installation()
+                return self._configure_new_installation(default_config)
             self._apply_upgrades()
             return config
         except NotFound as err:
             logger.debug(f"Cannot find previous installation: {err}")
-        return self._configure_new_installation()
+        return self._configure_new_installation(default_config)
+
+    def replace_config(self, **changes: Any) -> WorkspaceConfig | None:
+        """
+        Persist the list of workspaces where UCX is successfully installed in the config
+        """
+        try:
+            config = self.installation.load(WorkspaceConfig)
+            new_config = dataclasses.replace(config, **changes)
+            self.installation.save(new_config)
+        except (PermissionDenied, NotFound, ValueError):
+            logger.warning(f"Failed to replace config for {self.workspace_client.config.host}")
+            new_config = None
+        return new_config
 
     def _apply_upgrades(self):
         try:
-            upgrades = Upgrades(self._product_info, self._installation)
-            upgrades.apply(self._ws)
-        except NotFound as err:
+            self.upgrades.apply(self.workspace_client)
+        except (InvalidParameterValue, NotFound) as err:
             logger.warning(f"Installed version is too old: {err}")
-            return
-
-    def _configure_new_installation(self) -> WorkspaceConfig:
-        logger.info("Please answer a couple of questions to configure Unity Catalog migration")
-        HiveMetastoreLineageEnabler(self._ws).apply(self._prompts)
-        inventory_database = self._prompts.question(
-            "Inventory Database stored in hive_metastore", default="ucx", valid_regex=r"^\w+$"
-        )
-
-        self._check_inventory_database_exists(inventory_database)
-        warehouse_id = self._configure_warehouse()
-        configure_groups = ConfigureGroups(self._prompts)
-        configure_groups.run()
-        log_level = self._prompts.question("Log level", default="INFO").upper()
-        num_threads = int(self._prompts.question("Number of threads", default="8", valid_number=True))
 
-        policy_id, instance_profile, spark_conf_dict, instance_pool_id = self._policy_installer.create(
-            inventory_database
+    def _configure_new_installation(self, default_config: WorkspaceConfig | None = None) -> WorkspaceConfig:
+        if default_config is None:
+            default_config = self._prompt_for_new_installation()
+        HiveMetastoreLineageEnabler(self.workspace_client).apply(self.prompts, self._is_account_install)
+        self._check_inventory_database_exists(default_config.inventory_database)
+        warehouse_id = self.configure_warehouse()
+        policy_id, instance_profile, spark_conf_dict, instance_pool_id = self.policy_installer.create(
+            default_config.inventory_database
         )
 
-        # Check if terraform is being used
-        is_terraform_used = self._prompts.confirm("Do you use Terraform to deploy your infrastructure?")
+        # Save configurable values for table migration cluster
+        min_workers, max_workers, spark_conf_dict = self._config_table_migration(spark_conf_dict)
 
-        config = WorkspaceConfig(
-            inventory_database=inventory_database,
-            workspace_group_regex=configure_groups.workspace_group_regex,
-            workspace_group_replace=configure_groups.workspace_group_replace,
-            account_group_regex=configure_groups.account_group_regex,
-            group_match_by_external_id=configure_groups.group_match_by_external_id,  # type: ignore[arg-type]
-            include_group_names=configure_groups.include_group_names,
-            renamed_group_prefix=configure_groups.renamed_group_prefix,
+        config = dataclasses.replace(
+            default_config,
             warehouse_id=warehouse_id,
-            log_level=log_level,
-            num_threads=num_threads,
             instance_profile=instance_profile,
             spark_conf=spark_conf_dict,
+            min_workers=min_workers,
+            max_workers=max_workers,
             policy_id=policy_id,
             instance_pool_id=instance_pool_id,
-            is_terraform_used=is_terraform_used,
-            include_databases=self._select_databases(),
         )
-        self._installation.save(config)
-        ws_file_url = self._installation.workspace_link(config.__file__)
-        if self._prompts.confirm(f"Open config file in the browser and continue installing? {ws_file_url}"):
+        self.installation.save(config)
+        if self._is_account_install:
+            return config
+        ws_file_url = self.installation.workspace_link(config.__file__)
+        if self.prompts.confirm(f"Open config file in the browser and continue installing? {ws_file_url}"):
             webbrowser.open(ws_file_url)
         return config
 
+    def _config_table_migration(self, spark_conf_dict) -> tuple[int, int, dict]:
+        # parallelism will not be needed if backlog is fixed in https://databricks.atlassian.net/browse/ES-975874
+        if self._is_account_install:
+            return 1, 10, spark_conf_dict
+        parallelism = self.prompts.question(
+            "Parallelism for migrating dbfs root delta tables with deep clone", default="200", valid_number=True
+        )
+        if int(parallelism) > 200:
+            spark_conf_dict.update({'spark.sql.sources.parallelPartitionDiscovery.parallelism': parallelism})
+        # mix max workers for auto-scale migration job cluster
+        min_workers = int(
+            self.prompts.question(
+                "Min workers for auto-scale job cluster for table migration", default="1", valid_number=True
+            )
+        )
+        max_workers = int(
+            self.prompts.question(
+                "Max workers for auto-scale job cluster for table migration", default="10", valid_number=True
+            )
+        )
+        return min_workers, max_workers, spark_conf_dict
+
     def _select_databases(self):
-        selected_databases = self._prompts.question(
+        selected_databases = self.prompts.question(
             "Comma-separated list of databases to migrate. If not specified, we'll use all "
             "databases in hive_metastore",
             default="<ALL>",
         )
         if selected_databases != "<ALL>":
             return [x.strip() for x in selected_databases.split(",")]
         return None
 
-    def _configure_warehouse(self):
+    def configure_warehouse(self) -> str:
         def warehouse_type(_):
             return _.warehouse_type.value if not _.enable_serverless_compute else "SERVERLESS"
 
         pro_warehouses = {"[Create new PRO SQL warehouse]": "create_new"} | {
             f"{_.name} ({_.id}, {warehouse_type(_)}, {_.state.value})": _.id
-            for _ in self._ws.warehouses.list()
+            for _ in self.workspace_client.warehouses.list()
             if _.warehouse_type == EndpointInfoWarehouseType.PRO
         }
-        warehouse_id = self._prompts.choice_from_dict(
-            "Select PRO or SERVERLESS SQL warehouse to run assessment dashboards on", pro_warehouses
-        )
+        if self._is_account_install:
+            warehouse_id = "create_new"
+        else:
+            warehouse_id = self.prompts.choice_from_dict(
+                "Select PRO or SERVERLESS SQL warehouse to run assessment dashboards on", pro_warehouses
+            )
         if warehouse_id == "create_new":
-            new_warehouse = self._ws.warehouses.create(
+            new_warehouse = self.workspace_client.warehouses.create(
                 name=f"{WAREHOUSE_PREFIX} {time.time_ns()}",
                 spot_instance_policy=SpotInstancePolicy.COST_OPTIMIZED,
                 warehouse_type=CreateWarehouseRequestWarehouseType.PRO,
                 cluster_size="Small",
                 max_num_clusters=1,
             )
             warehouse_id = new_warehouse.id
         return warehouse_id
 
     def _check_inventory_database_exists(self, inventory_database: str):
         logger.info("Fetching installations...")
-        for installation in Installation.existing(self._ws, self._product_info.product_name()):
+        for installation in Installation.existing(self.workspace_client, self.product_info.product_name()):
             try:
                 config = installation.load(WorkspaceConfig)
                 if config.inventory_database == inventory_database:
                     raise AlreadyExists(
                         f"Inventory database '{inventory_database}' already exists in another installation"
                     )
-            except NotFound:
-                continue
-            except SerdeError:
+            except (PermissionDenied, NotFound, SerdeError):
                 continue
 
 
 class WorkspaceInstallation(InstallationMixin):
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         config: WorkspaceConfig,
         installation: Installation,
+        install_state: InstallState,
         sql_backend: SqlBackend,
         ws: WorkspaceClient,
-        workflows_installer: WorkflowsInstallation,
+        workflows_installer: WorkflowsDeployment,
         prompts: Prompts,
         product_info: ProductInfo,
+        skip_dashboards=False,
     ):
         self._config = config
         self._installation = installation
+        self._install_state = install_state
         self._ws = ws
         self._sql_backend = sql_backend
         self._workflows_installer = workflows_installer
         self._prompts = prompts
         self._product_info = product_info
+        environ = dict(os.environ.items())
+        self._is_account_install = environ.get("UCX_FORCE_INSTALL") == "account"
+        self._skip_dashboards = skip_dashboards
         super().__init__(config, installation, ws)
 
     @classmethod
     def current(cls, ws: WorkspaceClient):
+        # TODO: remove this method, it's no longer needed
         product_info = ProductInfo.from_class(WorkspaceConfig)
         installation = product_info.current_installation(ws)
+        install_state = InstallState.from_installation(installation)
         config = installation.load(WorkspaceConfig)
         sql_backend = StatementExecutionBackend(ws, config.warehouse_id)
         wheels = product_info.wheels(ws)
         prompts = Prompts()
         timeout = timedelta(minutes=2)
-        workflows_installer = WorkflowsInstallation(config, installation, ws, wheels, prompts, product_info, timeout)
+        tasks = Workflows.all().tasks()
+        workflows_installer = WorkflowsDeployment(
+            config,
+            installation,
+            install_state,
+            ws,
+            wheels,
+            product_info,
+            timeout,
+            tasks,
+        )
 
-        return cls(config, installation, sql_backend, ws, workflows_installer, prompts, product_info)
+        return cls(
+            config,
+            installation,
+            install_state,
+            sql_backend,
+            ws,
+            workflows_installer,
+            prompts,
+            product_info,
+        )
 
     @property
     def config(self):
         return self._config
 
     @property
     def folder(self):
         return self._installation.install_folder()
 
     def run(self):
         logger.info(f"Installing UCX v{self._product_info.version()}")
-        Threads.strict(
-            "installing components",
-            [
-                self._create_dashboards,
-                self._create_database,
-            ],
-        )
-        self._workflows_installer.create_jobs()
-        readme_url = self._create_readme()
+        install_tasks = [self._create_database]
+        if not self._skip_dashboards:
+            install_tasks.append(self._create_dashboards)
+        Threads.strict("installing components", install_tasks)
+        readme_url = self._workflows_installer.create_jobs(self._prompts)
+        if not self._is_account_install and self._prompts.confirm(f"Open job overview in your browser? {readme_url}"):
+            webbrowser.open(readme_url)
         logger.info(f"Installation completed successfully! Please refer to the {readme_url} for the next steps.")
 
-        if self._prompts.confirm("Do you want to trigger assessment job ?"):
+        if self.config.trigger_job:
             logger.info("Triggering the assessment workflow")
             self._trigger_workflow("assessment")
-
-    def config_file_link(self):
-        return self._installation.workspace_link('config.yml')
+        return True
 
     def _create_database(self):
         try:
             deploy_schema(self._sql_backend, self._config.inventory_database)
         except Exception as err:
             if "UNRESOLVED_COLUMN.WITH_SUGGESTION" in str(err):
                 msg = (
@@ -389,84 +490,37 @@
             raise err
 
     def _create_dashboards(self):
         logger.info("Creating dashboards...")
         local_query_files = find_project_root(__file__) / "src/databricks/labs/ucx/queries"
         dash = DashboardFromFiles(
             self._ws,
-            state=self._workflows_installer.state,
+            state=self._install_state,
             local_folder=local_query_files,
             remote_folder=f"{self._installation.install_folder()}/queries",
             name_prefix=self._name("UCX "),
             warehouse_id=self._warehouse_id,
             query_text_callback=self._config.replace_inventory_variable,
         )
         dash.create_dashboards()
 
-    def _create_readme(self) -> str:
-        debug_notebook_link = self._installation.workspace_markdown_link('debug notebook', 'DEBUG.py')
-        markdown = [
-            "# UCX - The Unity Catalog Migration Assistant",
-            f'To troubleshoot, see {debug_notebook_link}.\n',
-            "Here are the URLs and descriptions of workflows that trigger various stages of migration.",
-            "All jobs are defined with necessary cluster configurations and DBR versions.\n",
-        ]
-        for step_name in self.step_list():
-            if step_name not in self._workflows_installer.state.jobs:
-                logger.warning(f"Skipping step '{step_name}' since it was not deployed.")
-                continue
-            job_id = self._workflows_installer.state.jobs[step_name]
-            dashboard_link = ""
-            dashboards_per_step = [
-                d for d in self._workflows_installer.state.dashboards.keys() if d.startswith(step_name)
-            ]
-            for dash in dashboards_per_step:
-                if len(dashboard_link) == 0:
-                    dashboard_link += "Go to the one of the following dashboards after running the job:\n"
-                first, second = dash.replace("_", " ").title().split()
-                dashboard_url = (
-                    f"{self._ws.config.host}/sql/dashboards/{self._workflows_installer.state.dashboards[dash]}"
-                )
-                dashboard_link += f"  - [{first} ({second}) dashboard]({dashboard_url})\n"
-            job_link = f"[{self._name(step_name)}]({self._ws.config.host}#job/{job_id})"
-            markdown.append("---\n\n")
-            markdown.append(f"## {job_link}\n\n")
-            markdown.append(f"{dashboard_link}")
-            markdown.append("\nThe workflow consists of the following separate tasks:\n\n")
-            for task in self.sorted_tasks():
-                if task.workflow != step_name:
-                    continue
-                doc = self._config.replace_inventory_variable(task.doc)
-                markdown.append(f"### `{task.name}`\n\n")
-                markdown.append(f"{doc}\n")
-                markdown.append("\n\n")
-        preamble = ["# Databricks notebook source", "# MAGIC %md"]
-        intro = "\n".join(preamble + [f"# MAGIC {line}" for line in markdown])
-        self._installation.upload('README.py', intro.encode('utf8'))
-        readme_url = self._installation.workspace_link('README')
-        if self._prompts and self._prompts.confirm(f"Open job overview in your browser? {readme_url}"):
-            webbrowser.open(readme_url)
-        return readme_url
-
-    def _replace_inventory_variable(self, text: str) -> str:
-        return text.replace("$inventory", f"hive_metastore.{self._config.inventory_database}")
-
     def uninstall(self):
         if self._prompts and not self._prompts.confirm(
             "Do you want to uninstall ucx from the workspace too, this would "
             "remove ucx project folder, dashboards, queries and jobs"
         ):
             return
         # TODO: this is incorrect, fetch the remote version (that appeared only in Feb 2024)
         logger.info(f"Deleting UCX v{self._product_info.version()} from {self._ws.config.host}")
         try:
             self._installation.files()
         except NotFound:
             logger.error(f"Check if {self._installation.install_folder()} is present")
             return
+        self._check_and_fix_if_warehouse_does_not_exists()
         self._remove_database()
         self._remove_jobs()
         self._remove_warehouse()
         self._remove_policies()
         self._remove_secret_scope()
         self._installation.remove()
         logger.info("UnInstalling UCX complete")
@@ -493,18 +547,18 @@
             if self.config.uber_spn_id is not None:
                 self._ws.secrets.delete_scope(self.config.inventory_database)
         except NotFound:
             logger.error("Secret scope already deleted")
 
     def _remove_jobs(self):
         logger.info("Deleting jobs")
-        if not self._workflows_installer.state.jobs:
+        if not self._install_state.jobs:
             logger.error("No jobs present or jobs already deleted")
             return
-        for step_name, job_id in self._workflows_installer.state.jobs.items():
+        for step_name, job_id in self._install_state.jobs.items():
             try:
                 logger.info(f"Deleting {step_name} job_id={job_id}.")
                 self._ws.jobs.delete(job_id)
             except InvalidParameterValue:
                 logger.error(f"Already deleted: {step_name} job_id={job_id}.")
                 continue
 
@@ -513,32 +567,120 @@
             warehouse_name = self._ws.warehouses.get(self._config.warehouse_id).name
             if warehouse_name.startswith(WAREHOUSE_PREFIX):
                 logger.info(f"Deleting {warehouse_name}.")
                 self._ws.warehouses.delete(id=self._config.warehouse_id)
         except InvalidParameterValue:
             logger.error("Error accessing warehouse details")
 
-    def validate_and_run(self, step: str):
-        if not self._workflows_installer.validate_step(step):
-            self._workflows_installer.run_workflow(step)
-
     def _trigger_workflow(self, step: str):
-        job_id = int(self._workflows_installer.state.jobs[step])
+        job_id = int(self._install_state.jobs[step])
         job_url = f"{self._ws.config.host}#job/{job_id}"
         logger.debug(f"triggering {step} job: {self._ws.config.host}#job/{job_id}")
         self._ws.jobs.run_now(job_id)
         if self._prompts.confirm(f"Open {step} Job url that just triggered ? {job_url}"):
             webbrowser.open(job_url)
 
+    def _check_and_fix_if_warehouse_does_not_exists(self):
+        try:
+            self._ws.warehouses.get(self._config.warehouse_id)
+        except ResourceDoesNotExist:
+            logger.critical(f"warehouse with id {self._config.warehouse_id} does not exists anymore")
+            installer = WorkspaceInstaller(self._ws).replace(product_info=self._product_info, prompts=self._prompts)
+            warehouse_id = installer.configure_warehouse()
+            self._config = installer.replace_config(warehouse_id=warehouse_id)
+            self._sql_backend = StatementExecutionBackend(self._ws, self._config.warehouse_id)
+
+
+class AccountInstaller(AccountContext):
+    def _get_safe_account_client(self) -> AccountClient:
+        """
+        Get account client with the correct host based on the cloud provider
+        """
+        if self.account_client.config.is_account_client:
+            return self.account_client
+        w = WorkspaceClient(product="ucx", product_version=__version__)
+        host = w.config.environment.deployment_url("accounts")
+        account_id = self.prompts.question("Please provide the Databricks account id")
+        return AccountClient(host=host, account_id=account_id, product="ucx", product_version=__version__)
+
+    def _can_administer(self, workspace: Workspace):
+        try:
+            # check if user is a workspace admin
+            ws = self.account_client.get_workspace_client(workspace)
+            current_user = ws.current_user.me()
+            if current_user.groups is None:
+                return False
+            if "admins" not in [g.display for g in current_user.groups]:
+                logger.warning(
+                    f"{workspace.deployment_name}: User {current_user.user_name} is not a workspace admin. Skipping..."
+                )
+                return False
+            # check if user has access to workspace
+        except (PermissionDenied, NotFound, ValueError) as err:
+            logger.warning(f"{workspace.deployment_name}: Encounter error {err}. Skipping...")
+            return False
+        return True
+
+    def _get_accessible_workspaces(self):
+        """
+        Get all workspaces that the user has access to
+        """
+        accessible_workspaces = []
+        for workspace in self.account_client.workspaces.list():
+            if self._can_administer(workspace):
+                accessible_workspaces.append(workspace)
+        return accessible_workspaces
+
+    def _get_installer(self, workspace: Workspace) -> WorkspaceInstaller:
+        workspace_client = self.account_client.get_workspace_client(workspace)
+        logger.info(f"Installing UCX on workspace {workspace.deployment_name}")
+        return WorkspaceInstaller(workspace_client).replace(product_info=self.product_info, prompts=self.prompts)
+
+    def install_on_account(self):
+        ctx = AccountContext(self._get_safe_account_client())
+        default_config = None
+        confirmed = False
+        accessible_workspaces = self._get_accessible_workspaces()
+        msg = "\n".join([w.deployment_name for w in accessible_workspaces])
+        installed_workspaces = []
+        if not self.prompts.confirm(
+            f"UCX has detected the following workspaces available to install. \n{msg}\nDo you want to continue?"
+        ):
+            return
+
+        for workspace in accessible_workspaces:
+            logger.info(f"Installing UCX on workspace {workspace.deployment_name}")
+            installer = self._get_installer(workspace)
+            if not confirmed:
+                default_config = None
+            try:
+                default_config = installer.run(default_config)
+            except RuntimeWarning:
+                logger.info("Skipping workspace...")
+            # if user confirms to install on remaining workspaces with the same config, don't prompt again
+            installed_workspaces.append(workspace)
+            if confirmed:
+                continue
+            confirmed = self.prompts.confirm(
+                "Do you want to install UCX on the remaining workspaces with the same config?"
+            )
+
+        installed_workspace_ids = [w.workspace_id for w in installed_workspaces if w.workspace_id is not None]
+        for workspace in installed_workspaces:
+            installer = self._get_installer(workspace)
+            installer.replace_config(installed_workspace_ids=installed_workspace_ids)
+
+        # upload the json dump of workspace info in the .ucx folder
+        ctx.account_workspaces.sync_workspace_info(installed_workspaces)
+
 
 if __name__ == "__main__":
     logger = get_logger(__file__)
-    logger.setLevel("INFO")
-    app = ProductInfo.from_class(WorkspaceConfig)
-    workspace_client = WorkspaceClient(product="ucx", product_version=__version__)
-    try:
-        current = app.current_installation(workspace_client)
-    except NotFound:
-        current = Installation.assume_global(workspace_client, app.product_name())
-    prmpts = Prompts()
-    installer = WorkspaceInstaller(prmpts, current, workspace_client, app)
-    installer.run()
+
+    env = dict(os.environ.items())
+    force_install = env.get("UCX_FORCE_INSTALL")
+    if force_install == "account":
+        account_installer = AccountInstaller(AccountClient(product="ucx", product_version=__version__))
+        account_installer.install_on_account()
+    else:
+        workspace_installer = WorkspaceInstaller(WorkspaceClient(product="ucx", product_version=__version__))
+        workspace_installer.run()
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/aws.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/aws.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,42 +81,40 @@
     ]
 
     def __init__(self, profile: str, command_runner: Callable[[str], tuple[int, str, str]] = run_command):
         self._profile = profile
         self._command_runner = command_runner
 
     def validate_connection(self):
-        validate_command = f"sts get-caller-identity --profile {self._profile}"
+        validate_command = "sts get-caller-identity"
         result = self._run_json_command(validate_command)
         if result:
             logger.info(result)
             return result
         return None
 
     def list_role_policies(self, role_name: str):
-        list_policies_cmd = f"iam list-role-policies --profile {self._profile} --role-name {role_name}"
+        list_policies_cmd = f"iam list-role-policies --role-name {role_name}"
         policies = self._run_json_command(list_policies_cmd)
         if not policies:
             return []
         return policies.get("PolicyNames", [])
 
     def list_attached_policies_in_role(self, role_name: str):
-        list_attached_policies_cmd = (
-            f"iam list-attached-role-policies --profile {self._profile} --role-name {role_name}"
-        )
+        list_attached_policies_cmd = f"iam list-attached-role-policies --role-name {role_name}"
         policies = self._run_json_command(list_attached_policies_cmd)
         if not policies:
             return []
         attached_policies = []
         for policy in policies.get("AttachedPolicies", []):
             attached_policies.append(policy.get("PolicyArn"))
         return attached_policies
 
     def list_all_uc_roles(self) -> list[AWSRole]:
-        roles = self._run_json_command(f"iam list-roles --profile {self._profile}")
+        roles = self._run_json_command("iam list-roles")
         uc_roles: list[AWSRole] = []
         roles = roles.get("Roles")
         if not roles:
             logger.warning("list-roles couldn't find any roles")
             return uc_roles
         for role in roles:
             policy_document = role.get("AssumeRolePolicyDocument")
@@ -154,27 +152,22 @@
                 if single_principal in self.UC_MASTER_ROLES_ARN:
                     return True
             return False
         return principal in self.UC_MASTER_ROLES_ARN
 
     def get_role_policy(self, role_name, policy_name: str | None = None, attached_policy_arn: str | None = None):
         if policy_name:
-            get_policy = (
-                f"iam get-role-policy --profile {self._profile} --role-name {role_name} " f"--policy-name {policy_name}"
-            )
+            get_policy = f"iam get-role-policy --role-name {role_name} --policy-name {policy_name}"
         elif attached_policy_arn:
-            get_attached_policy = f"iam get-policy --profile {self._profile} --policy-arn {attached_policy_arn}"
+            get_attached_policy = f"iam get-policy --policy-arn {attached_policy_arn}"
             attached_policy = self._run_json_command(get_attached_policy)
             if not attached_policy:
                 return []
             policy_version = attached_policy["Policy"]["DefaultVersionId"]
-            get_policy = (
-                f"iam get-policy-version --profile {self._profile} --policy-arn {attached_policy_arn} "
-                f"--version-id {policy_version}"
-            )
+            get_policy = f"iam get-policy-version --policy-arn {attached_policy_arn} --version-id {policy_version}"
         else:
             logger.error("Failed to retrieve role. No role name or attached role ARN specified.")
             return []
         policy = self._run_json_command(get_policy)
         if not policy:
             return []
         if policy_name:
@@ -215,27 +208,27 @@
             s3_actions = [actions]
         return s3_actions
 
     def _aws_role_trust_doc(self, external_id="0000"):
         return self._get_json_for_cli(
             {
                 "Version": "2012-10-17",
-                "Statement": [
-                    {
-                        "Effect": "Allow",
-                        "Principal": {
-                            "AWS": "arn:aws:iam::414351767826:role/unity-catalog-prod-UCMasterRole-14S5ZJVKOTYTL"
-                        },
-                        "Action": "sts:AssumeRole",
-                        "Condition": {"StringEquals": {"sts:ExternalId": external_id}},
-                    }
-                ],
+                "Statement": [self._databricks_trust_statement(external_id)],
             }
         )
 
+    @staticmethod
+    def _databricks_trust_statement(external_id="0000"):
+        return {
+            "Effect": "Allow",
+            "Principal": {"AWS": "arn:aws:iam::414351767826:role/unity-catalog-prod-UCMasterRole-14S5ZJVKOTYTL"},
+            "Action": "sts:AssumeRole",
+            "Condition": {"StringEquals": {"sts:ExternalId": external_id}},
+        }
+
     def _aws_s3_policy(self, s3_prefixes, account_id, role_name, kms_key=None):
         """
         Create the UC IAM policy for the given S3 prefixes, account ID, role name, and KMS key.
         """
         s3_prefixes_strip = set()
         for path in s3_prefixes:
             match = re.match(AWSResources.S3_PATH_REGEX, path)
@@ -291,27 +284,52 @@
 
     def update_uc_trust_role(self, role_name: str, external_id: str = "0000") -> str | None:
         """
         Modify an existing IAM role for Unity Catalog to access the S3 buckets with the external ID
         captured from the UC credential.
         https://docs.databricks.com/en/connect/unity-catalog/storage-credentials.html
         """
+        role_document = self._run_json_command(f"iam get-role --role-name {role_name}")
+        if role_document is None:
+            logger.error(f"Role {role_name} doesn't exist")
+            return None
+        role = role_document.get("Role")
+        policy_document = role.get("AssumeRolePolicyDocument")
+        if policy_document and policy_document.get("Statement"):
+            for idx, statement in enumerate(policy_document["Statement"]):
+                effect = statement.get("Effect")
+                action = statement.get("Action")
+                principal = statement.get("Principal")
+                if not (effect and action and principal):
+                    continue
+                if effect != "Allow":
+                    continue
+                if action != "sts:AssumeRole":
+                    continue
+                principal = principal.get("AWS")
+                if not principal:
+                    continue
+                if not self._is_uc_principal(principal):
+                    continue
+                policy_document["Statement"][idx] = self._databricks_trust_statement(external_id)
+            policy_document_json = self._get_json_for_cli(policy_document)
+        else:
+            policy_document_json = self._aws_role_trust_doc(external_id)
         update_role = self._run_json_command(
-            f"iam update-assume-role-policy --role-name {role_name} --policy-document {self._aws_role_trust_doc(external_id)}"
+            f"iam update-assume-role-policy --role-name {role_name} --policy-document {policy_document_json}"
         )
         if not update_role:
             return None
         return update_role["Role"]["Arn"]
 
     def put_role_policy(
         self, role_name: str, policy_name: str, s3_prefixes: set[str], account_id: str, kms_key=None
     ) -> bool:
         if not self._run_command(
-            f"iam put-role-policy --role-name {role_name} "
-            f"--policy-name {policy_name} "
+            f"iam put-role-policy --role-name {role_name} --policy-name {policy_name} "
             f"--policy-document {self._aws_s3_policy(s3_prefixes, account_id, role_name, kms_key)}"
         ):
             return False
         return True
 
     def create_migration_role(self, role_name: str) -> str | None:
         aws_role_trust_doc = {
@@ -366,25 +384,25 @@
         for role in roles:
             if role["RoleName"] == role_name:
                 return True
         return False
 
     def _run_json_command(self, command: str):
         aws_cmd = shutil.which("aws")
-        code, output, error = self._command_runner(f"{aws_cmd} {command} --output json")
+        code, output, error = self._command_runner(f"{aws_cmd} {command} --profile {self._profile} --output json")
         if code != 0:
             logger.error(error)
             return None
         if output == "":
             return {}
         return json.loads(output)
 
     def _run_command(self, command: str):
         aws_cmd = shutil.which("aws")
-        code, _, error = self._command_runner(f"{aws_cmd} {command} --output json")
+        code, _, error = self._command_runner(f"{aws_cmd} {command} --profile {self._profile} --output json")
         if code != 0:
             logger.error(error)
             return False
         return True
 
     @staticmethod
     def _get_json_for_cli(input_json: dict) -> str:
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/azure.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/azure.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from collections.abc import Iterable
 from dataclasses import dataclass
 
 from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound
-from databricks.sdk.service.compute import ClusterSource, Policy
+from databricks.sdk.service.compute import ClusterSource, DataSecurityMode, Policy
 
 from databricks.labs.ucx.assessment.crawlers import azure_sp_conf_present_check, logger
 from databricks.labs.ucx.assessment.jobs import JobsMixin
 from databricks.labs.ucx.assessment.secrets import SecretsMixin
 from databricks.labs.ucx.framework.crawlers import CrawlerBase
 
 _STORAGE_ACCOUNT_PATTERN = r"(?:id|endpoint)(.*?)dfs"
@@ -20,20 +20,29 @@
 class AzureServicePrincipalInfo:
     # fs.azure.account.oauth2.client.id
     application_id: str
     # fs.azure.account.oauth2.client.secret: {{secrets/${local.secret_scope}/${local.secret_key}}}
     secret_scope: str | None = None
     # fs.azure.account.oauth2.client.secret: {{secrets/${local.secret_scope}/${local.secret_key}}}
     secret_key: str | None = None
-    # fs.azure.account.oauth2.client.endpoint: "https://login.microsoftonline.com/${local.tenant_id}/oauth2/token"
+    # fs.azure.account.oauth2.client.endpoint: https://login.microsoftonline.com/${local.tenant_id}/oauth2/token
     tenant_id: str | None = None
     # Azure Storage account to which the SP has been given access
     storage_account: str | None = None
 
 
+@dataclass
+class ServicePrincipalClusterMapping:
+    # this class is created separately as we need cluster to spn mapping
+    # Cluster id where the spn is used
+    cluster_id: str
+    # spn info data class
+    spn_info: set[AzureServicePrincipalInfo]
+
+
 class AzureServicePrincipalCrawler(CrawlerBase[AzureServicePrincipalInfo], JobsMixin, SecretsMixin):
     def __init__(self, ws: WorkspaceClient, sbe: SqlBackend, schema):
         super().__init__(sbe, "hive_metastore", schema, "azure_service_principals", AzureServicePrincipalInfo)
         self._ws = ws
 
     def snapshot(self) -> Iterable[AzureServicePrincipalInfo]:
         return self._snapshot(self._try_fetch, self._crawl)
@@ -167,7 +176,20 @@
                     secret_scope=secret_scope,
                     secret_key=secret_key,
                     tenant_id=tenant_id,
                     storage_account=storage_account,
                 )
             )
         return set_service_principals
+
+    def get_cluster_to_storage_mapping(self):
+        # this function gives a mapping between an interactive cluster and the spn used by it
+        # either directly or through a cluster policy.
+        set_service_principals = set[AzureServicePrincipalInfo]()
+        spn_cluster_mapping = []
+        for cluster in self._ws.clusters.list():
+            if cluster.cluster_source != ClusterSource.JOB and (
+                cluster.data_security_mode in [DataSecurityMode.LEGACY_SINGLE_USER, DataSecurityMode.NONE]
+            ):
+                set_service_principals = self._get_azure_spn_from_cluster_config(cluster)
+                spn_cluster_mapping.append(ServicePrincipalClusterMapping(cluster.cluster_id, set_service_principals))
+        return spn_cluster_mapping
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/clusters.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/clusters.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         if cluster.data_security_mode in unsupported_cluster_types:
             failures.append(f"cluster type not supported : {cluster.data_security_mode.value}")
 
         return failures
 
 
 class ClustersCrawler(CrawlerBase[ClusterInfo], CheckClusterMixin):
-    def __init__(self, ws: WorkspaceClient, sbe: SqlBackend, schema):
+    def __init__(self, ws: WorkspaceClient, sbe: SqlBackend, schema: str):
         super().__init__(sbe, "hive_metastore", schema, "clusters", ClusterInfo)
         self._ws = ws
 
     def _crawl(self) -> Iterable[ClusterInfo]:
         all_clusters = list(self._ws.clusters.list())
         return list(self._assess_clusters(all_clusters))
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/crawlers.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/crawlers.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/init_scripts.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/init_scripts.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/jobs.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from databricks.sdk.service import compute
 from databricks.sdk.service.compute import ClusterDetails
 from databricks.sdk.service.jobs import (
     BaseJob,
     BaseRun,
     DbtTask,
     GitSource,
-    ListRunsRunType,
     PythonWheelTask,
     RunConditionTask,
     RunTask,
+    RunType,
     SparkJarTask,
     SqlTask,
 )
 
 from databricks.labs.ucx.assessment.clusters import CheckClusterMixin
 from databricks.labs.ucx.assessment.crawlers import spark_version_compatibility
 from databricks.labs.ucx.framework.crawlers import CrawlerBase
@@ -178,15 +178,15 @@
 
     def _crawl(self) -> Iterable[SubmitRunInfo]:
         end = self._dt_to_ms(self._get_current_dttm())
         start = self._dt_to_ms(self._get_current_dttm() - timedelta(days=self._num_days_history))
         submit_runs = self._ws.jobs.list_runs(
             expand_tasks=True,
             completed_only=True,
-            run_type=ListRunsRunType.SUBMIT_RUN,
+            run_type=RunType.SUBMIT_RUN,
             start_time_from=start,
             start_time_to=end,
         )
         all_clusters = {c.cluster_id: c for c in self._ws.clusters.list()}
         return self._assess_job_runs(submit_runs, all_clusters)
 
     def _try_fetch(self) -> Iterable[SubmitRunInfo]:
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/pipelines.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/pipelines.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/assessment/secrets.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/assessment/secrets.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/aws/access.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/aws/access.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,32 +45,14 @@
         self._ws = ws
         self._locations = external_locations
         self._schema = schema
         self._aws_account_id = aws_account_id
         self._kms_key = kms_key
         self._filename = self.INSTANCE_PROFILES_FILE_NAMES
 
-    @classmethod
-    def for_cli(cls, ws: WorkspaceClient, installation, backend, aws, schema, kms_key=None):
-        config = installation.load(WorkspaceConfig)
-        caller_identity = aws.validate_connection()
-        locations = ExternalLocations(ws, backend, config.inventory_database)
-        if not caller_identity:
-            raise ResourceWarning("AWS CLI is not configured properly.")
-        return cls(
-            installation,
-            ws,
-            backend,
-            aws,
-            locations,
-            schema,
-            caller_identity.get("Account"),
-            kms_key,
-        )
-
     def create_uc_roles_cli(self, *, single_role=True, role_name="UC_ROLE", policy_name="UC_POLICY"):
         # Get the missing paths
         # Identify the S3 prefixes
         # Create the roles and policies for the missing S3 prefixes
         # If single_role is True, create a single role and policy for all the missing S3 prefixes
         # If single_role is False, create a role and policy for each missing S3 prefix
         missing_paths = self._identify_missing_paths()
@@ -81,25 +63,23 @@
                 s3_prefixes.add(missing_path)
         if single_role:
             if self._aws_resources.create_uc_role(role_name):
                 self._aws_resources.put_role_policy(
                     role_name, policy_name, s3_prefixes, self._aws_account_id, self._kms_key
                 )
         else:
-            role_id = 1
-            for s3_prefix in sorted(list(s3_prefixes)):
-                if self._aws_resources.create_uc_role(f"{role_name}-{role_id}"):
+            for idx, s3_prefix in enumerate(sorted(list(s3_prefixes))):
+                if self._aws_resources.create_uc_role(f"{role_name}-{idx+1}"):
                     self._aws_resources.put_role_policy(
-                        f"{role_name}-{role_id}",
-                        f"{policy_name}-{role_id}",
+                        f"{role_name}-{idx+1}",
+                        f"{policy_name}-{idx+1}",
                         {s3_prefix},
                         self._aws_account_id,
                         self._kms_key,
                     )
-                role_id += 1
 
     def update_uc_role_trust_policy(self, role_name, external_id="0000"):
         return self._aws_resources.update_uc_trust_role(role_name, external_id)
 
     def save_uc_compatible_roles(self):
         uc_role_access = list(self._get_role_access())
         if len(uc_role_access) == 0:
@@ -247,15 +227,15 @@
             return self._ws.cluster_policies.get(policy_id=policy_id)
         except NotFound as err:
             msg = f"UCX Policy {policy_id} not found, please reinstall UCX"
             logger.error(msg)
             raise NotFound(msg) from err
 
     @staticmethod
-    def _get_iam_role_from_cluster_policy(cluster_policy_definition: str) -> str | None:
+    def get_iam_role_from_cluster_policy(cluster_policy_definition: str) -> str | None:
         definition_dict = json.loads(cluster_policy_definition)
         if definition_dict.get("aws_attributes.instance_profile_arn") is not None:
             instance_profile_arn = definition_dict.get("aws_attributes.instance_profile_arn").get("value")
             logger.info(f"Migration instance profile is set to {instance_profile_arn}")
 
             return AWSInstanceProfile(instance_profile_arn).role_name
 
@@ -317,15 +297,15 @@
         s3_paths = {loc.location for loc in self._locations.snapshot()}
 
         if len(s3_paths) == 0:
             logger.info("No S3 paths to migrate found")
             return
 
         cluster_policy = self._get_cluster_policy(config.policy_id)
-        iam_role_name_in_cluster_policy = self._get_iam_role_from_cluster_policy(str(cluster_policy.definition))
+        iam_role_name_in_cluster_policy = self.get_iam_role_from_cluster_policy(str(cluster_policy.definition))
 
         iam_policy_name = f"UCX_MIGRATION_POLICY_{config.inventory_database}"
         if iam_role_name_in_cluster_policy and self.role_exists(iam_role_name_in_cluster_policy):
             if not prompts.confirm(
                 f"We have identified existing UCX migration role \"{iam_role_name_in_cluster_policy}\" "
                 f"in cluster policy \"{cluster_policy.name}\". "
                 f"Do you want to update the role's migration policy?"
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/aws/credentials.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/aws/credentials.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 import logging
 from dataclasses import dataclass
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.tui import Prompts
-from databricks.labs.lsql.backends import StatementExecutionBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors.platform import InvalidParameterValue
 from databricks.sdk.service.catalog import (
     AwsIamRoleRequest,
     Privilege,
     StorageCredentialInfo,
     ValidationResultResult,
 )
 
-from databricks.labs.ucx.assessment.aws import AWSResources, AWSRoleAction
+from databricks.labs.ucx.assessment.aws import AWSRoleAction
 from databricks.labs.ucx.aws.access import AWSResourcePermissions
-from databricks.labs.ucx.config import WorkspaceConfig
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class CredentialValidationResult:
     name: str
@@ -111,48 +109,22 @@
 
 
 class IamRoleMigration:
 
     def __init__(
         self,
         installation: Installation,
-        ws: WorkspaceClient,
         resource_permissions: AWSResourcePermissions,
         storage_credential_manager: CredentialManager,
     ):
         self._output_file = "aws_iam_role_migration_result.csv"
         self._installation = installation
-        self._ws = ws
         self._resource_permissions = resource_permissions
         self._storage_credential_manager = storage_credential_manager
 
-    @classmethod
-    def for_cli(cls, ws: WorkspaceClient, installation: Installation, aws: AWSResources, prompts: Prompts):
-        if not ws.config.is_aws:
-            logger.error("Workspace is not on AWS, please run this command on a Databricks on AWS workspaces.")
-            raise SystemExit()
-
-        msg = (
-            f"Have you reviewed the {AWSResourcePermissions.UC_ROLES_FILE_NAMES} "
-            "and confirm listed IAM roles to be migrated?"
-        )
-        if not prompts.confirm(msg):
-            raise SystemExit()
-
-        config = installation.load(WorkspaceConfig)
-        sql_backend = StatementExecutionBackend(ws, config.warehouse_id)
-
-        resource_permissions = AWSResourcePermissions.for_cli(
-            ws, installation, sql_backend, aws, config.inventory_database
-        )
-
-        storage_credential_manager = CredentialManager(ws)
-
-        return cls(installation, ws, resource_permissions, storage_credential_manager)
-
     @staticmethod
     def _print_action_plan(iam_list: list[AWSRoleAction]):
         # print action plan to console for customer to review.
         for iam in iam_list:
             logger.info(f"{iam.role_arn}: {iam.privilege} on {iam.resource_path}")
 
     def _generate_migration_list(self, include_names: set[str] | None = None) -> list[AWSRoleAction]:
@@ -173,14 +145,17 @@
 
     def save(self, migration_results: list[CredentialValidationResult]) -> str:
         return self._installation.save(migration_results, filename=self._output_file)
 
     def run(self, prompts: Prompts, include_names: set[str] | None = None) -> list[CredentialValidationResult]:
 
         iam_list = self._generate_migration_list(include_names)
+        if len(iam_list) == 0:
+            logger.info("No IAM Role to migrate")
+            return []
 
         plan_confirmed = prompts.confirm(
             "Above IAM roles will be migrated to UC storage credentials, please review and confirm."
         )
         if plan_confirmed is not True:
             return []
 
@@ -188,21 +163,21 @@
         for iam in iam_list:
             storage_credential = self._storage_credential_manager.create(iam)
             if storage_credential.aws_iam_role is None:
                 logger.error(f"Failed to create storage credential for IAM role: {iam.role_arn}")
                 continue
 
             self._resource_permissions.update_uc_role_trust_policy(
-                iam.role_arn, storage_credential.aws_iam_role.external_id
+                iam.role_name, storage_credential.aws_iam_role.external_id
             )
 
             execution_result.append(self._storage_credential_manager.validate(iam))
 
         if execution_result:
             results_file = self.save(execution_result)
             logger.info(
-                f"Completed migration from IAM Role to UC Storage credentials"
+                f"Completed migration from IAM Role to UC Storage credentials. "
                 f"Please check {results_file} for validation results"
             )
         else:
             logger.info("No IAM Role migrated to UC Storage credentials")
         return execution_result
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/azure/access.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/access.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,77 +1,68 @@
 import json
+import logging
 import uuid
 from dataclasses import dataclass
+from functools import partial
 
 from databricks.labs.blueprint.installation import Installation
+from databricks.labs.blueprint.parallel import ManyError, Threads
 from databricks.labs.blueprint.tui import Prompts
-from databricks.labs.lsql.backends import StatementExecutionBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound, ResourceAlreadyExists
 from databricks.sdk.service.catalog import Privilege
 
-from databricks.labs.ucx.assessment.crawlers import logger
 from databricks.labs.ucx.azure.resources import (
-    AzureAPIClient,
-    AzureResource,
+    AccessConnector,
     AzureResources,
     PrincipalSecret,
+    StorageAccount,
 )
 from databricks.labs.ucx.config import WorkspaceConfig
 from databricks.labs.ucx.hive_metastore.locations import ExternalLocations
 
 
+logger = logging.getLogger(__name__)
+
+
 @dataclass
 class StoragePermissionMapping:
     prefix: str
     client_id: str
     principal: str
     privilege: str
     type: str
     # Need this directory_id/tenant_id when create UC storage credentials using service principal
     directory_id: str | None = None
 
 
 class AzureResourcePermissions:
+    FILENAME = 'azure_storage_account_info.csv'
+
     def __init__(
         self,
         installation: Installation,
         ws: WorkspaceClient,
         azurerm: AzureResources,
         external_locations: ExternalLocations,
     ):
-        self._filename = 'azure_storage_account_info.csv'
         self._installation = installation
         self._locations = external_locations
         self._azurerm = azurerm
         self._ws = ws
         self._levels = {
             "Storage Blob Data Contributor": Privilege.WRITE_FILES,
             "Storage Blob Data Owner": Privilege.WRITE_FILES,
             "Storage Blob Data Reader": Privilege.READ_FILES,
         }
 
-    @classmethod
-    def for_cli(cls, ws: WorkspaceClient, product='ucx', include_subscriptions=None):
-        installation = Installation.current(ws, product)
-        config = installation.load(WorkspaceConfig)
-        sql_backend = StatementExecutionBackend(ws, config.warehouse_id)
-        azure_mgmt_client = AzureAPIClient(
-            ws.config.arm_environment.resource_manager_endpoint,
-            ws.config.arm_environment.service_management_endpoint,
-        )
-        graph_client = AzureAPIClient("https://graph.microsoft.com", "https://graph.microsoft.com")
-        azurerm = AzureResources(azure_mgmt_client, graph_client, include_subscriptions)
-        locations = ExternalLocations(ws, sql_backend, config.inventory_database)
-        return cls(installation, ws, azurerm, locations)
-
-    def _map_storage(self, storage: AzureResource) -> list[StoragePermissionMapping]:
-        logger.info(f"Fetching role assignment for {storage.storage_account}")
+    def _map_storage(self, storage: StorageAccount) -> list[StoragePermissionMapping]:
+        logger.info(f"Fetching role assignment for {storage.name}")
         out = []
-        for container in self._azurerm.containers(storage):
+        for container in self._azurerm.containers(storage.id):
             for role_assignment in self._azurerm.role_assignments(str(container)):
                 # one principal may be assigned multiple roles with overlapping dataActions, hence appearing
                 # here in duplicates. hence, role name -> permission level is not enough for the perfect scenario.
                 if role_assignment.role_name not in self._levels:
                     continue
                 privilege = self._levels[role_assignment.role_name].value
                 out.append(
@@ -92,59 +83,59 @@
             logger.warning(
                 "There are no external table present with azure storage account. "
                 "Please check if assessment job is run"
             )
             return None
         storage_account_infos = []
         for storage in self._azurerm.storage_accounts():
-            if storage.storage_account not in used_storage_accounts:
+            if storage.name not in used_storage_accounts:
                 continue
             for mapping in self._map_storage(storage):
                 storage_account_infos.append(mapping)
         if len(storage_account_infos) == 0:
             logger.error("No storage account found in current tenant with spn permission")
             return None
-        return self._installation.save(storage_account_infos, filename=self._filename)
+        return self._installation.save(storage_account_infos, filename=self.FILENAME)
 
     def _update_cluster_policy_definition(
         self,
         policy_definition: str,
-        storage_accounts: list[AzureResource],
+        storage_accounts: list[StorageAccount],
         uber_principal: PrincipalSecret,
         inventory_database: str,
     ) -> str:
         policy_dict = json.loads(policy_definition)
         tenant_id = self._azurerm.tenant_id()
         endpoint = f"https://login.microsoftonline.com/{tenant_id}/oauth2/token"
         for storage in storage_accounts:
-            policy_dict[
-                f"spark_conf.fs.azure.account.oauth2.client.id.{storage.storage_account}.dfs.core.windows.net"
-            ] = self._policy_config(uber_principal.client.client_id)
-            policy_dict[
-                f"spark_conf.fs.azure.account.oauth.provider.type.{storage.storage_account}.dfs.core.windows.net"
-            ] = self._policy_config("org.apache.hadoop.fs.azurebfs.oauth2.ClientCredsTokenProvider")
-            policy_dict[
-                f"spark_conf.fs.azure.account.oauth2.client.endpoint.{storage.storage_account}.dfs.core.windows.net"
-            ] = self._policy_config(endpoint)
-            policy_dict[f"spark_conf.fs.azure.account.auth.type.{storage.storage_account}.dfs.core.windows.net"] = (
+            policy_dict[f"spark_conf.fs.azure.account.oauth2.client.id.{storage.name}.dfs.core.windows.net"] = (
+                self._policy_config(uber_principal.client.client_id)
+            )
+            policy_dict[f"spark_conf.fs.azure.account.oauth.provider.type.{storage.name}.dfs.core.windows.net"] = (
+                self._policy_config("org.apache.hadoop.fs.azurebfs.oauth2.ClientCredsTokenProvider")
+            )
+            policy_dict[f"spark_conf.fs.azure.account.oauth2.client.endpoint.{storage.name}.dfs.core.windows.net"] = (
+                self._policy_config(endpoint)
+            )
+            policy_dict[f"spark_conf.fs.azure.account.auth.type.{storage.name}.dfs.core.windows.net"] = (
                 self._policy_config("OAuth")
             )
-            policy_dict[
-                f"spark_conf.fs.azure.account.oauth2.client.secret.{storage.storage_account}.dfs.core.windows.net"
-            ] = self._policy_config(f"{{secrets/{inventory_database}/uber_principal_secret}}")
+            policy_dict[f"spark_conf.fs.azure.account.oauth2.client.secret.{storage.name}.dfs.core.windows.net"] = (
+                self._policy_config(f"{{secrets/{inventory_database}/uber_principal_secret}}")
+            )
         return json.dumps(policy_dict)
 
     @staticmethod
     def _policy_config(value: str):
         return {"type": "fixed", "value": value}
 
     def _update_cluster_policy_with_spn(
         self,
         policy_id: str,
-        storage_accounts: list[AzureResource],
+        storage_accounts: list[StorageAccount],
         uber_principal: PrincipalSecret,
         inventory_database: str,
     ):
         try:
             policy_definition = ""
             cluster_policy = self._ws.cluster_policies.get(policy_id)
 
@@ -180,52 +171,95 @@
             logger.warning(
                 "There are no external table present with azure storage account. "
                 "Please check if assessment job is run"
             )
             return
         storage_account_info = []
         for storage in self._azurerm.storage_accounts():
-            if storage.storage_account in used_storage_accounts:
+            if storage.name in used_storage_accounts:
                 storage_account_info.append(storage)
         logger.info("Creating service principal")
         uber_principal = self._azurerm.create_service_principal(uber_principal_name)
         self._create_scope(uber_principal, inventory_database)
         config.uber_spn_id = uber_principal.client.client_id
         logger.info(
             f"Created service principal of client_id {config.uber_spn_id}. " f"Applying permission on storage accounts"
         )
         try:
-            self._apply_storage_permission(storage_account_info, uber_principal)
+            self._apply_storage_permission(
+                uber_principal.client.object_id, "STORAGE_BLOB_DATA_CONTRIBUTOR", *storage_account_info
+            )
             self._installation.save(config)
             self._update_cluster_policy_with_spn(policy_id, storage_account_info, uber_principal, inventory_database)
         except PermissionError:
             self._azurerm.delete_service_principal(uber_principal.client.object_id)
         logger.info(f"Update UCX cluster policy {policy_id} with spn connection details for storage accounts")
 
-    def _apply_storage_permission(self, storage_account_info: list[AzureResource], uber_principal: PrincipalSecret):
-        for storage in storage_account_info:
-            role_name = str(uuid.uuid4())
-            self._azurerm.apply_storage_permission(
-                uber_principal.client.object_id, storage, "STORAGE_BLOB_DATA_READER", role_name
-            )
-            logger.debug(
-                f"Storage Data Blob Reader permission applied for spn {uber_principal.client.client_id} "
-                f"to storage account {storage.storage_account}"
+    def _create_access_connector_for_storage_account(
+        self, storage_account: StorageAccount, role_name: str = "STORAGE_BLOB_DATA_READER"
+    ) -> AccessConnector:
+        access_connector = self._azurerm.create_or_update_access_connector(
+            storage_account.id.subscription_id,
+            storage_account.id.resource_group,
+            f"ac-{storage_account.name}",
+            storage_account.location,
+            tags={"CreatedBy": "ucx"},
+            wait_for_provisioning=True,
+        )
+        self._apply_storage_permission(access_connector.principal_id, role_name, storage_account)
+        return access_connector
+
+    def create_access_connectors_for_storage_accounts(self) -> list[AccessConnector]:
+        used_storage_accounts = self._get_storage_accounts()
+        if len(used_storage_accounts) == 0:
+            logger.warning(
+                "There are no external table present with azure storage account. "
+                "Please check if assessment job is run"
+            )
+            return []
+
+        tasks = []
+        for storage_account in self._azurerm.storage_accounts():
+            if storage_account.name not in used_storage_accounts:
+                continue
+            task = partial(
+                self._create_access_connector_for_storage_account,
+                storage_account=storage_account,
+                # Fine-grained access is configured within Databricks through unity
+                role_name="STORAGE_BLOB_DATA_CONTRIBUTOR",
             )
+            tasks.append(task)
+
+        thread_name = "Creating access connectors for storage accounts"
+        results, errors = Threads.gather(thread_name, tasks)
+        if len(errors) > 0:
+            raise ManyError(errors)
+        return list(results)
+
+    def _apply_storage_permission(
+        self,
+        principal_id: str,
+        role_name: str,
+        *storage_accounts: StorageAccount,
+    ):
+        for storage in storage_accounts:
+            role_guid = str(uuid.uuid4())
+            self._azurerm.apply_storage_permission(principal_id, storage, role_name, role_guid)
+            logger.debug(f"{role_name} permission applied for spn {principal_id} to storage account {storage.name}")
 
     def _create_scope(self, uber_principal: PrincipalSecret, inventory_database: str):
         logger.info(f"Creating secret scope {inventory_database}.")
         try:
             self._ws.secrets.create_scope(inventory_database)
         except ResourceAlreadyExists:
             logger.warning(f"Secret scope {inventory_database} already exists, using the same")
         self._ws.secrets.put_secret(inventory_database, "uber_principal_secret", string_value=uber_principal.secret)
 
     def load(self):
-        return self._installation.load(list[StoragePermissionMapping], filename=self._filename)
+        return self._installation.load(list[StoragePermissionMapping], filename=self.FILENAME)
 
     def _get_storage_accounts(self) -> list[str]:
         external_locations = self._locations.snapshot()
         storage_accounts = []
         for location in external_locations:
             if location.location.startswith("abfss://"):
                 start = location.location.index("@")
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/azure/credentials.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/credentials.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from dataclasses import dataclass
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.tui import Prompts
-from databricks.labs.lsql.backends import StatementExecutionBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors.platform import InvalidParameterValue
 from databricks.sdk.service.catalog import (
     AzureServicePrincipal,
     Privilege,
     StorageCredentialInfo,
     ValidationResultResult,
@@ -15,17 +14,14 @@
 
 from databricks.labs.ucx.assessment.azure import AzureServicePrincipalCrawler
 from databricks.labs.ucx.assessment.secrets import SecretsMixin
 from databricks.labs.ucx.azure.access import (
     AzureResourcePermissions,
     StoragePermissionMapping,
 )
-from databricks.labs.ucx.azure.resources import AzureAPIClient, AzureResources
-from databricks.labs.ucx.config import WorkspaceConfig
-from databricks.labs.ucx.hive_metastore.locations import ExternalLocations
 
 logger = logging.getLogger(__name__)
 
 
 # A dataclass to host service_principal info and its client_secret info
 @dataclass
 class ServicePrincipalMigrationInfo:
@@ -156,40 +152,14 @@
         self._output_file = "azure_service_principal_migration_result.csv"
         self._installation = installation
         self._ws = ws
         self._resource_permissions = resource_permissions
         self._sp_crawler = service_principal_crawler
         self._storage_credential_manager = storage_credential_manager
 
-    @classmethod
-    def for_cli(cls, ws: WorkspaceClient, installation: Installation, prompts: Prompts):
-        msg = (
-            "Have you reviewed the azure_storage_account_info.csv "
-            "and confirm listed service principals are allowed to be checked for migration?"
-        )
-        if not prompts.confirm(msg):
-            raise SystemExit()
-
-        config = installation.load(WorkspaceConfig)
-        sql_backend = StatementExecutionBackend(ws, config.warehouse_id)
-        azure_mgmt_client = AzureAPIClient(
-            ws.config.arm_environment.resource_manager_endpoint,
-            ws.config.arm_environment.service_management_endpoint,
-        )
-        graph_client = AzureAPIClient("https://graph.microsoft.com", "https://graph.microsoft.com")
-        azurerm = AzureResources(azure_mgmt_client, graph_client)
-        locations = ExternalLocations(ws, sql_backend, config.inventory_database)
-
-        resource_permissions = AzureResourcePermissions(installation, ws, azurerm, locations)
-        sp_crawler = AzureServicePrincipalCrawler(ws, sql_backend, config.inventory_database)
-
-        storage_credential_manager = StorageCredentialManager(ws)
-
-        return cls(installation, ws, resource_permissions, sp_crawler, storage_credential_manager)
-
     def _fetch_client_secret(self, sp_list: list[StoragePermissionMapping]) -> list[ServicePrincipalMigrationInfo]:
         # check AzureServicePrincipalInfo from AzureServicePrincipalCrawler, if AzureServicePrincipalInfo
         # has secret_scope and secret_key not empty, fetch the client_secret and put it to the client_secret field
         #
         # The input StoragePermissionMapping may have managed identity mixed in, we will ignore them for now, as
         # they won't have any client_secret, we will process managed identity in the future.
 
@@ -253,31 +223,52 @@
         self._print_action_plan(sp_candidates)
 
         return sp_list_with_secret
 
     def save(self, migration_results: list[StorageCredentialValidationResult]) -> str:
         return self._installation.save(migration_results, filename=self._output_file)
 
-    def run(self, prompts: Prompts, include_names: set[str] | None = None) -> list[StorageCredentialValidationResult]:
-
+    def _migrate_service_principals(
+        self, include_names: set[str] | None = None
+    ) -> list[StorageCredentialValidationResult]:
         sp_list_with_secret = self._generate_migration_list(include_names)
 
-        plan_confirmed = prompts.confirm(
-            "Above Azure Service Principals will be migrated to UC storage credentials, please review and confirm."
-        )
-        if plan_confirmed is not True:
-            return []
-
         execution_result = []
         for spn in sp_list_with_secret:
             self._storage_credential_manager.create_with_client_secret(spn)
             execution_result.append(self._storage_credential_manager.validate(spn.permission_mapping))
+        return execution_result
+
+    def _create_access_connectors_for_storage_accounts(self) -> list[StorageCredentialValidationResult]:
+        self._resource_permissions.create_access_connectors_for_storage_accounts()
+        return []
+
+    def run(self, prompts: Prompts, include_names: set[str] | None = None) -> list[StorageCredentialValidationResult]:
+        plan_confirmed = prompts.confirm(
+            "Above Azure Service Principals will be migrated to UC storage credentials, please review and confirm."
+        )
+        if plan_confirmed:
+            sp_results = self._migrate_service_principals(include_names)
+        else:
+            sp_results = []
+
+        plan_confirmed = prompts.confirm("Please confirm to create an access connector for each storage account.")
+        if plan_confirmed:
+            ac_results = self._create_access_connectors_for_storage_accounts()
+        else:
+            ac_results = []
 
-        if execution_result:
-            results_file = self.save(execution_result)
+        execution_results = sp_results + ac_results
+        if execution_results:
+            results_file = self.save(execution_results)
             logger.info(
-                f"Completed migration from Azure Service Principal to UC Storage credentials"
+                "Completed migration from Azure Service Principal to UC Storage credentials "
+                "and creation of Databricks Access Connectors for storage accounts "
                 f"Please check {results_file} for validation results"
             )
         else:
-            logger.info("No Azure Service Principal migrated to UC Storage credentials")
-        return execution_result
+            logger.info(
+                "No Azure Service Principal migrated to UC Storage credentials "
+                "nor Databricks Access Connectors created for storage accounts"
+            )
+
+        return execution_results
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/azure/locations.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/locations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import logging
 from urllib.parse import urlparse
 
-from databricks.labs.blueprint.installation import Installation
-from databricks.labs.lsql.backends import StatementExecutionBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors.platform import InvalidParameterValue, PermissionDenied
 
 from databricks.labs.ucx.azure.access import AzureResourcePermissions
-from databricks.labs.ucx.azure.resources import AzureAPIClient, AzureResources
-from databricks.labs.ucx.config import WorkspaceConfig
+from databricks.labs.ucx.azure.resources import AzureResources
 from databricks.labs.ucx.hive_metastore import ExternalLocations
 
 logger = logging.getLogger(__name__)
 
 
 class ExternalLocationsMigration:
     def __init__(
@@ -23,31 +20,14 @@
         azurerm: AzureResources,
     ):
         self._ws = ws
         self._hms_locations = hms_locations
         self._resource_permissions = resource_permissions
         self._azurerm = azurerm
 
-    @classmethod
-    def for_cli(cls, ws: WorkspaceClient, installation: Installation):
-        config = installation.load(WorkspaceConfig)
-        sql_backend = StatementExecutionBackend(ws, config.warehouse_id)
-        hms_locations = ExternalLocations(ws, sql_backend, config.inventory_database)
-
-        azure_mgmt_client = AzureAPIClient(
-            ws.config.arm_environment.resource_manager_endpoint,
-            ws.config.arm_environment.service_management_endpoint,
-        )
-        graph_client = AzureAPIClient("https://graph.microsoft.com", "https://graph.microsoft.com")
-        azurerm = AzureResources(azure_mgmt_client, graph_client)
-
-        resource_permissions = AzureResourcePermissions(installation, ws, azurerm, hms_locations)
-
-        return cls(ws, hms_locations, resource_permissions, azurerm)
-
     def _app_id_credential_name_mapping(self) -> tuple[dict[str, str], dict[str, str]]:
         # list all storage credentials.
         # generate the managed identity/service principal application id to credential name mapping.
         # return one mapping for all non read-only credentials and one mapping for all read-only credentials
         # TODO: considering put this logic into the StorageCredentialManager
         app_id_mapping_write = {}
         app_id_mapping_read = {}
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/azure/resources.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/azure/resources.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+import urllib.parse
+import time
 from collections.abc import Iterable
-from dataclasses import dataclass
+from dataclasses import dataclass, field
+from typing import Any
 
 from databricks.sdk.core import (
     ApiClient,
     AzureCliTokenSource,
     Config,
     credentials_provider,
 )
 from databricks.sdk.errors import NotFound, PermissionDenied, ResourceConflict
 
 from databricks.labs.ucx.assessment.crawlers import logger
 
 # https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles
-_ROLES = {"STORAGE_BLOB_DATA_READER": "2a2b9908-6ea1-4ae2-8e65-a410df84e7d1"}
+_ROLES = {
+    "STORAGE_BLOB_DATA_READER": "2a2b9908-6ea1-4ae2-8e65-a410df84e7d1",
+    "STORAGE_BLOB_DATA_CONTRIBUTOR": "ba92f5b4-2d11-453d-a403-e96b0029c9fe",
+}
 
 
 @dataclass
 class AzureSubscription:
     name: str
     subscription_id: str
     tenant_id: str
@@ -49,55 +55,160 @@
     def storage_account(self):
         return self._pairs.get("storageAccounts")
 
     @property
     def container(self):
         return self._pairs.get("containers")
 
+    @property
+    def access_connector(self):
+        return self._pairs.get("accessConnectors")
+
     def __eq__(self, other):
         if not isinstance(other, AzureResource):
             return NotImplemented
         return self._resource_id == other._resource_id
 
     def __repr__(self):
-        properties = ["subscription_id", "resource_group", "storage_account", "container"]
+        properties = ["subscription_id", "resource_group", "storage_account", "container", "access_connector"]
         pairs = [f"{_}={getattr(self, _)}" for _ in properties]
         return f'AzureResource<{", ".join(pairs)}>'
 
     def __str__(self):
         return self._resource_id
 
 
+class RawResource:
+    def __init__(self, raw_resource: dict[str, Any]):
+        if "id" not in raw_resource:
+            raise KeyError("Raw resource must contain an 'id' field")
+        self._id = AzureResource(raw_resource["id"])
+        self._raw_resource = raw_resource
+
+    @property
+    def id(self) -> AzureResource:
+        return self._id
+
+    def get(self, key: str, default: Any) -> Any:
+        return self._raw_resource.get(key, default)
+
+
 @dataclass
 class Principal:
     client_id: str
     display_name: str
     object_id: str
     # service principal will have type: "Application"
     # managed identity will have type: "ManagedIdentity"
     type: str
     # Need this directory_id/tenant_id when create UC storage credentials using service principal
     # it will be None if type is managed identity
     directory_id: str | None = None
 
 
 @dataclass
+class StorageAccount:
+    id: AzureResource
+    name: str
+    location: str
+
+    @classmethod
+    def from_raw_resource(cls, raw: RawResource) -> "StorageAccount":
+        if raw.id is None:
+            raise KeyError(f"Missing id: {raw}")
+
+        name = raw.get("name", "")
+        if name == "":
+            raise KeyError(f"Missing name: {raw}")
+
+        location = raw.get("location", "")
+        if location == "":
+            raise KeyError(f"Missing location: {raw}")
+
+        storage_account = cls(id=raw.id, name=name, location=location)
+        return storage_account
+
+
+@dataclass
 class PrincipalSecret:
     client: Principal
     secret: str
 
 
 @dataclass
 class AzureRoleAssignment:
     resource: AzureResource
     scope: AzureResource
     principal: Principal
     role_name: str
 
 
+@dataclass
+class AccessConnector:
+    id: AzureResource
+    name: str
+    location: str
+    provisioning_state: str  # https://learn.microsoft.com/en-us/rest/api/databricks/access-connectors/get?view=rest-databricks-2023-05-01&tabs=HTTP#provisioningstate
+    identity_type: str  # SystemAssigned or UserAssigned
+    principal_id: str
+    managed_identity_type: str | None = None  # str when identity_type is UserAssigned
+    client_id: str | None = None  # str when identity_type is UserAssigned
+    tenant_id: str | None = None  # str when identity_type is SystemAssigned
+    tags: dict[str, str] = field(default_factory=dict)
+
+    @classmethod
+    def from_raw_resource(cls, raw: RawResource) -> "AccessConnector":
+        if raw.id is None:
+            raise KeyError(f"Missing id: {raw}")
+
+        name = raw.get("name", "")
+        if name == "":
+            raise KeyError(f"Missing name: {raw}")
+
+        location = raw.get("location", "")
+        if location == "":
+            raise KeyError(f"Missing location: {raw}")
+
+        provisioning_state = raw.get("properties", {}).get("provisioningState", "")
+        if provisioning_state == "":
+            raise KeyError(f"Missing provisioning state: {raw}")
+
+        identity = raw.get("identity", {})
+        identity_type = identity.get("type")
+        if identity_type == "UserAssigned":
+            if len(identity.keys()) > 1:
+                raise KeyError(f"Multiple user assigned identities: {identity.keys()}")
+            if len(identity.keys()) == 0:
+                raise KeyError(f"No user assigned identity: {identity.keys()}")
+            managed_identity_id = list(identity.keys())[0]
+            principal_id = identity[managed_identity_id]["principalId"]
+            client_id = identity[managed_identity_id]["clientId"]
+            tenant_id = None
+        elif identity_type == "SystemAssigned":
+            principal_id = identity["principalId"]
+            managed_identity_id = client_id = None
+            tenant_id = identity["tenantId"]
+        else:
+            raise KeyError(f"Unsupported identity type: {identity_type}")
+
+        access_connector = cls(
+            id=raw.id,
+            name=name,
+            location=location,
+            provisioning_state=provisioning_state,
+            identity_type=identity_type,
+            principal_id=principal_id,
+            managed_identity_type=managed_identity_id,
+            client_id=client_id,
+            tenant_id=tenant_id,
+            tags=raw.get("tags", {}),
+        )
+        return access_connector
+
+
 class AzureAPIClient:
     def __init__(self, host_endpoint: str, service_endpoint: str):
         self.api_client = ApiClient(
             Config(
                 host=host_endpoint,
                 credentials_provider=self._provider_for(service_endpoint),
             )
@@ -113,41 +224,43 @@
                 token = token_source.token()
                 return {"Authorization": f"{token.token_type} {token.access_token}"}
 
             return inner
 
         return _credentials
 
-    def get(self, path: str, api_version: str | None = None):
+    def get(self, path: str, api_version: str | None = None, query: dict[str, str] | None = None):
         headers = {"Accept": "application/json"}
-        query = {}
+        _query: dict[str, str] = query or {}
         if api_version is not None:
-            query = {"api-version": api_version}
-        return self.api_client.do("GET", path, query, headers)
+            _query["api-version"] = api_version
+        return self.api_client.do("GET", path, _query, headers)
 
     def put(self, path: str, api_version: str | None = None, body: dict | None = None):
         headers = {"Content-Type": "application/json"}
         query: dict[str, str] = {}
         if api_version is not None:
-            query = {"api-version": api_version}
+            query["api-version"] = api_version
         if body is not None:
             return self.api_client.do("PUT", path, query, headers, body)
         return None
 
     def post(self, path: str, body: dict | None = None):
         headers = {"Content-Type": "application/json"}
         query: dict[str, str] = {}
         if body is not None:
             return self.api_client.do("POST", path, query, headers, body)
         return self.api_client.do("POST", path, query, headers)
 
-    def delete(self, path: str):
+    def delete(self, path: str, api_version: str | None = None):
         # this method is added only to be used in int test to delete the application once tests pass
         headers = {"Content-Type": "application/json"}
         query: dict[str, str] = {}
+        if api_version is not None:
+            query["api-version"] = api_version
         return self.api_client.do("DELETE", path, query, headers)
 
     def token(self):
         return self._token_source.token()
 
 
 class AzureResources:
@@ -200,32 +313,32 @@
         try:
             self._graph.delete(f"/v1.0/applications(appId='{principal_id}')")
         except PermissionDenied:
             msg = f"User doesnt have permission to delete application {principal_id}"
             logger.error(msg)
             raise PermissionDenied(msg) from None
 
-    def apply_storage_permission(self, principal_id: str, resource: AzureResource, role_name: str, role_guid: str):
+    def apply_storage_permission(
+        self, principal_id: str, storage_account: StorageAccount, role_name: str, role_guid: str
+    ):
         try:
             role_id = _ROLES[role_name]
-            path = f"{str(resource)}/providers/Microsoft.Authorization/roleAssignments/{role_guid}"
-            role_definition_id = (
-                f"/subscriptions/{resource.subscription_id}/providers/Microsoft.Authorization/roleDefinitions/{role_id}"
-            )
+            path = f"{storage_account.id}/providers/Microsoft.Authorization/roleAssignments/{role_guid}"
+            role_definition_id = f"/subscriptions/{storage_account.id.subscription_id}/providers/Microsoft.Authorization/roleDefinitions/{role_id}"
             body = {
                 "properties": {
                     "roleDefinitionId": role_definition_id,
                     "principalId": principal_id,
                     "principalType": "ServicePrincipal",
                 }
             }
             self._mgmt.put(path, "2022-04-01", body)
         except ResourceConflict:
             logger.warning(
-                f"Role assignment already exists for role {role_guid} on storage {resource.storage_account}"
+                f"Role assignment already exists for role {role_guid} on storage {storage_account.name}"
                 f" for spn {principal_id}."
             )
         except PermissionDenied:
             msg = (
                 "Permission denied. Please run this cmd under the identity of a user who has "
                 "create service principal permission."
             )
@@ -241,23 +354,25 @@
         for subscription in self._get_subscriptions():
             if subscription.tenant_id != tenant_id:
                 continue
             if subscription.subscription_id not in self._include_subscriptions:
                 continue
             yield subscription
 
-    def storage_accounts(self) -> Iterable[AzureResource]:
+    def storage_accounts(self) -> Iterable[StorageAccount]:
         for subscription in self.subscriptions():
             logger.info(f"Checking in subscription {subscription.name} for storage accounts")
             path = f"/subscriptions/{subscription.subscription_id}/providers/Microsoft.Storage/storageAccounts"
-            for storage in self._mgmt.get(path, "2023-01-01").get("value", []):
-                resource_id = storage.get("id")
-                if not resource_id:
-                    continue
-                yield AzureResource(resource_id)
+            for response in self._mgmt.get(path, "2023-01-01").get("value", []):
+                try:
+                    storage_account = StorageAccount.from_raw_resource(RawResource(response))
+                except KeyError:
+                    logger.warning(f"Failed parsing storage account: {response}")
+                else:
+                    yield storage_account
 
     def containers(self, storage: AzureResource):
         for raw in self._mgmt.get(f"{storage}/blobServices/default/containers", "2023-01-01").get("value", []):
             resource_id = raw.get("id")
             if not resource_id:
                 continue
             yield AzureResource(resource_id)
@@ -370,7 +485,100 @@
             # SystemAssigned managed identity does not have client_id in get access connector response
             # need to call graph api directoryObjects to fetch the client_id
             principal = self._get_principal(identity.get("principalId"))
             if not principal:
                 return None
             return principal.client_id
         return None
+
+    def get_access_connector(self, subscription_id: str, resource_group_name: str, name: str) -> AccessConnector | None:
+        """Get an access connector.
+
+        Docs:
+            https://learn.microsoft.com/en-us/rest/api/databricks/access-connectors/get?view=rest-databricks-2023-05-01&tabs=HTTP
+        """
+        url = f"/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Databricks/accessConnectors/{name}"
+        response = self._mgmt.get(url, api_version="2023-05-01")
+        raw = RawResource(response)
+        try:
+            access_connector = AccessConnector.from_raw_resource(raw)
+        except KeyError:
+            logger.warning(f"Tried getting non-existing access connector: {url}")
+            access_connector = None
+        return access_connector
+
+    def list_resources(self, subscription: AzureSubscription, resource_type: str) -> Iterable[RawResource]:
+        """List all resources of a type within subscription"""
+        query = {"api-version": "2020-06-01", "$filter": f"resourceType eq '{resource_type}'"}
+        while True:
+            res = self._mgmt.get(f"/subscriptions/{subscription.subscription_id}/resources", query=query)
+            for resource in res["value"]:
+                try:
+                    yield RawResource(resource)
+                except KeyError:
+                    logger.warning(f"Could not parse resource: {resource}")
+
+            next_link = res.get("nextLink", None)
+            if not next_link:
+                break
+            parsed_link = urllib.parse.urlparse(next_link)
+            query = dict(urllib.parse.parse_qsl(parsed_link.query))
+
+    def access_connectors(self) -> Iterable[AccessConnector]:
+        """List all access connector within subscription
+
+        Docs:
+            https://learn.microsoft.com/en-us/rest/api/databricks/access-connectors/list-by-subscription?view=rest-databricks-2023-05-01&tabs=HTTP
+        """
+        for subscription in self.subscriptions():
+            for raw in self.list_resources(subscription, "Microsoft.Databricks/accessConnectors"):
+                try:
+                    yield AccessConnector.from_raw_resource(raw)
+                except KeyError:
+                    logger.warning(f"Could not parse access connector: {raw}")
+
+    def create_or_update_access_connector(
+        self,
+        subscription_id: str,
+        resource_group_name: str,
+        name: str,
+        location: str,
+        tags: dict[str, str] | None,
+        *,
+        wait_for_provisioning: bool = False,
+        wait_for_provisioning_timeout_in_seconds: int = 300,
+    ) -> AccessConnector:
+        """Create access connector.
+
+        Docs:
+            https://learn.microsoft.com/en-us/rest/api/databricks/access-connectors/create-or-update?view=rest-databricks-2023-05-01&tabs=HTTP
+        """
+        url = f"/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Databricks/accessConnectors/{name}"
+        body = {
+            "location": location,
+            "identity": {"type": "SystemAssigned"},
+        }
+        if tags is not None:
+            body["tags"] = tags
+        self._mgmt.put(url, api_version="2023-05-01", body=body)
+
+        access_connector = self.get_access_connector(subscription_id, resource_group_name, name)
+
+        start_time = time.time()
+        if access_connector is None or (wait_for_provisioning and access_connector.provisioning_state != "Succeeded"):
+            if time.time() - start_time > wait_for_provisioning_timeout_in_seconds:
+                raise TimeoutError(f"Timeout waiting for creating or updating access connector: {url}")
+            time.sleep(5)
+
+            access_connector = self.get_access_connector(subscription_id, resource_group_name, name)
+            assert access_connector is not None
+
+        return access_connector
+
+    def delete_access_connector(self, subscription_id: str, resource_group_name: str, name: str) -> None:
+        """Delete an access connector.
+
+        Docs:
+            https://learn.microsoft.com/en-us/rest/api/databricks/access-connectors/delete?view=rest-databricks-2023-05-01&tabs=HTTP
+        """
+        url = f"/subscriptions/{subscription_id}/resourceGroups/{resource_group_name}/providers/Microsoft.Databricks/accessConnectors/{name}"
+        self._mgmt.delete(url, api_version="2023-05-01")
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/framework/crawlers.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/crawlers.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/framework/dashboards.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/dashboards.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,16 +223,16 @@
             dashboard = self._ws.dashboards.get(self._state.dashboards[dashboard_ref])
             assert dashboard.widgets is not None
             for widget in dashboard.widgets:
                 assert widget.id is not None
                 try:
                     self._ws.dashboard_widgets.delete(widget.id)
                 except TypeError:
-                    logger.warning("Type error in SDK API response, ES-1061370")
-                    # Tracking bug in ES-1061370
+                    pass
+                    # TODO: Tracking bug in ES-1061370. Remove after fix
             return
         dashboard = self._ws.dashboards.create(dashboard_name, run_as_role=RunAsRole.VIEWER, parent=parent_folder_id)
         assert dashboard.id is not None
         self._ws.dbsql_permissions.set(
             ObjectTypePlural.DASHBOARDS,
             dashboard.id,
             access_control_list=[AccessControl(group_name="users", permission_level=PermissionLevel.CAN_VIEW)],
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/framework/utils.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/framework/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/catalog_schema.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/catalog_schema.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,86 @@
 import logging
 from pathlib import PurePath
+import dataclasses
 
-from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.tui import Prompts
-from databricks.labs.lsql.backends import StatementExecutionBackend
+from databricks.labs.lsql.backends import SqlBackend
+from databricks.labs.ucx.hive_metastore.grants import PrincipalACL, Grant
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound
 
-from databricks.labs.ucx.config import WorkspaceConfig
 from databricks.labs.ucx.hive_metastore.mapping import TableMapping
 
 logger = logging.getLogger(__name__)
 
 
 class CatalogSchema:
-    def __init__(self, ws: WorkspaceClient, table_mapping: TableMapping):
+    def __init__(
+        self, ws: WorkspaceClient, table_mapping: TableMapping, principal_grants: PrincipalACL, sql_backend: SqlBackend
+    ):
         self._ws = ws
         self._table_mapping = table_mapping
         self._external_locations = self._ws.external_locations.list()
-
-    @classmethod
-    def for_cli(cls, ws: WorkspaceClient, installation: Installation):
-        config = installation.load(WorkspaceConfig)
-        sql_backend = StatementExecutionBackend(ws, config.warehouse_id)
-        table_mapping = TableMapping(installation, ws, sql_backend)
-        return cls(ws, table_mapping)
+        self._principal_grants = principal_grants
+        self._backend = sql_backend
 
     def create_all_catalogs_schemas(self, prompts: Prompts):
         candidate_catalogs, candidate_schemas = self._get_missing_catalogs_schemas()
         for candidate_catalog in candidate_catalogs:
             self._create_catalog_validate(candidate_catalog, prompts)
         for candidate_catalog, schemas in candidate_schemas.items():
             for candidate_schema in schemas:
                 self._create_schema(candidate_catalog, candidate_schema)
+        self._update_principal_acl()
+
+    def _update_principal_acl(self):
+        grants = self._get_catalog_schema_grants()
+        for grant in grants:
+            acl_migrate_sql = grant.uc_grant_sql()
+            if acl_migrate_sql is None:
+                logger.warning(f"Cannot identify UC grant for {grant.this_type_and_key()}. Skipping.")
+                continue
+            logger.debug(f"Migrating acls on {grant.this_type_and_key()} using SQL query: {acl_migrate_sql}")
+            self._backend.execute(acl_migrate_sql)
+
+    def _get_catalog_schema_grants(self):
+        catalog_grants: set[Grant] = set()
+        new_grants = []
+        src_trg_schema_mapping = self._get_database_source_target_mapping()
+        grants = self._principal_grants.get_interactive_cluster_grants()
+        # filter on grants to only get database level grants
+        database_grants = [grant for grant in grants if grant.table is None and grant.view is None]
+        for db_grant in database_grants:
+            new_grants.append(
+                dataclasses.replace(
+                    db_grant,
+                    # replace source database with taget UC database
+                    database=src_trg_schema_mapping[db_grant.database]['target_schema'],
+                    # replace hive_metastore with target UC catalog
+                    catalog=src_trg_schema_mapping[db_grant.database]['target_catalog'],
+                )
+            )
+        for grant in new_grants:
+            catalog_grants.add(dataclasses.replace(grant, database=None))
+        new_grants.extend(catalog_grants)
+        return new_grants
+
+    def _get_database_source_target_mapping(self) -> dict[str, dict]:
+        """generate a dictionary of source database in hive_metastore and its
+        mapping of target UC catalog and schema from the table mappings."""
+        src_trg_schema_mapping: dict[str, dict] = {}
+        table_mappings = self._table_mapping.load()
+        for mappings in table_mappings:
+            if mappings.src_schema not in src_trg_schema_mapping:
+                src_trg_schema_mapping[mappings.src_schema] = {
+                    'target_catalog': mappings.catalog_name,
+                    'target_schema': mappings.dst_schema,
+                }
+                continue
+        return src_trg_schema_mapping
 
     def _create_catalog_validate(self, catalog, prompts: Prompts):
         logger.info(f"Creating UC catalog: {catalog}")
         # create catalogs
         attempts = 3
         while True:
             catalog_storage = prompts.question(
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/locations.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/locations.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.lsql import Row
 from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound
 from databricks.sdk.service.catalog import ExternalLocationInfo
-
+from databricks.sdk.dbutils import FileInfo
 from databricks.labs.ucx.framework.crawlers import CrawlerBase, Result, ResultFn
 from databricks.labs.ucx.framework.utils import escape_sql_identifier
 from databricks.labs.ucx.hive_metastore.tables import Table
 
 logger = logging.getLogger(__name__)
 
 
@@ -31,38 +31,39 @@
     name: str
     source: str
 
 
 class ExternalLocations(CrawlerBase[ExternalLocation]):
     _prefix_size: ClassVar[list[int]] = [1, 12]
 
-    def __init__(self, ws: WorkspaceClient, sbe: SqlBackend, schema):
+    def __init__(self, ws: WorkspaceClient, sbe: SqlBackend, schema: str):
         super().__init__(sbe, "hive_metastore", schema, "external_locations", ExternalLocation)
         self._ws = ws
 
     def _external_locations(self, tables: list[Row], mounts) -> Iterable[ExternalLocation]:
         min_slash = 2
         external_locations: list[ExternalLocation] = []
         for table in tables:
             location = table.location
             if not location:
                 continue
             if location.startswith("dbfs:/mnt"):
-                location = self._resolve_mount(location, mounts)
+                location = self.resolve_mount(location, mounts)
             if (
                 not location.startswith("dbfs")
                 and (self._prefix_size[0] < location.find(":/") < self._prefix_size[1])
                 and not location.startswith("jdbc")
             ):
                 self._dbfs_locations(external_locations, location, min_slash)
             if location.startswith("jdbc"):
                 self._add_jdbc_location(external_locations, location, table)
         return external_locations
 
-    def _resolve_mount(self, location, mounts):
+    @staticmethod
+    def resolve_mount(location, mounts):
         for mount in mounts:
             if location[5:].startswith(mount.name.lower()):
                 location = location[5:].replace(mount.name, mount.source)
                 break
         return location
 
     @staticmethod
@@ -85,27 +86,26 @@
             external_locations.append(ExternalLocation(os.path.dirname(location) + "/", 1))
 
     def _add_jdbc_location(self, external_locations, location, table):
         dupe = False
         pattern = r"(\w+)=(.*?)(?=\s*,|\s*\])"
         # Find all matches in the input string
         # Storage properties is of the format
-        # "[personalAccessToken=*********(redacted), \
-        #  httpPath=/sql/1.0/warehouses/65b52fb5bd86a7be, host=dbc-test1-aa11.cloud.databricks.com, \
-        #  dbtable=samples.nyctaxi.trips]"
+        # "personalAccessToken=*********(redacted),
+        #  httpPath=/sql/1.0/warehouses/65b52fb5bd86a7be, host=dbc-test1-aa11.cloud.databricks.com,
+        #  dbtable=samples.nyctaxi.trips"
         matches = re.findall(pattern, table.storage_properties)
         # Create a dictionary from the matches
         result_dict = dict(matches)
         # Fetch the value of host from the newly created dict
         host = result_dict.get("host", "")
         port = result_dict.get("port", "")
         database = result_dict.get("database", "")
         httppath = result_dict.get("httpPath", "")
         provider = result_dict.get("provider", "")
-        # dbtable = result_dict.get("dbtable", "")
         # currently supporting databricks and mysql external tables
         # add other jdbc types
         if "databricks" in location.lower():
             jdbc_location = f"jdbc:databricks://{host};httpPath={httppath}"
         elif "mysql" in location.lower():
             jdbc_location = f"jdbc:mysql://{host}:{port}/{database}"
         elif not provider == "":
@@ -256,28 +256,32 @@
 @dataclass
 class TableInMount:
     format: str
     is_partitioned: bool
 
 
 class TablesInMounts(CrawlerBase[Table]):
+    TABLE_IN_MOUNT_DB = "mounted_"
 
     def __init__(
         self,
         backend: SqlBackend,
         ws: WorkspaceClient,
         inventory_database: str,
         mc: Mounts,
         include_mounts: list[str] | None = None,
         exclude_paths_in_mount: list[str] | None = None,
+        include_paths_in_mount: list[str] | None = None,
     ):
         super().__init__(backend, "hive_metastore", inventory_database, "tables", Table)
         self._dbutils = ws.dbutils
-        self._mc = mc
+        self._mounts_crawler = mc
         self._include_mounts = include_mounts
+        self._ws = ws
+        self._include_paths_in_mount = include_paths_in_mount
 
         irrelevant_patterns = {'_SUCCESS', '_committed_', '_started_'}
         if exclude_paths_in_mount:
             irrelevant_patterns.update(exclude_paths_in_mount)
         self._fiter_paths = irrelevant_patterns
 
     def snapshot(self) -> list[Table]:
@@ -300,82 +304,118 @@
     def _append_records(self, items: Sequence[Table]):
         logger.debug(f"[{self.full_name}] found {len(items)} new records for {self._table}")
         self._backend.save_table(self.full_name, items, Table, mode="overwrite")
 
     def _try_load(self) -> Iterable[Table]:
         """Tries to load table information from the database or throws TABLE_OR_VIEW_NOT_FOUND error"""
         for row in self._fetch(
-            f"SELECT * FROM {escape_sql_identifier(self.full_name)} WHERE NOT STARTSWITH(database, 'mounted_')"
+            f"SELECT * FROM {escape_sql_identifier(self.full_name)} WHERE NOT STARTSWITH(database, '{self.TABLE_IN_MOUNT_DB}')"
         ):
             yield Table(*row)
 
     def _crawl(self):
-        all_mounts = self._mc.snapshot()
+        all_mounts = self._mounts_crawler.snapshot()
         all_tables = []
         for mount in all_mounts:
             if self._include_mounts and mount.name not in self._include_mounts:
                 logger.info(f"Filtering mount {mount.name}")
                 continue
-            table_paths = self._find_delta_log_folders(mount.name)
-            logger.info(f"Found {len(table_paths)} in mount {mount.name}")
+            table_paths = {}
+            if self._include_paths_in_mount:
+                for path in self._include_paths_in_mount:
+                    table_paths.update(self._find_delta_log_folders(path))
+            else:
+                table_paths = self._find_delta_log_folders(mount.name)
+
             for path, entry in table_paths.items():
                 guess_table = os.path.basename(path)
                 table = Table(
                     catalog="hive_metastore",
-                    database=f"mounted_{mount.name.replace('/mnt/', '').replace('/', '_')}",
+                    database=f"{self.TABLE_IN_MOUNT_DB}{mount.name.replace('/mnt/', '').replace('/', '_')}",
                     name=guess_table,
                     object_type="EXTERNAL",
                     table_format=entry.format,
                     location=path.replace(f"dbfs:{mount.name}/", mount.source),
                     is_partitioned=entry.is_partitioned,
                 )
                 all_tables.append(table)
         return all_tables
 
-    def _find_delta_log_folders(self, root_dir, delta_log_folders=None) -> dict:
+    def _find_delta_log_folders(self, root_dir: str, delta_log_folders=None) -> dict:
         if delta_log_folders is None:
             delta_log_folders = {}
         logger.info(f"Listing {root_dir}")
         file_infos = self._dbutils.fs.ls(root_dir)
         for file_info in file_infos:
             if self._is_irrelevant(file_info.name) or file_info.path == root_dir:
                 logger.debug(f"Path {file_info.path} is irrelevant")
                 continue
 
             root_path = os.path.dirname(root_dir)
-            if self._path_is_delta(delta_log_folders, root_path):
-                if self._is_partitioned(file_info.name):
-                    logger.debug(f"Found partitioned delta {root_path}")
-                    delta_log_folders[root_path] = TableInMount(format="DELTA", is_partitioned=True)
-                    continue
-                logger.debug(f"Path {file_info.path} was identified as Delta, skipping")
+            previous_entry = delta_log_folders.get(root_path)
+            if previous_entry:
+                # Happens when first folder was _delta_log and next folders are partitioned folder
+                if (
+                    previous_entry.format == "DELTA"
+                    and self._is_partitioned(file_info.name)
+                    and not previous_entry.is_partitioned
+                ):
+                    delta_log_folders[root_path] = TableInMount(format=previous_entry.format, is_partitioned=True)
                 continue
 
-            if file_info.name == "_delta_log/":
-                logger.debug(f"Found delta table {root_path}")
-                if delta_log_folders.get(root_path) and delta_log_folders.get(root_path).is_partitioned:
-                    delta_log_folders[root_path] = TableInMount(format="DELTA", is_partitioned=True)
-                else:
-                    delta_log_folders[root_path] = TableInMount(format="DELTA", is_partitioned=False)
-            elif self._is_partitioned(file_info.name):
-                logger.debug(f"Found partitioned parquet {file_info.path}")
-                delta_log_folders[root_path] = TableInMount(format="PARQUET", is_partitioned=True)
-            elif self._is_parquet(file_info.name):
-                logger.debug(f"Found parquet {file_info.path}")
-                delta_log_folders[root_path] = TableInMount(format="PARQUET", is_partitioned=False)
+            if self._is_partitioned(file_info.name):
+                table_in_mount = self._find_partition_file_format(file_info.path)
+                if table_in_mount:
+                    delta_log_folders[root_path] = table_in_mount
+                continue
+
+            table_in_mount = self._assess_path(file_info)
+            if table_in_mount:
+                delta_log_folders[root_path] = table_in_mount
             else:
                 self._find_delta_log_folders(file_info.path, delta_log_folders)
 
         return delta_log_folders
 
-    def _path_is_delta(self, delta_log_folders, path: str) -> bool:
-        return delta_log_folders.get(path) and delta_log_folders.get(path).format == "DELTA"
+    def _find_partition_file_format(self, root_dir: str) -> TableInMount | None:
+        logger.info(f"Listing {root_dir}")
+        file_infos = self._dbutils.fs.ls(root_dir)
+        for file_info in file_infos:
+            path_extension = self._assess_path(file_info)
+            if path_extension:
+                return TableInMount(format=path_extension.format, is_partitioned=True)
+            if self._is_partitioned(file_info.name):
+                return self._find_partition_file_format(file_info.path)
+        return None
+
+    def _assess_path(self, file_info: FileInfo) -> TableInMount | None:
+        if file_info.name == "_delta_log/":
+            logger.debug(f"Found delta table {file_info.path}")
+            return TableInMount(format="DELTA", is_partitioned=False)
+        if self._is_csv(file_info.name):
+            logger.debug(f"Found csv {file_info.path}")
+            return TableInMount(format="CSV", is_partitioned=False)
+        if self._is_json(file_info.name):
+            logger.debug(f"Found json {file_info.path}")
+            return TableInMount(format="JSON", is_partitioned=False)
+        if self._is_parquet(file_info.name):
+            logger.debug(f"Found parquet {file_info.path}")
+            return TableInMount(format="PARQUET", is_partitioned=False)
+        return None
 
     def _is_partitioned(self, file_name: str) -> bool:
         return '=' in file_name
 
     def _is_parquet(self, file_name: str) -> bool:
         parquet_patterns = {'.parquet'}
         return any(pattern in file_name for pattern in parquet_patterns)
 
+    def _is_csv(self, file_name: str) -> bool:
+        csv_patterns = {'.csv'}
+        return any(pattern in file_name for pattern in csv_patterns)
+
+    def _is_json(self, file_name: str) -> bool:
+        json_patterns = {'.json'}
+        return any(pattern in file_name for pattern in json_patterns)
+
     def _is_irrelevant(self, file_name: str) -> bool:
         return any(pattern in file_name for pattern in self._fiter_paths)
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/mapping.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/mapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import re
 from collections.abc import Collection
 from dataclasses import dataclass
 from functools import partial
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.parallel import Threads
-from databricks.labs.lsql.backends import SqlBackend, StatementExecutionBackend
+from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import BadRequest, NotFound, ResourceConflict
+from databricks.sdk.service.catalog import TableInfo, SchemaInfo
 
 from databricks.labs.ucx.account import WorkspaceInfo
-from databricks.labs.ucx.config import WorkspaceConfig
 from databricks.labs.ucx.framework.utils import escape_sql_identifier
 from databricks.labs.ucx.hive_metastore import TablesCrawler
 from databricks.labs.ucx.hive_metastore.tables import Table
 
 logger = logging.getLogger(__name__)
 
 
@@ -35,62 +35,72 @@
             catalog_name=catalog_name,
             src_schema=table.database,
             dst_schema=table.database,
             src_table=table.name,
             dst_table=table.name,
         )
 
+    @classmethod
+    def from_src_dst(cls, src_table: TableInfo, dst_schema: SchemaInfo) -> "Rule":
+        return cls(
+            workspace_name="workspace",
+            catalog_name=str(dst_schema.catalog_name or ""),
+            src_schema=str(src_table.schema_name or ""),
+            dst_schema=str(dst_schema.name or ""),
+            src_table=str(src_table.name or ""),
+            dst_table=str(src_table.name or ""),
+        )
+
     @property
     def as_uc_table_key(self):
         return f"{self.catalog_name}.{self.dst_schema}.{self.dst_table}"
 
     @property
     def as_hms_table_key(self):
         return f"hive_metastore.{self.src_schema}.{self.src_table}"
 
 
 @dataclass
 class TableToMigrate:
     src: Table
     rule: Rule
 
+    def __hash__(self):
+        return hash(self.src)
+
+    def __eq__(self, other):
+        return isinstance(other, TableToMigrate) and self.src == other.src
+
 
 class TableMapping:
+    FILENAME = 'mapping.csv'
     UCX_SKIP_PROPERTY = "databricks.labs.ucx.skip"
 
     def __init__(self, installation: Installation, ws: WorkspaceClient, sql_backend: SqlBackend):
-        self._filename = 'mapping.csv'
         self._installation = installation
         self._ws = ws
         self._sql_backend = sql_backend
 
-    @classmethod
-    def current(cls, ws: WorkspaceClient, product='ucx'):
-        installation = Installation.current(ws, product)
-        config = installation.load(WorkspaceConfig)
-        sql_backend = StatementExecutionBackend(ws, config.warehouse_id)
-        return cls(installation, ws, sql_backend)
-
     def current_tables(self, tables: TablesCrawler, workspace_name: str, catalog_name: str):
         tables_snapshot = tables.snapshot()
         if len(tables_snapshot) == 0:
             msg = "No tables found. Please run: databricks labs ucx ensure-assessment-run"
             raise ValueError(msg)
         for table in tables_snapshot:
             yield Rule.initial(workspace_name, catalog_name, table)
 
     def save(self, tables: TablesCrawler, workspace_info: WorkspaceInfo) -> str:
         workspace_name = workspace_info.current()
         default_catalog_name = re.sub(r"\W+", "_", workspace_name)
         current_tables = self.current_tables(tables, workspace_name, default_catalog_name)
-        return self._installation.save(list(current_tables), filename=self._filename)
+        return self._installation.save(list(current_tables), filename=self.FILENAME)
 
     def load(self) -> list[Rule]:
         try:
-            return self._installation.load(list[Rule], filename=self._filename)
+            return self._installation.load(list[Rule], filename=self.FILENAME)
         except NotFound:
             msg = "Please run: databricks labs ucx table-mapping"
             raise ValueError(msg) from None
 
     def skip_table(self, schema: str, table: str):
         # Marks a table to be skipped in the migration process by applying a table property
         try:
@@ -145,16 +155,22 @@
         tasks = []
         for database in databases:
             tasks.append(partial(self._get_database_in_scope_task, database))
         return Threads.strict("checking databases for skip property", tasks)
 
     def _get_database_in_scope_task(self, database: str) -> str | None:
         describe = {}
-        for value in self._sql_backend.fetch(f"DESCRIBE SCHEMA EXTENDED {escape_sql_identifier(database)}"):
-            describe[value["database_description_item"]] = value["database_description_value"]
+        try:
+            for value in self._sql_backend.fetch(f"DESCRIBE SCHEMA EXTENDED {escape_sql_identifier(database)}"):
+                describe[value["database_description_item"]] = value["database_description_value"]
+        except NotFound:
+            logger.warning(
+                f"Schema hive_metastore.{database} no longer exists. Skipping its properties check and migration."
+            )
+            return None
         properties = describe.get("Properties", "")
         if not properties:
             return database
         if self.UCX_SKIP_PROPERTY in TablesCrawler.parse_database_props(properties.lower()):
             logger.info(f"Database {database} is marked to be skipped")
             return None
         return database
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/table_migrate.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/table_migrate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,147 +1,305 @@
 import dataclasses
-import datetime
 import logging
 from collections import defaultdict
 from collections.abc import Iterable
-from dataclasses import dataclass
 from functools import partial
 
-from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.parallel import Threads
-from databricks.labs.lsql.backends import SqlBackend, StatementExecutionBackend
+from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
 
-from databricks.labs.ucx.config import WorkspaceConfig
-from databricks.labs.ucx.framework.crawlers import CrawlerBase
-from databricks.labs.ucx.framework.utils import escape_sql_identifier
-from databricks.labs.ucx.hive_metastore import GrantsCrawler, TablesCrawler
-from databricks.labs.ucx.hive_metastore.grants import Grant
-from databricks.labs.ucx.hive_metastore.mapping import Rule, TableMapping
+from databricks.labs.ucx.hive_metastore import TablesCrawler, Mounts
+from databricks.labs.ucx.hive_metastore.grants import Grant, GrantsCrawler, PrincipalACL
+from databricks.labs.ucx.hive_metastore.locations import Mount, ExternalLocations
+from databricks.labs.ucx.hive_metastore.mapping import (
+    Rule,
+    TableMapping,
+    TableToMigrate,
+)
+from databricks.labs.ucx.hive_metastore.migration_status import MigrationStatusRefresher
 from databricks.labs.ucx.hive_metastore.tables import (
     AclMigrationWhat,
     MigrationCount,
     Table,
     What,
+    HiveSerdeType,
+)
+from databricks.labs.ucx.hive_metastore.view_migrate import (
+    ViewsMigrationSequencer,
+    ViewToMigrate,
 )
-from databricks.labs.ucx.hive_metastore.udfs import UdfsCrawler
 from databricks.labs.ucx.workspace_access.groups import GroupManager, MigratedGroup
 
 logger = logging.getLogger(__name__)
 
 
-@dataclass
-class MigrationStatus:
-    src_schema: str
-    src_table: str
-    dst_catalog: str | None = None
-    dst_schema: str | None = None
-    dst_table: str | None = None
-    update_ts: str | None = None
-
-    def destination(self):
-        return f"{self.dst_catalog}.{self.dst_schema}.{self.dst_table}".lower()
-
-
 class TablesMigrator:
     def __init__(
         self,
         table_crawler: TablesCrawler,
         grant_crawler: GrantsCrawler,
         ws: WorkspaceClient,
         backend: SqlBackend,
         table_mapping: TableMapping,
         group_manager: GroupManager,
         migration_status_refresher: 'MigrationStatusRefresher',
+        principal_grants: PrincipalACL,
     ):
         self._tc = table_crawler
         self._gc = grant_crawler
         self._backend = backend
         self._ws = ws
         self._tm = table_mapping
         self._group = group_manager
         self._migration_status_refresher = migration_status_refresher
         self._seen_tables: dict[str, str] = {}
-
-    @classmethod
-    def for_cli(cls, ws: WorkspaceClient, product='ucx'):
-        installation = Installation.current(ws, product)
-        config = installation.load(WorkspaceConfig)
-        sql_backend = StatementExecutionBackend(ws, config.warehouse_id)
-        table_crawler = TablesCrawler(sql_backend, config.inventory_database)
-        udfs_crawler = UdfsCrawler(sql_backend, config.inventory_database)
-        grants_crawler = GrantsCrawler(table_crawler, udfs_crawler)
-        table_mapping = TableMapping(installation, ws, sql_backend)
-        group_manager = GroupManager(sql_backend, ws, config.inventory_database)
-        migration_status_refresher = MigrationStatusRefresher(ws, sql_backend, config.inventory_database, table_crawler)
-        return cls(
-            table_crawler, grants_crawler, ws, sql_backend, table_mapping, group_manager, migration_status_refresher
-        )
+        self._principal_grants = principal_grants
 
     def index(self):
+        # TODO: remove this method
         return self._migration_status_refresher.index()
 
-    def migrate_tables(self, *, what: What | None = None, acl_strategy: list[AclMigrationWhat] | None = None):
+    def migrate_tables(
+        self,
+        what: What,
+        acl_strategy: list[AclMigrationWhat] | None = None,
+        mounts_crawler: Mounts | None = None,
+        hiveserde_in_place_migrate: bool = False,
+    ):
+        if what in [What.DB_DATASET, What.UNKNOWN]:
+            logger.error(f"Can't migrate tables with type {what.name}")
+            return None
+        all_grants_to_migrate = None if acl_strategy is None else self._gc.snapshot()
+        all_migrated_groups = None if acl_strategy is None else self._group.snapshot()
+        all_principal_grants = None if acl_strategy is None else self._principal_grants.get_interactive_cluster_grants()
         self._init_seen_tables()
+        # mounts will be used to replace the mnt based table location in the DDL for hiveserde table in-place migration
+        mounts: list[Mount] = []
+        if mounts_crawler:
+            mounts = list(mounts_crawler.snapshot())
+        if what == What.VIEW:
+            return self._migrate_views(acl_strategy, all_grants_to_migrate, all_migrated_groups, all_principal_grants)
+        return self._migrate_tables(
+            what,
+            acl_strategy,
+            all_grants_to_migrate,
+            all_migrated_groups,
+            all_principal_grants,
+            mounts,
+            hiveserde_in_place_migrate,
+        )
+
+    def _migrate_tables(
+        self,
+        what: What,
+        acl_strategy,
+        all_grants_to_migrate,
+        all_migrated_groups,
+        all_principal_grants,
+        mounts: list[Mount],
+        hiveserde_in_place_migrate: bool = False,
+    ):
         tables_to_migrate = self._tm.get_tables_to_migrate(self._tc)
+        tables_in_scope = filter(lambda t: t.src.what == what, tables_to_migrate)
         tasks = []
-        if acl_strategy is not None:
-            grants_to_migrate = self._gc.snapshot()
-            migrated_groups = self._group.snapshot()
-        else:
-            acl_strategy = []
-        for table in tables_to_migrate:
-            grants = []
-            if what is not None and table.src.what != what:
-                continue
-            if AclMigrationWhat.LEGACY_TACL in acl_strategy:
-                grants.extend(self._match_grants(table.src, grants_to_migrate, migrated_groups))
-            tasks.append(partial(self._migrate_table, table.src, table.rule, grants))
+        for table in tables_in_scope:
+            grants = self._compute_grants(
+                table.src, acl_strategy, all_grants_to_migrate, all_migrated_groups, all_principal_grants
+            )
+            tasks.append(partial(self._migrate_table, table, grants, mounts, hiveserde_in_place_migrate))
         Threads.strict("migrate tables", tasks)
+        if not tasks:
+            logger.info(f"No tables found to migrate with type {what.name}")
+        # the below is useful for testing
+        return tasks
 
-    def _migrate_table(self, src_table: Table, rule: Rule, grants: list[Grant] | None = None):
-        if self._table_already_migrated(rule.as_uc_table_key):
-            logger.info(f"Table {src_table.key} already migrated to {rule.as_uc_table_key}")
+    def _migrate_views(self, acl_strategy, all_grants_to_migrate, all_migrated_groups, all_principal_grants):
+        tables_to_migrate = self._tm.get_tables_to_migrate(self._tc)
+        self._migration_status_refresher.reset()
+        all_tasks = []
+        sequencer = ViewsMigrationSequencer(tables_to_migrate, self.index())
+        batches = sequencer.sequence_batches()
+        for batch in batches:
+            tasks = []
+            for view in batch:
+                grants = self._compute_grants(
+                    view.src, acl_strategy, all_grants_to_migrate, all_migrated_groups, all_principal_grants
+                )
+                tasks.append(
+                    partial(
+                        self._migrate_view,
+                        view,
+                        grants,
+                    )
+                )
+            Threads.strict("migrate views", tasks)
+            self._migration_status_refresher.reset()
+            all_tasks.extend(tasks)
+        return all_tasks
+
+    def _compute_grants(
+        self, table: Table, acl_strategy, all_grants_to_migrate, all_migrated_groups, all_principal_grants
+    ):
+        if acl_strategy is None:
+            acl_strategy = []
+        grants = []
+        if AclMigrationWhat.LEGACY_TACL in acl_strategy:
+            grants.extend(self._match_grants(table, all_grants_to_migrate, all_migrated_groups))
+        if AclMigrationWhat.PRINCIPAL in acl_strategy:
+            grants.extend(self._match_grants(table, all_principal_grants, all_migrated_groups))
+        return grants
+
+    def _migrate_table(
+        self,
+        src_table: TableToMigrate,
+        grants: list[Grant],
+        mounts: list[Mount],
+        hiveserde_in_place_migrate: bool = False,
+    ):
+        if self._table_already_migrated(src_table.rule.as_uc_table_key):
+            logger.info(f"Table {src_table.src.key} already migrated to {src_table.rule.as_uc_table_key}")
             return True
-        if src_table.what == What.DBFS_ROOT_DELTA:
-            return self._migrate_dbfs_root_table(src_table, rule, grants)
-        if src_table.what == What.EXTERNAL_SYNC:
-            return self._migrate_external_table(src_table, rule, grants)
-        if src_table.what == What.VIEW:
-            return self._migrate_view(src_table, rule, grants)
-        logger.info(f"Table {src_table.key} is not supported for migration")
+        if src_table.src.what == What.DBFS_ROOT_DELTA:
+            return self._migrate_dbfs_root_table(src_table.src, src_table.rule, grants)
+        if src_table.src.what == What.DBFS_ROOT_NON_DELTA:
+            return self._migrate_table_create_ctas(src_table.src, src_table.rule, grants, mounts)
+        if src_table.src.what == What.EXTERNAL_SYNC:
+            return self._migrate_external_table(src_table.src, src_table.rule, grants)
+        if src_table.src.what == What.EXTERNAL_HIVESERDE:
+            # This hiveserde_in_place_migrate is used to determine if current hiveserde migration should use in-place migration or CTAS.
+            # We will provide two workflows for hiveserde table migration:
+            # 1. One will migrate all hiveserde tables using CTAS which we officially support.
+            # 2. The other one will migrate certain types of hiveserde in place, which is technically working, but the user
+            # need to accept the risk that the old files created by hiveserde may not be processed correctly by Spark
+            # datasource in corner cases.
+            # User will need to decide which workflow to runs first which will migrate the hiveserde tables and mark the
+            # `upgraded_to` property and hence those tables will be skipped in the migration workflow runs later.
+            if hiveserde_in_place_migrate:
+                return self._migrate_external_table_hiveserde_in_place(src_table.src, src_table.rule, grants, mounts)
+            return self._migrate_table_create_ctas(src_table.src, src_table.rule, grants, mounts)
+        if src_table.src.what == What.EXTERNAL_NO_SYNC:
+            # use CTAS if table cannot be upgraded using SYNC and table is not hiveserde table
+            return self._migrate_table_create_ctas(src_table.src, src_table.rule, grants, mounts)
+        logger.info(f"Table {src_table.src.key} is not supported for migration")
         return True
 
+    def _migrate_view(
+        self,
+        src_view: ViewToMigrate,
+        grants: list[Grant] | None = None,
+    ):
+        if self._table_already_migrated(src_view.rule.as_uc_table_key):
+            logger.info(f"View {src_view.src.key} already migrated to {src_view.rule.as_uc_table_key}")
+            return True
+        if self._view_can_be_migrated(src_view):
+            return self._migrate_view_table(src_view, grants)
+        logger.info(f"View {src_view.src.key} is not supported for migration")
+        return True
+
+    def _view_can_be_migrated(self, view: ViewToMigrate):
+        # dependencies have already been computed, therefore an empty dict is good enough
+        for table in view.dependencies:
+            if not self.index().get(table.schema, table.name):
+                logger.info(f"View {view.src.key} cannot be migrated because {table.key} is not migrated yet")
+                return False
+        return True
+
+    def _migrate_view_table(self, src_view: ViewToMigrate, grants: list[Grant] | None = None):
+        view_migrate_sql = self._sql_migrate_view(src_view)
+        logger.debug(f"Migrating view {src_view.src.key} to using SQL query: {view_migrate_sql}")
+        self._backend.execute(view_migrate_sql)
+        self._backend.execute(src_view.src.sql_alter_to(src_view.rule.as_uc_table_key))
+        self._backend.execute(src_view.src.sql_alter_from(src_view.rule.as_uc_table_key, self._ws.get_workspace_id()))
+        return self._migrate_acl(src_view.src, src_view.rule, grants)
+
+    def _sql_migrate_view(self, src_view: ViewToMigrate) -> str:
+        # We have to fetch create statement this way because of columns in:
+        # CREATE VIEW x.y (col1, col2) AS SELECT * FROM w.t
+        create_statement = self._backend.fetch(f"SHOW CREATE TABLE {src_view.src.safe_sql_key}")
+        src_view.src.view_text = next(iter(create_statement))["createtab_stmt"]
+        migration_index = self._migration_status_refresher.index()
+        return src_view.sql_migrate_view(migration_index)
+
     def _migrate_external_table(self, src_table: Table, rule: Rule, grants: list[Grant] | None = None):
         target_table_key = rule.as_uc_table_key
         table_migrate_sql = src_table.sql_migrate_external(target_table_key)
         logger.debug(f"Migrating external table {src_table.key} to using SQL query: {table_migrate_sql}")
         # have to wrap the fetch result with iter() for now, because StatementExecutionBackend returns iterator but RuntimeBackend returns list.
         sync_result = next(iter(self._backend.fetch(table_migrate_sql)))
         if sync_result.status_code != "SUCCESS":
             logger.warning(
                 f"SYNC command failed to migrate {src_table.key} to {target_table_key}. Status code: {sync_result.status_code}. Description: {sync_result.description}"
             )
             return False
         self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
         return self._migrate_acl(src_table, rule, grants)
 
+    def _migrate_external_table_hiveserde_in_place(
+        self,
+        src_table: Table,
+        rule: Rule,
+        grants: list[Grant],
+        mounts: list[Mount],
+    ):
+        # verify hive serde type
+        hiveserde_type = src_table.hiveserde_type(self._backend)
+        if hiveserde_type in [
+            HiveSerdeType.NOT_HIVESERDE,
+            HiveSerdeType.OTHER_HIVESERDE,
+            HiveSerdeType.INVALID_HIVESERDE_INFO,
+        ]:
+            logger.warning(f"{src_table.key} table can only be migrated using CTAS.")
+            return False
+
+        # if the src table location is using mount, resolve the mount location so it will be used in the updated DDL
+        dst_table_location = None
+        if mounts and src_table.is_dbfs_mnt:
+            dst_table_location = ExternalLocations.resolve_mount(src_table.location, mounts)
+
+        table_migrate_sql = src_table.sql_migrate_external_hiveserde_in_place(
+            rule.catalog_name, rule.dst_schema, rule.dst_table, self._backend, hiveserde_type, dst_table_location
+        )
+        if not table_migrate_sql:
+            logger.error(
+                f"Failed to generate in-place migration DDL for {src_table.key}, skip the in-place migration. It can be migrated in CTAS workflow"
+            )
+            return False
+
+        logger.debug(
+            f"Migrating external table {src_table.key} to {rule.as_uc_table_key} using SQL query: {table_migrate_sql}"
+        )
+        self._backend.execute(table_migrate_sql)
+        self._backend.execute(src_table.sql_alter_to(rule.as_uc_table_key))
+        self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
+        return self._migrate_acl(src_table, rule, grants)
+
     def _migrate_dbfs_root_table(self, src_table: Table, rule: Rule, grants: list[Grant] | None = None):
         target_table_key = rule.as_uc_table_key
         table_migrate_sql = src_table.sql_migrate_dbfs(target_table_key)
-        logger.debug(f"Migrating managed table {src_table.key} to using SQL query: {table_migrate_sql}")
+        logger.debug(
+            f"Migrating managed table {src_table.key} to {rule.as_uc_table_key} using SQL query: {table_migrate_sql}"
+        )
         self._backend.execute(table_migrate_sql)
         self._backend.execute(src_table.sql_alter_to(rule.as_uc_table_key))
         self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
         return self._migrate_acl(src_table, rule, grants)
 
-    def _migrate_view(self, src_table: Table, rule: Rule, grants: list[Grant] | None = None):
-        target_table_key = rule.as_uc_table_key
-        table_migrate_sql = src_table.sql_migrate_view(target_table_key)
-        logger.debug(f"Migrating view {src_table.key} to using SQL query: {table_migrate_sql}")
+    def _migrate_table_create_ctas(self, src_table: Table, rule: Rule, grants: list[Grant], mounts: list[Mount]):
+        if src_table.what not in [What.EXTERNAL_NO_SYNC, What.EXTERNAL_HIVESERDE]:
+            table_migrate_sql = src_table.sql_migrate_ctas_managed(rule.as_uc_table_key)
+        elif not src_table.location:
+            table_migrate_sql = src_table.sql_migrate_ctas_managed(rule.as_uc_table_key)
+        else:
+            # if external table and src tabel location is not missing, migrate to external UC table
+            dst_table_location = src_table.location + "_ctas_migrated"
+            if mounts and src_table.is_dbfs_mnt:
+                dst_table_location = ExternalLocations.resolve_mount(src_table.location, mounts) + "_ctas_migrated"
+            table_migrate_sql = src_table.sql_migrate_ctas_external(rule.as_uc_table_key, dst_table_location)
+        logger.debug(f"Migrating table {src_table.key} to {rule.as_uc_table_key} using SQL query: {table_migrate_sql}")
         self._backend.execute(table_migrate_sql)
         self._backend.execute(src_table.sql_alter_to(rule.as_uc_table_key))
         self._backend.execute(src_table.sql_alter_from(rule.as_uc_table_key, self._ws.get_workspace_id()))
         return self._migrate_acl(src_table, rule, grants)
 
     def _migrate_acl(self, src: Table, rule: Rule, grants: list[Grant] | None):
         if grants is None:
@@ -270,87 +428,7 @@
             if table.name not in (grant.table, grant.view):
                 continue
             matched_group = [g.name_in_account for g in migrated_groups if g.name_in_workspace == grant.principal]
             if len(matched_group) > 0:
                 grant = dataclasses.replace(grant, principal=matched_group[0])
             matched_grants.append(grant)
         return matched_grants
-
-
-class MigrationIndex:
-    def __init__(self, tables: list[MigrationStatus]):
-        self._index = {(ms.src_schema, ms.src_table): ms for ms in tables}
-
-    def is_migrated(self, schema: str, table: str) -> bool:
-        """Check if a table is migrated."""
-        return self.get(schema, table) is not None
-
-    def get(self, schema: str, table: str) -> MigrationStatus | None:
-        """Get the migration status for a table. If the table is not migrated, return None."""
-        dst = self._index.get((schema.lower(), table.lower()))
-        if not dst or not dst.dst_table:
-            return None
-        return dst
-
-
-class MigrationStatusRefresher(CrawlerBase[MigrationStatus]):
-    def __init__(self, ws: WorkspaceClient, sbe: SqlBackend, schema, table_crawler: TablesCrawler):
-        super().__init__(sbe, "hive_metastore", schema, "migration_status", MigrationStatus)
-        self._ws = ws
-        self._table_crawler = table_crawler
-
-    def snapshot(self) -> Iterable[MigrationStatus]:
-        return self._snapshot(self._try_fetch, self._crawl)
-
-    def index(self) -> MigrationIndex:
-        return MigrationIndex(list(self.snapshot()))
-
-    def get_seen_tables(self) -> dict[str, str]:
-        seen_tables: dict[str, str] = {}
-        for schema in self._iter_schemas():
-            for table in self._ws.tables.list(catalog_name=schema.catalog_name, schema_name=schema.name):
-                if not table.properties:
-                    continue
-                if "upgraded_from" not in table.properties:
-                    continue
-                if not table.full_name:
-                    logger.warning(f"The table {table.name} in {schema.name} has no full name")
-                    continue
-                seen_tables[table.full_name.lower()] = table.properties["upgraded_from"].lower()
-        return seen_tables
-
-    def is_migrated(self, schema: str, table: str) -> bool:
-        result = self._backend.fetch(f"SHOW TBLPROPERTIES {escape_sql_identifier(schema + '.' + table)}")
-        for value in result:
-            if value["key"] == "upgraded_to":
-                logger.info(f"{schema}.{table} is set as migrated")
-                return True
-        logger.info(f"{schema}.{table} is set as not migrated")
-        return False
-
-    def _crawl(self) -> Iterable[MigrationStatus]:
-        all_tables = self._table_crawler.snapshot()
-        reverse_seen = {v: k for k, v in self.get_seen_tables().items()}
-        timestamp = datetime.datetime.now(datetime.timezone.utc).timestamp()
-        for table in all_tables:
-            src_schema = table.database.lower()
-            src_table = table.name.lower()
-            table_migration_status = MigrationStatus(
-                src_schema=src_schema,
-                src_table=src_table,
-                update_ts=str(timestamp),
-            )
-            if table.key in reverse_seen and self.is_migrated(src_schema, src_table):
-                target_table = reverse_seen[table.key]
-                if len(target_table.split(".")) == 3:
-                    table_migration_status.dst_catalog = target_table.split(".")[0]
-                    table_migration_status.dst_schema = target_table.split(".")[1]
-                    table_migration_status.dst_table = target_table.split(".")[2]
-            yield table_migration_status
-
-    def _try_fetch(self) -> Iterable[MigrationStatus]:
-        for row in self._fetch(f"SELECT * FROM {self._schema}.{self._table}"):
-            yield MigrationStatus(*row)
-
-    def _iter_schemas(self):
-        for catalog in self._ws.catalogs.list():
-            yield from self._ws.schemas.list(catalog_name=catalog.name)
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/table_move.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/table_move.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 from functools import partial
 
-from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.parallel import Threads
-from databricks.labs.lsql.backends import SqlBackend, StatementExecutionBackend
+from databricks.labs.lsql.backends import SqlBackend
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound
 from databricks.sdk.service.catalog import (
     PermissionsChange,
     Privilege,
     SecurableType,
     TableType,
 )
 
-from databricks.labs.ucx.config import WorkspaceConfig
 from databricks.labs.ucx.framework.utils import escape_sql_identifier
 from databricks.labs.ucx.hive_metastore.table_migrate import logger
 
 
 class TableMove:
     def __init__(self, ws: WorkspaceClient, backend: SqlBackend):
         self._backend = backend
         self._fetch = backend.fetch
         self._execute = backend.execute
         self._ws = ws
 
-    @classmethod
-    def for_cli(cls, ws: WorkspaceClient, product='ucx'):
-        installation = Installation.current(ws, product)
-        config = installation.load(WorkspaceConfig)
-        sql_backend = StatementExecutionBackend(ws, config.warehouse_id)
-        return cls(ws, sql_backend)
-
     def move(
         self,
         from_catalog: str,
         from_schema: str,
         from_table: str,
         to_catalog: str,
         to_schema: str,
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/table_size.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/table_size.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/tables.scala` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/tables.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/udfs.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/udfs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from collections.abc import Iterable
 from dataclasses import dataclass
 from functools import partial
 
 from databricks.labs.blueprint.parallel import Threads
 from databricks.labs.lsql.backends import SqlBackend
-from databricks.sdk.errors import Unknown
+from databricks.sdk.errors import Unknown, NotFound
 
 from databricks.labs.ucx.framework.crawlers import CrawlerBase
 from databricks.labs.ucx.framework.utils import escape_sql_identifier
 
 logger = logging.getLogger(__name__)
 
 
@@ -83,14 +83,17 @@
             for (udf,) in self._fetch(
                 f"SHOW USER FUNCTIONS FROM {escape_sql_identifier(catalog)}.{escape_sql_identifier(database)};"
             ):
                 if not udf.startswith(f"{catalog}.{database}"):
                     continue
                 udf_name = udf[udf.rfind(".") + 1 :]  # remove catalog and database info from the name
                 yield partial(self._describe, catalog, database, udf_name)
+        except NotFound:
+            # This make the integration test more robust as many test schemas are being created and deleted quickly.
+            logger.warning(f"Schema {catalog}.{database} no longer existed")
         except Unknown as err:
             logger.error(f"Problem with {database}: {err}")
 
     def _describe(self, catalog: str, database: str, udf: str) -> Udf | None:
         """Fetches metadata like udf type, input, returns, data access and body
         if specified for a specific udf within the given catalog and database.
         """
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/hive_metastore/verification.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/hive_metastore/verification.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,16 +24,16 @@
             current_metastore = self._ws.metastores.current()
             if current_metastore:
                 self.default_catalog_name = current_metastore.default_catalog_name
                 self.metastore_id = current_metastore.metastore_id
                 self.workspace_id = current_metastore.workspace_id
                 return True
             raise MetastoreNotFoundError
-        except PermissionDenied:
-            logger.error("Permission Denied while trying to access metastore")
+        except PermissionDenied as err:
+            logger.error(f"Cannot access metastore: {err}")
             return False
 
 
 class MetastoreNotFoundError(Exception):
     def __init__(self, message="Metastore not found in the workspace"):
         self.message = message
         super().__init__(self.message)
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/installer/hms_lineage.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/hms_lineage.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,30 +22,34 @@
 logger = logging.getLogger(__name__)
 
 
 class HiveMetastoreLineageEnabler:
     def __init__(self, ws: WorkspaceClient):
         self._ws = ws
 
-    def apply(self, prompts: Prompts):
+    def apply(self, prompts: Prompts, is_account_install: bool = False):
         script = self._check_lineage_spark_config_exists()
         if script:
             if script.enabled:
                 logger.info("HMS lineage init script already exists and enabled")
                 return
-            if prompts.confirm("HMS lineage collection init script is disabled, do you want to enable it?"):
+            if is_account_install or prompts.confirm(
+                "HMS lineage collection init script is disabled, do you want to enable it?"
+            ):
                 logger.info("Enabling Global Init Script...")
                 self._enable_global_init_script(script)
             return
         logger.info(
             "HMS Lineage feature creates one system table named system.hms_to_uc_migration.table_access and "
             "helps in your migration process from HMS to UC by allowing you to programmatically query HMS "
             "lineage data."
         )
-        if prompts.confirm("No HMS lineage collection init script exists, do you want to create one?"):
+        if is_account_install or prompts.confirm(
+            "No HMS lineage collection init script exists, do you want to create one?"
+        ):
             logger.info("Creating Global Init Script...")
             self._add_global_init_script()
 
     def _check_lineage_spark_config_exists(self) -> GlobalInitScriptDetailsWithContent | None:
         for script in self._ws.global_init_scripts.list():
             if not script.script_id:
                 continue
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/installer/policy.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from databricks.labs.blueprint.installer import InstallState
 from databricks.labs.blueprint.tui import Prompts
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import NotFound
 from databricks.sdk.service import compute
 from databricks.sdk.service.sql import GetWorkspaceWarehouseConfigResponse
 
+
 logger = logging.getLogger(__name__)
 
 
 class ClusterPolicyInstaller:
     def __init__(self, installation: Installation, ws: WorkspaceClient, prompts: Prompts):
         self._ws = ws
         self._installation = installation
@@ -85,38 +86,44 @@
             logger.warning(
                 f"Instance pool id {instance_pool_id} does not exist. Will not set instance pool in the cluster policy. You can manually edit the cluster policy after installation."
             )
             return None
 
     def _definition(self, conf: dict, instance_profile: str | None, instance_pool_id: str | None) -> str:
         latest_lts_dbr = self._ws.clusters.select_spark_version(latest=True, long_term_support=True)
+        node_type_id = self._ws.clusters.select_node_type(local_disk=True, min_memory_gb=16)
         policy_definition = {
             "spark_version": self._policy_config(latest_lts_dbr),
-            "node_type_id": self._policy_config(self._ws.clusters.select_node_type(local_disk=True)),
+            "node_type_id": self._policy_config(node_type_id),
         }
-        if instance_pool_id:
-            policy_definition["instance_pool_id"] = self._policy_config(instance_pool_id)
-            # 'node_type_id' cannot be supplied when an instance pool ID is provided
-            policy_definition.pop("node_type_id")
         for key, value in conf.items():
             policy_definition[f"spark_conf.{key}"] = self._policy_config(value)
+        # set the availability to on demand
         if self._ws.config.is_aws:
             if instance_profile:
                 policy_definition["aws_attributes.instance_profile_arn"] = self._policy_config(instance_profile)
             policy_definition["aws_attributes.availability"] = self._policy_config(
                 compute.AwsAvailability.ON_DEMAND.value
             )
         elif self._ws.config.is_azure:
             policy_definition["azure_attributes.availability"] = self._policy_config(
                 compute.AzureAvailability.ON_DEMAND_AZURE.value
             )
         else:
             policy_definition["gcp_attributes.availability"] = self._policy_config(
                 compute.GcpAvailability.ON_DEMAND_GCP.value
             )
+        if instance_pool_id:
+            policy_definition["instance_pool_id"] = self._policy_config(instance_pool_id)
+            # 'node_type_id' cannot be supplied when an instance pool ID is provided
+            policy_definition.pop("node_type_id")
+            # 'availability' cannot be supplied when an instance pool ID is provided
+            policy_definition.pop("aws_attributes.availability", "")
+            policy_definition.pop("azure_attributes.availability", "")
+            policy_definition.pop("gcp_attributes.availability", "")
         return json.dumps(policy_definition)
 
     @staticmethod
     def _extract_external_hive_metastore_conf(cluster_policy):
         spark_conf_dict = {}
         instance_profile = None
         if cluster_policy.get("aws_attributes.instance_profile_arn") is not None:
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/installer/workflows.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/installer/workflows.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import logging
+import os.path
 import re
 import sys
 import webbrowser
+from collections.abc import Iterator
 from dataclasses import replace
-from datetime import timedelta
+from datetime import datetime, timedelta
+from io import StringIO
 from pathlib import Path
 from typing import Any
 
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.blueprint.installer import InstallState
 from databricks.labs.blueprint.parallel import ManyError
 from databricks.labs.blueprint.tui import Prompts
@@ -34,27 +37,29 @@
     TooManyRequests,
     Unauthenticated,
     Unknown,
 )
 from databricks.sdk.retries import retried
 from databricks.sdk.service import compute, jobs
 from databricks.sdk.service.jobs import RunLifeCycleState, RunResultState
+from databricks.sdk.service.workspace import ObjectType
 
 import databricks
 from databricks.labs.ucx.config import WorkspaceConfig
 from databricks.labs.ucx.configure import ConfigureClusterOverrides
-from databricks.labs.ucx.framework.tasks import _TASKS, Task
+from databricks.labs.ucx.framework.tasks import Task
+from databricks.labs.ucx.installer.logs import PartialLogRecord, parse_logs
 from databricks.labs.ucx.installer.mixins import InstallationMixin
-from databricks.labs.ucx.runtime import main
 
 logger = logging.getLogger(__name__)
 
 EXTRA_TASK_PARAMS = {
     "job_id": "{{job_id}}",
     "run_id": "{{run_id}}",
+    "attempt": "{{job.repair_count}}",
     "parent_run_id": "{{parent_run_id}}",
 }
 DEBUG_NOTEBOOK = """# Databricks notebook source
 # MAGIC %md
 # MAGIC # Debug companion for UCX installation (see [README]({readme_link}))
 # MAGIC
 # MAGIC Production runs are supposed to be triggered through the following jobs: {job_links}
@@ -90,114 +95,65 @@
 dbutils.library.restartPython()
 
 # COMMAND ----------
 
 from databricks.labs.ucx.runtime import main
 
 main(f'--config=/Workspace{config_file}',
+     f'--workflow=' + dbutils.widgets.get('workflow'),
      f'--task=' + dbutils.widgets.get('task'),
      f'--job_id=' + dbutils.widgets.get('job_id'),
      f'--run_id=' + dbutils.widgets.get('run_id'),
+     f'--attempt=' + dbutils.widgets.get('attempt'),
      f'--parent_run_id=' + dbutils.widgets.get('parent_run_id'))
 """
 
 
-class WorkflowsInstallation(InstallationMixin):
-    def __init__(
-        self,
-        config: WorkspaceConfig,
-        installation: Installation,
-        ws: WorkspaceClient,
-        wheels: WheelsV2,
-        prompts: Prompts,
-        product_info: ProductInfo,
-        verify_timeout: timedelta,
-    ):
-        self._config = config
-        self._installation = installation
+class DeployedWorkflows:
+    def __init__(self, ws: WorkspaceClient, install_state: InstallState, verify_timeout: timedelta):
         self._ws = ws
-        self._state = InstallState.from_installation(installation)
-        self._wheels = wheels
-        self._prompts = prompts
-        self._product_info = product_info
+        self._install_state = install_state
         self._verify_timeout = verify_timeout
-        self._this_file = Path(__file__)
-        super().__init__(config, installation, ws)
-
-    @classmethod
-    def current(cls, ws: WorkspaceClient):
-        product_info = ProductInfo.from_class(WorkspaceConfig)
-        installation = product_info.current_installation(ws)
-        config = installation.load(WorkspaceConfig)
-        wheels = product_info.wheels(ws)
-        prompts = Prompts()
-        timeout = timedelta(minutes=2)
-
-        return cls(config, installation, ws, wheels, prompts, product_info, timeout)
-
-    @property
-    def state(self):
-        return self._state
 
     def run_workflow(self, step: str):
-        job_id = int(self._state.jobs[step])
+        # this dunder variable is hiding this method from tracebacks, making it cleaner
+        # for the user to see the actual error without too much noise.
+        __tracebackhide__ = True  # pylint: disable=unused-variable
+        job_id = int(self._install_state.jobs[step])
         logger.debug(f"starting {step} job: {self._ws.config.host}#job/{job_id}")
         job_initial_run = self._ws.jobs.run_now(job_id)
         if job_initial_run.run_id:
             try:
                 self._ws.jobs.wait_get_run_job_terminated_or_skipped(run_id=job_initial_run.run_id)
             except OperationFailed as err:
+                logger.info('---------- REMOTE LOGS --------------')
+                self._relay_logs(step, job_initial_run.run_id)
+                logger.info('---------- END REMOTE LOGS ----------')
                 job_run = self._ws.jobs.get_run(job_initial_run.run_id)
                 raise self._infer_error_from_job_run(job_run) from err
             return
         raise NotFound(f"job run not found for {step}")
 
-    def create_jobs(self):
-        logger.debug(f"Creating jobs from tasks in {main.__name__}")
-        remote_wheel = self._upload_wheel()
-        desired_steps = {t.workflow for t in _TASKS.values() if t.cloud_compatible(self._ws.config)}
-        wheel_runner = None
-
-        if self._config.override_clusters:
-            wheel_runner = self._upload_wheel_runner(remote_wheel)
-        for step_name in desired_steps:
-            settings = self._job_settings(step_name, remote_wheel)
-            if self._config.override_clusters:
-                settings = self._apply_cluster_overrides(settings, self._config.override_clusters, wheel_runner)
-            self._deploy_workflow(step_name, settings)
-
-        for step_name, job_id in self._state.jobs.items():
-            if step_name not in desired_steps:
-                try:
-                    logger.info(f"Removing job_id={job_id}, as it is no longer needed")
-                    self._ws.jobs.delete(job_id)
-                except InvalidParameterValue:
-                    logger.warning(f"step={step_name} does not exist anymore for some reason")
-                    continue
-
-        self._state.save()
-        self._create_debug(remote_wheel)
-
     def repair_run(self, workflow):
         try:
             job_id, run_id = self._repair_workflow(workflow)
             run_details = self._ws.jobs.get_run(run_id=run_id, include_history=True)
             latest_repair_run_id = run_details.repair_history[-1].id
             job_url = f"{self._ws.config.host}#job/{job_id}/run/{run_id}"
-            logger.debug(f"Repair Running {workflow} job: {job_url}")
+            logger.debug(f"Repairing {workflow} job: {job_url}")
             self._ws.jobs.repair_run(run_id=run_id, rerun_all_failed_tasks=True, latest_repair_id=latest_repair_run_id)
             webbrowser.open(job_url)
         except InvalidParameterValue as e:
-            logger.warning(f"skipping {workflow}: {e}")
+            logger.warning(f"Skipping {workflow}: {e}")
         except TimeoutError:
             logger.warning(f"Skipping the {workflow} due to time out. Please try after sometime")
 
     def latest_job_status(self) -> list[dict]:
         latest_status = []
-        for step, job_id in self._state.jobs.items():
+        for step, job_id in self._install_state.jobs.items():
             job_state = None
             start_time = None
             try:
                 job_runs = list(self._ws.jobs.list_runs(job_id=int(job_id), limit=1))
             except InvalidParameterValue as e:
                 logger.warning(f"skipping {step}: {e}")
                 continue
@@ -217,15 +173,15 @@
                         "<never run>" if not (job_runs and start_time) else self._readable_timedelta(start_time)
                     ),
                 }
             )
         return latest_status
 
     def validate_step(self, step: str) -> bool:
-        job_id = int(self.state.jobs[step])
+        job_id = int(self._install_state.jobs[step])
         logger.debug(f"Validating {step} workflow: {self._ws.config.host}#job/{job_id}")
         current_runs = list(self._ws.jobs.list_runs(completed_only=False, job_id=job_id))
         for run in current_runs:
             if run.state and run.state.result_state == RunResultState.SUCCESS:
                 return True
         for run in current_runs:
             if (
@@ -235,47 +191,110 @@
             ):
                 logger.info("Identified a run in progress waiting for run completion")
                 self._ws.jobs.wait_get_run_job_terminated_or_skipped(run_id=run.run_id)
                 run_new_state = self._ws.jobs.get_run(run_id=run.run_id).state
                 return run_new_state is not None and run_new_state.result_state == RunResultState.SUCCESS
         return False
 
-    @property
-    def _config_file(self):
-        return f"{self._installation.install_folder()}/config.yml"
+    def relay_logs(self, workflow: str | None = None):
+        latest_run = None
+        if not workflow:
+            runs = []
+            for step in self._install_state.jobs:
+                try:
+                    _, latest_run = self._latest_job_run(step)
+                    runs.append((step, latest_run))
+                except InvalidParameterValue:
+                    continue
+            if not runs:
+                logger.warning("No jobs to relay logs for")
+                return
+            runs = sorted(runs, key=lambda x: x[1].start_time, reverse=True)
+            workflow, latest_run = runs[0]
+        if not latest_run:
+            assert workflow is not None
+            _, latest_run = self._latest_job_run(workflow)
+        self._relay_logs(workflow, latest_run.run_id)
+
+    def _relay_logs(self, workflow, run_id):
+        for record in self._fetch_logs(workflow, run_id):
+            task_logger = logging.getLogger(record.component)
+            task_logger.setLevel(logger.getEffectiveLevel())
+            log_level = logging.getLevelName(record.level)
+            task_logger.log(log_level, record.message)
+
+    def _fetch_logs(self, workflow: str, run_id: str) -> Iterator[PartialLogRecord]:
+        log_path = f'{self._install_state.install_folder()}/logs/{workflow}'
+        run_folders = []
+        for run_folder in self._ws.workspace.list(log_path):
+            if not run_folder.path or run_folder.object_type != ObjectType.DIRECTORY:
+                continue
+            if f'run-{run_id}-' not in run_folder.path:
+                continue
+            run_folders.append(run_folder.path)
+        if not run_folders:
+            return
+        # sort folders based on the last repair attempt
+        last_attempt = sorted(run_folders, key=lambda _: int(_.split('-')[-1]), reverse=True)[0]
+        for object_info in self._ws.workspace.list(last_attempt):
+            if not object_info.path:
+                continue
+            if '.log' not in object_info.path:
+                continue
+            task_name = os.path.basename(object_info.path).split('.')[0]
+            with self._ws.workspace.download(object_info.path) as raw_file:
+                text_io = StringIO(raw_file.read().decode())
+            for record in parse_logs(text_io):
+                yield replace(record, component=f'{record.component}:{task_name}')
 
-    def _job_cluster_spark_conf(self, cluster_key: str):
-        conf_from_installation = self._config.spark_conf if self._config.spark_conf else {}
-        if cluster_key == "main":
-            spark_conf = {
-                "spark.databricks.cluster.profile": "singleNode",
-                "spark.master": "local[*]",
-            }
-            return spark_conf | conf_from_installation
-        if cluster_key == "tacl":
-            return {"spark.databricks.acl.sqlOnly": "true"} | conf_from_installation
-        if cluster_key == "table_migration":
-            return {"spark.sql.sources.parallelPartitionDiscovery.parallelism": "200"} | conf_from_installation
-        return conf_from_installation
+    @staticmethod
+    def _readable_timedelta(epoch):
+        when = datetime.utcfromtimestamp(epoch)
+        duration = datetime.now() - when
+        data = {}
+        data["days"], remaining = divmod(duration.total_seconds(), 86_400)
+        data["hours"], remaining = divmod(remaining, 3_600)
+        data["minutes"], data["seconds"] = divmod(remaining, 60)
+
+        time_parts = ((name, round(value)) for (name, value) in data.items())
+        time_parts = [f"{value} {name[:-1] if value == 1 else name}" for name, value in time_parts if value > 0]
+        if len(time_parts) > 0:
+            time_parts.append("ago")
+        if time_parts:
+            return " ".join(time_parts)
+        return "less than 1 second ago"
 
-    def _deploy_workflow(self, step_name: str, settings):
-        if step_name in self._state.jobs:
-            try:
-                job_id = int(self._state.jobs[step_name])
-                logger.info(f"Updating configuration for step={step_name} job_id={job_id}")
-                return self._ws.jobs.reset(job_id, jobs.JobSettings(**settings))
-            except InvalidParameterValue:
-                del self._state.jobs[step_name]
-                logger.warning(f"step={step_name} does not exist anymore for some reason")
-                return self._deploy_workflow(step_name, settings)
-        logger.info(f"Creating new job configuration for step={step_name}")
-        new_job = self._ws.jobs.create(**settings)
-        assert new_job.job_id is not None
-        self._state.jobs[step_name] = str(new_job.job_id)
-        return None
+    def _repair_workflow(self, workflow):
+        job_id, latest_job_run = self._latest_job_run(workflow)
+        retry_on_attribute_error = retried(on=[AttributeError], timeout=self._verify_timeout)
+        retried_check = retry_on_attribute_error(self._get_result_state)
+        state_value = retried_check(job_id)
+        logger.info(f"The status for the latest run is {state_value}")
+        if state_value != "FAILED":
+            raise InvalidParameterValue("job is not in FAILED state hence skipping repair")
+        run_id = latest_job_run.run_id
+        return job_id, run_id
+
+    def _latest_job_run(self, workflow: str):
+        job_id = self._install_state.jobs.get(workflow)
+        if not job_id:
+            raise InvalidParameterValue("job does not exists hence skipping repair")
+        job_runs = list(self._ws.jobs.list_runs(job_id=job_id, limit=1))
+        if not job_runs:
+            raise InvalidParameterValue("job is not initialized yet. Can't trigger repair run now")
+        latest_job_run = job_runs[0]
+        return job_id, latest_job_run
+
+    def _get_result_state(self, job_id):
+        job_runs = list(self._ws.jobs.list_runs(job_id=job_id, limit=1))
+        latest_job_run = job_runs[0]
+        if not latest_job_run.state.result_state:
+            raise AttributeError("no result state in job run")
+        job_state = latest_job_run.state.result_state.value
+        return job_state
 
     def _infer_error_from_job_run(self, job_run) -> Exception:
         errors: list[Exception] = []
         timeouts: list[DeadlineExceeded] = []
         assert job_run.tasks is not None
         for run_task in job_run.tasks:
             error = self._infer_error_from_task_run(run_task)
@@ -340,97 +359,258 @@
             DataLoss,
             ValueError,
             KeyError,
         ]
         constructors: dict[re.Pattern, type[Exception]] = {
             re.compile(r".*\[TABLE_OR_VIEW_NOT_FOUND] (.*)"): NotFound,
             re.compile(r".*\[SCHEMA_NOT_FOUND] (.*)"): NotFound,
+            re.compile(r".*\[TimeoutException] (.*)"): TimeoutError,
         }
         for klass in needles:
             constructors[re.compile(f".*{klass.__name__}: (.*)")] = klass
         for pattern, klass in constructors.items():
             match = pattern.match(haystack)
             if match:
                 return klass(match.group(1))
         return Unknown(haystack)
 
-    def _upload_wheel(self):
+
+class WorkflowsDeployment(InstallationMixin):
+    def __init__(  # pylint: disable=too-many-arguments
+        self,
+        config: WorkspaceConfig,
+        installation: Installation,
+        install_state: InstallState,
+        ws: WorkspaceClient,
+        wheels: WheelsV2,
+        product_info: ProductInfo,
+        verify_timeout: timedelta,
+        tasks: list[Task],
+        skip_dashboards=False,
+    ):
+        self._config = config
+        self._installation = installation
+        self._ws = ws
+        self._install_state = install_state
+        self._wheels = wheels
+        self._product_info = product_info
+        self._verify_timeout = verify_timeout
+        self._tasks = tasks
+        self._this_file = Path(__file__)
+        self._skip_dashboards = skip_dashboards
+        super().__init__(config, installation, ws)
+
+    def create_jobs(self, prompts):
+        remote_wheel = self._upload_wheel(prompts)
+        desired_workflows = {t.workflow for t in self._tasks if t.cloud_compatible(self._ws.config)}
+        wheel_runner = None
+
+        if self._config.override_clusters:
+            wheel_runner = self._upload_wheel_runner(remote_wheel)
+        for workflow_name in desired_workflows:
+            settings = self._job_settings(workflow_name, remote_wheel)
+            if self._config.override_clusters:
+                settings = self._apply_cluster_overrides(
+                    workflow_name,
+                    settings,
+                    self._config.override_clusters,
+                    wheel_runner,
+                )
+            self._deploy_workflow(workflow_name, settings)
+
+        for workflow_name, job_id in self._install_state.jobs.items():
+            if workflow_name not in desired_workflows:
+                try:
+                    logger.info(f"Removing job_id={job_id}, as it is no longer needed")
+                    self._ws.jobs.delete(job_id)
+                except InvalidParameterValue:
+                    logger.warning(f"step={workflow_name} does not exist anymore for some reason")
+                    continue
+
+        self._install_state.save()
+        self._create_debug(remote_wheel)
+        return self._create_readme()
+
+    @property
+    def _config_file(self):
+        return f"{self._installation.install_folder()}/config.yml"
+
+    def _is_testing(self):
+        return self._product_info.product_name() != "ucx"
+
+    def _create_readme(self) -> str:
+        debug_notebook_link = self._installation.workspace_markdown_link('debug notebook', 'DEBUG.py')
+        markdown = [
+            "# UCX - The Unity Catalog Migration Assistant",
+            f'To troubleshoot, see {debug_notebook_link}.\n',
+            "Here are the URLs and descriptions of workflows that trigger various stages of migration.",
+            "All jobs are defined with necessary cluster configurations and DBR versions.\n",
+        ]
+        for step_name in self._step_list():
+            if step_name not in self._install_state.jobs:
+                logger.warning(f"Skipping step '{step_name}' since it was not deployed.")
+                continue
+            job_id = self._install_state.jobs[step_name]
+            dashboard_link = ""
+            if not self._skip_dashboards:
+                dashboard_link = self._create_dashboard_links(step_name, dashboard_link)
+            job_link = f"[{self._name(step_name)}]({self._ws.config.host}#job/{job_id})"
+            markdown.append("---\n\n")
+            markdown.append(f"## {job_link}\n\n")
+            markdown.append(f"{dashboard_link}")
+            markdown.append("\nThe workflow consists of the following separate tasks:\n\n")
+            for task in self._tasks:
+                if self._is_testing() and task.is_testing():
+                    continue
+                if task.workflow != step_name:
+                    continue
+                doc = self._config.replace_inventory_variable(task.doc)
+                markdown.append(f"### `{task.name}`\n\n")
+                markdown.append(f"{doc}\n")
+                markdown.append("\n\n")
+        preamble = ["# Databricks notebook source", "# MAGIC %md"]
+        intro = "\n".join(preamble + [f"# MAGIC {line}" for line in markdown])
+        self._installation.upload('README.py', intro.encode('utf8'))
+        readme_url = self._installation.workspace_link('README')
+        return readme_url
+
+    def _create_dashboard_links(self, step_name, dashboard_link):
+        dashboards_per_step = [d for d in self._install_state.dashboards.keys() if d.startswith(step_name)]
+        for dash in dashboards_per_step:
+            if len(dashboard_link) == 0:
+                dashboard_link += "Go to the one of the following dashboards after running the job:\n"
+            first, second = dash.replace("_", " ").title().split()
+            dashboard_url = f"{self._ws.config.host}/sql/dashboards/{self._install_state.dashboards[dash]}"
+            dashboard_link += f"  - [{first} ({second}) dashboard]({dashboard_url})\n"
+        return dashboard_link
+
+    def _step_list(self) -> list[str]:
+        step_list = []
+        for task in self._tasks:
+            if self._is_testing() and task.is_testing():
+                continue
+            if task.workflow not in step_list:
+                step_list.append(task.workflow)
+        return step_list
+
+    def _job_cluster_spark_conf(self, cluster_key: str):
+        conf_from_installation = self._config.spark_conf if self._config.spark_conf else {}
+        if cluster_key == "main":
+            spark_conf = {
+                "spark.databricks.cluster.profile": "singleNode",
+                "spark.master": "local[*]",
+            }
+            return spark_conf | conf_from_installation
+        if cluster_key == "tacl":
+            return {"spark.databricks.acl.sqlOnly": "true"} | conf_from_installation
+        if cluster_key == "table_migration":
+            return {"spark.sql.sources.parallelPartitionDiscovery.parallelism": "200"} | conf_from_installation
+        return conf_from_installation
+
+    def _deploy_workflow(self, step_name: str, settings):
+        if step_name in self._install_state.jobs:
+            try:
+                job_id = int(self._install_state.jobs[step_name])
+                logger.info(f"Updating configuration for step={step_name} job_id={job_id}")
+                return self._ws.jobs.reset(job_id, jobs.JobSettings(**settings))
+            except InvalidParameterValue:
+                del self._install_state.jobs[step_name]
+                logger.warning(f"step={step_name} does not exist anymore for some reason")
+                return self._deploy_workflow(step_name, settings)
+        logger.info(f"Creating new job configuration for step={step_name}")
+        new_job = self._ws.jobs.create(**settings)
+        assert new_job.job_id is not None
+        self._install_state.jobs[step_name] = str(new_job.job_id)
+        return None
+
+    def _upload_wheel(self, prompts: Prompts):
         with self._wheels:
             try:
                 self._wheels.upload_to_dbfs()
             except PermissionDenied as err:
-                if not self._prompts:
+                if not prompts:
                     raise RuntimeWarning("no Prompts instance found") from err
                 logger.warning(f"Uploading wheel file to DBFS failed, DBFS is probably write protected. {err}")
-                configure_cluster_overrides = ConfigureClusterOverrides(self._ws, self._prompts.choice_from_dict)
+                configure_cluster_overrides = ConfigureClusterOverrides(self._ws, prompts.choice_from_dict)
                 self._config.override_clusters = configure_cluster_overrides.configure()
                 self._installation.save(self._config)
             return self._wheels.upload_to_wsfs()
 
     def _upload_wheel_runner(self, remote_wheel: str):
         # TODO: we have to be doing this workaround until ES-897453 is solved in the platform
         code = TEST_RUNNER_NOTEBOOK.format(remote_wheel=remote_wheel, config_file=self._config_file).encode("utf8")
         return self._installation.upload(f"wheels/wheel-test-runner-{self._product_info.version()}.py", code)
 
     @staticmethod
-    def _apply_cluster_overrides(settings: dict[str, Any], overrides: dict[str, str], wheel_runner: str) -> dict:
+    def _apply_cluster_overrides(
+        workflow_name: str,
+        settings: dict[str, Any],
+        overrides: dict[str, str],
+        wheel_runner: str,
+    ) -> dict:
         settings["job_clusters"] = [_ for _ in settings["job_clusters"] if _.job_cluster_key not in overrides]
         for job_task in settings["tasks"]:
             if job_task.job_cluster_key is None:
                 continue
             if job_task.job_cluster_key in overrides:
                 job_task.existing_cluster_id = overrides[job_task.job_cluster_key]
                 job_task.job_cluster_key = None
                 job_task.libraries = None
             if job_task.python_wheel_task is not None:
                 job_task.python_wheel_task = None
-                params = {"task": job_task.task_key} | EXTRA_TASK_PARAMS
-                job_task.notebook_task = jobs.NotebookTask(notebook_path=wheel_runner, base_parameters=params)
+                widget_values = {"task": job_task.task_key, 'workflow': workflow_name} | EXTRA_TASK_PARAMS
+                job_task.notebook_task = jobs.NotebookTask(notebook_path=wheel_runner, base_parameters=widget_values)
         return settings
 
     def _job_settings(self, step_name: str, remote_wheel: str):
         email_notifications = None
         if not self._config.override_clusters and "@" in self._my_username:
             # set email notifications only if we're running the real
             # installation and not the integration test.
             email_notifications = jobs.JobEmailNotifications(
                 on_success=[self._my_username], on_failure=[self._my_username]
             )
-        tasks = sorted(
-            [t for t in _TASKS.values() if t.workflow == step_name],
-            key=lambda _: _.name,
-        )
+        job_tasks = []
+        job_clusters: set[str] = {Task.job_cluster}
+        for task in self._tasks:
+            if task.workflow != step_name:
+                continue
+            if self._skip_dashboards and task.dashboard:
+                continue
+            job_clusters.add(task.job_cluster)
+            job_tasks.append(self._job_task(task, remote_wheel))
+        job_tasks.append(self._job_parse_logs_task(job_tasks, step_name, remote_wheel))
         version = self._product_info.version()
         version = version if not self._ws.config.is_gcp else version.replace("+", "-")
         return {
             "name": self._name(step_name),
             "tags": {"version": f"v{version}"},
-            "job_clusters": self._job_clusters({t.job_cluster for t in tasks}),
+            "job_clusters": self._job_clusters(job_clusters),
             "email_notifications": email_notifications,
-            "tasks": [self._job_task(task, remote_wheel) for task in tasks],
+            "tasks": job_tasks,
         }
 
     def _job_task(self, task: Task, remote_wheel: str) -> jobs.Task:
         jobs_task = jobs.Task(
             task_key=task.name,
             job_cluster_key=task.job_cluster,
-            depends_on=[jobs.TaskDependency(task_key=d) for d in _TASKS[task.name].dependencies()],
+            depends_on=[jobs.TaskDependency(task_key=d) for d in task.dependencies()],
         )
         if task.dashboard:
             # dashboards are created in parallel to wheel uploads, so we'll just retry
             retry_on_attribute_error = retried(on=[KeyError], timeout=self._verify_timeout)
             retried_job_dashboard_task = retry_on_attribute_error(self._job_dashboard_task)
             return retried_job_dashboard_task(jobs_task, task)
         if task.notebook:
             return self._job_notebook_task(jobs_task, task)
-        return self._job_wheel_task(jobs_task, task, remote_wheel)
+        return self._job_wheel_task(jobs_task, task.workflow, remote_wheel)
 
     def _job_dashboard_task(self, jobs_task: jobs.Task, task: Task) -> jobs.Task:
         assert task.dashboard is not None
-        dashboard_id = self._state.dashboards[task.dashboard]
+        dashboard_id = self._install_state.dashboards[task.dashboard]
         return replace(
             jobs_task,
             job_cluster_key=None,
             sql_task=jobs.SqlTask(
                 warehouse_id=self._warehouse_id,
                 dashboard=jobs.SqlTaskDashboard(dashboard_id=dashboard_id),
             ),
@@ -450,29 +630,33 @@
                     "task": task.name,
                     "config": f"/Workspace{self._config_file}",
                 }
                 | EXTRA_TASK_PARAMS,
             ),
         )
 
-    def _job_wheel_task(self, jobs_task: jobs.Task, task: Task, remote_wheel: str) -> jobs.Task:
-        if "table_migration" in task.job_cluster:
+    def _job_wheel_task(self, jobs_task: jobs.Task, workflow: str, remote_wheel: str) -> jobs.Task:
+        if jobs_task.job_cluster_key is not None and "table_migration" in jobs_task.job_cluster_key:
             # Shared mode cluster cannot use dbfs, need to use WSFS
             libraries = [compute.Library(whl=f"/Workspace{remote_wheel}")]
         else:
-            # TODO: check when we can install wheels from WSFS properly
-            # None UC cluster cannot use WSFS, need to use dbfs
+            # TODO: https://github.com/databrickslabs/ucx/issues/1098
             libraries = [compute.Library(whl=f"dbfs:{remote_wheel}")]
+        named_parameters = {
+            "config": f"/Workspace{self._config_file}",
+            "workflow": workflow,
+            "task": jobs_task.task_key,
+        }
         return replace(
             jobs_task,
             libraries=libraries,
             python_wheel_task=jobs.PythonWheelTask(
                 package_name="databricks_labs_ucx",
                 entry_point="runtime",  # [project.entry-points.databricks] in pyproject.toml
-                named_parameters={"task": task.name, "config": f"/Workspace{self._config_file}"} | EXTRA_TASK_PARAMS,
+                named_parameters=named_parameters | EXTRA_TASK_PARAMS,
             ),
         )
 
     def _job_clusters(self, names: set[str]):
         clusters = []
         if "main" in names:
             clusters.append(
@@ -496,14 +680,15 @@
                         spark_conf=self._job_cluster_spark_conf("tacl"),
                         num_workers=1,  # ShowPermissionsCommand needs a worker
                         policy_id=self._config.policy_id,
                     ),
                 )
             )
         if "table_migration" in names:
+            # TODO: rename to "user-isolation", so that we can use it in group migration workflows
             clusters.append(
                 jobs.JobCluster(
                     job_cluster_key="table_migration",
                     new_cluster=compute.ClusterSpec(
                         data_security_mode=compute.DataSecurityMode.USER_ISOLATION,
                         spark_conf=self._job_cluster_spark_conf("table_migration"),
                         policy_id=self._config.policy_id,
@@ -512,42 +697,27 @@
                             min_workers=self._config.min_workers,
                         ),
                     ),
                 )
             )
         return clusters
 
+    def _job_parse_logs_task(self, job_tasks: list[jobs.Task], workflow: str, remote_wheel: str) -> jobs.Task:
+        jobs_task = jobs.Task(
+            task_key="parse_logs",
+            job_cluster_key=Task.job_cluster,
+            # The task dependents on all previous tasks.
+            depends_on=[jobs.TaskDependency(task_key=task.task_key) for task in job_tasks],
+            run_if=jobs.RunIf.ALL_DONE,
+        )
+        return self._job_wheel_task(jobs_task, workflow, remote_wheel)
+
     def _create_debug(self, remote_wheel: str):
         readme_link = self._installation.workspace_link('README')
         job_links = ", ".join(
             f"[{self._name(step_name)}]({self._ws.config.host}#job/{job_id})"
-            for step_name, job_id in self._state.jobs.items()
+            for step_name, job_id in self._install_state.jobs.items()
         )
         content = DEBUG_NOTEBOOK.format(
             remote_wheel=remote_wheel, readme_link=readme_link, job_links=job_links, config_file=self._config_file
         ).encode("utf8")
         self._installation.upload('DEBUG.py', content)
-
-    def _repair_workflow(self, workflow):
-        job_id = self._state.jobs.get(workflow)
-        if not job_id:
-            raise InvalidParameterValue("job does not exists hence skipping repair")
-        job_runs = list(self._ws.jobs.list_runs(job_id=job_id, limit=1))
-        if not job_runs:
-            raise InvalidParameterValue("job is not initialized yet. Can't trigger repair run now")
-        latest_job_run = job_runs[0]
-        retry_on_attribute_error = retried(on=[AttributeError], timeout=self._verify_timeout)
-        retried_check = retry_on_attribute_error(self._get_result_state)
-        state_value = retried_check(job_id)
-        logger.info(f"The status for the latest run is {state_value}")
-        if state_value != "FAILED":
-            raise InvalidParameterValue("job is not in FAILED state hence skipping repair")
-        run_id = latest_job_run.run_id
-        return job_id, run_id
-
-    def _get_result_state(self, job_id):
-        job_runs = list(self._ws.jobs.list_runs(job_id=job_id, limit=1))
-        latest_job_run = job_runs[0]
-        if not latest_job_run.state.result_state:
-            raise AttributeError("no result state in job run")
-        job_state = latest_job_run.state.result_state.value
-        return job_state
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/mixins/fixtures.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from collections.abc import Callable, Generator, MutableMapping
 from datetime import timedelta
 from pathlib import Path
 from typing import BinaryIO
 
 import pytest
 from databricks.labs.lsql.backends import StatementExecutionBackend
+from databricks.labs.blueprint.commands import CommandExecutor
 from databricks.sdk import AccountClient, WorkspaceClient
 from databricks.sdk.core import DatabricksError
 from databricks.sdk.errors import NotFound, ResourceConflict
 from databricks.sdk.retries import retried
 from databricks.sdk.service import compute, iam, jobs, pipelines, sql, workspace
 from databricks.sdk.service._internal import Wait
 from databricks.sdk.service.catalog import (
@@ -40,18 +41,17 @@
 from databricks.sdk.service.sql import (
     CreateWarehouseRequestWarehouseType,
     GetResponse,
     ObjectTypePlural,
     Query,
     QueryInfo,
 )
-from databricks.sdk.service.workspace import ImportFormat
+from databricks.sdk.service.workspace import ImportFormat, Language
 
 from databricks.labs.ucx.workspace_access.groups import MigratedGroup
-from databricks.labs.ucx.workspace_access.manager import PermissionManager
 
 # this file will get to databricks-labs-pytester project and be maintained/refactored there
 # pylint: disable=redefined-outer-name,too-many-try-statements,import-outside-toplevel,unnecessary-lambda,too-complex,invalid-name
 
 logger = logging.getLogger(__name__)
 
 
@@ -158,19 +158,14 @@
         host=debug_env["DATABRICKS_HOST"],
         account_id=debug_env["DATABRICKS_ACCOUNT_ID"],
         product=product_name,
         product_version=product_version,
     )
 
 
-@pytest.fixture
-def permission_manager(ws, sql_backend, inventory_schema) -> PermissionManager:
-    return PermissionManager.factory(ws, sql_backend, inventory_schema)
-
-
 def _permissions_mapping():
     from databricks.sdk.service.iam import PermissionLevel
 
     def _simple(_, object_id):
         return object_id
 
     def _path(ws, path):
@@ -557,20 +552,28 @@
         return scope, principal
 
     yield from factory("secret scope acl", create, lambda x: ws.secrets.delete_acl(x[0], x[1]))
 
 
 @pytest.fixture
 def make_notebook(ws, make_random):
-    def create(*, path: str | None = None, content: BinaryIO | None = None, **kwargs):
+    def create(
+        *,
+        path: str | None = None,
+        content: BinaryIO | None = None,
+        language: Language = Language.PYTHON,
+        format: ImportFormat = ImportFormat.SOURCE,  # pylint:  disable=redefined-builtin
+        overwrite: bool = False,
+    ) -> str:
         if path is None:
-            path = f"/Users/{ws.current_user.me().user_name}/sdk-{make_random(4)}.py"
+            path = f"/Users/{ws.current_user.me().user_name}/sdk-{make_random(4)}"
         if content is None:
             content = io.BytesIO(b"print(1)")
-        ws.workspace.upload(path, content, **kwargs)
+        path = str(path)
+        ws.workspace.upload(path, content, language=language, format=format, overwrite=overwrite)
         return path
 
     yield from factory("notebook", create, lambda x: ws.workspace.delete(x))
 
 
 @pytest.fixture
 def make_directory(ws, make_random):
@@ -698,15 +701,15 @@
                     "spark.databricks.cluster.profile": "singleNode",
                     "spark.master": "local[*]",
                 }
             else:
                 kwargs["spark_conf"] = {"spark.databricks.cluster.profile": "singleNode", "spark.master": "local[*]"}
             kwargs["custom_tags"] = {"ResourceClass": "SingleNode"}
         if "instance_pool_id" not in kwargs:
-            kwargs["node_type_id"] = ws.clusters.select_node_type(local_disk=True)
+            kwargs["node_type_id"] = ws.clusters.select_node_type(local_disk=True, min_memory_gb=16)
 
         return ws.clusters.create(
             cluster_name=cluster_name,
             spark_version=spark_version,
             autotermination_minutes=autotermination_minutes,
             **kwargs,
         )
@@ -739,15 +742,15 @@
 
 @pytest.fixture
 def make_instance_pool(ws, make_random):
     def create(*, instance_pool_name=None, node_type_id=None, **kwargs):
         if instance_pool_name is None:
             instance_pool_name = f"sdk-{make_random(4)}"
         if node_type_id is None:
-            node_type_id = ws.clusters.select_node_type(local_disk=True)
+            node_type_id = ws.clusters.select_node_type(local_disk=True, min_memory_gb=16)
         return ws.instance_pools.create(instance_pool_name, node_type_id, **kwargs)
 
     yield from factory("instance pool", create, lambda item: ws.instance_pools.delete(item.instance_pool_id))
 
 
 @pytest.fixture
 def make_job(ws, make_random, make_notebook):
@@ -762,30 +765,30 @@
             if task_spark_conf:
                 kwargs["tasks"] = [
                     jobs.Task(
                         task_key=make_random(4),
                         description=make_random(4),
                         new_cluster=compute.ClusterSpec(
                             num_workers=1,
-                            node_type_id=ws.clusters.select_node_type(local_disk=True),
+                            node_type_id=ws.clusters.select_node_type(local_disk=True, min_memory_gb=16),
                             spark_version=ws.clusters.select_spark_version(latest=True),
                             spark_conf=task_spark_conf,
                         ),
                         notebook_task=jobs.NotebookTask(notebook_path=make_notebook()),
                         timeout_seconds=0,
                     )
                 ]
             else:
                 kwargs["tasks"] = [
                     jobs.Task(
                         task_key=make_random(4),
                         description=make_random(4),
                         new_cluster=compute.ClusterSpec(
                             num_workers=1,
-                            node_type_id=ws.clusters.select_node_type(local_disk=True),
+                            node_type_id=ws.clusters.select_node_type(local_disk=True, min_memory_gb=16),
                             spark_version=ws.clusters.select_spark_version(latest=True),
                         ),
                         notebook_task=jobs.NotebookTask(notebook_path=make_notebook()),
                         timeout_seconds=0,
                     )
                 ]
         job = ws.jobs.create(**kwargs)
@@ -818,15 +821,15 @@
         if "name" not in kwargs:
             kwargs["name"] = f"sdk-{make_random(4)}"
         if "libraries" not in kwargs:
             kwargs["libraries"] = [pipelines.PipelineLibrary(notebook=pipelines.NotebookLibrary(path=make_notebook()))]
         if "clusters" not in kwargs:
             kwargs["clusters"] = [
                 pipelines.PipelineCluster(
-                    node_type_id=ws.clusters.select_node_type(local_disk=True),
+                    node_type_id=ws.clusters.select_node_type(local_disk=True, min_memory_gb=16),
                     label="default",
                     num_workers=1,
                     custom_tags={
                         "cluster_type": "default",
                     },
                 )
             ]
@@ -947,57 +950,70 @@
         schema_info = SchemaInfo(catalog_name=catalog_name, name=name, full_name=full_name)
         logger.info(
             f"Schema {schema_info.full_name}: "
             f"{ws.config.host}/explore/data/{schema_info.catalog_name}/{schema_info.name}"
         )
         return schema_info
 
-    yield from factory(
-        "schema",
-        create,
-        lambda schema_info: sql_backend.execute(f"DROP SCHEMA IF EXISTS {schema_info.full_name} CASCADE"),
-    )
+    def remove(schema_info: SchemaInfo):
+        try:
+            sql_backend.execute(f"DROP SCHEMA IF EXISTS {schema_info.full_name} CASCADE")
+        except RuntimeError as e:
+            if "SCHEMA_NOT_FOUND" in str(e):
+                logger.warning("Schema was already dropped while executing the test", exc_info=e)
+            else:
+                raise e
+
+    yield from factory("schema", create, remove)
 
 
 @pytest.fixture
 # pylint: disable-next=too-many-statements
 def make_table(ws, sql_backend, make_schema, make_random) -> Generator[Callable[..., TableInfo], None, None]:
-    def create(
+    def create(  # pylint: disable=too-many-locals,too-many-arguments
         *,
         catalog_name="hive_metastore",
         schema_name: str | None = None,
         name: str | None = None,
         ctas: str | None = None,
         non_delta: bool = False,
         external: bool = False,
         external_csv: str | None = None,
         view: bool = False,
         tbl_properties: dict[str, str] | None = None,
+        hiveserde_ddl: str | None = None,
+        storage_override: str | None = None,
     ) -> TableInfo:
         if schema_name is None:
             schema = make_schema(catalog_name=catalog_name)
             catalog_name = schema.catalog_name
             schema_name = schema.name
         if name is None:
             name = f"ucx_T{make_random(4)}".lower()
         table_type: TableType | None = None
         data_source_format = None
         storage_location = None
+        view_text = None
         full_name = f"{catalog_name}.{schema_name}.{name}".lower()
         ddl = f'CREATE {"VIEW" if view else "TABLE"} {full_name}'
         if view:
             table_type = TableType.VIEW
+            view_text = ctas
         if ctas is not None:
             # temporary (if not view)
             ddl = f"{ddl} AS {ctas}"
         elif non_delta:
-            table_type = TableType.MANAGED  # pylint: disable=redefined-variable-type
+            table_type = TableType.EXTERNAL  # pylint: disable=redefined-variable-type
             data_source_format = DataSourceFormat.JSON
-            storage_location = "dbfs:/databricks-datasets/iot-stream/data-device"
-            ddl = f"{ddl} USING json LOCATION '{storage_location}'"
+            storage_location = f"dbfs:/tmp/ucx_test_{make_random(4)}"
+            # Modified, otherwise it will identify the table as a DB Dataset
+            ddl = (
+                f"{ddl} USING json location '{storage_location}' as SELECT * FROM "
+                f"JSON.`dbfs:/databricks-datasets/iot-stream/data-device`"
+            )
         elif external_csv is not None:
             table_type = TableType.EXTERNAL
             data_source_format = DataSourceFormat.CSV
             storage_location = external_csv
             ddl = f"{ddl} USING CSV OPTIONS (header=true) LOCATION '{storage_location}'"
         elif external:
             # external table
@@ -1012,23 +1028,30 @@
             data_source_format = DataSourceFormat.DELTA
             storage_location = f"dbfs:/user/hive/warehouse/{schema_name}/{name}"
             ddl = f"{ddl} (id INT, value STRING)"
         if tbl_properties:
             str_properties = ",".join([f" '{k}' = '{v}' " for k, v in tbl_properties.items()])
             ddl = f"{ddl} TBLPROPERTIES ({str_properties})"
 
+        if hiveserde_ddl:
+            ddl = hiveserde_ddl
+            data_source_format = None
+            table_type = TableType.EXTERNAL
+            storage_location = storage_override
+
         sql_backend.execute(ddl)
         table_info = TableInfo(
             catalog_name=catalog_name,
             schema_name=schema_name,
             name=name,
             full_name=full_name,
             properties=tbl_properties,
             storage_location=storage_location,
             table_type=table_type,
+            view_definition=view_text,
             data_source_format=data_source_format,
         )
         logger.info(
             f"Table {table_info.full_name}: "
             f"{ws.config.host}/explore/data/{table_info.catalog_name}/{table_info.schema_name}/{table_info.name}"
         )
         return table_info
@@ -1177,16 +1200,56 @@
         except RuntimeError as e:
             logger.info(f"Can't remove feature table {e}")
 
     yield from factory("Feature table", create, remove)
 
 
 @pytest.fixture
-def make_dbfs_data_copy(ws):
+def make_dbfs_data_copy(ws, make_cluster, env_or_skip):
+    if ws.config.is_aws:
+        cmd_exec = CommandExecutor(ws.clusters, ws.command_execution, lambda: env_or_skip("TEST_WILDCARD_CLUSTER_ID"))
+
     def create(*, src_path: str, dst_path: str):
-        ws.dbfs.copy(src_path, dst_path, recursive=True)
+        if ws.config.is_aws:
+            cmd_exec.run(f"dbutils.fs.cp('{src_path}', '{dst_path}', recurse=True)")
+        else:
+            ws.dbfs.copy(src_path, dst_path, recursive=True)
         return dst_path
 
     def remove(dst_path: str):
-        ws.dbfs.delete(dst_path, recursive=True)
+        if ws.config.is_aws:
+            cmd_exec.run(f"dbutils.fs.rm('{dst_path}', recurse=True)")
+        else:
+            ws.dbfs.delete(dst_path, recursive=True)
 
     yield from factory("make_dbfs_data_copy", create, remove)
+
+
+@pytest.fixture
+def make_mounted_location(make_random, make_dbfs_data_copy, env_or_skip):
+    # make a copy of src data to a new location to avoid overlapping UC table path that will fail other
+    # external table migration tests
+    existing_mounted_location = f'dbfs:/mnt/{env_or_skip("TEST_MOUNT_NAME")}/a/b/c'
+    new_mounted_location = f'dbfs:/mnt/{env_or_skip("TEST_MOUNT_NAME")}/a/b/{make_random(4)}'
+    make_dbfs_data_copy(src_path=existing_mounted_location, dst_path=new_mounted_location)
+    return new_mounted_location
+
+
+@pytest.fixture
+def make_storage_dir(ws, env_or_skip):
+    if ws.config.is_aws:
+        cmd_exec = CommandExecutor(ws.clusters, ws.command_execution, lambda: env_or_skip("TEST_WILDCARD_CLUSTER_ID"))
+
+    def create(*, path: str):
+        if ws.config.is_aws:
+            cmd_exec.run(f"dbutils.fs.mkdirs('{path}')")
+        else:
+            ws.dbfs.mkdirs(path)
+        return path
+
+    def remove(path: str):
+        if ws.config.is_aws:
+            cmd_exec.run(f"dbutils.fs.rm('{path}', recurse=True)")
+        else:
+            ws.dbfs.delete(path, recursive=True)
+
+    yield from factory("make_storage_dir", create, remove)
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/mixins/redash.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/mixins/redash.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/00_0_metastore_assignment.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/01_0_group_migration.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/02_0_data_modeling.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/03_0_data_migration.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/estimates/03_5_data_migration_complexity.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/00_0_interactive.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/01_0_compute_access_mode_limitation_summary.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/02_0_cluster_summary.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/interactive/03_0_cluster_summary.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/02_2_count_table_by_storage.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/10_0_all_tables.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/assessment/main/10_0_database_summary.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/views/code_patterns.sql` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/code_patterns.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/views/grant_detail.sql` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/grant_detail.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/views/misc_patterns.sql` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/misc_patterns.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/views/objects.sql` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/objects.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/queries/views/table_estimates.sql` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/queries/views/table_estimates.sql`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/source_code/base.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,14 +78,33 @@
     @abstractmethod
     def name(self) -> str: ...
 
     @abstractmethod
     def apply(self, code: str) -> str: ...
 
 
+# The default schema to use when the schema is not specified in a table reference
+# See: https://spark.apache.org/docs/3.0.0-preview/sql-ref-syntax-qry-select-usedb.html
+DEFAULT_SCHEMA = 'default'
+
+
+@dataclass
+class CurrentSessionState:
+    """
+    A data class that represents the current state of a session.
+
+    This class can be used to track various aspects of a session, such as the current schema.
+
+    Attributes:
+        schema (str): The current schema of the session. If not provided, it defaults to 'DEFAULT_SCHEMA'.
+    """
+
+    schema: str = DEFAULT_SCHEMA
+
+
 class SequentialLinter(Linter):
     def __init__(self, linters: list[Linter]):
         self._linters = linters
 
     def lint(self, code: str) -> Iterable[Advice]:
         for linter in self._linters:
             yield from linter.lint(code)
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/source_code/lsp.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/lsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from pathlib import Path
 from typing import Any
 from urllib.parse import parse_qsl
 
 from databricks.labs.blueprint.logger import install_logger
 from databricks.sdk.service.workspace import Language
 
-from databricks.labs.ucx.hive_metastore.table_migrate import (
-    MigrationIndex,
+from databricks.labs.ucx.hive_metastore.migration_status import (
     MigrationStatus,
 )
+from databricks.labs.ucx.hive_metastore.migration_status import MigrationIndex
 from databricks.labs.ucx.source_code.base import (
     Advice,
     Advisory,
     Convention,
     Deprecation,
     Failure,
 )
@@ -297,15 +297,14 @@
         logger.debug(f"Received:\n{raw}")
 
         rng = Range.from_dict(raw['range'])
         response = self._lsp_server.quickfix(raw['file_uri'], rng, raw['code'])
 
         raw = json.dumps(response.as_dict()).encode('utf-8')
         self.wfile.write(raw)
-        # self.wfile.flush()
 
     def do_GET(self):  # pylint: disable=invalid-name
         if not self.path.startswith('/lint'):
             self.send_error(400, 'Wrong input')
             return
         parts = self.path.split('?')
         if len(parts) != 2:
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/source_code/redash.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/source_code/redash.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.15.0_added_cluster_policy.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.16.0_changing_cluster_table_schema.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/upgrades/v0.20.0_add_is_partitioned_column.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/clusters.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/clusters.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/generic.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/generic.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     TemporarilyUnavailable,
 )
 from databricks.sdk.retries import retried
 from databricks.sdk.service import iam, ml
 from databricks.sdk.service.iam import PermissionLevel
 
 from databricks.labs.ucx.framework.crawlers import CrawlerBase
-from databricks.labs.ucx.workspace_access.base import AclSupport, Permissions
+from databricks.labs.ucx.workspace_access.base import AclSupport, Permissions, StaticListing
 from databricks.labs.ucx.workspace_access.groups import MigrationState
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class GenericPermissionsInfo:
@@ -56,24 +56,36 @@
     def __iter__(self):
         started = datetime.datetime.now()
         for item in self._func():
             yield GenericPermissionsInfo(getattr(item, self._id_attribute), self._object_type)
         since = datetime.datetime.now() - started
         logger.info(f"Listed {self._object_type} in {since}")
 
+    def __repr__(self):
+        return f"Listing({self._object_type} via {self._func.__qualname__})"
+
 
 class GenericPermissionsSupport(AclSupport):
     def __init__(
-        self, ws: WorkspaceClient, listings: list[Listing], verify_timeout: timedelta | None = timedelta(minutes=1)
+        self,
+        ws: WorkspaceClient,
+        listings: list[Listing],
+        verify_timeout: timedelta | None = timedelta(minutes=1),
+        include_object_permissions: list[str] | None = None,
     ):
         self._ws = ws
         self._listings = listings
         self._verify_timeout = verify_timeout
+        self._include_object_permissions = include_object_permissions
 
     def get_crawler_tasks(self):
+        if self._include_object_permissions:
+            for item in StaticListing(self._include_object_permissions, self.object_types()):
+                yield partial(self._crawler_task, item.object_type, item.object_id)
+            return
         for listing in self._listings:
             for info in listing:
                 yield partial(self._crawler_task, info.request_type, info.object_id)
 
     def object_types(self) -> set[str]:
         all_object_types = set()
         for listing in self._listings:
@@ -130,15 +142,15 @@
             if all(elem in remote_permission_as_request for elem in acl):
                 return True
             msg = (
                 f"Couldn't find permission for object type {object_type} with id {object_id}\n"
                 f"acl to be applied={acl}\n"
                 f"acl found in the object={remote_permission_as_request}\n"
             )
-            raise ValueError(msg)
+            raise NotFound(msg)
         return False
 
     def get_verify_task(self, item: Permissions) -> Callable[[], bool]:
         acl = iam.ObjectPermissions.from_dict(json.loads(item.raw))
         if not acl.access_control_list:
             raise ValueError(
                 f"Access control list not present for object type " f"{item.object_type} and object id {item.object_id}"
@@ -152,15 +164,15 @@
 
         update_retry_on_value_error = retried(
             on=retryable_exceptions, timeout=self._verify_timeout  # type: ignore[arg-type]
         )
         update_retried_check = update_retry_on_value_error(self._safe_update_permissions)
         update_retried_check(object_type, object_id, acl)
 
-        retry_on_value_error = retried(on=[*retryable_exceptions, ValueError], timeout=self._verify_timeout)
+        retry_on_value_error = retried(on=retryable_exceptions, timeout=self._verify_timeout)
         retried_check = retry_on_value_error(self._verify)
         return retried_check(object_type, object_id, acl)
 
     @rate_limited(max_requests=100)
     def _crawler_task(self, object_type: str, object_id: str) -> Permissions | None:
         objects_with_owner_permission = ["jobs", "pipelines"]
 
@@ -294,14 +306,17 @@
                         service_principal_name=_item.service_principal_name,
                         user_name=_item.user_name,
                         permission_level=permission.permission_level,
                     )
                 )
         return acl_requests
 
+    def __repr__(self):
+        return f"GenericPermissionsSupport({self._listings})"
+
 
 class WorkspaceListing(Listing, CrawlerBase[WorkspaceObjectInfo]):
     def __init__(
         self,
         ws: WorkspaceClient,
         sql_backend: SqlBackend,
         inventory_database: str,
@@ -371,14 +386,17 @@
         for _object in self.snapshot():
             request_type = self._convert_object_type_to_request_type(_object)
             if not request_type:
                 continue
             assert _object.object_id is not None
             yield GenericPermissionsInfo(str(_object.object_id), request_type)
 
+    def __repr__(self):
+        return f"WorkspaceListing(start_path={self._start_path})"
+
 
 def models_listing(ws: WorkspaceClient, num_threads: int):
     def inner() -> Iterator[ml.ModelDatabricks]:
         tasks = []
         for model in ws.model_registry.list_models():
             tasks.append(partial(ws.model_registry.get_model, name=model.name))
         models, errors = Threads.gather("listing model ids", tasks, num_threads)
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/groups.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,17 @@
 
     def generate_migrated_groups(self):
         workspace_groups = self.get_filtered_groups()
         for group in workspace_groups.values():
             temporary_name = f"{self.renamed_groups_prefix}{group.display_name}"
             account_group = self.account_groups_in_account.get(group.display_name)
             if not account_group:
-                logger.info(f"Couldn't find a matching account group for {group.display_name} group")
+                logger.info(
+                    f"Couldn't find a matching account group for {group.display_name} group using name matching"
+                )
                 continue
             yield MigratedGroup(
                 id_in_workspace=group.id,
                 name_in_workspace=group.display_name,
                 name_in_account=group.display_name,
                 temporary_name=temporary_name,
                 external_id=account_group.external_id,
@@ -237,29 +239,27 @@
 
     def generate_migrated_groups(self):
         workspace_groups = self.get_filtered_groups()
         account_groups_by_id = {group.external_id: group for group in self.account_groups_in_account.values()}
         for group in workspace_groups.values():
             temporary_name = f"{self.renamed_groups_prefix}{group.display_name}"
             account_group = account_groups_by_id.get(group.external_id)
-            if account_group:
-                yield MigratedGroup(
-                    id_in_workspace=group.id,
-                    name_in_workspace=group.display_name,
-                    name_in_account=account_group.display_name,
-                    temporary_name=temporary_name,
-                    external_id=account_group.external_id,
-                    members=json.dumps([gg.as_dict() for gg in group.members]) if group.members else None,
-                    roles=json.dumps([gg.as_dict() for gg in group.roles]) if group.roles else None,
-                    entitlements=(
-                        json.dumps([gg.as_dict() for gg in group.entitlements]) if group.entitlements else None
-                    ),
-                )
-            else:
+            if not account_group:
                 logger.info(f"Couldn't find a matching account group for {group.display_name} group with external_id")
+                continue
+            yield MigratedGroup(
+                id_in_workspace=group.id,
+                name_in_workspace=group.display_name,
+                name_in_account=account_group.display_name,
+                temporary_name=temporary_name,
+                external_id=account_group.external_id,
+                members=json.dumps([gg.as_dict() for gg in group.members]) if group.members else None,
+                roles=json.dumps([gg.as_dict() for gg in group.roles]) if group.roles else None,
+                entitlements=(json.dumps([gg.as_dict() for gg in group.entitlements]) if group.entitlements else None),
+            )
 
 
 class RegexSubStrategy(GroupMigrationStrategy):
     def __init__(
         self,
         workspace_groups_in_workspace,
         account_groups_in_account,
@@ -281,20 +281,26 @@
     def generate_migrated_groups(self):
         workspace_groups = self.get_filtered_groups()
         for group in workspace_groups.values():
             temporary_name = f"{self.renamed_groups_prefix}{group.display_name}"
             name_in_account = self._safe_sub(
                 group.display_name, self.workspace_group_regex, self.workspace_group_replace
             )
+            account_group = self.account_groups_in_account.get(name_in_account)
+            if not account_group:
+                logger.info(
+                    f"Couldn't find a matching account group for {group.display_name} group with regex substitution"
+                )
+                continue
             yield MigratedGroup(
                 id_in_workspace=group.id,
                 name_in_workspace=group.display_name,
                 name_in_account=name_in_account,
                 temporary_name=temporary_name,
-                external_id=self.account_groups_in_account[name_in_account].external_id,
+                external_id=account_group.external_id,
                 members=json.dumps([gg.as_dict() for gg in group.members]) if group.members else None,
                 roles=json.dumps([gg.as_dict() for gg in group.roles]) if group.roles else None,
                 entitlements=json.dumps([gg.as_dict() for gg in group.entitlements]) if group.entitlements else None,
             )
 
 
 class RegexMatchStrategy(GroupMigrationStrategy):
@@ -325,29 +331,31 @@
         account_groups_by_match = {
             self._safe_match(group_name, self.account_group_regex): group
             for group_name, group in self.account_groups_in_account.items()
         }
         for group_match, ws_group in workspace_groups_by_match.items():
             temporary_name = f"{self.renamed_groups_prefix}{ws_group.display_name}"
             account_group = account_groups_by_match.get(group_match)
-            if account_group:
-                yield MigratedGroup(
-                    id_in_workspace=ws_group.id,
-                    name_in_workspace=ws_group.display_name,
-                    name_in_account=account_group.display_name,
-                    temporary_name=temporary_name,
-                    external_id=account_group.external_id,
-                    members=json.dumps([gg.as_dict() for gg in ws_group.members]) if ws_group.members else None,
-                    roles=json.dumps([gg.as_dict() for gg in ws_group.roles]) if ws_group.roles else None,
-                    entitlements=(
-                        json.dumps([gg.as_dict() for gg in ws_group.entitlements]) if ws_group.entitlements else None
-                    ),
+            if not account_group:
+                logger.info(
+                    f"Couldn't find a matching account group for {ws_group.display_name} group with regex matching"
                 )
-            else:
-                logger.info(f"Couldn't find a match for group {ws_group.display_name}")
+                continue
+            yield MigratedGroup(
+                id_in_workspace=ws_group.id,
+                name_in_workspace=ws_group.display_name,
+                name_in_account=account_group.display_name,
+                temporary_name=temporary_name,
+                external_id=account_group.external_id,
+                members=json.dumps([gg.as_dict() for gg in ws_group.members]) if ws_group.members else None,
+                roles=json.dumps([gg.as_dict() for gg in ws_group.roles]) if ws_group.roles else None,
+                entitlements=(
+                    json.dumps([gg.as_dict() for gg in ws_group.entitlements]) if ws_group.entitlements else None
+                ),
+            )
 
 
 class GroupManager(CrawlerBase[MigratedGroup]):
     _SYSTEM_GROUPS: ClassVar[list[str]] = ["users", "admins", "account users"]
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/listing.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/listing.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/redash.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/redash.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from databricks.labs.blueprint.limiter import rate_limited
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.errors import InternalError, NotFound, PermissionDenied
 from databricks.sdk.retries import retried
 from databricks.sdk.service import sql
 from databricks.sdk.service.sql import ObjectTypePlural, SetResponse
 
-from databricks.labs.ucx.workspace_access.base import AclSupport, Permissions
+from databricks.labs.ucx.workspace_access.base import AclSupport, Permissions, StaticListing
 from databricks.labs.ucx.workspace_access.groups import MigrationState
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class SqlPermissionsInfo:
@@ -35,41 +35,50 @@
         self._request_type = request_type
         self.object_type = request_type.value
 
     def __iter__(self):
         for item in self._func():
             yield SqlPermissionsInfo(item.id, self._request_type)
 
+    def __repr__(self):
+        return f"Listing({self.object_type} via {self._func.__qualname__})"
+
 
 class RedashPermissionsSupport(AclSupport):
     def __init__(
         self,
         ws: WorkspaceClient,
         listings: list[Listing],
         set_permissions_timeout: timedelta | None = timedelta(minutes=1),
         # Group information in Redash are cached for up to 10 minutes causing inconsistencies.
         # If a group is renamed, the old name may still be returned by the dbsql get permissions api.
         # Note that the update/set API is strongly consistent and is not affected by this behaviour.
         # The validation step should keep retrying for at least 10 mins until the get api returns the new group name.
         # More details here: https://databricks.atlassian.net/browse/ES-992619
         verify_timeout: timedelta | None = timedelta(minutes=11),
+        include_object_permissions: list[str] | None = None,
     ):
         self._ws = ws
         self._listings = listings
         self._set_permissions_timeout = set_permissions_timeout
         self._verify_timeout = verify_timeout
+        self._include_object_permissions = include_object_permissions
 
     @staticmethod
     def _is_item_relevant(item: Permissions, migration_state: MigrationState) -> bool:
         permissions_response = sql.GetResponse.from_dict(json.loads(item.raw))
         assert permissions_response.access_control_list is not None
         mentioned_groups = [acl.group_name for acl in permissions_response.access_control_list]
         return any(g in mentioned_groups for g in [info.name_in_workspace for info in migration_state.groups])
 
     def get_crawler_tasks(self):
+        if self._include_object_permissions:
+            for item in StaticListing(self._include_object_permissions, self.object_types()):
+                yield partial(self._crawler_task, item.object_id, item.object_type)
+            return
         for listing in self._listings:
             for item in listing:
                 yield partial(self._crawler_task, item.object_id, item.request_type)
 
     def object_types(self) -> set[str]:
         all_object_types = set()
         for listing in self._listings:
@@ -152,15 +161,15 @@
             if all(elem in remote_permission.access_control_list for elem in acl):
                 return True
             msg = (
                 f"Couldn't find permission for object type {object_type} with id {object_id}\n"
                 f"acl to be applied={acl}\n"
                 f"acl found in the object={remote_permission}\n"
             )
-            raise ValueError(msg)
+            raise NotFound(msg)
         return False
 
     def get_verify_task(self, item: Permissions) -> Callable[[], bool]:
         acl = sql.GetResponse.from_dict(json.loads(item.raw))
         if not acl.access_control_list:
             raise ValueError(
                 f"Access control list not present for object type " f"{item.object_type} and object id {item.object_id}"
@@ -174,15 +183,15 @@
         This affects the way how we prepare the new ACL request.
         """
 
         set_retry_on_value_error = retried(on=[InternalError, ValueError], timeout=self._set_permissions_timeout)
         set_retried_check = set_retry_on_value_error(self._safe_set_permissions)
         set_retried_check(object_type, object_id, acl)
 
-        retry_on_value_error = retried(on=[InternalError, ValueError], timeout=self._verify_timeout)
+        retry_on_value_error = retried(on=[InternalError, NotFound], timeout=self._verify_timeout)
         retried_check = retry_on_value_error(self._verify)
         return retried_check(object_type, object_id, acl)
 
     def _prepare_new_acl(
         self, acl: list[sql.AccessControl], migration_state: MigrationState
     ) -> list[sql.AccessControl]:
         """
@@ -253,14 +262,17 @@
         except PermissionDenied:
             logger.warning(f"Permission denied: {object_type} {object_id}")
             return None
         except NotFound:
             logger.warning(f"Deleted on platform: {object_type} {object_id}")
             return None
 
+    def __repr__(self):
+        return f"RedashPermissionsSupport({self._listings})"
+
 
 def redash_listing_wrapper(
     func: Callable[..., list], object_type: sql.ObjectTypePlural
 ) -> Callable[..., Iterable[SqlPermissionsInfo]]:
     def wrapper() -> Iterable[SqlPermissionsInfo]:
         for item in func():
             yield SqlPermissionsInfo(
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/scim.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/scim.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,36 +14,46 @@
     PermissionDenied,
     ResourceConflict,
 )
 from databricks.sdk.retries import retried
 from databricks.sdk.service import iam
 from databricks.sdk.service.iam import Group, Patch, PatchSchema
 
-from databricks.labs.ucx.workspace_access.base import AclSupport, Permissions
+from databricks.labs.ucx.workspace_access.base import AclSupport, Permissions, StaticListing
 from databricks.labs.ucx.workspace_access.groups import MigrationState
 
 logger = logging.getLogger(__name__)
 
 
 class ScimSupport(AclSupport):
-    def __init__(self, ws: WorkspaceClient, verify_timeout: timedelta | None = timedelta(minutes=1)):
+    def __init__(
+        self,
+        ws: WorkspaceClient,
+        verify_timeout: timedelta | None = timedelta(minutes=1),
+        include_object_permissions: list[str] | None = None,
+    ):
         self._ws = ws
         self._verify_timeout = verify_timeout
+        self._include_object_permissions = include_object_permissions
         self._snapshot = {}
         # TODO: we may need to inject GroupManager here for proper group listing
         for group in self._ws.groups.list(attributes="id,displayName,meta,roles,entitlements"):
             if not group.display_name:
                 continue
             self._snapshot[group.display_name] = group
 
     @staticmethod
     def _is_item_relevant(item: Permissions, migration_state: MigrationState) -> bool:
         return any(g.id_in_workspace == item.object_id for g in migration_state.groups)
 
     def get_crawler_tasks(self):
+        if self._include_object_permissions:
+            for item in StaticListing(self._include_object_permissions, self.object_types()):
+                yield partial(self._crawler_task, item.object_id, item.object_type)
+            return
         for group in self._snapshot.values():
             meta = group.meta
             if not meta:
                 continue
             if meta.resource_type != "WorkspaceGroup":
                 continue
             if group.roles and len(group.roles) > 0:
```

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/secrets.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/secrets.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/databricks/labs/ucx/workspace_access/tacl.py` & `databricks_labs_ucx-0.22.0/databricks/labs/ucx/workspace_access/tacl.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 import functools
 import json
 from collections.abc import Callable, Iterator
 from datetime import timedelta
 from functools import partial
 
 from databricks.labs.lsql.backends import SqlBackend
+from databricks.sdk.errors import NotFound
 from databricks.sdk.retries import retried
 
-from databricks.labs.ucx.hive_metastore import GrantsCrawler
-from databricks.labs.ucx.hive_metastore.grants import Grant
-from databricks.labs.ucx.workspace_access.base import AclSupport, Permissions
+from databricks.labs.ucx.hive_metastore.grants import Grant, GrantsCrawler
+from databricks.labs.ucx.workspace_access.base import AclSupport, Permissions, StaticListing
 from databricks.labs.ucx.workspace_access.groups import MigrationState
 
 
 class TableAclSupport(AclSupport):
     def __init__(
         self,
         grants_crawler: GrantsCrawler,
         sql_backend: SqlBackend,
         verify_timeout: timedelta | None = timedelta(minutes=1),
+        include_object_permissions: list[str] | None = None,
     ):
         self._grants_crawler = grants_crawler
         self._sql_backend = sql_backend
         self._verify_timeout = verify_timeout
+        self._include_object_permissions = include_object_permissions
 
     def get_crawler_tasks(self) -> Iterator[Callable[..., Permissions | None]]:
         # Table ACL permissions (grant/revoke and ownership) are not atomic. When granting the permissions,
         # the service would first get all existing permissions, append with the new permissions,
         # and set the full list in the database. If there are concurrent grant requests,
         # both requests might succeed and emit the audit logs, but what actually happens could be that
         # the new permission list from one request overrides the other one, causing permissions loss.
@@ -40,17 +42,25 @@
         # For example, the following table grants:
         # * GRANT SELECT ON TABLE hive_metastore.db_a.table_a TO group_a
         # * GRANT MODIFY ON TABLE hive_metastore.db_a.table_a TO group_a
         # will be folded and executed in one statement/transaction:
         # * GRANT SELECT, MODIFY ON TABLE hive_metastore.db_a.table_a TO group_a
         # The exception is the "OWN" permission which must be set using a separate ALTER statement.
 
+        include_objects = set[tuple[str, str]]()
+        if self._include_object_permissions:
+            for item in StaticListing(self._include_object_permissions, self.object_types()):
+                include_objects.add((item.object_type, item.object_id))
+
         folded_actions = collections.defaultdict(set)
         for grant in self._grants_crawler.snapshot():
-            key = (grant.principal, grant.this_type_and_key())
+            type_and_key = grant.this_type_and_key()
+            if include_objects and type_and_key not in include_objects:
+                continue
+            key = (grant.principal, type_and_key)
             folded_actions[key].add(grant.action_type)
 
         def inner(object_type: str, object_id: str, grant: Grant) -> Permissions:
             return Permissions(object_type=object_type, object_id=object_id, raw=json.dumps(dataclasses.asdict(grant)))
 
         for (principal, (object_type, object_id)), actions in folded_actions.items():
             grant = self._from_reduced(object_type, object_id, principal, ", ".join(sorted(actions)))
@@ -104,15 +114,15 @@
         could cause permission lost due to limitations in the Table ACLs.
         More info here: https://databricks.atlassian.net/browse/ES-976290
         """
         for sql in grant.hive_grant_sql():
             self._sql_backend.execute(sql)
 
         object_type, object_id = grant.this_type_and_key()
-        retry_on_value_error = retried(on=[ValueError], timeout=self._verify_timeout)
+        retry_on_value_error = retried(on=[NotFound], timeout=self._verify_timeout)
         retried_check = retry_on_value_error(self._verify)
         return retried_check(object_type, object_id, grant)
 
     def _verify(self, object_type: str, object_id: str, acl: Grant) -> bool:
         grant_dict = dataclasses.asdict(acl)
         del grant_dict["action_type"]
         del grant_dict["principal"]
@@ -124,13 +134,13 @@
             if all(action_type in on_current_principal for action_type in acl_action_types):
                 return True
             msg = (
                 f"Couldn't find permission for object type {object_type}, id {object_id} and principal {acl.principal}\n"
                 f"acl to be applied={acl_action_types}\n"
                 f"acl found in the object={on_current_principal}\n"
             )
-            raise ValueError(msg)
+            raise NotFound(msg)
         return False
 
     def get_verify_task(self, item: Permissions) -> Callable[[], bool]:
         grant = Grant(**json.loads(item.raw))
         return partial(self._verify, item.object_type, item.object_id, grant)
```

### Comparing `databricks_labs_ucx-0.21.0/.gitignore` & `databricks_labs_ucx-0.22.0/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/LICENSE` & `databricks_labs_ucx-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_ucx-0.21.0/NOTICE` & `databricks_labs_ucx-0.22.0/NOTICE`

 * *Files 11% similar despite different names*

```diff
@@ -10,7 +10,11 @@
 
 This software contains code from the following open source projects, licensed under the MIT License.
 
 PyYAML - https://github.com/yaml/pyyaml
 Copyright (c) 2017-2021 Ingy döt Net
 Copyright (c) 2006-2016 Kirill Simonov
 License - https://github.com/yaml/pyyaml/blob/main/LICENSE
+
+SQLGlot - https://sqlglot.com
+Copyright (c) 2023 Toby Mao
+License - https://github.com/tobymao/sqlglot/blob/main/LICENSE
```

### Comparing `databricks_labs_ucx-0.21.0/README.md` & `databricks_labs_ucx-0.22.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 Databricks Labs UCX
 ===
 ![UCX by Databricks Labs](docs/logo-no-background.png)
 
 The companion for upgrading to Unity Catalog. After [installation](#install-ucx), ensure to [trigger](#ensure-assessment-run-command) the [assessment workflow](#assessment-workflow), 
 so that you'll be able to [scope the migration](docs/assessment.md) and execute the [group migration workflow](#group-migration-workflow). 
-[`<installation_path>/README`](#readme-notebook) contains further instructions and explanations of these workflows.
-More workflows, like [migrating tables](docs/table_upgrade.md) and notebook code is coming in the future releases. 
+[`<installation_path>/README`](#readme-notebook) contains further instructions and explanations of these workflows. 
+Then you can execute [table migration workflow](#table-migration-workflow).
+More workflows, like notebook code migration is coming in the future releases. 
 UCX exposes a number of command line utilities accessible via `databricks labs ucx`.
 
-For questions, troubleshooting or bug fixes, please see your Databricks account team or submit [an issue](https://github.com/databrickslabs/ucx/issues). 
+For questions, troubleshooting or bug fixes, please see our [troubleshooting guide](docs/troubleshooting.md) or submit [an issue](https://github.com/databrickslabs/ucx/issues). 
 See [contributing instructions](CONTRIBUTING.md) to help improve this project.
 
 [![build](https://github.com/databrickslabs/ucx/actions/workflows/push.yml/badge.svg)](https://github.com/databrickslabs/ucx/actions/workflows/push.yml) [![codecov](https://codecov.io/github/databrickslabs/ucx/graph/badge.svg?token=p0WKAfW5HQ)](https://codecov.io/github/databrickslabs/ucx)  [![lines of code](https://tokei.rs/b1/github/databrickslabs/ucx)]([https://codecov.io/github/databrickslabs/ucx](https://github.com/databrickslabs/ucx))
 
 <!-- TOC -->
 * [Databricks Labs UCX](#databricks-labs-ucx)
 * [Installation](#installation)
   * [Authenticate Databricks CLI](#authenticate-databricks-cli)
   * [Install UCX](#install-ucx)
   * [[ADVANCED] Force install over existing UCX](#advanced-force-install-over-existing-ucx)
+  * [[ADVANCED] Installing UCX on all workspaces within a Databricks account](#advanced-installing-ucx-on-all-workspaces-within-a-databricks-account)
   * [Upgrading UCX for newer versions](#upgrading-ucx-for-newer-versions)
   * [Uninstall UCX](#uninstall-ucx)
 * [Migration process](#migration-process)
 * [Workflows](#workflows)
   * [Readme notebook](#readme-notebook)
   * [Assessment workflow](#assessment-workflow)
   * [Group migration workflow](#group-migration-workflow)
   * [Debug notebook](#debug-notebook)
   * [Debug logs](#debug-logs)
+  * [Table Migration Workflow](#table-migration-workflow)
+    * [Dependency CLI commands](#dependency-cli-commands)
+    * [Table Migration Workflow Tasks](#table-migration-workflow-tasks)
+    * [Other considerations](#other-considerations)
 * [Utility commands](#utility-commands)
+  * [`logs` command](#logs-command)
   * [`ensure-assessment-run` command](#ensure-assessment-run-command)
   * [`repair-run` command](#repair-run-command)
   * [`workflows` command](#workflows-command)
   * [`open-remote-config` command](#open-remote-config-command)
   * [`installations` command](#installations-command)
+* [Metastore related commands](#metastore-related-commands)
+  * [`show-all-metastores` command](#show-all-metastores-command)
+  * [`assign-metastore` command](#assign-metastore-command)
 * [Table migration commands](#table-migration-commands)
   * [`principal-prefix-access` command](#principal-prefix-access-command)
     * [Access for AWS S3 Buckets](#access-for-aws-s3-buckets)
     * [Access for Azure Storage Accounts](#access-for-azure-storage-accounts)
   * [`create-uber-principal` command](#create-uber-principal-command)
   * [`migrate-credentials` command](#migrate-credentials-command)
   * [`validate-external-locations` command](#validate-external-locations-command)
@@ -158,14 +168,27 @@
 
 * `UCX_FORCE_INSTALL=user databricks labs install ucx` - will force the installation to be for user only
 * `UCX_FORCE_INSTALL=global databricks labs install ucx` - will force the installation to be for root only
 
 
 [[back to top](#databricks-labs-ucx)]
 
+## [ADVANCED] Installing UCX on all workspaces within a Databricks account
+Setting the environment variable `UCX_FORCE_INSTALL` to 'account' will install UCX on all workspaces within a Databricks account.
+
+* `UCX_FORCE_INSTALL=account databricks labs install ucx`
+
+After the first installation, UCX will prompt the user to confirm whether to install UCX on the remaining workspaces with the same answers. If confirmed, the remaining installations will be completed silently.
+
+This installation mode will automatically select the following options:
+* Automatically create and enable HMS lineage init script
+* Automatically create a new SQL warehouse for UCX assessment
+
+[[back to top](#databricks-labs-ucx)]
+
 ## Upgrading UCX for newer versions
 
 Verify that UCX is installed
 
 ```commandline
 databricks labs installed
 
@@ -200,15 +223,15 @@
 ![macos_uninstall_ucx](docs/macos_4_databrickslabsmac_uninstallucx.gif)
 
 [[back to top](#databricks-labs-ucx)]
 
 # Migration process
 
 On the high level, the steps in migration process start with the [assessment workflow](#assessment-workflow), 
-followed by [group migration](#group-migration-workflow), [table migration](#table-migration-commands), 
+followed by [group migration](#group-migration-workflow), [table migration workflow](#table-migration-workflow), 
 finalised with the [code migration](#code-migration-commands). It can be described as:
 
 ```mermaid
 flowchart TD
     subgraph workspace-admin
         assessment --> group-migration
         group-migration --> table-migration
@@ -300,15 +323,15 @@
 
 See the [detailed design](docs/local-group-migration.md) of this workflow. It helps you to upgrade all Databricks workspace assets:
 Legacy Table ACLs, Entitlements, AWS instance profiles, Clusters, Cluster policies, Instance Pools, 
 Databricks SQL warehouses, Delta Live Tables, Jobs, MLflow experiments, MLflow registry, SQL Dashboards & Queries,
 SQL Alerts, Token and Password usage permissions that are set on the workspace level, Secret scopes, Notebooks,
 Directories, Repos, and Files. 
 
-Once done with the group migration, proceed to [table migration](#table-migration-commands).
+Once done with the group migration, proceed to [table migration workflow](#table-migration-workflow).
 
 Use [`validate-groups-membership` command](#validate-groups-membership-command) for extra confidence.
 If you don't have matching account groups, please run [`create-account-groups` command](#create-account-groups-command).
 
 The group migration workflow is designed to migrate workspace-local groups to account-level groups in the Unity Catalog (UC) environment. It ensures that all the necessary groups are available in the workspace with the correct permissions, and removes any unnecessary groups and permissions. The tasks in the group migration workflow depend on the output of the assessment workflow and can be executed in sequence to ensure a successful migration. The output of each task is stored in Delta tables in the `$inventory_database` schema, which can be used for further analysis and decision-making. The group migration workflow can be executed multiple times to ensure that all the groups are migrated successfully and that all the necessary permissions are assigned.
 
 1. `crawl_groups`: This task scans all groups for the local group migration scope.
@@ -338,16 +361,112 @@
 flush the logs every 10 minutes.
 
 To enable debug logs of [command-line interface](#authenticate-databricks-cli), 
 simply add `--debug` flag to any command.
 
 [[back to top](#databricks-labs-ucx)]
 
+## Table Migration Workflow
+
+The table migration workflow comprises multiple workflows and tasks designed to migrate tables from the Hive Metastore to the Unity Catalog. The subsequent diagram illustrates the workflow's tasks and their dependency CLI commands. 
+```mermaid
+flowchart TB
+    subgraph CLI
+      sync-workspace-info[sync-workspace-info] --> create_table_mapping[create-table-mapping]
+      create_table_mapping[create-table-mapping] --> create_catalogs_schemas[create-catalogs-schemas]
+      create_uber_principal[create-uber-principal]
+      principal_prefix_access[principal-prefix-access] --> migrate_credentials[migrate-credentials]
+      migrate_credentials --> migrate_locations[migrate-locations]
+      migrate_locations --> create_catalogs_schemas
+    end
+    
+    create_uber_principal --> workflow
+    create_table_mapping --> workflow
+    create_catalogs_schemas --> workflow
+    
+    subgraph workflow[Table Migration Workflows]
+      subgraph mt_workflow[workflow: migrate-tables]
+        dbfs_root_delta_mt_task[migrate_dbfs_root_delta_tables]
+        external_tables_sync_mt_task[migrate_external_tables_sync]
+        view_mt_task[roadmap: migrate_views]
+        dbfs_root_delta_mt_task --> view_mt_task
+        external_tables_sync_mt_task --> view_mt_task
+      end
+      
+      subgraph mt_ctas_wf[roadmap workflow: migrate-tables-ctas]
+        ctas_mt_task[migrate_tables_ctas] --> view_mt_task_ctas[roadmap: migrate_views]
+      end
+  
+      subgraph mt_serde_inplace_wf[roadmap workflow: migrate-external-hiveserde-tables-in-place-experimental]
+        serde_inplace_mt_task[migrate_external_hiveserde_tables_in_place_experimental] --> view_mt_task_inplace[roadmap: migrate_views]
+      end
+  
+      subgraph mt_in_mounts_wf[roadmap workflow: migrate-tables-in-mounts-experimental]
+        scan_tables_in_mounts_experimental_task[scan_tables_in_mounts_experimental] --> 
+        migrate_tables_in_mounts_experimental[migrate_tables_in_mounts_experimental]
+      end
+    end
+    
+    classDef roadmap stroke:Green,stroke-width:2px,color:Green,stroke-dasharray: 8 3
+    class view_mt_task roadmap;
+    class mt_ctas_wf,ctas_mt_task,view_mt_task_ctas roadmap;
+    class mt_serde_inplace_wf,serde_inplace_mt_task,view_mt_task_inplace roadmap;
+    class mt_in_mounts_wf,scan_tables_in_mounts_experimental_task,migrate_tables_in_mounts_experimental roadmap;
+```
+More details can be found in the [design of table migration](docs/table_upgrade.md)
+
+### Dependency CLI commands
+- [`create-table-mapping`](#create-table-mapping-command) - Create `mapping.csv` which will be used by the workflow to identify the targets catalog, schema, table of the HMS table to be migrated. User should review and update the mapping file accordingly before proceeding with the migration workflow.
+- [`principal-prefix-access`](#principal-prefix-access-command) - Identify all the storages used in the workspace and corresponding Azure Service Principal or IAM role that are used in the workspace. It outputs `azure_storage_account_info.csv` or `uc_roles_access.csv` which will be later used by [`migrate-credentials`](#migrate-credentials-command) command to create UC storage credentials. The csv can be edited to control which IAM roles or Azure Service Principals should be used to create UC storage credentials later.
+- [`migrate-credentials`](#migrate-credentials-command) - Create UC storage credentials based on the Azure Service Principal or IAM role (`azure_storage_account_info.csv` or `uc_roles_access.csv`) identified by [`principal-prefix-access`](#principal-prefix-access-command) command.
+- [`migrate-locations`](#migrate-locations-command) - Create missing external locations in the Unity Catalog. 
+- [`create-catalogs-schemas`](#create-catalogs-schemas-command) - Create missing catalogs and schemas in the Unity Catalog. The candidate catalogs and schemas is based on `mapping.csv`
+- [`create-uber-principal`](#create-uber-principal-command) - Create an Uber Principal with access to all storages used in the workspace. This principal will be used by the workflow job cluster to migrate all the tables in the workspace.
+
+[`create-table-mapping`](#create-table-mapping-command) and [`create-uber-principal`](#create-uber-principal-command) are required to run the workflow. While other commands are optional, as long as the UC storage credentials, external locations, catalogs and schemas needed for successful migration are created.
+
+To control the scope of the table migration, consider utilizing a combination of editing `mapping.csv`, employing [`skip`](#skip-command) command, and [`revert-migrated-tables`](#revert-migrated-tables-command) command.
+
+See more details in [Table migration commands](#table-migration-commands)
+
+### Table Migration Workflow Tasks
+- `migrate_dbfs_root_delta_tables` - Migrate delta tables from the DBFS root using deep clone, along with legacy table ACL migrated if any.
+- `migrate_external_tables_sync` - Migrate external tables using [`SYNC`](https://docs.databricks.com/en/sql/language-manual/sql-ref-syntax-aux-sync.html) command, along with legacy table ACL migrated if any.
+- Following workflows/tasks are on the roadmap and being developed:
+  - Migrate view
+  - Migrate tables using CTAS
+  - Optionally and experimentally in place migrate ParquetHiveSerDe, OrcSerde, AvroSerDe, LazySimpleSerDe, JsonSerDe, OpenCSVSerde tables.
+  - Experimentally migrate Delta and Parquet data found in dbfs mount but not registered as Hive Metastore table into UC tables.
+
+### Other considerations
+- You may need to run the workflow multiple times to ensure all the tables are migrated successfully in phases.
+- If your delta tables in DBFS root have large number of files, consider:
+  - Setting higher Min and Max workers for auto-scale when being asked during the UCX installation. More nodes/cores in the cluster means more concurrency for calling cloud storage api to copy files when deep cloning the delta tables.
+  - Setting higher "Parallelism for migrating dbfs root delta tables with deep clone" (default 200) when being asked during the UCX installation. This controls the number of Spark task/partition to be created for deep clone.
+- Consider create an instance pool, and set the instance pool id when being asked during the UCX installation. This instance pool will be put into the cluster policy used by all UCX workflows job clusters.
+- You may also manually edit the job cluster configration per job or per task after the workflows are deployed.
+
+[[back to top](#databricks-labs-ucx)]
+
 # Utility commands
 
+## `logs` command
+
+```text
+$ databricks labs ucx logs [--workflow WORKFLOW_NAME] [--debug]
+```
+
+This command displays the logs of the last run of the specified workflow. If no workflow is specified, it displays 
+the logs of the workflow that was run the last. This command is useful for developers and administrators who want to 
+check the logs of the last run of a workflow and ensure that it was executed as expected. It can also be used for 
+debugging purposes when a workflow is not behaving as expected. By default, only `INFO`, `WARNING`, and `ERROR` logs
+are displayed. To display `DEBUG` logs, use the `--debug` flag.
+
+[[back to top](#databricks-labs-ucx)] 
+
 ## `ensure-assessment-run` command
 
 ```commandline
 databricks labs ucx ensure-assessment-run
 ```
 
 This command ensures that the [assessment workflow](#assessment-workflow) was run on a workspace. 
@@ -446,17 +565,46 @@
 This command displays the [installations](#installation) by different users on the same workspace. It fetches all 
 the installations where the `ucx` package is installed and prints their details in JSON format. This command is useful 
 for administrators who want to see which users have installed `ucx` and where. It can also be used to debug issues 
 related to multiple installations of `ucx` on the same workspace.
 
 [[back to top](#databricks-labs-ucx)]
 
+# Metastore related commands
+
+These commands are used to assign a Unity Catalog metastore to a workspace. The metastore assignment is a pre-requisite
+for any further migration steps.
+
+[[back to top](#databricks-labs-ucx)]
+
+## `show-all-metastores` command
+
+```text
+databricks labs ucx show-all-metastores [--workspace-id <workspace-id>]
+```
+
+This command lists all the metastores available to be assigned to a workspace. If no workspace is specified, it lists
+all the metastores available in the account. This command is useful when there are multiple metastores available within
+a region and you want to see which ones are available for assignment.
+
+[[back to top](#databricks-labs-ucx)]
+
+## `assign-metastore` command
+
+```text
+databricks labs ucx assign-metastore --workspace-id <workspace-id> [--metastore-id <metastore-id>]
+```
+
+This command assigns a metastore to a workspace with `workspace-id`. If there is only a single metastore in the workspace
+region, it will be automatically assigned to the workspace. If there are multiple metastores available, you need to specify
+the metastore id of the metastore you want to assign to the workspace.
+
 # Table migration commands
 
-These commands are vital part of [table migration](docs/table_upgrade.md) process and require 
+These commands are vital part of [table migration workflow](#table-migration-workflow) process and require 
 the [assessment workflow](#assessment-workflow) and 
 [group migration workflow](#group-migration-workflow) to be completed. 
 See the [migration process diagram](#migration-process) to understand the role of the table migration commands in 
 the migration process. 
 
 The first step is to run the [`principal-prefix-access` command](#principal-prefix-access-command) to identify all 
 the storage accounts used by tables in the workspace and their permissions on each storage account.
@@ -529,15 +677,15 @@
 
 **Requires Cloud IAM admin privileges.** Once the [`assessment` workflow](#assessment-workflow) complete, you should run 
 this command to creates a service principal with the _**read-only access to all storage**_ used by tables in this 
 workspace and configure the [UCX Cluster Policy](#installation) with the details of it. Once migration is complete, this
 service principal should be unprovisioned. On Azure, it creates a principal with `Storage Blob Data Reader` role 
 assignment on every storage account using Azure Resource Manager APIs.
 
-Once done, proceed to the launching the [table migration workflow](#table-migration-commands).
+This command is one of prerequisites for the [table migration workflow](#table-migration-workflow).
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `migrate-credentials` command
 
 ```commandline
 databricks labs ucx migrate-credentials
@@ -603,27 +751,29 @@
 easier in your favorite spreadsheet application.
 
 Once you're done with this command, [create catalogs and schemas](#create-catalogs-schemas-command). During 
 multiple runs of the table migration workflow, you can use the [`revert-migrated-tables` command](#revert-migrated-tables-command)
 to revert the tables that were migrated in the previous run. You can also skip the tables that you don't want to migrate
 using the [`skip` command](#skip-command).
 
+This command is one of prerequisites for the [table migration workflow](#table-migration-workflow).
+
 Once you're done with table migration, proceed to the [code migration](#code-migration-commands).
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `skip` command
 
 ```text
 databricks labs ucx skip --schema X [--table Y]  
 ```
 
 Anywhere after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
 
-This command allows users to skip certain schemas or tables during the [table migration](docs/table_upgrade.md) process.
+This command allows users to skip certain schemas or tables during the [table migration](#table-migration-workflow) process.
 The command takes `--schema` and optionally `--table` flags to specify the schema and table to skip. If no `--table` flag 
 is provided, all tables in the specified HMS database are skipped.
 This command is useful to temporarily disable migration on a particular schema or table.
 
 Once you're done with table migration, proceed to the [code migration](#code-migration-commands).
 
 [[back to top](#databricks-labs-ucx)]
@@ -632,42 +782,40 @@
 
 ```text
 databricks labs ucx revert-migrated-tables --schema X --table Y [--delete-managed]  
 ```
 
 Anywhere after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
 
-This command removes the `upgraded_from` property on a migrated table for re-migration in the [table upgrade](docs/table_upgrade.md) process. 
+This command removes the `upgraded_from` property on a migrated table for re-migration in the [table migration](#table-migration-workflow) process. 
 This command is useful for developers and administrators who want to revert the migration of a table. It can also be used 
 to debug issues related to table migration.
 
 Go back to the [`create-table-mapping` command](#create-table-mapping-command) after you're done with this command.
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `create-catalogs-schemas` command
 
 ```text
 databricks labs ucx create-catalogs-schemas
 ```
 After [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command to have the required UC catalogs and schemas created.
-This command is supposed to be run before migrating tables to UC.
-
-Once you're done with this command, proceed to the [table migration workflow](#table-migration-commands).
+This command is supposed to be run before migrating tables to UC using [table migration workflow](#table-migration-workflow).
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `move` command
 
 ```text
 databricks labs ucx move --from-catalog A --from-schema B --from-table C --to-catalog D --to-schema E  
 ```
 
 This command moves a UC table/tables from one schema to another schema after
-the [table upgrade](docs/table_upgrade.md) process. This is useful for developers and administrators who want 
+the [table migration](#table-migration-workflow) process. This is useful for developers and administrators who want 
 to adjust their catalog structure after tables upgrade.
 
 Users will be prompted whether tables/view are dropped after moving to new schema. This only applies to `MANAGED` tables and views.
 
 This command moves different table types differently:
 - `MANAGED` tables are deep-cloned to the new schema. 
 - `EXTERNAL` tables are dropped from the original schema, then created in the target schema using the same location. 
@@ -691,28 +839,28 @@
 
 [[back to top](#databricks-labs-ucx)]
 
 # Code migration commands
 
 See the [migration process diagram](#migration-process) to understand the role of the code migration commands in the migration process.
 
-After you're done with the [table migration](#table-migration-commands), you can proceed to the code migration.
+After you're done with the [table migration](#table-migration-workflow), you can proceed to the code migration.
 
 Once you're done with the code migration, you can run the [`cluster-remap` command](#cluster-remap-command) to remap the
 clusters to be UC compatible.
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `migrate-local-code` command
 
 ```text
 databricks labs ucx migrate-local-code
 ```
 
-**(Experimental)** Once [table migration](#table-migration-commands) is complete, you can run this command to 
+**(Experimental)** Once [table migration](#table-migration-workflow) is complete, you can run this command to 
 migrate all python and SQL files in the current working directory. This command is highly experimental and
 at the moment only supports Python and SQL files and discards code comments and formatting during 
 the automated transformation process.
 
 [[back to top](#databricks-labs-ucx)]
 
 # Cross-workspace installations
@@ -740,15 +888,15 @@
 14:07:10  INFO [d.l.blueprint.parallel][finding_ucx_installations_0] finding ucx installations 20/88, rps: 32.110/sec
 14:07:11  INFO [d.l.blueprint.parallel][finding_ucx_installations_18] finding ucx installations 30/88, rps: 39.786/sec
 ...
 ```
 
 **Requires Databricks Account Administrator privileges.** This command uploads the workspace config to all workspaces 
 in the account where `ucx` is installed. This command is necessary to create an immutable default catalog mapping for
-[table migration](docs/table_upgrade.md) process and is the prerequisite 
+[table migration](#table-migration-workflow) process and is the prerequisite 
 for [`create-table-mapping` command](#create-table-mapping-command).
 
 If you cannot get account administrator privileges in reasonable time, you can take the risk and 
 run [`manual-workspace-info` command](#manual-workspace-info-command) to enter Databricks Workspace IDs and Databricks 
 Workspace names. 
 
 [[back to top](#databricks-labs-ucx)]
@@ -811,15 +959,15 @@
 ```
 
 This command validates the groups to see if the groups at the account level and workspace level have different membership.
 This command is useful for administrators who want to ensure that the groups have the correct membership. It can also be
 used to debug issues related to group membership. See [group migration](docs/local-group-migration.md) and 
 [group migration](#group-migration-workflow) for more details.
 
-Once you're done with this command, proceed to the [table migration](#table-migration-commands).
+Valid group membership is important to ensure users has correct access after legacy table ACL is migrated in [table migration workflow](#table-migration-workflow)
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `cluster-remap` command
 
 ```text
 $ databricks labs ucx cluster-remap
```

### Comparing `databricks_labs_ucx-0.21.0/pyproject.toml` & `databricks_labs_ucx-0.22.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,18 +40,19 @@
     "Intended Audience :: System Administrators",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Topic :: Software Development :: Libraries",
     "Topic :: Utilities",
 ]
 
-dependencies = ["databricks-sdk==0.23.0",
-                "databricks-labs-lsql~=0.3.0",
+dependencies = ["databricks-sdk~=0.26.0",
+                "databricks-labs-lsql~=0.4.0",
                 "databricks-labs-blueprint~=0.4.3",
-                "PyYAML>=6.0.0,<7.0.0"]
+                "PyYAML>=6.0.0,<7.0.0",
+                "sqlglot>=23.9,<23.12"]
 
 [project.entry-points.databricks]
 runtime = "databricks.labs.ucx.runtime:main"
 
 [project.urls]
 Issues = "https://github.com/databricks/ucx/issues"
 Source = "https://github.com/databricks/ucx"
@@ -59,18 +60,18 @@
 [tool.hatch.version]
 path = "src/databricks/labs/ucx/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
     "black~=24.3.0",
     "coverage[toml]~=7.4.4",
-    "isort~=5.13.2",
     "mypy~=1.9.0",
     "pylint~=3.1.0",
     "pylint-pytest==2.0.0a0",
+    "databricks-labs-pylint~=0.4.0",
     "pytest~=8.1.0",
     "pytest-cov~=4.1.0",
     "pytest-mock~=3.14.0",
     "pytest-timeout~=2.3.1",
     "pytest-xdist~=3.5.0",
     "ruff~=0.3.4",
     "types-PyYAML~=6.0.12",
@@ -82,30 +83,24 @@
 # store virtual env as the child of this folder. Helps VSCode (and PyCharm) to run better
 path = ".venv"
 
 [tool.hatch.envs.default.scripts]
 test        = "pytest -n 4 --cov src --cov-report=xml --timeout 30 tests/unit --durations 20"
 coverage    = "pytest -n auto --cov src tests/unit --timeout 30 --cov-report=html --durations 20"
 integration = "pytest -n 10 --cov src tests/integration --durations 20"
-fmt         = ["isort .",
-               "black .",
+fmt         = ["black .",
                "ruff check . --fix",
-               "mypy .",
+               "mypy --disable-error-code 'annotation-unchecked' .",
                "pylint --output-format=colorized -j 0 src tests"]
 verify      = ["black --check .",
-               "isort . --check-only",
                "ruff .",
                "mypy .",
                "pylint --output-format=colorized -j 0 src tests"]
 lint         = ["pylint --output-format=colorized -j 0 src tests"]
 
-[tool.isort]
-skip_glob = ["notebooks/*.py"]
-profile = "black"
-
 [tool.pytest.ini_options]
 # TODO: remove `-p no:warnings`
 addopts = "--no-header -p no:warnings"
 cache_dir = ".venv/pytest-cache"
 
 [tool.black]
 target-version = ["py310"]
@@ -214,30 +209,31 @@
 # for modules/projects where namespaces are manipulated during runtime and thus
 # existing member attributes cannot be deduced by static analysis). It supports
 # qualified module names, as well as Unix pattern matching.
 # ignored-modules =
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
-init-hook='import sys; sys.path.append("tests/pylint")'
+#init-hook=''
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
 # number of processors available to use, and will cap the count on Windows to
 # avoid hangs.
 jobs = 0
 
 # Control the amount of potential inferred values when inferring a single object.
 # This can help the performance when dealing with large functions or complex,
 # nested conditions.
 limit-inference-results = 100
 
 # List of plugins (as comma separated values of python module names) to load,
 # usually to register additional checkers.
 load-plugins = [
-    "testing",
+    "databricks.labs.pylint.mocking",
+    "databricks.labs.pylint.eradicate",
     "pylint_pytest",
     "pylint.extensions.bad_builtin",
     "pylint.extensions.broad_try_clause",
     "pylint.extensions.check_elif",
     "pylint.extensions.code_style",
     "pylint.extensions.confusing_elif",
     "pylint.extensions.comparison_placement",
@@ -288,30 +284,30 @@
 
 # Naming style matching correct attribute names.
 attr-naming-style = "snake_case"
 
 # Regular expression matching correct attribute names. Overrides attr-naming-
 # style. If left empty, attribute names will be checked with the set naming
 # style.
-attr-rgx = "[a-z_][a-z0-9_]{2,}$"
+attr-rgx = "[a-z_][a-z0-9_]{1,}$"
 
 # Bad variable names which should always be refused, separated by a comma.
 bad-names = ["foo", "bar", "baz", "toto", "tutu", "tata"]
 
 # Bad variable names regexes, separated by a comma. If names match any regex,
 # they will always be refused
 # bad-names-rgxs =
 
 # Naming style matching correct class attribute names.
 class-attribute-naming-style = "any"
 
 # Regular expression matching correct class attribute names. Overrides class-
 # attribute-naming-style. If left empty, class attribute names will be checked
 # with the set naming style.
-class-attribute-rgx = "([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$"
+class-attribute-rgx = "([A-Za-z_][A-Za-z0-9_]{1,30}|(__.*__))$"
 
 # Naming style matching correct class constant names.
 class-const-naming-style = "UPPER_CASE"
 
 # Regular expression matching correct class constant names. Overrides class-
 # const-naming-style. If left empty, class constant names will be checked with
 # the set naming style.
@@ -370,15 +366,15 @@
 inlinevar-rgx = "[A-Za-z_][A-Za-z0-9_]*$"
 
 # Naming style matching correct method names.
 method-naming-style = "snake_case"
 
 # Regular expression matching correct method names. Overrides method-naming-
 # style. If left empty, method names will be checked with the set naming style.
-method-rgx = "[a-z_][a-z0-9_]{2,}$"
+method-rgx = "(([a-z_][a-z0-9_]{2,})|(visit_.*))$"
 
 # Naming style matching correct module names.
 module-naming-style = "snake_case"
 
 # Regular expression matching correct module names. Overrides module-naming-
 # style. If left empty, module names will be checked with the set naming style.
 module-rgx = "(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$"
```

### Comparing `databricks_labs_ucx-0.21.0/PKG-INFO` & `databricks_labs_ucx-0.22.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: databricks-labs-ucx
-Version: 0.21.0
+Version: 0.22.0
 Summary: UCX - Unity Catalog Migration Toolkit
 Project-URL: Issues, https://github.com/databricks/ucx/issues
 Project-URL: Source, https://github.com/databricks/ucx
 Author-email: Serge Smertin <serge.smertin@databricks.com>
 Maintainer-email: Serge Smertin <serge.smertin@databricks.com>, Liran Bareket <liran.bareket@databricks.com>, Marcin Wojtyczka <marcin.wojtyczka@databricks.com>, Ziyuan Qin <ziyuan.qin@databricks.com>, William Conti <william.conti@databricks.com>, Hari Selvarajan <hari.selvarajan@databricks.com>, Vuong Nguyen <vuong.nguyen@databricks.com>
 License-File: LICENSE
 License-File: NOTICE
@@ -22,55 +22,66 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Requires-Dist: databricks-labs-blueprint~=0.4.3
-Requires-Dist: databricks-labs-lsql~=0.3.0
-Requires-Dist: databricks-sdk==0.23.0
+Requires-Dist: databricks-labs-lsql~=0.4.0
+Requires-Dist: databricks-sdk~=0.26.0
 Requires-Dist: pyyaml<7.0.0,>=6.0.0
+Requires-Dist: sqlglot<23.12,>=23.9
 Description-Content-Type: text/markdown
 
 Databricks Labs UCX
 ===
 ![UCX by Databricks Labs](docs/logo-no-background.png)
 
 The companion for upgrading to Unity Catalog. After [installation](#install-ucx), ensure to [trigger](#ensure-assessment-run-command) the [assessment workflow](#assessment-workflow), 
 so that you'll be able to [scope the migration](docs/assessment.md) and execute the [group migration workflow](#group-migration-workflow). 
-[`<installation_path>/README`](#readme-notebook) contains further instructions and explanations of these workflows.
-More workflows, like [migrating tables](docs/table_upgrade.md) and notebook code is coming in the future releases. 
+[`<installation_path>/README`](#readme-notebook) contains further instructions and explanations of these workflows. 
+Then you can execute [table migration workflow](#table-migration-workflow).
+More workflows, like notebook code migration is coming in the future releases. 
 UCX exposes a number of command line utilities accessible via `databricks labs ucx`.
 
-For questions, troubleshooting or bug fixes, please see your Databricks account team or submit [an issue](https://github.com/databrickslabs/ucx/issues). 
+For questions, troubleshooting or bug fixes, please see our [troubleshooting guide](docs/troubleshooting.md) or submit [an issue](https://github.com/databrickslabs/ucx/issues). 
 See [contributing instructions](CONTRIBUTING.md) to help improve this project.
 
 [![build](https://github.com/databrickslabs/ucx/actions/workflows/push.yml/badge.svg)](https://github.com/databrickslabs/ucx/actions/workflows/push.yml) [![codecov](https://codecov.io/github/databrickslabs/ucx/graph/badge.svg?token=p0WKAfW5HQ)](https://codecov.io/github/databrickslabs/ucx)  [![lines of code](https://tokei.rs/b1/github/databrickslabs/ucx)]([https://codecov.io/github/databrickslabs/ucx](https://github.com/databrickslabs/ucx))
 
 <!-- TOC -->
 * [Databricks Labs UCX](#databricks-labs-ucx)
 * [Installation](#installation)
   * [Authenticate Databricks CLI](#authenticate-databricks-cli)
   * [Install UCX](#install-ucx)
   * [[ADVANCED] Force install over existing UCX](#advanced-force-install-over-existing-ucx)
+  * [[ADVANCED] Installing UCX on all workspaces within a Databricks account](#advanced-installing-ucx-on-all-workspaces-within-a-databricks-account)
   * [Upgrading UCX for newer versions](#upgrading-ucx-for-newer-versions)
   * [Uninstall UCX](#uninstall-ucx)
 * [Migration process](#migration-process)
 * [Workflows](#workflows)
   * [Readme notebook](#readme-notebook)
   * [Assessment workflow](#assessment-workflow)
   * [Group migration workflow](#group-migration-workflow)
   * [Debug notebook](#debug-notebook)
   * [Debug logs](#debug-logs)
+  * [Table Migration Workflow](#table-migration-workflow)
+    * [Dependency CLI commands](#dependency-cli-commands)
+    * [Table Migration Workflow Tasks](#table-migration-workflow-tasks)
+    * [Other considerations](#other-considerations)
 * [Utility commands](#utility-commands)
+  * [`logs` command](#logs-command)
   * [`ensure-assessment-run` command](#ensure-assessment-run-command)
   * [`repair-run` command](#repair-run-command)
   * [`workflows` command](#workflows-command)
   * [`open-remote-config` command](#open-remote-config-command)
   * [`installations` command](#installations-command)
+* [Metastore related commands](#metastore-related-commands)
+  * [`show-all-metastores` command](#show-all-metastores-command)
+  * [`assign-metastore` command](#assign-metastore-command)
 * [Table migration commands](#table-migration-commands)
   * [`principal-prefix-access` command](#principal-prefix-access-command)
     * [Access for AWS S3 Buckets](#access-for-aws-s3-buckets)
     * [Access for Azure Storage Accounts](#access-for-azure-storage-accounts)
   * [`create-uber-principal` command](#create-uber-principal-command)
   * [`migrate-credentials` command](#migrate-credentials-command)
   * [`validate-external-locations` command](#validate-external-locations-command)
@@ -191,14 +202,27 @@
 
 * `UCX_FORCE_INSTALL=user databricks labs install ucx` - will force the installation to be for user only
 * `UCX_FORCE_INSTALL=global databricks labs install ucx` - will force the installation to be for root only
 
 
 [[back to top](#databricks-labs-ucx)]
 
+## [ADVANCED] Installing UCX on all workspaces within a Databricks account
+Setting the environment variable `UCX_FORCE_INSTALL` to 'account' will install UCX on all workspaces within a Databricks account.
+
+* `UCX_FORCE_INSTALL=account databricks labs install ucx`
+
+After the first installation, UCX will prompt the user to confirm whether to install UCX on the remaining workspaces with the same answers. If confirmed, the remaining installations will be completed silently.
+
+This installation mode will automatically select the following options:
+* Automatically create and enable HMS lineage init script
+* Automatically create a new SQL warehouse for UCX assessment
+
+[[back to top](#databricks-labs-ucx)]
+
 ## Upgrading UCX for newer versions
 
 Verify that UCX is installed
 
 ```commandline
 databricks labs installed
 
@@ -233,15 +257,15 @@
 ![macos_uninstall_ucx](docs/macos_4_databrickslabsmac_uninstallucx.gif)
 
 [[back to top](#databricks-labs-ucx)]
 
 # Migration process
 
 On the high level, the steps in migration process start with the [assessment workflow](#assessment-workflow), 
-followed by [group migration](#group-migration-workflow), [table migration](#table-migration-commands), 
+followed by [group migration](#group-migration-workflow), [table migration workflow](#table-migration-workflow), 
 finalised with the [code migration](#code-migration-commands). It can be described as:
 
 ```mermaid
 flowchart TD
     subgraph workspace-admin
         assessment --> group-migration
         group-migration --> table-migration
@@ -333,15 +357,15 @@
 
 See the [detailed design](docs/local-group-migration.md) of this workflow. It helps you to upgrade all Databricks workspace assets:
 Legacy Table ACLs, Entitlements, AWS instance profiles, Clusters, Cluster policies, Instance Pools, 
 Databricks SQL warehouses, Delta Live Tables, Jobs, MLflow experiments, MLflow registry, SQL Dashboards & Queries,
 SQL Alerts, Token and Password usage permissions that are set on the workspace level, Secret scopes, Notebooks,
 Directories, Repos, and Files. 
 
-Once done with the group migration, proceed to [table migration](#table-migration-commands).
+Once done with the group migration, proceed to [table migration workflow](#table-migration-workflow).
 
 Use [`validate-groups-membership` command](#validate-groups-membership-command) for extra confidence.
 If you don't have matching account groups, please run [`create-account-groups` command](#create-account-groups-command).
 
 The group migration workflow is designed to migrate workspace-local groups to account-level groups in the Unity Catalog (UC) environment. It ensures that all the necessary groups are available in the workspace with the correct permissions, and removes any unnecessary groups and permissions. The tasks in the group migration workflow depend on the output of the assessment workflow and can be executed in sequence to ensure a successful migration. The output of each task is stored in Delta tables in the `$inventory_database` schema, which can be used for further analysis and decision-making. The group migration workflow can be executed multiple times to ensure that all the groups are migrated successfully and that all the necessary permissions are assigned.
 
 1. `crawl_groups`: This task scans all groups for the local group migration scope.
@@ -371,16 +395,112 @@
 flush the logs every 10 minutes.
 
 To enable debug logs of [command-line interface](#authenticate-databricks-cli), 
 simply add `--debug` flag to any command.
 
 [[back to top](#databricks-labs-ucx)]
 
+## Table Migration Workflow
+
+The table migration workflow comprises multiple workflows and tasks designed to migrate tables from the Hive Metastore to the Unity Catalog. The subsequent diagram illustrates the workflow's tasks and their dependency CLI commands. 
+```mermaid
+flowchart TB
+    subgraph CLI
+      sync-workspace-info[sync-workspace-info] --> create_table_mapping[create-table-mapping]
+      create_table_mapping[create-table-mapping] --> create_catalogs_schemas[create-catalogs-schemas]
+      create_uber_principal[create-uber-principal]
+      principal_prefix_access[principal-prefix-access] --> migrate_credentials[migrate-credentials]
+      migrate_credentials --> migrate_locations[migrate-locations]
+      migrate_locations --> create_catalogs_schemas
+    end
+    
+    create_uber_principal --> workflow
+    create_table_mapping --> workflow
+    create_catalogs_schemas --> workflow
+    
+    subgraph workflow[Table Migration Workflows]
+      subgraph mt_workflow[workflow: migrate-tables]
+        dbfs_root_delta_mt_task[migrate_dbfs_root_delta_tables]
+        external_tables_sync_mt_task[migrate_external_tables_sync]
+        view_mt_task[roadmap: migrate_views]
+        dbfs_root_delta_mt_task --> view_mt_task
+        external_tables_sync_mt_task --> view_mt_task
+      end
+      
+      subgraph mt_ctas_wf[roadmap workflow: migrate-tables-ctas]
+        ctas_mt_task[migrate_tables_ctas] --> view_mt_task_ctas[roadmap: migrate_views]
+      end
+  
+      subgraph mt_serde_inplace_wf[roadmap workflow: migrate-external-hiveserde-tables-in-place-experimental]
+        serde_inplace_mt_task[migrate_external_hiveserde_tables_in_place_experimental] --> view_mt_task_inplace[roadmap: migrate_views]
+      end
+  
+      subgraph mt_in_mounts_wf[roadmap workflow: migrate-tables-in-mounts-experimental]
+        scan_tables_in_mounts_experimental_task[scan_tables_in_mounts_experimental] --> 
+        migrate_tables_in_mounts_experimental[migrate_tables_in_mounts_experimental]
+      end
+    end
+    
+    classDef roadmap stroke:Green,stroke-width:2px,color:Green,stroke-dasharray: 8 3
+    class view_mt_task roadmap;
+    class mt_ctas_wf,ctas_mt_task,view_mt_task_ctas roadmap;
+    class mt_serde_inplace_wf,serde_inplace_mt_task,view_mt_task_inplace roadmap;
+    class mt_in_mounts_wf,scan_tables_in_mounts_experimental_task,migrate_tables_in_mounts_experimental roadmap;
+```
+More details can be found in the [design of table migration](docs/table_upgrade.md)
+
+### Dependency CLI commands
+- [`create-table-mapping`](#create-table-mapping-command) - Create `mapping.csv` which will be used by the workflow to identify the targets catalog, schema, table of the HMS table to be migrated. User should review and update the mapping file accordingly before proceeding with the migration workflow.
+- [`principal-prefix-access`](#principal-prefix-access-command) - Identify all the storages used in the workspace and corresponding Azure Service Principal or IAM role that are used in the workspace. It outputs `azure_storage_account_info.csv` or `uc_roles_access.csv` which will be later used by [`migrate-credentials`](#migrate-credentials-command) command to create UC storage credentials. The csv can be edited to control which IAM roles or Azure Service Principals should be used to create UC storage credentials later.
+- [`migrate-credentials`](#migrate-credentials-command) - Create UC storage credentials based on the Azure Service Principal or IAM role (`azure_storage_account_info.csv` or `uc_roles_access.csv`) identified by [`principal-prefix-access`](#principal-prefix-access-command) command.
+- [`migrate-locations`](#migrate-locations-command) - Create missing external locations in the Unity Catalog. 
+- [`create-catalogs-schemas`](#create-catalogs-schemas-command) - Create missing catalogs and schemas in the Unity Catalog. The candidate catalogs and schemas is based on `mapping.csv`
+- [`create-uber-principal`](#create-uber-principal-command) - Create an Uber Principal with access to all storages used in the workspace. This principal will be used by the workflow job cluster to migrate all the tables in the workspace.
+
+[`create-table-mapping`](#create-table-mapping-command) and [`create-uber-principal`](#create-uber-principal-command) are required to run the workflow. While other commands are optional, as long as the UC storage credentials, external locations, catalogs and schemas needed for successful migration are created.
+
+To control the scope of the table migration, consider utilizing a combination of editing `mapping.csv`, employing [`skip`](#skip-command) command, and [`revert-migrated-tables`](#revert-migrated-tables-command) command.
+
+See more details in [Table migration commands](#table-migration-commands)
+
+### Table Migration Workflow Tasks
+- `migrate_dbfs_root_delta_tables` - Migrate delta tables from the DBFS root using deep clone, along with legacy table ACL migrated if any.
+- `migrate_external_tables_sync` - Migrate external tables using [`SYNC`](https://docs.databricks.com/en/sql/language-manual/sql-ref-syntax-aux-sync.html) command, along with legacy table ACL migrated if any.
+- Following workflows/tasks are on the roadmap and being developed:
+  - Migrate view
+  - Migrate tables using CTAS
+  - Optionally and experimentally in place migrate ParquetHiveSerDe, OrcSerde, AvroSerDe, LazySimpleSerDe, JsonSerDe, OpenCSVSerde tables.
+  - Experimentally migrate Delta and Parquet data found in dbfs mount but not registered as Hive Metastore table into UC tables.
+
+### Other considerations
+- You may need to run the workflow multiple times to ensure all the tables are migrated successfully in phases.
+- If your delta tables in DBFS root have large number of files, consider:
+  - Setting higher Min and Max workers for auto-scale when being asked during the UCX installation. More nodes/cores in the cluster means more concurrency for calling cloud storage api to copy files when deep cloning the delta tables.
+  - Setting higher "Parallelism for migrating dbfs root delta tables with deep clone" (default 200) when being asked during the UCX installation. This controls the number of Spark task/partition to be created for deep clone.
+- Consider create an instance pool, and set the instance pool id when being asked during the UCX installation. This instance pool will be put into the cluster policy used by all UCX workflows job clusters.
+- You may also manually edit the job cluster configration per job or per task after the workflows are deployed.
+
+[[back to top](#databricks-labs-ucx)]
+
 # Utility commands
 
+## `logs` command
+
+```text
+$ databricks labs ucx logs [--workflow WORKFLOW_NAME] [--debug]
+```
+
+This command displays the logs of the last run of the specified workflow. If no workflow is specified, it displays 
+the logs of the workflow that was run the last. This command is useful for developers and administrators who want to 
+check the logs of the last run of a workflow and ensure that it was executed as expected. It can also be used for 
+debugging purposes when a workflow is not behaving as expected. By default, only `INFO`, `WARNING`, and `ERROR` logs
+are displayed. To display `DEBUG` logs, use the `--debug` flag.
+
+[[back to top](#databricks-labs-ucx)] 
+
 ## `ensure-assessment-run` command
 
 ```commandline
 databricks labs ucx ensure-assessment-run
 ```
 
 This command ensures that the [assessment workflow](#assessment-workflow) was run on a workspace. 
@@ -479,17 +599,46 @@
 This command displays the [installations](#installation) by different users on the same workspace. It fetches all 
 the installations where the `ucx` package is installed and prints their details in JSON format. This command is useful 
 for administrators who want to see which users have installed `ucx` and where. It can also be used to debug issues 
 related to multiple installations of `ucx` on the same workspace.
 
 [[back to top](#databricks-labs-ucx)]
 
+# Metastore related commands
+
+These commands are used to assign a Unity Catalog metastore to a workspace. The metastore assignment is a pre-requisite
+for any further migration steps.
+
+[[back to top](#databricks-labs-ucx)]
+
+## `show-all-metastores` command
+
+```text
+databricks labs ucx show-all-metastores [--workspace-id <workspace-id>]
+```
+
+This command lists all the metastores available to be assigned to a workspace. If no workspace is specified, it lists
+all the metastores available in the account. This command is useful when there are multiple metastores available within
+a region and you want to see which ones are available for assignment.
+
+[[back to top](#databricks-labs-ucx)]
+
+## `assign-metastore` command
+
+```text
+databricks labs ucx assign-metastore --workspace-id <workspace-id> [--metastore-id <metastore-id>]
+```
+
+This command assigns a metastore to a workspace with `workspace-id`. If there is only a single metastore in the workspace
+region, it will be automatically assigned to the workspace. If there are multiple metastores available, you need to specify
+the metastore id of the metastore you want to assign to the workspace.
+
 # Table migration commands
 
-These commands are vital part of [table migration](docs/table_upgrade.md) process and require 
+These commands are vital part of [table migration workflow](#table-migration-workflow) process and require 
 the [assessment workflow](#assessment-workflow) and 
 [group migration workflow](#group-migration-workflow) to be completed. 
 See the [migration process diagram](#migration-process) to understand the role of the table migration commands in 
 the migration process. 
 
 The first step is to run the [`principal-prefix-access` command](#principal-prefix-access-command) to identify all 
 the storage accounts used by tables in the workspace and their permissions on each storage account.
@@ -562,15 +711,15 @@
 
 **Requires Cloud IAM admin privileges.** Once the [`assessment` workflow](#assessment-workflow) complete, you should run 
 this command to creates a service principal with the _**read-only access to all storage**_ used by tables in this 
 workspace and configure the [UCX Cluster Policy](#installation) with the details of it. Once migration is complete, this
 service principal should be unprovisioned. On Azure, it creates a principal with `Storage Blob Data Reader` role 
 assignment on every storage account using Azure Resource Manager APIs.
 
-Once done, proceed to the launching the [table migration workflow](#table-migration-commands).
+This command is one of prerequisites for the [table migration workflow](#table-migration-workflow).
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `migrate-credentials` command
 
 ```commandline
 databricks labs ucx migrate-credentials
@@ -636,27 +785,29 @@
 easier in your favorite spreadsheet application.
 
 Once you're done with this command, [create catalogs and schemas](#create-catalogs-schemas-command). During 
 multiple runs of the table migration workflow, you can use the [`revert-migrated-tables` command](#revert-migrated-tables-command)
 to revert the tables that were migrated in the previous run. You can also skip the tables that you don't want to migrate
 using the [`skip` command](#skip-command).
 
+This command is one of prerequisites for the [table migration workflow](#table-migration-workflow).
+
 Once you're done with table migration, proceed to the [code migration](#code-migration-commands).
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `skip` command
 
 ```text
 databricks labs ucx skip --schema X [--table Y]  
 ```
 
 Anywhere after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
 
-This command allows users to skip certain schemas or tables during the [table migration](docs/table_upgrade.md) process.
+This command allows users to skip certain schemas or tables during the [table migration](#table-migration-workflow) process.
 The command takes `--schema` and optionally `--table` flags to specify the schema and table to skip. If no `--table` flag 
 is provided, all tables in the specified HMS database are skipped.
 This command is useful to temporarily disable migration on a particular schema or table.
 
 Once you're done with table migration, proceed to the [code migration](#code-migration-commands).
 
 [[back to top](#databricks-labs-ucx)]
@@ -665,42 +816,40 @@
 
 ```text
 databricks labs ucx revert-migrated-tables --schema X --table Y [--delete-managed]  
 ```
 
 Anywhere after [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command.
 
-This command removes the `upgraded_from` property on a migrated table for re-migration in the [table upgrade](docs/table_upgrade.md) process. 
+This command removes the `upgraded_from` property on a migrated table for re-migration in the [table migration](#table-migration-workflow) process. 
 This command is useful for developers and administrators who want to revert the migration of a table. It can also be used 
 to debug issues related to table migration.
 
 Go back to the [`create-table-mapping` command](#create-table-mapping-command) after you're done with this command.
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `create-catalogs-schemas` command
 
 ```text
 databricks labs ucx create-catalogs-schemas
 ```
 After [`create-table-mapping` command](#create-table-mapping-command) is executed, you can run this command to have the required UC catalogs and schemas created.
-This command is supposed to be run before migrating tables to UC.
-
-Once you're done with this command, proceed to the [table migration workflow](#table-migration-commands).
+This command is supposed to be run before migrating tables to UC using [table migration workflow](#table-migration-workflow).
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `move` command
 
 ```text
 databricks labs ucx move --from-catalog A --from-schema B --from-table C --to-catalog D --to-schema E  
 ```
 
 This command moves a UC table/tables from one schema to another schema after
-the [table upgrade](docs/table_upgrade.md) process. This is useful for developers and administrators who want 
+the [table migration](#table-migration-workflow) process. This is useful for developers and administrators who want 
 to adjust their catalog structure after tables upgrade.
 
 Users will be prompted whether tables/view are dropped after moving to new schema. This only applies to `MANAGED` tables and views.
 
 This command moves different table types differently:
 - `MANAGED` tables are deep-cloned to the new schema. 
 - `EXTERNAL` tables are dropped from the original schema, then created in the target schema using the same location. 
@@ -724,28 +873,28 @@
 
 [[back to top](#databricks-labs-ucx)]
 
 # Code migration commands
 
 See the [migration process diagram](#migration-process) to understand the role of the code migration commands in the migration process.
 
-After you're done with the [table migration](#table-migration-commands), you can proceed to the code migration.
+After you're done with the [table migration](#table-migration-workflow), you can proceed to the code migration.
 
 Once you're done with the code migration, you can run the [`cluster-remap` command](#cluster-remap-command) to remap the
 clusters to be UC compatible.
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `migrate-local-code` command
 
 ```text
 databricks labs ucx migrate-local-code
 ```
 
-**(Experimental)** Once [table migration](#table-migration-commands) is complete, you can run this command to 
+**(Experimental)** Once [table migration](#table-migration-workflow) is complete, you can run this command to 
 migrate all python and SQL files in the current working directory. This command is highly experimental and
 at the moment only supports Python and SQL files and discards code comments and formatting during 
 the automated transformation process.
 
 [[back to top](#databricks-labs-ucx)]
 
 # Cross-workspace installations
@@ -773,15 +922,15 @@
 14:07:10  INFO [d.l.blueprint.parallel][finding_ucx_installations_0] finding ucx installations 20/88, rps: 32.110/sec
 14:07:11  INFO [d.l.blueprint.parallel][finding_ucx_installations_18] finding ucx installations 30/88, rps: 39.786/sec
 ...
 ```
 
 **Requires Databricks Account Administrator privileges.** This command uploads the workspace config to all workspaces 
 in the account where `ucx` is installed. This command is necessary to create an immutable default catalog mapping for
-[table migration](docs/table_upgrade.md) process and is the prerequisite 
+[table migration](#table-migration-workflow) process and is the prerequisite 
 for [`create-table-mapping` command](#create-table-mapping-command).
 
 If you cannot get account administrator privileges in reasonable time, you can take the risk and 
 run [`manual-workspace-info` command](#manual-workspace-info-command) to enter Databricks Workspace IDs and Databricks 
 Workspace names. 
 
 [[back to top](#databricks-labs-ucx)]
@@ -844,15 +993,15 @@
 ```
 
 This command validates the groups to see if the groups at the account level and workspace level have different membership.
 This command is useful for administrators who want to ensure that the groups have the correct membership. It can also be
 used to debug issues related to group membership. See [group migration](docs/local-group-migration.md) and 
 [group migration](#group-migration-workflow) for more details.
 
-Once you're done with this command, proceed to the [table migration](#table-migration-commands).
+Valid group membership is important to ensure users has correct access after legacy table ACL is migrated in [table migration workflow](#table-migration-workflow)
 
 [[back to top](#databricks-labs-ucx)]
 
 ## `cluster-remap` command
 
 ```text
 $ databricks labs ucx cluster-remap
```

