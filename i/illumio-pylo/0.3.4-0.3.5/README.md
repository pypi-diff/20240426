# Comparing `tmp/illumio_pylo-0.3.4.tar.gz` & `tmp/illumio_pylo-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "illumio_pylo-0.3.4.tar", last modified: Wed Apr 10 12:13:52 2024, max compression
+gzip compressed data, was "illumio_pylo-0.3.5.tar", last modified: Fri Apr 26 14:52:26 2024, max compression
```

## Comparing `illumio_pylo-0.3.4.tar` & `illumio_pylo-0.3.5.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.973493 illumio_pylo-0.3.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.957493 illumio_pylo-0.3.4/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.953493 illumio_pylo-0.3.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.957493 illumio_pylo-0.3.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.github/workflows/doxygen-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.github/workflows/make-binaries.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-10 12:13:52.973493 illumio_pylo-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.961493 illumio_pylo-0.3.4/dev_playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/check_unique_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/check_unique_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/delete_all_workloads.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/delete_unused_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/explorer_report_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    27080 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/export_rules_to_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/generate-random-workloads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/healthcheck_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/import-labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/import_workloads_placeholders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/iplists_stats_duplicates_unused_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/recalculate_explorer_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/recalculate_explorer_logs_multithreaded.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/rules_exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/rules_exporter_special.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/test_change_workload_desc.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/test_query2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/test_securityprincipals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14824 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/ven_idle_to_illumination.py
--rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/dev_playground/ven_reassign_pce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.961493 illumio_pylo-0.3.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/examples/explorer_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/examples/extend_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.965493 illumio_pylo-0.3.4/illumio_pylo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.965493 illumio_pylo-0.3.4/illumio_pylo/API/
--rw-r--r--   0 runner    (1001) docker     (127)    60500 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/APIConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/AuditLog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/ClusterHealth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/CredentialsManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    47590 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/Explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/JsonPayloadTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/RuleSearchQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/API/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/AgentStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.965493 illumio_pylo-0.3.4/illumio_pylo/Helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21890 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Helpers/exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Helpers/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/IPList.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/IPMap.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/LabelCommon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/LabelGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    19809 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/LabelStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/LabeledObject.py
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/ReferenceTracker.py
--rw-r--r--   0 runner    (1001) docker     (127)    26352 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Ruleset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/RulesetStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/SecurityPrincipal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8280 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/SoftwareVersion.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/VirtualService.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/VirtualServiceStore.py
--rw-r--r--   0 runner    (1001) docker     (127)    19677 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/Workload.py
--rw-r--r--   0 runner    (1001) docker     (127)    10947 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/WorkloadStore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/WorkloadStoreSubClasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.965493 illumio_pylo-0.3.4/illumio_pylo/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/NativeParsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.969493 illumio_pylo-0.3.4/illumio_pylo/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/credential_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/iplist_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/iplist_import_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/ruleset_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/update_pce_objects_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.969493 illumio_pylo-0.3.4/illumio_pylo/cli/commands/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/utils/LabelCreation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_compatibility_report_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    19579 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_duplicate_remover.py
--rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_idle_to_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_upgrader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_reset_names_to_null.py
--rw-r--r--   0 runner    (1001) docker     (127)    28484 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_used_in_rule_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.969493 illumio_pylo-0.3.4/illumio_pylo/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    74257 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/docs/Doxygen
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.973493 illumio_pylo-0.3.4/illumio_pylo/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/credentials.example.json
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/health_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.973493 illumio_pylo-0.3.4/illumio_pylo/utilities/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/resources/iplists-import-example.csv
--rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/resources/iplists-import-example.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/resources/workload-exporter-filter-example.csv
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/resources/workloads-import-example.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/illumio_pylo/utilities/resources/workloads-import-example.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 12:13:52.973493 illumio_pylo-0.3.4/illumio_pylo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-10 12:13:52.000000 illumio_pylo-0.3.4/illumio_pylo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-10 12:13:52.000000 illumio_pylo-0.3.4/illumio_pylo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 12:13:52.000000 illumio_pylo-0.3.4/illumio_pylo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 12:13:52.000000 illumio_pylo-0.3.4/illumio_pylo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 12:13:52.000000 illumio_pylo-0.3.4/illumio_pylo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 12:13:52.973493 illumio_pylo-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-10 12:13:45.000000 illumio_pylo-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.776455 illumio_pylo-0.3.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.760455 illumio_pylo-0.3.5/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.760455 illumio_pylo-0.3.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.760455 illumio_pylo-0.3.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/.github/workflows/doxygen-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/.github/workflows/make-binaries.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    10172 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-26 14:52:26.776455 illumio_pylo-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.764455 illumio_pylo-0.3.5/dev_playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/check_unique_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/check_unique_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/delete_all_workloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/delete_unused_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/explorer_report_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27080 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/export_rules_to_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/generate-random-workloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/healthcheck_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/import-labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/import_workloads_placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/iplists_stats_duplicates_unused_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/recalculate_explorer_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/recalculate_explorer_logs_multithreaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/rules_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/rules_exporter_special.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/test_change_workload_desc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/test_query2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/test_securityprincipals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14824 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/ven_idle_to_illumination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7700 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/dev_playground/ven_reassign_pce.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.764455 illumio_pylo-0.3.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/examples/explorer_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/examples/extend_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.768455 illumio_pylo-0.3.5/illumio_pylo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.772455 illumio_pylo-0.3.5/illumio_pylo/API/
+-rw-r--r--   0 runner    (1001) docker     (127)    60633 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/API/APIConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/API/AuditLog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/API/ClusterHealth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/API/CredentialsManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47590 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/API/Explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7984 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/API/JsonPayloadTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/API/RuleSearchQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/API/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/AgentStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/Exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.772455 illumio_pylo-0.3.5/illumio_pylo/Helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/Helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21890 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/Helpers/exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/Helpers/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/IPList.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/IPMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/Label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/LabelCommon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/LabelGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19917 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/LabelStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/LabeledObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/Organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/Query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/ReferenceTracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26827 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/Rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/Ruleset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/RulesetStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/SecurityPrincipal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/Service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/SoftwareVersion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/VirtualService.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/VirtualServiceStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19910 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/Workload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/WorkloadStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6093 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/WorkloadStoreSubClasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.772455 illumio_pylo-0.3.5/illumio_pylo/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/NativeParsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.776455 illumio_pylo-0.3.5/illumio_pylo/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/credential_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/iplist_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/iplist_import_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/ruleset_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/update_pce_objects_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.776455 illumio_pylo-0.3.5/illumio_pylo/cli/commands/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/utils/LabelCreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/ven_compatibility_report_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19579 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/ven_duplicate_remover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/ven_idle_to_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/ven_upgrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/workload_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18939 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/workload_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/workload_reset_names_to_null.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28484 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/workload_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/cli/commands/workload_used_in_rule_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.776455 illumio_pylo-0.3.5/illumio_pylo/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    74257 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/docs/Doxygen
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.776455 illumio_pylo-0.3.5/illumio_pylo/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/utilities/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/utilities/credentials.example.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/utilities/health_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.776455 illumio_pylo-0.3.5/illumio_pylo/utilities/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/utilities/resources/iplists-import-example.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/utilities/resources/iplists-import-example.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/utilities/resources/workload-exporter-filter-example.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/utilities/resources/workloads-import-example.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/illumio_pylo/utilities/resources/workloads-import-example.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:52:26.776455 illumio_pylo-0.3.5/illumio_pylo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12249 2024-04-26 14:52:26.000000 illumio_pylo-0.3.5/illumio_pylo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-26 14:52:26.000000 illumio_pylo-0.3.5/illumio_pylo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:52:26.000000 illumio_pylo-0.3.5/illumio_pylo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-26 14:52:26.000000 illumio_pylo-0.3.5/illumio_pylo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 14:52:26.000000 illumio_pylo-0.3.5/illumio_pylo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:52:26.776455 illumio_pylo-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-26 14:52:20.000000 illumio_pylo-0.3.5/setup.py
```

### Comparing `illumio_pylo-0.3.4/.devcontainer/devcontainer.json` & `illumio_pylo-0.3.5/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/.github/workflows/doxygen-publish.yml` & `illumio_pylo-0.3.5/.github/workflows/doxygen-publish.yml`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/.github/workflows/make-binaries.yml` & `illumio_pylo-0.3.5/.github/workflows/make-binaries.yml`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/.github/workflows/python-publish.yml` & `illumio_pylo-0.3.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/LICENSE` & `illumio_pylo-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/PKG-INFO` & `illumio_pylo-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: illumio_pylo
-Version: 0.3.4
+Version: 0.3.5
 Summary: A set of tools and library for working with Illumio PCE
 Home-page: https://github.com/cpainchaud/pylo
 Author: Christophe Painchaud
 Author-email: shellescape@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `illumio_pylo-0.3.4/README.md` & `illumio_pylo-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/check_unique_hostnames.py` & `illumio_pylo-0.3.5/dev_playground/check_unique_hostnames.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/check_unique_services.py` & `illumio_pylo-0.3.5/dev_playground/check_unique_services.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/delete_all_workloads.py` & `illumio_pylo-0.3.5/dev_playground/delete_all_workloads.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/delete_unused_services.py` & `illumio_pylo-0.3.5/dev_playground/delete_unused_services.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/explorer_report_exporter.py` & `illumio_pylo-0.3.5/dev_playground/explorer_report_exporter.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/export_rules_to_firewall.py` & `illumio_pylo-0.3.5/dev_playground/export_rules_to_firewall.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/generate-random-workloads.py` & `illumio_pylo-0.3.5/dev_playground/generate-random-workloads.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/healthcheck_log.py` & `illumio_pylo-0.3.5/dev_playground/healthcheck_log.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/import-labels.py` & `illumio_pylo-0.3.5/dev_playground/import-labels.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/import_workloads_placeholders.py` & `illumio_pylo-0.3.5/dev_playground/import_workloads_placeholders.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/iplists_stats_duplicates_unused_finder.py` & `illumio_pylo-0.3.5/dev_playground/iplists_stats_duplicates_unused_finder.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/recalculate_explorer_logs.py` & `illumio_pylo-0.3.5/dev_playground/recalculate_explorer_logs.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/recalculate_explorer_logs_multithreaded.py` & `illumio_pylo-0.3.5/dev_playground/recalculate_explorer_logs_multithreaded.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/rules_exporter.py` & `illumio_pylo-0.3.5/dev_playground/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/rules_exporter_special.py` & `illumio_pylo-0.3.5/dev_playground/rules_exporter_special.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/test.py` & `illumio_pylo-0.3.5/dev_playground/test.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/test_change_workload_desc.py` & `illumio_pylo-0.3.5/dev_playground/test_change_workload_desc.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/test_query.py` & `illumio_pylo-0.3.5/dev_playground/test_query.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/test_query2.py` & `illumio_pylo-0.3.5/dev_playground/test_query2.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/test_securityprincipals.py` & `illumio_pylo-0.3.5/dev_playground/test_securityprincipals.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/ven_idle_to_illumination.py` & `illumio_pylo-0.3.5/dev_playground/ven_idle_to_illumination.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/dev_playground/ven_reassign_pce.py` & `illumio_pylo-0.3.5/dev_playground/ven_reassign_pce.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/examples/explorer_query.py` & `illumio_pylo-0.3.5/examples/explorer_query.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/examples/extend_cli.py` & `illumio_pylo-0.3.5/examples/extend_cli.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/API/APIConnector.py` & `illumio_pylo-0.3.5/illumio_pylo/API/APIConnector.py`

 * *Files 0% similar despite different names*

```diff
@@ -621,20 +621,22 @@
         for item in response:
             if item['created_by']['href'] == '/users/0':
                 return item['href']
 
         return None
 
     def objects_ven_get(self,
-                             include_deleted=False,
-                             filter_by_ip: str = None,
-                             filter_by_label: Optional[WorkloadsGetQueryLabelFilterJsonStructure] = None,
-                             filter_by_name: str = None,
-                             max_results: int = None,
-                             async_mode=True) -> List[VenObjectJsonStructure]:
+                        include_deleted=False,
+                        filter_by_ip: str = None,
+                        filter_by_label: Optional[WorkloadsGetQueryLabelFilterJsonStructure] = None,
+                        filter_by_name: str = None,
+                        max_results: int = None,
+                        async_mode=True,
+                        representation: Optional[Literal['ven_labels']] = None
+                        ) -> List[VenObjectJsonStructure]:
         path = '/vens'
         data = {}
 
         if include_deleted:
             data['include_deleted'] = 'yes'
 
         if filter_by_ip is not None:
@@ -648,15 +650,14 @@
             data['name'] = filter_by_name
 
         if max_results is not None:
             data['max_results'] = max_results
 
         return self.do_get_call(path=path, async_call=async_mode, params=data)
 
-
     def objects_workload_get(self,
                              include_deleted=False,
                              filter_by_ip: str = None,
                              filter_by_label: WorkloadsGetQueryLabelFilterJsonStructure=None,
                              filter_by_name: str = None,
                              filter_by_managed: bool = None,
                              filer_by_policy_health: Literal['active', 'warning', 'error'] = None,
@@ -931,26 +932,28 @@
 
     def object_network_device_endpoints_get(self, network_device_href: str) -> List[NetworkDeviceEndpointObjectJsonStructure]:
         path = '{}/network_endpoints'.format(network_device_href)
         data = {}
 
         return self.do_get_call(path=path, async_call=False, include_org_id=False )
 
-    def object_network_device_endpoint_create(self, network_device_href: str, name: str, endpoint_type: Literal['switch_port'], workloads_href: List[str]) -> List[NetworkDeviceEndpointObjectJsonStructure]:
+    def object_network_device_endpoint_create(self, network_device_href: str, name: str,
+                                              endpoint_type: Literal['switch_port'], workloads_href: List[str]) \
+            -> List[NetworkDeviceEndpointObjectJsonStructure]:
+
         path = '{}/network_endpoints'.format(network_device_href)
 
-        worklaods_href_objects = []
+        workloads_href_objects = []
         for workload_href in workloads_href:
-            worklaods_href_objects.append({'href': workload_href})
+            workloads_href_objects.append({'href': workload_href})
 
-        data = { 'config': { 'name': name, 'endpoint_type': endpoint_type }, 'workloads': worklaods_href_objects}
+        data = {'config': {'name': name, 'endpoint_type': endpoint_type}, 'workloads': workloads_href_objects}
 
         return self.do_post_call(path=path, async_call=False, include_org_id=False, json_arguments=data, json_output_expected=True)
 
-
     def objects_ruleset_get(self, max_results: int = None, async_mode=True) -> List[RulesetObjectJsonStructure]:
         path = '/sec_policy/draft/rule_sets'
         data = {}
 
         if max_results is not None:
             data['max_results'] = max_results
 
@@ -1065,15 +1068,15 @@
             'consuming_security_principals': consuming_security_principals,
             'resolve_labels_as': {'providers': resolve_providers, 'consumers': resolve_consumers,},
             'consumers': consumers_json,
             'providers': providers_json,
             'ingress_services': services_json
         }
 
-        path = ruleset_href+'/sec_rules'
+        path = ruleset_href + '/sec_rules'
 
         return self.do_post_call(path, json_arguments=data, json_output_expected=True, include_org_id=False)
 
     def objects_securityprincipal_get(self, max_results: int = None, async_mode=True) -> List[SecurityPrincipalObjectJsonStructure]:
         path = '/security_principals'
         data = {}
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/API/AuditLog.py` & `illumio_pylo-0.3.5/illumio_pylo/API/AuditLog.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/API/ClusterHealth.py` & `illumio_pylo-0.3.5/illumio_pylo/API/ClusterHealth.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/API/CredentialsManager.py` & `illumio_pylo-0.3.5/illumio_pylo/API/CredentialsManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import base64
 from hashlib import sha256
 from typing import Dict, TypedDict, Union, List, Optional
 import json
 import os
 from cryptography.fernet import Fernet
+from cryptography.hazmat.primitives.ciphers.aead import ChaCha20Poly1305
 from ..Exception import PyloEx
 from .. import log
 
 try:
     import paramiko
 except ImportError:
     log.debug("Paramiko library not found, SSH based encryption will not be available")
@@ -118,27 +119,27 @@
         if credential_profile.name.lower() == fqdn_or_profile_name.lower():
             return credential_profile
         if credential_profile.fqdn.lower() == fqdn_or_profile_name.lower():
             return credential_profile
 
     if fail_with_an_exception:
         raise PyloEx("No profile found in credential file '{}' with fqdn: {}".
-                    format(credential_file, fqdn_or_profile_name))
+                     format(credential_file, fqdn_or_profile_name))
 
     return None
 
 
 def list_potential_credential_files() -> List[str]:
     """
     List the potential locations where a credential file could be found and return them if they exist
     :return:
     """
     potential_credential_files = []
-    if os.environ.get('Pylo_CREDENTIAL_FILE', None) is not None:
-        potential_credential_files.append(os.environ.get('Pylo_CREDENTIAL_FILE'))
+    if os.environ.get('PYLO_CREDENTIAL_FILE', None) is not None:
+        potential_credential_files.append(os.environ.get('PYLO_CREDENTIAL_FILE'))
     potential_credential_files.append(os.path.expanduser("~/.pylo/credentials.json"))
     potential_credential_files.append(os.path.join(os.getcwd(), "credentials.json"))
 
     return [file for file in potential_credential_files if os.path.exists(file)]
 
 
 def get_all_credentials() -> List[CredentialProfile]:
@@ -149,15 +150,15 @@
     credential_files = list_potential_credential_files()
     credentials = []
     for file in credential_files:
         credentials.extend(get_all_credentials_from_file(file))
     return credentials
 
 
-def create_credential_in_file(file_full_path: str, data: CredentialFileEntry, overwrite_existing_profile = False) -> str:
+def create_credential_in_file(file_full_path: str, data: CredentialFileEntry, overwrite_existing_profile=False) -> str:
     """
     Create a credential in a file and return the full path to the file
     :param file_full_path:
     :param data:
     :param overwrite_existing_profile:
     :return:
     """
@@ -169,73 +170,65 @@
         with open(file_full_path, 'r') as f:
             credentials: CredentialsFileType = json.load(f)
             if isinstance(credentials, list):
                 # check if the profile already exists
                 for profile in credentials:
                     if profile['name'].lower() == data['name'].lower():
                         if overwrite_existing_profile:
-                            profile = data
+                            # profile is a dict, remove of all its entries
+                            for key in list(profile.keys()):
+                                del profile[key]
+                            profile.update(data)
                             break
                         else:
                             raise PyloEx("Profile with name {} already exists in file {}".format(data['name'], file_full_path))
                 credentials.append(data)
             else:
                 if data['name'].lower() == credentials['name'].lower():
                     if overwrite_existing_profile:
                         credentials = data
                     else:
                         raise PyloEx("Profile with name {} already exists in file {}".format(data['name'], file_full_path))
                 else:
                     credentials = [credentials, data]
     else:
-            credentials = [data]
+        credentials = [data]
 
     # write to the file
     with open(file_full_path, 'w') as f:
         json.dump(credentials, f, indent=4)
 
     return file_full_path
 
+
 def create_credential_in_default_file(data: CredentialFileEntry) -> str:
     """
     Create a credential in the default credential file and return the full path to the file
     :param data:
     :return:
     """
     file_path = os.path.expanduser("~/.pylo/credentials.json")
     create_credential_in_file(os.path.expanduser(file_path), data)
     return file_path
 
 
-def encrypt_api_key_with_paramiko_ssh_key_fernet(ssh_key: paramiko.AgentKey, api_key: str) -> str:
-    def encrypt(raw: str, key: bytes) -> bytes:
-        """
-
-        :param raw:
-        :param key:
-        :return: base64 encoded encrypted string
-        """
-        f = Fernet(base64.urlsafe_b64encode(key))
-        token = f.encrypt(bytes(raw, 'utf-8'))
-        return token
-
-
-    # generate a random 128bit key
-    session_key_to_sign = os.urandom(32)
-
-    signed_message = ssh_key.sign_ssh_data(session_key_to_sign)
-
-    # use SHA256 to hash the signed message and use it as final AES 256 key
-    encryption_key = sha256(signed_message).digest()
-    #print("Encryption key: {}".format(encryption_key.hex()))
-    encrypted_text = encrypt(api_key, encryption_key)
-
-    api_key = "$encrypted$:ssh-Fernet:{}:{}:{}".format(base64.urlsafe_b64encode(ssh_key.get_fingerprint()).decode('utf-8'),
-                                                       base64.urlsafe_b64encode(session_key_to_sign).decode('utf-8'),
-                                                       encrypted_text.decode('utf-8'))
+def encrypt_api_key_with_paramiko_ssh_key_chacha20poly1305(ssh_key: paramiko.AgentKey, api_key: str) -> str:
+    seed_key_to_be_signed = os.urandom(32)
+    signed_seed_key = ssh_key.sign_ssh_data(seed_key_to_be_signed)
+    encryption_key = sha256(signed_seed_key).digest()
+
+    nonce = seed_key_to_be_signed[:12]
+    chacha20_object = ChaCha20Poly1305(encryption_key)
+
+    encrypted_text = chacha20_object.encrypt(nonce, bytes(api_key, 'utf-8'), ssh_key.get_fingerprint())
+
+    api_key = "$encrypted$:ssh-ChaCha20Poly1305:{}:{}:{}".format(
+        base64.urlsafe_b64encode(ssh_key.get_fingerprint()).decode('utf-8'),
+        base64.urlsafe_b64encode(seed_key_to_be_signed).decode('utf-8'),
+        base64.urlsafe_b64encode(encrypted_text).decode('utf-8'))
 
     return api_key
 
 
 def decrypt_api_key_with_paramiko_ssh_key_fernet(encrypted_api_key_payload: str) -> str:
     def decrypt(token_b64_encoded: str, key: bytes):
         f = Fernet(base64.urlsafe_b64encode(key))
@@ -247,40 +240,66 @@
         raise PyloEx("Invalid encrypted API key format")
 
     # get the fingerprint and the session key
     fingerprint = base64.urlsafe_b64decode(api_key_parts[2])
     session_key = base64.urlsafe_b64decode(api_key_parts[3])
     encrypted_api_key = api_key_parts[4]
 
-    # find the key in the agent
-    keys = paramiko.Agent().get_keys()
-    found_key = None
-    for key in keys:
-        if key.get_fingerprint() == fingerprint:
-            found_key = key
-            break
-
-    if found_key is None:
+    ssh_key = find_ssh_key_from_fingerprint(fingerprint)
+    if ssh_key is None:
         raise PyloEx("No key found in the agent with fingerprint {}".format(fingerprint.hex()))
 
     # sign the session key
-    signed_session_key = found_key.sign_ssh_data(session_key)
+    signed_session_key = ssh_key.sign_ssh_data(session_key)
     encryption_key = sha256(signed_session_key).digest()
-    #print("Encryption key: {}".format(encryption_key.hex()))
-    #print("Encrypted from KEY fingerprint: {}".format(fingerprint.hex()))
+    # print("Encryption key: {}".format(encryption_key.hex()))
+    # print("Encrypted from KEY fingerprint: {}".format(fingerprint.hex()))
 
     return decrypt(token_b64_encoded=encrypted_api_key,
                    key=encryption_key
                    )
 
+
+def decrypt_api_key_with_paramiko_ssh_key_chacha20poly1305(encrypted_api_key_payload: str) -> str:
+    api_key_parts = encrypted_api_key_payload.split(":")
+    if len(api_key_parts) != 5:
+        raise PyloEx("Invalid encrypted API key format")
+
+    fingerprint = base64.urlsafe_b64decode(api_key_parts[2])
+    seed_key_to_be_signed = base64.urlsafe_b64decode(api_key_parts[3])
+    encrypted_api_key = base64.urlsafe_b64decode(api_key_parts[4])
+
+    ssh_key = find_ssh_key_from_fingerprint(fingerprint)
+    if ssh_key is None:
+        raise PyloEx("No key found in the agent with fingerprint {}".format(fingerprint.hex()))
+
+    signed_session_key = ssh_key.sign_ssh_data(seed_key_to_be_signed)
+    encryption_key = sha256(signed_session_key).digest()
+
+    chacha20_object = ChaCha20Poly1305(encryption_key)
+    nonce = seed_key_to_be_signed[:12]
+
+    return chacha20_object.decrypt(nonce, encrypted_api_key, ssh_key.get_fingerprint()).decode('utf-8')
+
+
 def decrypt_api_key(encrypted_api_key_payload: str) -> str:
     # detect the encryption method
     if not encrypted_api_key_payload.startswith("$encrypted$:"):
         raise PyloEx("Invalid encrypted API key format")
     if encrypted_api_key_payload.startswith("$encrypted$:ssh-Fernet:"):
         return decrypt_api_key_with_paramiko_ssh_key_fernet(encrypted_api_key_payload)
+    elif encrypted_api_key_payload.startswith("$encrypted$:ssh-ChaCha20Poly1305:"):
+        return decrypt_api_key_with_paramiko_ssh_key_chacha20poly1305(encrypted_api_key_payload)
 
     raise PyloEx("Unsupported encryption method: {}".format(encrypted_api_key_payload.split(":")[1]))
 
 
 def is_api_key_encrypted(encrypted_api_key_payload: str) -> bool:
-    return encrypted_api_key_payload.startswith("$encrypted$:")
+    return encrypted_api_key_payload.startswith("$encrypted$:")
+
+
+def find_ssh_key_from_fingerprint(fingerprint: bytes) -> Optional[paramiko.AgentKey]:
+    keys = paramiko.Agent().get_keys()
+    for key in keys:
+        if key.get_fingerprint() == fingerprint:
+            return key
+    return None
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/API/Explorer.py` & `illumio_pylo-0.3.5/illumio_pylo/API/Explorer.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/API/JsonPayloadTypes.py` & `illumio_pylo-0.3.5/illumio_pylo/API/JsonPayloadTypes.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/API/RuleSearchQuery.py` & `illumio_pylo-0.3.5/illumio_pylo/API/RuleSearchQuery.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/AgentStore.py` & `illumio_pylo-0.3.5/illumio_pylo/AgentStore.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 from typing import *
 
 # version_regex = re.compile(r"^(?P<major>[0-9]+)\.(?P<middle>[0-9]+)\.(?P<minor>[0-9]+)-(?P<build>[0-9]+)(u[0-9]+)?$")
 
 
 class VENAgent(pylo.ReferenceTracker):
 
+    __slots__ = ['href', 'owner', 'workload', 'software_version', '_last_heartbeat', '_status_security_policy_sync_state',
+                 '_status_security_policy_applied_at', '_status_rule_count', 'mode', 'raw_json']
+
     def __init__(self, href: str, owner: 'pylo.AgentStore', workload: 'pylo.Workload' = None):
         pylo.ReferenceTracker.__init__(self)
         self.href: str = href
         self.owner: 'pylo.AgentStore' = owner
         self.workload: Optional['pylo.Workload'] = workload
 
         self.software_version: Optional['pylo.SoftwareVersion'] = None
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/Exception.py` & `illumio_pylo-0.3.5/illumio_pylo/Exception.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/Helpers/exports.py` & `illumio_pylo-0.3.5/illumio_pylo/Helpers/exports.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/Helpers/functions.py` & `illumio_pylo-0.3.5/illumio_pylo/Helpers/functions.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/IPList.py` & `illumio_pylo-0.3.5/illumio_pylo/IPList.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,15 @@
 from .API.JsonPayloadTypes import IPListObjectJsonStructure
 from illumio_pylo import log
 from .Helpers import *
 
 
 class IPList(pylo.ReferenceTracker):
 
-    """
-    :type owner: IPListStore
-    :type description: str|None
-    :type raw_entries: dict[str,str]
-    """
-    name: str
-    href: str
+    __slots__ = ['owner', 'name', 'href', 'description', 'raw_json', 'raw_entries']
 
     def __init__(self, name: str, href: str, owner: 'pylo.IPListStore', description=None):
         """
         :type name: str
         :type href: str
         :type owner: IPListStore
         """
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/IPMap.py` & `illumio_pylo-0.3.5/illumio_pylo/IPMap.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 mask = 0
 for i in range(32):
     mask |= 1 << i
     masks.append(mask)
 
 
 class IP4Map:
+
+    __slots__ = ['_entries']
+
     def __init__(self):
         self._entries = []
 
     @staticmethod
     def ip_entry_from_text(entry: str, ignore_ipv6=True) -> Optional[List[int]]:
         new_entry = None
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/Label.py` & `illumio_pylo-0.3.5/illumio_pylo/Label.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/LabelCommon.py` & `illumio_pylo-0.3.5/illumio_pylo/LabelCommon.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Union
 from .Exception import PyloEx
 from .LabelStore import label_type_role, label_type_env, label_type_loc, label_type_app, LabelStore
 
 
 class LabelCommon:
 
+    __slots__ = ['owner', 'name', 'href', 'type']
+
     def __init__(self, name: str, href: str, label_type: str, owner: LabelStore):
         self.owner: LabelStore = owner
         self.name: str = name
         self.href: str = href
         self.type = label_type
 
     def is_label(self) -> bool:
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/LabelGroup.py` & `illumio_pylo-0.3.5/illumio_pylo/LabelGroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from illumio_pylo import Label
 from .API.JsonPayloadTypes import LabelGroupObjectJsonStructure
 
 
 class LabelGroup(pylo.ReferenceTracker, pylo.LabelCommon):
 
+    __slots__ = ['_members_by_href', 'raw_json']
+
     def __init__(self, name: str, href: str, label_type: str, owner):
         pylo.ReferenceTracker.__init__(self)
         pylo.LabelCommon.__init__(self, name, href, label_type, owner)
         self._members_by_href: Dict[str, Union['pylo.Label', 'pylo.LabelGroup']] = {}
         self.raw_json: Optional[LabelGroupObjectJsonStructure] = None
 
     def load_from_json(self):
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/LabelStore.py` & `illumio_pylo-0.3.5/illumio_pylo/LabelStore.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,16 @@
             result: List[Union['pylo.Label', 'pylo.LabelGroup']] = []
             for label_type in type_order:
                 for label in label_list:
                     if label.type == label_type:
                         result.append(label)
             return result
 
+    __slots__ = ['owner', '_items_by_href', 'label_types', 'label_types_as_set', 'label_resolution_cache']
+
     def __init__(self, owner: 'pylo.Organization'):
         self.owner: "pylo.Organization" = owner
         self._items_by_href: Dict[str, Union[pylo.Label, pylo.LabelGroup]] = {}
         self.label_types: List[str] = []
         self.label_types_as_set: Set[str] = set()
 
         self.label_resolution_cache: Optional[Dict[str, Union[pylo.Label, pylo.LabelGroup]]] = None
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/LabeledObject.py` & `illumio_pylo-0.3.5/illumio_pylo/LabeledObject.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Dict, Optional, List, Union, Iterable
 import illumio_pylo as pylo
 
 
 class LabeledObject:
 
+    __slots__ = ['_labels']
+
     def __init__(self):
         self._labels: Dict[str, 'pylo.Label'] = {}
 
     def get_label(self, key: str) -> Optional['pylo.Label']:
         return self._labels.get(key)
 
     def get_labels_dict(self):
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/Organization.py` & `illumio_pylo-0.3.5/illumio_pylo/Organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 import illumio_pylo as pylo
 from .API.JsonPayloadTypes import PCEObjectsJsonStructure, PCECacheFileJsonStructure
 from .API.CredentialsManager import get_credentials_from_file
 
 
 class Organization:
 
+    __slots__ = ['id', 'connector', 'LabelStore', 'IPListStore', 'WorkloadStore', 'VirtualServiceStore', 'AgentStore',
+                 'ServiceStore', 'RulesetStore', 'SecurityPrincipalStore', 'pce_version']
+
     def __init__(self, org_id):
         self.id: int = org_id
         self.connector: Optional['pylo.APIConnector'] = None
         self.LabelStore: 'pylo.LabelStore' = pylo.LabelStore(self)
         self.IPListStore: 'pylo.IPListStore' = pylo.IPListStore(self)
         self.WorkloadStore: 'pylo.WorkloadStore' = pylo.WorkloadStore(self)
         self.VirtualServiceStore: 'pylo.VirtualServiceStore' = pylo.VirtualServiceStore(self)
@@ -54,15 +57,15 @@
                                            credential_file: str = None,
                                            list_of_objects_to_load: Optional[List['pylo.ObjectTypes']] = None,
                                            include_deleted_workloads: bool = False,
                                            callback_api_objects_downloaded: Callable = None) -> 'Organization':
         """
         Credentials files will be looked for in the following order:
         1. The path provided in the credential_file argument
-        2. The path provided in the Pylo_CREDENTIAL_FILE environment variable
+        2. The path provided in the PYLO_CREDENTIAL_FILE environment variable
         3. The path ~/.pylo/credentials.json
         4. Current working directory credentials.json
         :param fqdn_or_profile_name:
         :param credential_file:
         :param list_of_objects_to_load:
         :param include_deleted_workloads:
         :param callback_api_objects_downloaded: callback function that will be called after each API has finished downloading all objects
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/Query.py` & `illumio_pylo-0.3.5/illumio_pylo/Query.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/ReferenceTracker.py` & `illumio_pylo-0.3.5/illumio_pylo/ReferenceTracker.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/Rule.py` & `illumio_pylo-0.3.5/illumio_pylo/Rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 
     def count_payloads(self) -> int:
         return len(self.json_payload)
 
 
 class Rule:
 
+    __slots__ = ['owner', 'description', 'services', 'providers', 'consumers', 'consuming_principals', 'href', 'enabled',
+                 'secure_connect', 'unscoped_consumers', 'stateless', 'machine_auth', 'raw_json', 'batch_update_stack']
+
     def __init__(self, owner: 'Ruleset'):
         self.owner: Ruleset = owner
         self.description: Optional[str] = None
         self.services: RuleServiceContainer = RuleServiceContainer(self)
         self.providers: RuleHostContainer = RuleHostContainer(self, 'providers')
         self.consumers: RuleHostContainer = RuleHostContainer(self, 'consumers')
         self.consuming_principals: RuleSecurityPrincipalContainer = RuleSecurityPrincipalContainer(self)
@@ -119,14 +122,17 @@
         """
         if self.batch_update_stack is None:
             raise pylo.PyloEx("Workload was not in 'update stacking' mode")
         return self.batch_update_stack.count_payloads()
 
 
 class RuleSecurityPrincipalContainer(pylo.Referencer):
+
+    __slots__ = ['owner', '_items']
+
     def __init__(self, owner: 'pylo.Rule'):
         Referencer.__init__(self)
         self.owner = owner
         self._items: Dict[SecurityPrincipal, SecurityPrincipal] = {}  # type:
 
     def load_from_json(self, data):
         ss_store = self.owner.owner.owner.owner.SecurityPrincipalStore  # make it a local variable for fast lookups
@@ -136,14 +142,17 @@
             if found_object is None:
                 raise pylo.PyloEx(f"Could not find SecurityPrincipal with href '{wanted_href}' inside rule href '{self.owner.href}' and Ruleset named '{self.owner.owner.name}'")
             found_object.add_reference(self)
             self._items[found_object] = found_object
 
 
 class DirectServiceInRule:
+
+    __slots__ = ['protocol', 'port', 'to_port']
+
     def __init__(self, proto: int, port: int = None, toport: int = None):
         self.protocol = proto
         self.port = port
         self.to_port = toport
 
     def is_tcp(self):
         return self.protocol == 6
@@ -241,14 +250,17 @@
         if not port_input.isdigit():
             raise PyloEx("Invalid port provided: '{}' in string '{}'".format(port_input, txt))
 
         return DirectServiceInRule(protocol_int, port=int(port_input))
 
 
 class RuleServiceContainer(pylo.Referencer):
+
+    __slots__ = ['owner', '_items', '_direct_services', '_cached_port_map']
+
     def __init__(self, owner: 'pylo.Rule'):
         Referencer.__init__(self)
         self.owner = owner
         self._items: Dict[Service, Service] = {}
         self._direct_services: List[DirectServiceInRule] = []
         self._cached_port_map: Optional[PortMap] = None
 
@@ -376,14 +388,17 @@
 
         self._cached_port_map = result
 
         return result
 
 
 class RuleHostContainer(pylo.Referencer):
+
+    __slots__ = ['owner', '_items', 'name', '_hasAllWorkloads']
+
     def __init__(self, owner: 'pylo.Rule', name: str):
         Referencer.__init__(self)
         self.owner = owner
         self._items: Dict[RuleActorsAcceptableTypes, RuleActorsAcceptableTypes] = {}
         self.name = name
         self._hasAllWorkloads = False
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/Ruleset.py` & `illumio_pylo-0.3.5/illumio_pylo/Ruleset.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import re
 
 ruleset_id_extraction_regex = re.compile(r"^/orgs/([0-9]+)/sec_policy/([0-9]+)?(draft)?/rule_sets/(?P<id>[0-9]+)$")
 
 
 class RulesetScope:
 
+    __slots__ = ['owner', 'scope_entries']
+
     def __init__(self, owner: 'pylo.Ruleset'):
         self.owner: 'pylo.Ruleset' = owner
         self.scope_entries: Dict['pylo.RulesetScopeEntry', 'pylo.RulesetScopeEntry'] = {}
 
     def load_from_json(self, data: List[List[RulesetScopeEntryLineJsonStructure]]):
         for scope_json in data:
             scope_entry = pylo.RulesetScopeEntry(self)
@@ -35,14 +37,16 @@
         for scope_entry in self.scope_entries:
             if scope_entry.is_all_all_all():
                 return True
         return False
 
 class RulesetScopeEntry:
 
+    __slots__ = ['owner', '_labels']
+
     def __init__(self, owner: 'pylo.RulesetScope'):
         self.owner: pylo.RulesetScope = owner
         self._labels: Dict[str, Union['pylo.Label', 'pylo.LabelGroup']] = {}
 
     def load_from_json(self, data: List[RulesetScopeEntryLineJsonStructure]):
         #log.error(pylo.nice_json(data))
         l_store = self.owner.owner.owner.owner.LabelStore
@@ -140,14 +144,16 @@
         :return:
         """
         return self._labels.get('app')
 
 
 class Ruleset:
 
+    __slots__ = ['owner', 'href', 'name', 'description', 'scopes', '_rules_by_href', '_rules', 'disabled']
+
     def __init__(self, owner: 'pylo.RulesetStore'):
         self.owner: 'pylo.RulesetStore' = owner
         self.href: Optional[str] = None
         self.name: str = ''
         self.description: str = ''
         self.scopes: 'pylo.RulesetScope' = pylo.RulesetScope(self)
         # must keep an ordered list of rules while the dict by href is there for quick searches
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/RulesetStore.py` & `illumio_pylo-0.3.5/illumio_pylo/RulesetStore.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import illumio_pylo as pylo
 from illumio_pylo import log, Organization, PyloEx, Rule, Ruleset
 from .Helpers import nice_json
 
 
 class RulesetStore:
 
+    __slots__ = ['owner', '_items_by_href']
+
     def __init__(self, owner: 'pylo.Organization'):
         self.owner: pylo.Organization = owner
         self._items_by_href: Dict[str, 'pylo.Ruleset'] = {}
 
     @property
     def rulesets(self) -> List['pylo.Ruleset']:
         """
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/SecurityPrincipal.py` & `illumio_pylo-0.3.5/illumio_pylo/SecurityPrincipal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Optional
 import illumio_pylo as pylo
 from .Helpers import nice_json
 from illumio_pylo import log
 
 
 class SecurityPrincipal(pylo.ReferenceTracker):
+
+    __slots__ = ['owner', 'name', 'href', 'sid', 'deleted', 'raw_json']
+
     def __init__(self, name: str, href: str, owner: 'pylo.SecurityPrincipalStore'):
         pylo.ReferenceTracker.__init__(self)
         self.owner: 'pylo.SecurityPrincipalStore' = owner
         self.name: str = name
         self.href: str = href
         self.sid: Optional[str] = None
         self.deleted: bool = False
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/Service.py` & `illumio_pylo-0.3.5/illumio_pylo/Service.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from .API.JsonPayloadTypes import ServiceHrefRef
 from illumio_pylo import log
 from .Helpers import *
 from typing import *
 
 
 class PortMap:
+
+    __slots__ = ['_tcp_map', '_udp_map', '_protocol_map']
+
     def __init__(self):
         self._tcp_map: List[List[2]] = []  # [start, end]
         self._udp_map: List[List[2]] = []  # [start, end]
         self._protocol_map = {}
 
     def copy(self) -> 'PortMap':
         new_map = PortMap()
@@ -95,14 +98,17 @@
             return my_list[0]
 
         self._tcp_map.sort(key=first_entry)
         self._udp_map.sort(key=first_entry)
 
 
 class ServiceEntry:
+
+    __slots__ = ['protocol', 'port', 'to_port', 'icmp_code', 'icmp_type']
+
     def __init__(self, protocol: int, port: int = None, to_port: Optional[int] = None, icmp_code: Optional[int] = None,
                  icmp_type: Optional[int] = None):
         self.protocol = protocol
         self.port: int = port
         self.to_port: Optional[int] = to_port
         self.icmp_type: Optional[int] = icmp_type
         self.icmp_code: Optional[int] = icmp_code
@@ -156,14 +162,16 @@
             return str(self.port) + '-' + str(self.to_port) + '/tcp'
 
         return str(self.protocol) + '/proto'
 
 
 class Service(pylo.ReferenceTracker):
 
+    __slots__ = ['name', 'href', 'owner', 'entries', 'description', 'processName', 'deleted', 'raw_json']
+
     def __init__(self, name: str, href: str, owner: 'pylo.ServiceStore'):
         pylo.ReferenceTracker.__init__(self)
 
         self.owner: 'pylo.ServiceStore' = owner
         self.name: str = name
         self.href: str = href
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/SoftwareVersion.py` & `illumio_pylo-0.3.5/illumio_pylo/SoftwareVersion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 import re
 
 version_regex = re.compile(r"^(?P<major>[0-9]+)\.(?P<middle>[0-9]+)\.(?P<minor>[0-9]+)(-(?P<build>[0-9]+))?(.*)?$")
 
 
 class SoftwareVersion:
 
-    """
-    :type version_string: str
-    """
+    __slots__ = ['version_string', 'is_unknown', 'major', 'middle', 'minor', 'build']
 
     def __init__(self, version_string: str):
         self.version_string = version_string
 
         self.is_unknown = False
         self.major = 0
         self.middle = 0
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/VirtualService.py` & `illumio_pylo-0.3.5/illumio_pylo/VirtualService.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import Optional
 from .API.JsonPayloadTypes import VirtualServiceObjectJsonStructure
 import illumio_pylo as pylo
 
 
 class VirtualService(pylo.ReferenceTracker):
+
+    __slots__ = ['owner', 'name', 'href', 'raw_json']
+
     def __init__(self, name: str, href: str, owner: 'pylo.VirtualServiceStore'):
         pylo.ReferenceTracker.__init__(self)
         self.owner = owner
         self.name: str = name
         self.href: str = href
 
         self.raw_json: Optional[VirtualServiceObjectJsonStructure] = None
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/VirtualServiceStore.py` & `illumio_pylo-0.3.5/illumio_pylo/VirtualServiceStore.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import illumio_pylo as pylo
 from illumio_pylo import log
 from .API.JsonPayloadTypes import VirtualServiceObjectJsonStructure
 
 
 class VirtualServiceStore:
 
+    __slots__ = ['owner', 'items_by_href', 'itemsByName']
+
     def __init__(self, owner: 'pylo.Organization'):
         self.owner: 'pylo.Organization' = owner
         self.items_by_href: Dict[str, 'pylo.VirtualService'] = {}
         self.itemsByName: Dict[str, 'pylo.VirtualService'] = {}
 
     def load_virtualservices_from_json(self, json_list: List[VirtualServiceObjectJsonStructure]):
         for json_item in json_list:
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/Workload.py` & `illumio_pylo-0.3.5/illumio_pylo/Workload.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,17 @@
         return len(self.json_payload)
 
 
 
 
 class Workload(pylo.ReferenceTracker, pylo.Referencer, LabeledObject):
 
+    __slots__ = ['owner', 'name', 'href', 'forced_name', 'hostname', 'description', 'interfaces', 'online', 'os_id',
+                 'os_detail', 'ven_agent', 'unmanaged', 'temporary', 'deleted', 'raw_json', '_batch_update_stack']
+
     def __init__(self, name: str, href: str, owner: 'pylo.WorkloadStore'):
         ReferenceTracker.__init__(self)
         Referencer.__init__(self)
         LabeledObject.__init__(self)
         self.owner = owner
         self.name: str = name
         self.href: str = href
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/WorkloadStore.py` & `illumio_pylo-0.3.5/illumio_pylo/WorkloadStore.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from typing import Optional, List, Union, Set, Iterable
 
 from .WorkloadStoreSubClasses import UnmanagedWorkloadDraft, UnmanagedWorkloadDraftMultiCreatorManager
 
 
 class WorkloadStore:
 
+    __slots__ = ['owner', 'itemsByHRef']
+
     def __init__(self, owner: 'Organization'):
         self.owner: Organization = owner
         self.itemsByHRef: Dict[str, Workload] = {}
 
     def load_workloads_from_json(self, json_list):
         for json_item in json_list:
             self.add_workload_from_json(json_item)
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/WorkloadStoreSubClasses.py` & `illumio_pylo-0.3.5/illumio_pylo/WorkloadStoreSubClasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     draft: UnmanagedWorkloadDraft
     external_tracker_id: Any
     success: bool
     message: str
     workload: Optional[pylo.Workload] = None
     workload_href: Optional[str] = None
 
+
 class UnmanagedWorkloadDraftMultiCreatorManager:
     def __init__(self, owner: 'pylo.WorkloadStore'):
 
 
         self.owner = owner
         self.drafts: List[UnmanagedWorkloadDraft] = []
         self._external_tracker_ids: List[Any] = []
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/__init__.py` & `illumio_pylo-0.3.5/illumio_pylo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-__version__ = "0.3.4"
+__version__ = "0.3.5"
 
-import os
-import sys
 from typing import Callable
 
 from .tmp import *
 from .Helpers import *
 
 from .Exception import PyloEx, PyloApiEx, PyloApiTooManyRequestsEx, PyloApiUnexpectedSyntax, PyloObjectNotFound, PyloApiRequestForbiddenEx
 from .SoftwareVersion import SoftwareVersion
@@ -56,15 +54,15 @@
                                            credential_file: str = None,
                                            list_of_objects_to_load: Optional[List['pylo.ObjectTypes']] = None,
                                            include_deleted_workloads: bool = False,
                                            callback_api_objects_downloaded: Callable = None) -> Organization:
     """
     Credentials files will be looked for in the following order:
     1. The path provided in the credential_file argument
-    2. The path provided in the Pylo_CREDENTIAL_FILE environment variable
+    2. The path provided in the PYLO_CREDENTIAL_FILE environment variable
     3. The path ~/.pylo/credentials.json
     4. Current working directory credentials.json
     :param fqdn_or_profile_name:
     :param credential_file:
     :param list_of_objects_to_load:
     :param include_deleted_workloads:
     :param callback_api_objects_downloaded: callback function that will be called after each API has finished downloading all objects
@@ -73,12 +71,11 @@
     return Organization.get_from_api_using_credential_file(fqdn_or_profile_name=fqdn_or_profile_name,
                                                            credential_file=credential_file,
                                                            list_of_objects_to_load=list_of_objects_to_load,
                                                            include_deleted_workloads=include_deleted_workloads,
                                                            callback_api_objects_downloaded=callback_api_objects_downloaded)
 
 
-
 ignoreWorkloadsWithSameName = True
 
 objectNotFound = object()
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/NativeParsers.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/NativeParsers.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/__init__.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/__init__.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/credential_manager.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/credential_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 import os
 
 import paramiko
 
 import illumio_pylo as pylo
 import click
 from illumio_pylo.API.CredentialsManager import get_all_credentials, create_credential_in_file, CredentialFileEntry, \
-    create_credential_in_default_file, encrypt_api_key_with_paramiko_ssh_key_fernet, decrypt_api_key_with_paramiko_ssh_key_fernet, \
-    get_credentials_from_file
+    create_credential_in_default_file,  \
+    get_credentials_from_file, encrypt_api_key_with_paramiko_ssh_key_chacha20poly1305, \
+    decrypt_api_key_with_paramiko_ssh_key_chacha20poly1305, decrypt_api_key_with_paramiko_ssh_key_fernet
 
 from illumio_pylo import log
 from . import Command
 
 
 command_name = "cred-manager"
 objects_load_filter = None
@@ -24,15 +25,14 @@
     sub_parser = parser.add_subparsers(dest='sub_command', required=True)
     list_parser = sub_parser.add_parser('list', help='List all credentials')
 
     test_parser = sub_parser.add_parser('test', help='Test a credential')
     test_parser.add_argument('--name', required=False, type=str, default=None,
                              help='Name of the credential profile to test')
 
-
     create_parser = sub_parser.add_parser('create', help='Create a new credential')
     create_parser.add_argument('--name', required=False, type=str, default=None,
                      help='Name of the credential')
     create_parser.add_argument('--fqdn', required=False, type=str, default=None,
                                  help='FQDN of the PCE')
     create_parser.add_argument('--port', required=False, type=int, default=None,
                                  help='Port of the PCE')
@@ -42,28 +42,26 @@
                                     help='API user')
     create_parser.add_argument('--verify-ssl', required=False, type=bool, default=None,
                                  help='Verify SSL')
 
 
 def __main(args, **kwargs):
     if args['sub_command'] == 'list':
+        table = PrettyTable(field_names=["Name", "URL", "API User", "Originating File"])
+        # all should be left justified
+        table.align = "l"
+
         credentials = get_all_credentials()
         # sort credentials by name
         credentials.sort(key=lambda x: x.name)
 
-        # print credentials in a nice table
-        table_template = " {:<19} {:<40} {:<22} {:<25}"
-        print(table_template.format("Name", "URL", "API User", "Originating File"))
-
         for credential in credentials:
-            print(table_template.format(credential.name,
-                                        credential.fqdn + ':' + str(credential.port),
-                                        credential.api_user,
-                                        credential.originating_file)
-                  )
+            table.add_row([credential.name, credential.fqdn, credential.api_user, credential.originating_file])
+
+        print(table)
 
     elif args['sub_command'] == 'create':
 
         wanted_name = args['name']
         if wanted_name is None:
             wanted_name = click.prompt('> Input a Profile Name (ie: prod-pce)', type=str)
 
@@ -132,18 +130,19 @@
 
             index_of_selected_key = click.prompt('> Select key by ID#', type=click.IntRange(0, len(ssh_keys)-1))
             selected_ssh_key = ssh_keys[index_of_selected_key]
             print("Selected key: {} | {} | {}".format(selected_ssh_key.get_name(),
                                                       selected_ssh_key.get_fingerprint().hex(),
                                                       selected_ssh_key.comment))
             print(" * encrypting API key with selected key (you may be prompted by your SSH agent for confirmation or PIN code) ...", flush=True, end="")
-            encrypted_api_key = encrypt_api_key_with_paramiko_ssh_key_fernet(ssh_key=selected_ssh_key, api_key=api_key)
+            # encrypted_api_key = encrypt_api_key_with_paramiko_ssh_key_fernet(ssh_key=selected_ssh_key, api_key=api_key)
+            encrypted_api_key = encrypt_api_key_with_paramiko_ssh_key_chacha20poly1305(ssh_key=selected_ssh_key, api_key=api_key)
             print("OK!")
             print(" * trying to decrypt the encrypted API key...", flush=True, end="")
-            decrypted_api_key = decrypt_api_key_with_paramiko_ssh_key_fernet(encrypted_api_key_payload=encrypted_api_key)
+            decrypted_api_key = decrypt_api_key_with_paramiko_ssh_key_chacha20poly1305(encrypted_api_key_payload=encrypted_api_key)
             if decrypted_api_key != api_key:
                 raise pylo.PyloEx("Decrypted API key does not match original API key")
             print("OK!")
             credentials_data["api_key"] = encrypted_api_key
 
 
         cwd = os.getcwd()
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/iplist_analyzer.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/iplist_analyzer.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/iplist_import_from_file.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/iplist_import_from_file.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/ruleset_export.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/ruleset_export.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/update_pce_objects_cache.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/update_pce_objects_cache.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/utils/LabelCreation.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/utils/LabelCreation.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/utils/misc.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/utils/misc.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_compatibility_report_export.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/ven_compatibility_report_export.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_duplicate_remover.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/ven_duplicate_remover.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_idle_to_visibility.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/ven_idle_to_visibility.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/ven_upgrader.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/ven_upgrader.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_export.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/workload_export.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_import.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/workload_import.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_reset_names_to_null.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/workload_reset_names_to_null.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_update.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/workload_update.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/cli/commands/workload_used_in_rule_finder.py` & `illumio_pylo-0.3.5/illumio_pylo/cli/commands/workload_used_in_rule_finder.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/docs/Doxygen` & `illumio_pylo-0.3.5/illumio_pylo/docs/Doxygen`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/tmp.py` & `illumio_pylo-0.3.5/illumio_pylo/tmp.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,22 +33,41 @@
 
 def find_connector_or_die(obj) -> 'pylo.APIConnector':
     """
     Find the APIConnector object in the object or its owner recursively. Will raise an exception if not found
     :param obj:
     :return:
     """
-    connector = obj.__dict__.get('connector')  # type: pylo.APIConnector
-    if connector is None:
-        owner = obj.__dict__.get('owner')
-        if owner is None:
-            raise Exception("Could not find a Connector object")
-        return find_connector_or_die(owner)
 
-    return connector
+    connector = None
+
+    # check if object has a __dict__ attribute
+    if not hasattr(obj, '__dict__'):
+        # check if it's in __slots__
+        if hasattr(obj, '__slots__'):
+            if 'connector' in obj.__slots__:
+                connector = obj.__getattribute__('connector')
+                if connector is not None:
+                    return connector
+                raise Exception("Could not find a Connector object")
+            if 'owner' in obj.__slots__:
+                owner = obj.__getattribute__('owner')
+                if owner is None:
+                    raise Exception("Could not find a Connector object")
+                return find_connector_or_die(owner)
+        raise Exception("Could not find a Connector object")
+    else:
+        connector = obj.__dict__.get('connector')  # type: pylo.APIConnector
+        if connector is None:
+            owner = obj.__dict__.get('owner')
+            if owner is None:
+                raise Exception("Could not find a Connector object")
+            return find_connector_or_die(owner)
+
+        return connector
 
 
 class IDTranslationTable:
     """docstring fo ID_TranslationTable."""
 
     def __init__(self):
         self.OldToNew = {}
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo/utilities/health_monitoring.py` & `illumio_pylo-0.3.5/illumio_pylo/utilities/health_monitoring.py`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/utilities/resources/iplists-import-example.xlsx` & `illumio_pylo-0.3.5/illumio_pylo/utilities/resources/iplists-import-example.xlsx`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo/utilities/resources/workloads-import-example.xlsx` & `illumio_pylo-0.3.5/illumio_pylo/utilities/resources/workloads-import-example.xlsx`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/illumio_pylo.egg-info/PKG-INFO` & `illumio_pylo-0.3.5/illumio_pylo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: illumio_pylo
-Version: 0.3.4
+Version: 0.3.5
 Summary: A set of tools and library for working with Illumio PCE
 Home-page: https://github.com/cpainchaud/pylo
 Author: Christophe Painchaud
 Author-email: shellescape@gmail.com
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `illumio_pylo-0.3.4/illumio_pylo.egg-info/SOURCES.txt` & `illumio_pylo-0.3.5/illumio_pylo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/pyproject.toml` & `illumio_pylo-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `illumio_pylo-0.3.4/setup.py` & `illumio_pylo-0.3.5/setup.py`

 * *Files identical despite different names*

